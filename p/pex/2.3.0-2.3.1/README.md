# Comparing `tmp/pex-2.3.0.tar.gz` & `tmp/pex-2.3.1.tar.gz`

## Comparing `pex-2.3.0.tar` & `pex-2.3.1.tar`

### file list

```diff
@@ -1,1069 +1,1071 @@
--rw-r--r--   0        0        0   103858 2020-02-02 00:00:00.000000 pex-2.3.0/CHANGES.md
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 pex-2.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pex-2.3.0/RELEASE.rst
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pex-2.3.0/docs-requirements.txt
--rwxr-xr-x   0        0        0     3366 2020-02-02 00:00:00.000000 pex-2.3.0/dtox.sh
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pex-2.3.0/mypy.ini
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 pex-2.3.0/tox.ini
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pex-2.3.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     8388 2020-02-02 00:00:00.000000 pex-2.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pex-2.3.0/.github/workflows/doc-site.yml
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pex-2.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pex-2.3.0/assets/download.svg
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pex-2.3.0/assets/github.svg
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pex-2.3.0/assets/pdf.svg
--rw-r--r--   0        0        0    25424 2020-02-02 00:00:00.000000 pex-2.3.0/assets/pex-icon-512.png
--rw-r--r--   0        0        0    25312 2020-02-02 00:00:00.000000 pex-2.3.0/assets/pex-icon-512x512.png
--rw-r--r--   0        0        0    34315 2020-02-02 00:00:00.000000 pex-2.3.0/assets/pex-logo-dark.png
--rw-r--r--   0        0        0    35372 2020-02-02 00:00:00.000000 pex-2.3.0/assets/pex-logo-light.png
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 pex-2.3.0/assets/pex.svg
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pex-2.3.0/assets/python.svg
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pex-2.3.0/build-backend/pex_build/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/build-backend/pex_build/hatchling/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 pex-2.3.0/build-backend/pex_build/hatchling/build.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pex-2.3.0/build-backend/pex_build/hatchling/build_hook.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pex-2.3.0/build-backend/pex_build/hatchling/hooks.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 pex-2.3.0/build-backend/pex_build/hatchling/metadata_hook.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pex-2.3.0/build-backend/pex_build.dist-info/entry_points.txt
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 pex-2.3.0/docker/base/Dockerfile
--rwxr-xr-x   0        0        0     1190 2020-02-02 00:00:00.000000 pex-2.3.0/docker/base/install_pythons.sh
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pex-2.3.0/docker/cache/Dockerfile
--rwxr-xr-x   0        0        0      822 2020-02-02 00:00:00.000000 pex-2.3.0/docker/cache/populate_cache.sh
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pex-2.3.0/docker/user/Dockerfile
--rwxr-xr-x   0        0        0      372 2020-02-02 00:00:00.000000 pex-2.3.0/docker/user/create_docker_image_user.sh
--rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 pex-2.3.0/docs/buildingpex.rst
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 pex-2.3.0/docs/conf.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 pex-2.3.0/docs/index.rst
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 pex-2.3.0/docs/recipes.rst
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pex-2.3.0/docs/whatispex.rst
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pex-2.3.0/docs/_ext/sphinx_pex/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 pex-2.3.0/docs/_ext/sphinx_pex/vars.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/docs/_static/pex-icon.png -> ../../assets/pex-icon-512.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/docs/_static/pex-logo-dark.png -> ../../assets/pex-logo-dark.png
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/docs/_static/pex-logo-light.png -> ../../assets/pex-logo-light.png
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pex-2.3.0/docs/_templates/search.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pex-2.3.0/docs/api/vars.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/__init__.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pex-2.3.0/pex/__main__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pex-2.3.0/pex/argparse.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pex-2.3.0/pex/asserts.py
--rw-r--r--   0        0        0    12917 2020-02-02 00:00:00.000000 pex-2.3.0/pex/atomic_directory.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pex-2.3.0/pex/attrs.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 pex-2.3.0/pex/auth.py
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 pex-2.3.0/pex/bootstrap.py
--rw-r--r--   0        0        0    28253 2020-02-02 00:00:00.000000 pex-2.3.0/pex/common.py
--rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 pex-2.3.0/pex/compatibility.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 pex-2.3.0/pex/compiler.py
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 pex-2.3.0/pex/dependency_manager.py
--rw-r--r--   0        0        0    39146 2020-02-02 00:00:00.000000 pex-2.3.0/pex/dist_metadata.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 pex-2.3.0/pex/enum.py
--rw-r--r--   0        0        0    33997 2020-02-02 00:00:00.000000 pex-2.3.0/pex/environment.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 pex-2.3.0/pex/exclude_configuration.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 pex-2.3.0/pex/executor.py
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 pex-2.3.0/pex/fetcher.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 pex-2.3.0/pex/finders.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pex-2.3.0/pex/fingerprinted_distribution.py
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 pex-2.3.0/pex/hashing.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 pex-2.3.0/pex/inherit_path.py
--rw-r--r--   0        0        0    62887 2020-02-02 00:00:00.000000 pex-2.3.0/pex/interpreter.py
--rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 pex-2.3.0/pex/interpreter_constraints.py
--rw-r--r--   0        0        0    27970 2020-02-02 00:00:00.000000 pex-2.3.0/pex/jobs.py
--rw-r--r--   0        0        0    21690 2020-02-02 00:00:00.000000 pex-2.3.0/pex/layout.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 pex-2.3.0/pex/network_configuration.py
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pex-2.3.0/pex/orderedset.py
--rw-r--r--   0        0        0    18333 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pep_376.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pep_425.py
--rw-r--r--   0        0        0    11944 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pep_427.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pep_440.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pep_503.py
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pep_508.py
--rw-r--r--   0        0        0    34423 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pex.py
--rw-r--r--   0        0        0    29527 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pex_bootstrapper.py
--rw-r--r--   0        0        0    35644 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pex_builder.py
--rw-r--r--   0        0        0    21630 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pex_info.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pex_warnings.py
--rw-r--r--   0        0        0    13748 2020-02-02 00:00:00.000000 pex-2.3.0/pex/platforms.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pth.py
--rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pyenv.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 pex-2.3.0/pex/rank.py
--rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 pex-2.3.0/pex/requirements.py
--rw-r--r--   0        0        0    58885 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolver.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pex-2.3.0/pex/result.py
--rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 pex-2.3.0/pex/sh_boot.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 pex-2.3.0/pex/sorted_tuple.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 pex-2.3.0/pex/targets.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tracer.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pex-2.3.0/pex/typing.py
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 pex-2.3.0/pex/util.py
--rw-r--r--   0        0        0    33969 2020-02-02 00:00:00.000000 pex-2.3.0/pex/variables.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pex-2.3.0/pex/version.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 pex-2.3.0/pex/wheel.py
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 pex-2.3.0/pex/ziputils.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/bin/__init__.py
--rwxr-xr-x   0        0        0    43108 2020-02-02 00:00:00.000000 pex-2.3.0/pex/bin/pex.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pex-2.3.0/pex/build_system/__init__.py
--rw-r--r--   0        0        0     9917 2020-02-02 00:00:00.000000 pex-2.3.0/pex/build_system/pep_517.py
--rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 pex-2.3.0/pex/build_system/pep_518.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/cli/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pex-2.3.0/pex/cli/__main__.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 pex-2.3.0/pex/cli/command.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pex-2.3.0/pex/cli/pex.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 pex-2.3.0/pex/cli/commands/__init__.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 pex-2.3.0/pex/cli/commands/docs.py
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pex-2.3.0/pex/cli/commands/interpreter.py
--rw-r--r--   0        0        0    68920 2020-02-02 00:00:00.000000 pex-2.3.0/pex/cli/commands/lock.py
--rw-r--r--   0        0        0    16628 2020-02-02 00:00:00.000000 pex-2.3.0/pex/cli/commands/venv.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/commands/__init__.py
--rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 pex-2.3.0/pex/commands/command.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/distutils/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/distutils/commands/__init__.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 pex-2.3.0/pex/distutils/commands/bdist_pex.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pex-2.3.0/pex/docs/__init__.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pex-2.3.0/pex/docs/command.py
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 pex-2.3.0/pex/docs/server.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/__init__.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/download_observer.py
--rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/installation.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/local_project.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/log_analyzer.py
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/tailer.py
--rw-r--r--   0        0        0    28069 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/tool.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/vcs.py
--rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/version.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/foreign_platform/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/foreign_platform/markers.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/foreign_platform/requires_python.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pex-2.3.0/pex/pip/foreign_platform/tags.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/__init__.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/config.py
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/configured_resolve.py
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/configured_resolver.py
--rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/downloads.py
--rw-r--r--   0        0        0    19225 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/lock_resolver.py
--rw-r--r--   0        0        0    32283 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/locked_resolve.py
--rw-r--r--   0        0        0    24303 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/locker.py
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/locker_patches.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/path_mappings.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/pex_repository_resolver.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/requirement_configuration.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/requirement_options.py
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/resolved_requirement.py
--rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/resolver_configuration.py
--rw-r--r--   0        0        0    25682 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/resolver_options.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/resolvers.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/target_configuration.py
--rw-r--r--   0        0        0    11066 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/target_options.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/lockfile/__init__.py
--rw-r--r--   0        0        0    20351 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/lockfile/create.py
--rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/lockfile/download_manager.py
--rw-r--r--   0        0        0    16083 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/lockfile/json_codec.py
--rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/lockfile/model.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/lockfile/subset.py
--rw-r--r--   0        0        0    30824 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/lockfile/updater.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/pep_691/__init__.py
--rw-r--r--   0        0        0     8950 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/pep_691/api.py
--rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/pep_691/fingerprint_service.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 pex-2.3.0/pex/resolve/pep_691/model.py
--rw-r--r--   0        0        0    25318 2020-02-02 00:00:00.000000 pex-2.3.0/pex/third_party/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/__main__.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/command.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/main.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/commands/__init__.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/commands/digraph.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/commands/graph.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/commands/info.py
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/commands/interpreter.py
--rw-r--r--   0        0        0    17057 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/commands/repository.py
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pex-2.3.0/pex/tools/commands/venv.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/README.md
--rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/__init__.py
--rw-r--r--   0        0        0    18350 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/.layout.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/__init__.py
--rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/__init__.pyi
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/_cmp.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/_cmp.pyi
--rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/_compat.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/_config.py
--rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/_funcs.py
--rw-r--r--   0        0        0   102691 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/_make.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/_next_gen.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/_version_info.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/_version_info.pyi
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/converters.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/converters.pyi
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/exceptions.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/exceptions.pyi
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/filters.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/filters.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/py.typed
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/setters.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/setters.pyi
--rw-r--r--   0        0        0    15966 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/validators.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attr/validators.pyi
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs/__init__.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs/__init__.pyi
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs/converters.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs/exceptions.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs/filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs/py.typed
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs/setters.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs/validators.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/AUTHORS.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/LICENSE
--rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/METADATA
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/WHEEL
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/top_level.txt
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/.layout.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/constraints.txt
--rw-r--r--   0        0        0   273365 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/pyparsing.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/__about__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/_compat.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/_structures.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/_typing.py
--rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/py.typed
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/requirements.py
--rw-r--r--   0        0        0    32208 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/specifiers.py
--rw-r--r--   0        0        0    29561 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/tags.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/utils.py
--rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/METADATA
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/WHEEL
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/LICENSE
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/METADATA
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/WHEEL
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/top_level.txt
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/.layout.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/constraints.txt
--rw-r--r--   0        0        0   273365 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/pyparsing.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/_structures.py
--rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/markers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/py.typed
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0    15147 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/METADATA
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/WHEEL
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/top_level.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/INSTALLER
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/LICENSE
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/METADATA
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/WHEEL
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/top_level.txt
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/.layout.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/__init__.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/constraints.txt
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_elffile.py
--rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_musllinux.py
--rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/markers.py
--rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/py.typed
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/specifiers.py
--rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/tags.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/utils.py
--rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/METADATA
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/WHEEL
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/.layout.json
--rwxr-xr-x   0        0        0      383 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/.prefix/bin/pip
--rwxr-xr-x   0        0        0      383 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/.prefix/bin/pip3
--rwxr-xr-x   0        0        0      383 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/.prefix/bin/pip3.8
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/__init__.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/__main__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/__init__.py
--rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/build_env.py
--rw-r--r--   0        0        0    12249 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cache.py
--rw-r--r--   0        0        0    13904 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/configuration.py
--rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/exceptions.py
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/locations.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/main.py
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11816 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     9337 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    28618 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    16455 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     7315 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/help.py
--rw-r--r--   0        0        0    27410 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    22070 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37454 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/index.py
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/link.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/download.py
--rw-r--r--   0        0        0     8121 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    15449 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/check.py
--rw-r--r--   0        0        0    10411 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    22460 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/install/legacy.py
--rw-r--r--   0        0        0    31247 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16135 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    18594 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    33420 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     7887 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_tracker.py
--rw-r--r--   0        0        0    23771 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    18234 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    20035 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    18946 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11634 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/distutils_args.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    28047 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/parallel.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/pkg_resources.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/typing.py
--rw-r--r--   0        0        0     9488 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    15599 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    12558 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    23767 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/appdirs.py
--rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/contextlib2.py
--rw-r--r--   0        0        0    43628 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distro.py
--rw-r--r--   0        0        0    79875 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/ipaddress.py
--rw-r--r--   0        0        0   273394 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pyparsing.py
--rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/retrying.py
--rw-r--r--   0        0        0    34159 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/six.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    14149 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   281608 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31254 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0     9411 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/compat.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    31621 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20715 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25777 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    19643 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0    12839 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    17948 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langcyrillicmodel.py
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    25481 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    12485 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41408 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51059 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    21066 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    52100 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    38962 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    17180 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/scripts.py
--rw-r--r--   0        0        0    96768 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/t32.exe
--rw-r--r--   0        0        0   105984 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    59845 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23391 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/version.py
--rw-r--r--   0        0        0    90112 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/w32.exe
--rw-r--r--   0        0        0    99840 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    41144 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/__init__.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/misc.py
--rw-r--r--   0        0        0    25707 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/shutil.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/sysconfig.cfg
--rw-r--r--   0        0        0    26854 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/sysconfig.py
--rw-r--r--   0        0        0    92628 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/tarfile.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/__init__.py
--rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_ihatexml.py
--rw-r--r--   0        0        0    32353 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_inputstream.py
--rw-r--r--   0        0        0    77040 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_tokenizer.py
--rw-r--r--   0        0        0     4931 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_utils.py
--rw-r--r--   0        0        0    83464 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/constants.py
--rw-r--r--   0        0        0   117186 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/html5parser.py
--rw-r--r--   0        0        0    15759 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/serializer.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/_base.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/py.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/__init__.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/base.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/lint.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/optionaltags.py
--rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/sanitizer.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/whitespace.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/__init__.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/genshi.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/sax.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/__init__.py
--rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/base.py
--rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/dom.py
--rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/etree.py
--rw-r--r--   0        0        0    14766 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/etree_lxml.py
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/__init__.py
--rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/base.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/dom.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/etree.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/genshi.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    42350 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   202084 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/msgpack/_version.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    37133 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/_typing.py
--rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    32208 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    29561 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/__init__.py
--rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/_in_process.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/build.py
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/check.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/compat.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/dirtools.py
--rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/envbuild.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/meta.py
--rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/wrappers.py
--rw-r--r--   0        0        0   108277 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/progress/__init__.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/progress/bar.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/progress/counter.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/progress/spinner.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    21548 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18430 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    34373 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30135 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    30355 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    16538 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/toml/__init__.py
--rw-r--r--   0        0        0    38954 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/toml/decoder.py
--rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/toml/encoder.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/toml/ordered.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/toml/tz.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    37133 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19763 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    28203 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    16795 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34303 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17649 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13908 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    32536 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    21366 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    16281 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    13981 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/INSTALLER
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/METADATA
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/top_level.txt
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/.layout.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/__init__.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/easy_install.py
--rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/.prefix/bin/easy_install
--rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/.prefix/bin/easy_install-3.8
--rw-r--r--   0        0        0   109513 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/py31compat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0   232055 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/pyparsing.py
--rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/six.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    28025 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_imp.py
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/archive_util.py
--rw-r--r--   0        0        0    10153 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/build_meta.py
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/cli-32.exe
--rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/cli-64.exe
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/cli.exe
--rw-r--r--   0        0        0    21571 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/config.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/dep_util.py
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/depends.py
--rw-r--r--   0        0        0    51749 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/dist.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/errors.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/extension.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/glob.py
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/gui-32.exe
--rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/gui-64.exe
--rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/gui.exe
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/installer.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/launch.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/lib2to3_ex.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/monkey.py
--rw-r--r--   0        0        0    47209 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/msvc.py
--rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/namespaces.py
--rw-r--r--   0        0        0    42090 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/package_index.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/py27compat.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/py31compat.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/py33compat.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/py34compat.py
--rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/script.tmpl
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/site-patch.py
--rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/ssl_support.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/version.py
--rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/wheel.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/windows_support.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0   232055 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/pyparsing.py
--rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/six.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    27778 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    12933 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/alias.py
--rw-r--r--   0        0        0    18880 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/bdist_wininst.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    13284 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/build_py.py
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/develop.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    90093 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    27330 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/install.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/register.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/rotate.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/setopt.py
--rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/test.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/upload.py
--rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/INSTALLER
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/LICENSE
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/METADATA
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/WHEEL
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/dependency_links.txt
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/entry_points.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/top_level.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/zip-safe
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/.layout.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/__init__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/constraints.txt
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml/__init__.py
--rw-r--r--   0        0        0    39064 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml/decoder.py
--rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml/encoder.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml/ordered.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml/tz.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/INSTALLER
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/LICENSE
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/METADATA
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/WHEEL
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pex-2.3.0/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/top_level.txt
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pex-2.3.0/pex/venv/README.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/pex/venv/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 pex-2.3.0/pex/venv/bin_path.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pex-2.3.0/pex/venv/install_scope.py
--rw-r--r--   0        0        0    37346 2020-02-02 00:00:00.000000 pex-2.3.0/pex/venv/installer.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pex-2.3.0/pex/venv/installer_configuration.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 pex-2.3.0/pex/venv/installer_options.py
--rw-r--r--   0        0        0    19086 2020-02-02 00:00:00.000000 pex-2.3.0/pex/venv/virtualenv.py
--rw-r--r--   0        0        0   106996 2020-02-02 00:00:00.000000 pex-2.3.0/pex/venv/virtualenv_16.7.12_py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 pex-2.3.0/scripts/build_cache_image.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 pex-2.3.0/scripts/build_docs.py
--rwxr-xr-x   0        0        0      919 2020-02-02 00:00:00.000000 pex-2.3.0/scripts/embed_virtualenv.py
--rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 pex-2.3.0/scripts/format.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pex-2.3.0/scripts/lint.py
--rwxr-xr-x   0        0        0     6874 2020-02-02 00:00:00.000000 pex-2.3.0/scripts/package.py
--rwxr-xr-x   0        0        0     2052 2020-02-02 00:00:00.000000 pex-2.3.0/scripts/typecheck.py
--rw-r--r--   0        0        0    28315 2020-02-02 00:00:00.000000 pex-2.3.0/testing/__init__.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 pex-2.3.0/testing/build_system.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 pex-2.3.0/testing/cli.py
--rw-r--r--   0        0        0   188335 2020-02-02 00:00:00.000000 pex-2.3.0/testing/devpi-server.lock
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 pex-2.3.0/testing/devpi.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pex-2.3.0/testing/dist_metadata.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 pex-2.3.0/testing/docker.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pex-2.3.0/testing/find_links.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pex-2.3.0/testing/pep_427.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 pex-2.3.0/testing/resolve.py
--rwxr-xr-x   0        0        0     5733 2020-02-02 00:00:00.000000 pex-2.3.0/testing/bin/run_tests.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pex-2.3.0/testing/data/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/testing/data/locks/__init__.py
--rw-r--r--   0        0        0    74149 2020-02-02 00:00:00.000000 pex-2.3.0/testing/data/locks/mitmproxy.lock.json
--rw-r--r--   0        0        0    32794 2020-02-02 00:00:00.000000 pex-2.3.0/testing/data/locks/requests.lock.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/testing/data/platforms/__init__.py
--rw-r--r--   0        0        0    27259 2020-02-02 00:00:00.000000 pex-2.3.0/testing/data/platforms/macosx_10_13_x86_64-cp-36-m.tags.txt
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pex-2.3.0/tests/conftest.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_atomic_directory.py
--rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_bdist_pex.py
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_common.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_compatibility.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_compiler.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_dependency_manager.py
--rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_dist_metadata.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_enum.py
--rw-r--r--   0        0        0    18758 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_environment.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_execution_mode.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_executor.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_fetcher.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_finders.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_hashing.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_inherits_path_option.py
--rw-r--r--   0        0        0    21742 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_interpreter.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_interpreter_constraints.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_jobs.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_packaging.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pep_376.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pep_425.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pep_508.py
--rw-r--r--   0        0        0    35048 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pex.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pex_binary.py
--rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pex_bootstrapper.py
--rw-r--r--   0        0        0    19744 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pex_builder.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pex_info.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pex_warnings.py
--rw-r--r--   0        0        0    13412 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pip.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_platform.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pth.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_pyvenv_cfg.py
--rw-r--r--   0        0        0    21280 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_requirements.py
--rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_resolver.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_sorted_tuple.py
--rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_targets.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_third_party.py
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_util.py
--rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_variables.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_vendor.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 pex-2.3.0/tests/test_zip_utils.py
--rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 pex-2.3.0/tests/bin/test_sh_boot.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pex-2.3.0/tests/build_system/test_issue_2125.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 pex-2.3.0/tests/build_system/test_pep_517.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 pex-2.3.0/tests/build_system/test_pep_518.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 pex-2.3.0/tests/commands/test_command.py
--rw-r--r--   0        0        0    25660 2020-02-02 00:00:00.000000 pex-2.3.0/tests/example_packages/MarkupSafe-1.0-cp27-cp27mu-linux_x86_64.whl
--rw-r--r--   0        0        0    32074 2020-02-02 00:00:00.000000 pex-2.3.0/tests/example_packages/PyAthena-1.11.5-py2.py3-none-any.whl
--rw-r--r--   0        0        0    37477 2020-02-02 00:00:00.000000 pex-2.3.0/tests/example_packages/PyAthena-1.9.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   983623 2020-02-02 00:00:00.000000 pex-2.3.0/tests/example_packages/aws_cfn_bootstrap-1.4-py2-none-any.whl
--rw-r--r--   0        0        0    56975 2020-02-02 00:00:00.000000 pex-2.3.0/tests/example_packages/pyparsing-2.1.10-py2.py3-none-any.whl
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_downloads.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_excludes.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_executuon_mode_venv.py
--rw-r--r--   0        0        0     9769 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_inject_env_and_args.py
--rw-r--r--   0        0        0    70470 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_integration.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_interpreter.py
--rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_interpreter_selection.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1017.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1018.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1025.py
--rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1031.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1179.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1201.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1202.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1218.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1225.py
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1232.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1302.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1316.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1336.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1422.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1447.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1479.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1520.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1537.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1540.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1550.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1560.py
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1597.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1598.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1656.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1683.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1726.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1730.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1802.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1809.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1817.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1825.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1856.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1861.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1870.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1872.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1879.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1933.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1936.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1949.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_1995.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2001.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2006.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2023.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2038.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2073.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2087.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2088.py
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2134.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2183.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2186.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2203.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2235.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2324.py
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2343.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2348.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2355.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2389.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2391.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_2739.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_434.py
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_539.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_598.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_661.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_729.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_736.py
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_745.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_749.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_898.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_899.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_940.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_issue_996.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_layout.py
--rw-r--r--   0        0        0    18513 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_lock_resolver.py
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_locked_resolve.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_no_pre_install_wheels.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_pep_427.py
--rw-r--r--   0        0        0    15453 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_pex_bootstrapper.py
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_pex_entry_points.py
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_pex_import.py
--rw-r--r--   0        0        0     7528 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_reexec.py
--rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_reproducible.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_setproctitle.py
--rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_sh_boot.py
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_shebang_length_limit.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/test_variables.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/build_system/__init__.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/build_system/test_issue_2063.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/build_system/test_issue_2125.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/build_system/test_pep_517.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/build_system/test_pep_518.py
--rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_export.py
--rw-r--r--   0        0        0    28994 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_export_subset.lock.json
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_export_subset.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_interpreter_inspect.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_1413.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_1665.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_1667.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_1688.py
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_1711.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_1734.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_1741.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_1801.py
--rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_1821.py
--rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_2050.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_2057.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_2059.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_2098.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_2211.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_issue_2268.py
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_local_project_lock.py
--rw-r--r--   0        0        0    75942 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_lock.py
--rw-r--r--   0        0        0    11780 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_lock_resolve_auth.py
--rw-r--r--   0        0        0    44293 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_lock_sync.py
--rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_lock_update.py
--rw-r--r--   0        0        0    14794 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_lock_update_issues_2332_2334.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_vcs_lock.py
--rw-r--r--   0        0        0    14349 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_venv_create.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/cli/commands/test_venv_inspect.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/resolve/__init__.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/resolve/test_issue_1918.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/resolve/test_issue_2092.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/resolve/pep_691/__init__.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/resolve/pep_691/test_api.py
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/tools/commands/test_issue_2105.py
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/tools/commands/test_venv.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/conftest.py
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_install_wheel_multiple_site_packages_dirs.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_issue_1630.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_issue_1637.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_issue_1641.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_issue_1668.py
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_issue_1745.py
--rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_issue_2065.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_issue_2160.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_issue_2248.py
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 pex-2.3.0/tests/integration/venv_ITs/test_virtualenv.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 pex-2.3.0/tests/pip/test_tailer.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pex-2.3.0/tests/pip/test_version.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/conftest.py
--rw-r--r--   0        0        0    33531 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/test_locked_resolve.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/test_locker.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/test_path_mappings.py
--rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/test_pex_repository_resolver.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/test_resolved_requirement.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/test_resolver_options.py
--rw-r--r--   0        0        0    19764 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/test_target_options.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/lockfile/__init__.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/lockfile/test_download_manager.py
--rw-r--r--   0        0        0    18814 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/lockfile/test_json_codec.py
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/lockfile/test_lockfile.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/pep_691/__init__.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/pep_691/test_api.py
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/pep_691/test_fingerprint_service.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 pex-2.3.0/tests/resolve/pep_691/test_model.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/tools/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.0/tests/tools/commands/__init__.py
--rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 pex-2.3.0/tests/tools/commands/test_interpreter_command.py
--rw-r--r--   0        0        0     9683 2020-02-02 00:00:00.000000 pex-2.3.0/tests/tools/commands/test_repository.py
--rw-r--r--   0        0        0    27931 2020-02-02 00:00:00.000000 pex-2.3.0/tests/tools/commands/test_venv.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pex-2.3.0/.gitignore
--rw-r--r--   0        0        0    11323 2020-02-02 00:00:00.000000 pex-2.3.0/LICENSE
--rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 pex-2.3.0/README.rst
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pex-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 pex-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0   104036 2020-02-02 00:00:00.000000 pex-2.3.1/CHANGES.md
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 pex-2.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pex-2.3.1/RELEASE.rst
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pex-2.3.1/docs-requirements.txt
+-rwxr-xr-x   0        0        0     3366 2020-02-02 00:00:00.000000 pex-2.3.1/dtox.sh
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pex-2.3.1/mypy.ini
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 pex-2.3.1/tox.ini
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pex-2.3.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0     8388 2020-02-02 00:00:00.000000 pex-2.3.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pex-2.3.1/.github/workflows/doc-site.yml
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 pex-2.3.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pex-2.3.1/assets/download.svg
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pex-2.3.1/assets/github.svg
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pex-2.3.1/assets/pdf.svg
+-rw-r--r--   0        0        0    25424 2020-02-02 00:00:00.000000 pex-2.3.1/assets/pex-icon-512.png
+-rw-r--r--   0        0        0    25312 2020-02-02 00:00:00.000000 pex-2.3.1/assets/pex-icon-512x512.png
+-rw-r--r--   0        0        0    34315 2020-02-02 00:00:00.000000 pex-2.3.1/assets/pex-logo-dark.png
+-rw-r--r--   0        0        0    35372 2020-02-02 00:00:00.000000 pex-2.3.1/assets/pex-logo-light.png
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 pex-2.3.1/assets/pex.svg
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pex-2.3.1/assets/python.svg
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pex-2.3.1/build-backend/pex_build/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/build-backend/pex_build/hatchling/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 pex-2.3.1/build-backend/pex_build/hatchling/build.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pex-2.3.1/build-backend/pex_build/hatchling/build_hook.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pex-2.3.1/build-backend/pex_build/hatchling/hooks.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 pex-2.3.1/build-backend/pex_build/hatchling/metadata_hook.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pex-2.3.1/build-backend/pex_build.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 pex-2.3.1/docker/base/Dockerfile
+-rwxr-xr-x   0        0        0     1190 2020-02-02 00:00:00.000000 pex-2.3.1/docker/base/install_pythons.sh
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 pex-2.3.1/docker/cache/Dockerfile
+-rwxr-xr-x   0        0        0      822 2020-02-02 00:00:00.000000 pex-2.3.1/docker/cache/populate_cache.sh
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 pex-2.3.1/docker/user/Dockerfile
+-rwxr-xr-x   0        0        0      372 2020-02-02 00:00:00.000000 pex-2.3.1/docker/user/create_docker_image_user.sh
+-rw-r--r--   0        0        0    18698 2020-02-02 00:00:00.000000 pex-2.3.1/docs/buildingpex.rst
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 pex-2.3.1/docs/conf.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 pex-2.3.1/docs/index.rst
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 pex-2.3.1/docs/recipes.rst
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pex-2.3.1/docs/whatispex.rst
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 pex-2.3.1/docs/_ext/sphinx_pex/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 pex-2.3.1/docs/_ext/sphinx_pex/vars.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/docs/_static/pex-icon.png -> ../../assets/pex-icon-512.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/docs/_static/pex-logo-dark.png -> ../../assets/pex-logo-dark.png
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/docs/_static/pex-logo-light.png -> ../../assets/pex-logo-light.png
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pex-2.3.1/docs/_templates/search.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pex-2.3.1/docs/api/vars.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/__init__.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pex-2.3.1/pex/__main__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pex-2.3.1/pex/argparse.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pex-2.3.1/pex/asserts.py
+-rw-r--r--   0        0        0    12917 2020-02-02 00:00:00.000000 pex-2.3.1/pex/atomic_directory.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pex-2.3.1/pex/attrs.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 pex-2.3.1/pex/auth.py
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 pex-2.3.1/pex/bootstrap.py
+-rw-r--r--   0        0        0    28253 2020-02-02 00:00:00.000000 pex-2.3.1/pex/common.py
+-rw-r--r--   0        0        0     8734 2020-02-02 00:00:00.000000 pex-2.3.1/pex/compatibility.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 pex-2.3.1/pex/compiler.py
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 pex-2.3.1/pex/dependency_manager.py
+-rw-r--r--   0        0        0    39146 2020-02-02 00:00:00.000000 pex-2.3.1/pex/dist_metadata.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 pex-2.3.1/pex/enum.py
+-rw-r--r--   0        0        0    33997 2020-02-02 00:00:00.000000 pex-2.3.1/pex/environment.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 pex-2.3.1/pex/exclude_configuration.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 pex-2.3.1/pex/executor.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 pex-2.3.1/pex/fetcher.py
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 pex-2.3.1/pex/finders.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pex-2.3.1/pex/fingerprinted_distribution.py
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 pex-2.3.1/pex/hashing.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 pex-2.3.1/pex/inherit_path.py
+-rw-r--r--   0        0        0    62887 2020-02-02 00:00:00.000000 pex-2.3.1/pex/interpreter.py
+-rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 pex-2.3.1/pex/interpreter_constraints.py
+-rw-r--r--   0        0        0    27970 2020-02-02 00:00:00.000000 pex-2.3.1/pex/jobs.py
+-rw-r--r--   0        0        0    21690 2020-02-02 00:00:00.000000 pex-2.3.1/pex/layout.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 pex-2.3.1/pex/network_configuration.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 pex-2.3.1/pex/orderedset.py
+-rw-r--r--   0        0        0    18333 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pep_376.py
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pep_425.py
+-rw-r--r--   0        0        0    11944 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pep_427.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pep_440.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pep_503.py
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pep_508.py
+-rw-r--r--   0        0        0    34423 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pex.py
+-rw-r--r--   0        0        0    29527 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pex_bootstrapper.py
+-rw-r--r--   0        0        0    35644 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pex_builder.py
+-rw-r--r--   0        0        0    21630 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pex_info.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pex_warnings.py
+-rw-r--r--   0        0        0    13748 2020-02-02 00:00:00.000000 pex-2.3.1/pex/platforms.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pth.py
+-rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pyenv.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 pex-2.3.1/pex/rank.py
+-rw-r--r--   0        0        0    25077 2020-02-02 00:00:00.000000 pex-2.3.1/pex/requirements.py
+-rw-r--r--   0        0        0    58885 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolver.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pex-2.3.1/pex/result.py
+-rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 pex-2.3.1/pex/sh_boot.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 pex-2.3.1/pex/sorted_tuple.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 pex-2.3.1/pex/targets.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tracer.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 pex-2.3.1/pex/typing.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 pex-2.3.1/pex/util.py
+-rw-r--r--   0        0        0    33969 2020-02-02 00:00:00.000000 pex-2.3.1/pex/variables.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pex-2.3.1/pex/version.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 pex-2.3.1/pex/wheel.py
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 pex-2.3.1/pex/ziputils.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/bin/__init__.py
+-rwxr-xr-x   0        0        0    43108 2020-02-02 00:00:00.000000 pex-2.3.1/pex/bin/pex.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pex-2.3.1/pex/build_system/__init__.py
+-rw-r--r--   0        0        0     9917 2020-02-02 00:00:00.000000 pex-2.3.1/pex/build_system/pep_517.py
+-rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 pex-2.3.1/pex/build_system/pep_518.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/cli/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 pex-2.3.1/pex/cli/__main__.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 pex-2.3.1/pex/cli/command.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pex-2.3.1/pex/cli/pex.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 pex-2.3.1/pex/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 pex-2.3.1/pex/cli/commands/docs.py
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 pex-2.3.1/pex/cli/commands/interpreter.py
+-rw-r--r--   0        0        0    68920 2020-02-02 00:00:00.000000 pex-2.3.1/pex/cli/commands/lock.py
+-rw-r--r--   0        0        0    16628 2020-02-02 00:00:00.000000 pex-2.3.1/pex/cli/commands/venv.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/commands/__init__.py
+-rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 pex-2.3.1/pex/commands/command.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/distutils/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/distutils/commands/__init__.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 pex-2.3.1/pex/distutils/commands/bdist_pex.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pex-2.3.1/pex/docs/__init__.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pex-2.3.1/pex/docs/command.py
+-rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 pex-2.3.1/pex/docs/server.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/__init__.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/download_observer.py
+-rw-r--r--   0        0        0    11030 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/installation.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/local_project.py
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/log_analyzer.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/tailer.py
+-rw-r--r--   0        0        0    28069 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/tool.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/vcs.py
+-rw-r--r--   0        0        0     9574 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/version.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/foreign_platform/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/foreign_platform/markers.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/foreign_platform/requires_python.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pex-2.3.1/pex/pip/foreign_platform/tags.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/__init__.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/config.py
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/configured_resolve.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/configured_resolver.py
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/downloads.py
+-rw-r--r--   0        0        0    19473 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/lock_resolver.py
+-rw-r--r--   0        0        0    32283 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/locked_resolve.py
+-rw-r--r--   0        0        0    24303 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/locker.py
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/locker_patches.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/path_mappings.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/pex_repository_resolver.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/requirement_configuration.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/requirement_options.py
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/resolved_requirement.py
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/resolver_configuration.py
+-rw-r--r--   0        0        0    25682 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/resolver_options.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/resolvers.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/target_configuration.py
+-rw-r--r--   0        0        0    11066 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/target_options.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/lockfile/__init__.py
+-rw-r--r--   0        0        0    20415 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/lockfile/create.py
+-rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/lockfile/download_manager.py
+-rw-r--r--   0        0        0    16083 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/lockfile/json_codec.py
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/lockfile/model.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/lockfile/subset.py
+-rw-r--r--   0        0        0    30824 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/lockfile/updater.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/pep_691/__init__.py
+-rw-r--r--   0        0        0     8950 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/pep_691/api.py
+-rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/pep_691/fingerprint_service.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 pex-2.3.1/pex/resolve/pep_691/model.py
+-rw-r--r--   0        0        0    25318 2020-02-02 00:00:00.000000 pex-2.3.1/pex/third_party/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/__main__.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/command.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/main.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/commands/__init__.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/commands/digraph.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/commands/graph.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/commands/info.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/commands/interpreter.py
+-rw-r--r--   0        0        0    17057 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/commands/repository.py
+-rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 pex-2.3.1/pex/tools/commands/venv.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/README.md
+-rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/__init__.py
+-rw-r--r--   0        0        0    18350 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/__init__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/.layout.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/__init__.py
+-rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/__init__.pyi
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/_cmp.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/_cmp.pyi
+-rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/_compat.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/_config.py
+-rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/_funcs.py
+-rw-r--r--   0        0        0   102691 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/_make.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/_next_gen.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/_version_info.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/_version_info.pyi
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/converters.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/converters.pyi
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/exceptions.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/exceptions.pyi
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/filters.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/filters.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/py.typed
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/setters.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/setters.pyi
+-rw-r--r--   0        0        0    15966 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/validators.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attr/validators.pyi
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs/__init__.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs/__init__.pyi
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs/converters.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs/exceptions.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs/filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs/py.typed
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs/setters.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs/validators.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/AUTHORS.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/LICENSE
+-rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/WHEEL
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/.layout.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/constraints.txt
+-rw-r--r--   0        0        0   273365 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/pyparsing.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/_structures.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/_typing.py
+-rw-r--r--   0        0        0     9741 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/py.typed
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/requirements.py
+-rw-r--r--   0        0        0    32208 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/specifiers.py
+-rw-r--r--   0        0        0    29561 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/tags.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/utils.py
+-rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0    13299 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/WHEEL
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/WHEEL
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/top_level.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/.layout.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/constraints.txt
+-rw-r--r--   0        0        0   273365 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/pyparsing.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/_structures.py
+-rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/markers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/py.typed
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0    15147 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/METADATA
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/WHEEL
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/top_level.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/WHEEL
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/top_level.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/.layout.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/constraints.txt
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/py.typed
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/METADATA
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/.layout.json
+-rwxr-xr-x   0        0        0      383 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/.prefix/bin/pip
+-rwxr-xr-x   0        0        0      383 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/.prefix/bin/pip3
+-rwxr-xr-x   0        0        0      383 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/.prefix/bin/pip3.8
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/__init__.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/__main__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/__init__.py
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    12249 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13904 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/locations.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/main.py
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    11816 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     9337 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    28618 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10388 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    16455 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     7315 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0    27410 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    11519 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    22070 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37454 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4751 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    11652 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     8121 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    15449 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0    10411 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    22460 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0        0        0    31247 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16135 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    18594 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    33420 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     7887 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_tracker.py
+-rw-r--r--   0        0        0    23771 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    18234 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    20035 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    18946 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11634 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    28047 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/parallel.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/pkg_resources.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/typing.py
+-rw-r--r--   0        0        0     9488 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    15599 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5564 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    12558 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    23767 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    25907 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/appdirs.py
+-rw-r--r--   0        0        0    16915 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/contextlib2.py
+-rw-r--r--   0        0        0    43628 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distro.py
+-rw-r--r--   0        0        0    79875 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/ipaddress.py
+-rw-r--r--   0        0        0   273394 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pyparsing.py
+-rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/retrying.py
+-rw-r--r--   0        0        0    34159 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/six.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    14149 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   281608 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31254 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0     9411 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/compat.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    31621 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20715 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25777 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    19643 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0    12839 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    17948 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langcyrillicmodel.py
+-rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    25481 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    12485 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41408 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51059 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    21066 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    52100 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    38962 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    17180 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    96768 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0        0        0   105984 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    59845 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23391 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    90112 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0        0        0    99840 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    41144 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/__init__.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/misc.py
+-rw-r--r--   0        0        0    25707 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/shutil.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/sysconfig.cfg
+-rw-r--r--   0        0        0    26854 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/sysconfig.py
+-rw-r--r--   0        0        0    92628 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/tarfile.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/__init__.py
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_ihatexml.py
+-rw-r--r--   0        0        0    32353 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_inputstream.py
+-rw-r--r--   0        0        0    77040 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_tokenizer.py
+-rw-r--r--   0        0        0     4931 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_utils.py
+-rw-r--r--   0        0        0    83464 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/constants.py
+-rw-r--r--   0        0        0   117186 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/html5parser.py
+-rw-r--r--   0        0        0    15759 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/serializer.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/_base.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/py.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/base.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/lint.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/optionaltags.py
+-rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/sanitizer.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/whitespace.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/__init__.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/genshi.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/sax.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/base.py
+-rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/dom.py
+-rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/etree.py
+-rw-r--r--   0        0        0    14766 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/__init__.py
+-rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/dom.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/etree.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/genshi.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    42350 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   202084 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/msgpack/_version.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    37133 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/_typing.py
+-rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    32208 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    29561 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/__init__.py
+-rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/_in_process.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/build.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/check.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/colorlog.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/compat.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/dirtools.py
+-rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/envbuild.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/meta.py
+-rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/wrappers.py
+-rw-r--r--   0        0        0   108277 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/progress/__init__.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/progress/bar.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/progress/counter.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/progress/spinner.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21548 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18430 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    34373 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30135 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    30355 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    16538 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/toml/__init__.py
+-rw-r--r--   0        0        0    38954 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/toml/decoder.py
+-rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/toml/encoder.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/toml/ordered.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/toml/tz.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    37133 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19763 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    28203 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    16795 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34303 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17649 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13908 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    32536 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    21366 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    16281 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    13981 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/top_level.txt
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/.layout.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/__init__.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/easy_install.py
+-rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/.prefix/bin/easy_install
+-rwxr-xr-x   0        0        0      392 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/.prefix/bin/easy_install-3.8
+-rw-r--r--   0        0        0   109513 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/__init__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0        0        0   232055 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/pyparsing.py
+-rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/six.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    28025 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0     8157 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_deprecation_warning.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_imp.py
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/archive_util.py
+-rw-r--r--   0        0        0    10153 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/build_meta.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/cli-32.exe
+-rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/cli-64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/cli.exe
+-rw-r--r--   0        0        0    21571 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/config.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/depends.py
+-rw-r--r--   0        0        0    51749 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/dist.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/errors.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/extension.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/glob.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/gui-32.exe
+-rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/gui-64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/gui.exe
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/installer.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/launch.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/lib2to3_ex.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/monkey.py
+-rw-r--r--   0        0        0    47209 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/msvc.py
+-rw-r--r--   0        0        0     3338 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/namespaces.py
+-rw-r--r--   0        0        0    42090 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/package_index.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/py27compat.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/py31compat.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/py33compat.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/py34compat.py
+-rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/script.tmpl
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/site-patch.py
+-rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/ssl_support.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/version.py
+-rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/wheel.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/windows_support.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0   232055 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/pyparsing.py
+-rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/six.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    27778 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    12933 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/alias.py
+-rw-r--r--   0        0        0    18880 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/bdist_wininst.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    13284 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0    10036 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/develop.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    90093 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    27330 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/install.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/register.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/setopt.py
+-rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/test.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/LICENSE
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/WHEEL
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/dependency_links.txt
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/top_level.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/zip-safe
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/.layout.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/__init__.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/constraints.txt
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml/__init__.py
+-rw-r--r--   0        0        0    39064 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml/decoder.py
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml/encoder.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml/ordered.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml/tz.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/METADATA
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/WHEEL
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pex-2.3.1/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pex-2.3.1/pex/venv/README.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/pex/venv/__init__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 pex-2.3.1/pex/venv/bin_path.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 pex-2.3.1/pex/venv/install_scope.py
+-rw-r--r--   0        0        0    37346 2020-02-02 00:00:00.000000 pex-2.3.1/pex/venv/installer.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 pex-2.3.1/pex/venv/installer_configuration.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 pex-2.3.1/pex/venv/installer_options.py
+-rw-r--r--   0        0        0    19086 2020-02-02 00:00:00.000000 pex-2.3.1/pex/venv/virtualenv.py
+-rw-r--r--   0        0        0   106996 2020-02-02 00:00:00.000000 pex-2.3.1/pex/venv/virtualenv_16.7.12_py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 pex-2.3.1/scripts/build_cache_image.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 pex-2.3.1/scripts/build_docs.py
+-rwxr-xr-x   0        0        0      919 2020-02-02 00:00:00.000000 pex-2.3.1/scripts/embed_virtualenv.py
+-rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 pex-2.3.1/scripts/format.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pex-2.3.1/scripts/lint.py
+-rwxr-xr-x   0        0        0     6874 2020-02-02 00:00:00.000000 pex-2.3.1/scripts/package.py
+-rwxr-xr-x   0        0        0     2052 2020-02-02 00:00:00.000000 pex-2.3.1/scripts/typecheck.py
+-rw-r--r--   0        0        0    28315 2020-02-02 00:00:00.000000 pex-2.3.1/testing/__init__.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 pex-2.3.1/testing/build_system.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 pex-2.3.1/testing/cli.py
+-rw-r--r--   0        0        0   188335 2020-02-02 00:00:00.000000 pex-2.3.1/testing/devpi-server.lock
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 pex-2.3.1/testing/devpi.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pex-2.3.1/testing/dist_metadata.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 pex-2.3.1/testing/docker.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 pex-2.3.1/testing/find_links.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pex-2.3.1/testing/pep_427.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 pex-2.3.1/testing/resolve.py
+-rwxr-xr-x   0        0        0     5733 2020-02-02 00:00:00.000000 pex-2.3.1/testing/bin/run_tests.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 pex-2.3.1/testing/data/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/testing/data/locks/__init__.py
+-rw-r--r--   0        0        0    74149 2020-02-02 00:00:00.000000 pex-2.3.1/testing/data/locks/mitmproxy.lock.json
+-rw-r--r--   0        0        0    32794 2020-02-02 00:00:00.000000 pex-2.3.1/testing/data/locks/requests.lock.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/testing/data/platforms/__init__.py
+-rw-r--r--   0        0        0    34707 2020-02-02 00:00:00.000000 pex-2.3.1/testing/data/platforms/complete_platform_linux_x86-64_py11.json
+-rw-r--r--   0        0        0    27259 2020-02-02 00:00:00.000000 pex-2.3.1/testing/data/platforms/macosx_10_13_x86_64-cp-36-m.tags.txt
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 pex-2.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_atomic_directory.py
+-rw-r--r--   0        0        0     7969 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_bdist_pex.py
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_common.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_compatibility.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_compiler.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_dependency_manager.py
+-rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_dist_metadata.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_enum.py
+-rw-r--r--   0        0        0    18758 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_environment.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_execution_mode.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_executor.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_fetcher.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_finders.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_hashing.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_inherits_path_option.py
+-rw-r--r--   0        0        0    21742 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_interpreter.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_interpreter_constraints.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_jobs.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_packaging.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pep_376.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pep_425.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pep_508.py
+-rw-r--r--   0        0        0    35048 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pex.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pex_binary.py
+-rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pex_bootstrapper.py
+-rw-r--r--   0        0        0    19744 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pex_builder.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pex_info.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pex_warnings.py
+-rw-r--r--   0        0        0    13412 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pip.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_platform.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pth.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_pyvenv_cfg.py
+-rw-r--r--   0        0        0    21280 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_requirements.py
+-rw-r--r--   0        0        0    24256 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_resolver.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_sorted_tuple.py
+-rw-r--r--   0        0        0    11798 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_targets.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_third_party.py
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_util.py
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_variables.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_vendor.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 pex-2.3.1/tests/test_zip_utils.py
+-rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 pex-2.3.1/tests/bin/test_sh_boot.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pex-2.3.1/tests/build_system/test_issue_2125.py
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 pex-2.3.1/tests/build_system/test_pep_517.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 pex-2.3.1/tests/build_system/test_pep_518.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 pex-2.3.1/tests/commands/test_command.py
+-rw-r--r--   0        0        0    25660 2020-02-02 00:00:00.000000 pex-2.3.1/tests/example_packages/MarkupSafe-1.0-cp27-cp27mu-linux_x86_64.whl
+-rw-r--r--   0        0        0    32074 2020-02-02 00:00:00.000000 pex-2.3.1/tests/example_packages/PyAthena-1.11.5-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    37477 2020-02-02 00:00:00.000000 pex-2.3.1/tests/example_packages/PyAthena-1.9.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   983623 2020-02-02 00:00:00.000000 pex-2.3.1/tests/example_packages/aws_cfn_bootstrap-1.4-py2-none-any.whl
+-rw-r--r--   0        0        0    56975 2020-02-02 00:00:00.000000 pex-2.3.1/tests/example_packages/pyparsing-2.1.10-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_downloads.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_excludes.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_executuon_mode_venv.py
+-rw-r--r--   0        0        0     9769 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_inject_env_and_args.py
+-rw-r--r--   0        0        0    70470 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_integration.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_interpreter.py
+-rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_interpreter_selection.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1017.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1018.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1025.py
+-rw-r--r--   0        0        0     3750 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1031.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1179.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1201.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1202.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1218.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1225.py
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1232.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1302.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1316.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1336.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1422.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1447.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1479.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1520.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1537.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1540.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1550.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1560.py
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1597.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1598.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1656.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1683.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1726.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1730.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1802.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1809.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1817.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1825.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1856.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1861.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1870.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1872.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1879.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1933.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1936.py
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1949.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_1995.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2001.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2006.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2023.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2038.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2073.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2087.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2088.py
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2134.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2183.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2186.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2203.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2235.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2324.py
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2343.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2348.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2355.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2389.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2391.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2395.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_2739.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_434.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_539.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_598.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_661.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_729.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_736.py
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_745.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_749.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_898.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_899.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_940.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_issue_996.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_layout.py
+-rw-r--r--   0        0        0    18513 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_lock_resolver.py
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_locked_resolve.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_no_pre_install_wheels.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_pep_427.py
+-rw-r--r--   0        0        0    15453 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_pex_bootstrapper.py
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_pex_entry_points.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_pex_import.py
+-rw-r--r--   0        0        0     7528 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_reexec.py
+-rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_reproducible.py
+-rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_setproctitle.py
+-rw-r--r--   0        0        0     7709 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_sh_boot.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_shebang_length_limit.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/test_variables.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/build_system/__init__.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/build_system/test_issue_2063.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/build_system/test_issue_2125.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/build_system/test_pep_517.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/build_system/test_pep_518.py
+-rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_export.py
+-rw-r--r--   0        0        0    28994 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_export_subset.lock.json
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_export_subset.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_interpreter_inspect.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_1413.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_1665.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_1667.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_1688.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_1711.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_1734.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_1741.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_1801.py
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_1821.py
+-rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_2050.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_2057.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_2059.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_2098.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_2211.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_issue_2268.py
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_local_project_lock.py
+-rw-r--r--   0        0        0    75942 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_lock.py
+-rw-r--r--   0        0        0    11780 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_lock_resolve_auth.py
+-rw-r--r--   0        0        0    44293 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_lock_sync.py
+-rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_lock_update.py
+-rw-r--r--   0        0        0    14794 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_lock_update_issues_2332_2334.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_vcs_lock.py
+-rw-r--r--   0        0        0    14349 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_venv_create.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/cli/commands/test_venv_inspect.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/resolve/__init__.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/resolve/test_issue_1918.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/resolve/test_issue_2092.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/resolve/pep_691/__init__.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/resolve/pep_691/test_api.py
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/tools/commands/test_issue_2105.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/tools/commands/test_venv.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/conftest.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_install_wheel_multiple_site_packages_dirs.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_issue_1630.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_issue_1637.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_issue_1641.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_issue_1668.py
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_issue_1745.py
+-rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_issue_2065.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_issue_2160.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_issue_2248.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 pex-2.3.1/tests/integration/venv_ITs/test_virtualenv.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 pex-2.3.1/tests/pip/test_tailer.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pex-2.3.1/tests/pip/test_version.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/__init__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/conftest.py
+-rw-r--r--   0        0        0    33531 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/test_locked_resolve.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/test_locker.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/test_path_mappings.py
+-rw-r--r--   0        0        0    13570 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/test_pex_repository_resolver.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/test_resolved_requirement.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/test_resolver_options.py
+-rw-r--r--   0        0        0    19764 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/test_target_options.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/lockfile/__init__.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/lockfile/test_download_manager.py
+-rw-r--r--   0        0        0    18814 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/lockfile/test_json_codec.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/lockfile/test_lockfile.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/pep_691/__init__.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/pep_691/test_api.py
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/pep_691/test_fingerprint_service.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 pex-2.3.1/tests/resolve/pep_691/test_model.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/tools/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pex-2.3.1/tests/tools/commands/__init__.py
+-rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 pex-2.3.1/tests/tools/commands/test_interpreter_command.py
+-rw-r--r--   0        0        0     9683 2020-02-02 00:00:00.000000 pex-2.3.1/tests/tools/commands/test_repository.py
+-rw-r--r--   0        0        0    27931 2020-02-02 00:00:00.000000 pex-2.3.1/tests/tools/commands/test_venv.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pex-2.3.1/.gitignore
+-rw-r--r--   0        0        0    11323 2020-02-02 00:00:00.000000 pex-2.3.1/LICENSE
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 pex-2.3.1/README.rst
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 pex-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 pex-2.3.1/PKG-INFO
```

### Comparing `pex-2.3.0/CHANGES.md` & `pex-2.3.1/CHANGES.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Release Notes
 
+## 2.3.1
+
+This release fixes Pex to respect lock file interpreter constraints and
+target systems when downloading artifacts.
+
+* Fix lock downloads to use all lock info. (#2396)
+
 ## 2.3.0
 
 This release introduces `pex3 lock sync` as a higher-level tool that
 can be used to create and maintain a lock as opposed to using a
 combination of `pex3 lock create` and `pex3 lock update`. When there is
 no existing lock file, `pex3 lock sync --lock lock.json ...` is
 equivalent to `pex3 lock create --output lock.json ...`, it creates a
```

### Comparing `pex-2.3.0/CONTRIBUTING.md` & `pex-2.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/RELEASE.rst` & `pex-2.3.1/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/dtox.sh` & `pex-2.3.1/dtox.sh`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/mypy.ini` & `pex-2.3.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tox.ini` & `pex-2.3.1/tox.ini`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/.github/workflows/ci.yml` & `pex-2.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/.github/workflows/doc-site.yml` & `pex-2.3.1/.github/workflows/doc-site.yml`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/.github/workflows/release.yml` & `pex-2.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/assets/download.svg` & `pex-2.3.1/assets/download.svg`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/assets/github.svg` & `pex-2.3.1/assets/github.svg`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/assets/pdf.svg` & `pex-2.3.1/assets/pdf.svg`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/assets/pex-icon-512.png` & `pex-2.3.1/assets/pex-icon-512.png`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/assets/pex-icon-512x512.png` & `pex-2.3.1/assets/pex-icon-512x512.png`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/assets/pex-logo-dark.png` & `pex-2.3.1/assets/pex-logo-dark.png`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/assets/pex-logo-light.png` & `pex-2.3.1/assets/pex-logo-light.png`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/assets/pex.svg` & `pex-2.3.1/assets/pex.svg`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/assets/python.svg` & `pex-2.3.1/assets/python.svg`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/build-backend/pex_build/hatchling/build.py` & `pex-2.3.1/build-backend/pex_build/hatchling/build.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/build-backend/pex_build/hatchling/build_hook.py` & `pex-2.3.1/build-backend/pex_build/hatchling/build_hook.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/build-backend/pex_build/hatchling/hooks.py` & `pex-2.3.1/build-backend/pex_build/hatchling/hooks.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/build-backend/pex_build/hatchling/metadata_hook.py` & `pex-2.3.1/build-backend/pex_build/hatchling/metadata_hook.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docker/base/Dockerfile` & `pex-2.3.1/docker/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docker/base/install_pythons.sh` & `pex-2.3.1/docker/base/install_pythons.sh`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docker/cache/Dockerfile` & `pex-2.3.1/docker/cache/Dockerfile`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docker/cache/populate_cache.sh` & `pex-2.3.1/docker/cache/populate_cache.sh`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docker/user/Dockerfile` & `pex-2.3.1/docker/user/Dockerfile`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docs/buildingpex.rst` & `pex-2.3.1/docs/buildingpex.rst`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docs/conf.py` & `pex-2.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docs/index.rst` & `pex-2.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docs/recipes.rst` & `pex-2.3.1/docs/recipes.rst`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docs/whatispex.rst` & `pex-2.3.1/docs/whatispex.rst`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docs/_ext/sphinx_pex/__init__.py` & `pex-2.3.1/docs/_ext/sphinx_pex/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docs/_ext/sphinx_pex/vars.py` & `pex-2.3.1/docs/_ext/sphinx_pex/vars.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/docs/_templates/search.html` & `pex-2.3.1/docs/_templates/search.html`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/argparse.py` & `pex-2.3.1/pex/argparse.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/asserts.py` & `pex-2.3.1/pex/asserts.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/atomic_directory.py` & `pex-2.3.1/pex/atomic_directory.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/auth.py` & `pex-2.3.1/pex/auth.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/bootstrap.py` & `pex-2.3.1/pex/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/common.py` & `pex-2.3.1/pex/common.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/compatibility.py` & `pex-2.3.1/pex/compatibility.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/compiler.py` & `pex-2.3.1/pex/compiler.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/dependency_manager.py` & `pex-2.3.1/pex/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/dist_metadata.py` & `pex-2.3.1/pex/dist_metadata.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/enum.py` & `pex-2.3.1/pex/enum.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/environment.py` & `pex-2.3.1/pex/environment.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/exclude_configuration.py` & `pex-2.3.1/pex/exclude_configuration.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/executor.py` & `pex-2.3.1/pex/executor.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/fetcher.py` & `pex-2.3.1/pex/fetcher.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/finders.py` & `pex-2.3.1/pex/finders.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/fingerprinted_distribution.py` & `pex-2.3.1/pex/fingerprinted_distribution.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/hashing.py` & `pex-2.3.1/pex/hashing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/inherit_path.py` & `pex-2.3.1/pex/inherit_path.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/interpreter.py` & `pex-2.3.1/pex/interpreter.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/interpreter_constraints.py` & `pex-2.3.1/pex/interpreter_constraints.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/jobs.py` & `pex-2.3.1/pex/jobs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/layout.py` & `pex-2.3.1/pex/layout.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/network_configuration.py` & `pex-2.3.1/pex/network_configuration.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/orderedset.py` & `pex-2.3.1/pex/orderedset.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pep_376.py` & `pex-2.3.1/pex/pep_376.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pep_425.py` & `pex-2.3.1/pex/pep_425.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pep_427.py` & `pex-2.3.1/pex/pep_427.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pep_440.py` & `pex-2.3.1/pex/pep_440.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pep_503.py` & `pex-2.3.1/pex/pep_503.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pep_508.py` & `pex-2.3.1/pex/pep_508.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pex.py` & `pex-2.3.1/pex/pex.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pex_bootstrapper.py` & `pex-2.3.1/pex/pex_bootstrapper.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pex_builder.py` & `pex-2.3.1/pex/pex_builder.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pex_info.py` & `pex-2.3.1/pex/pex_info.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pex_warnings.py` & `pex-2.3.1/pex/pex_warnings.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/platforms.py` & `pex-2.3.1/pex/platforms.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pth.py` & `pex-2.3.1/pex/pth.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pyenv.py` & `pex-2.3.1/pex/pyenv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/rank.py` & `pex-2.3.1/pex/rank.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/requirements.py` & `pex-2.3.1/pex/requirements.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolver.py` & `pex-2.3.1/pex/resolver.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/result.py` & `pex-2.3.1/pex/result.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/sh_boot.py` & `pex-2.3.1/pex/sh_boot.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/sorted_tuple.py` & `pex-2.3.1/pex/sorted_tuple.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/targets.py` & `pex-2.3.1/pex/targets.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/tracer.py` & `pex-2.3.1/pex/tracer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/typing.py` & `pex-2.3.1/pex/typing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/util.py` & `pex-2.3.1/pex/util.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/variables.py` & `pex-2.3.1/pex/variables.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/wheel.py` & `pex-2.3.1/pex/wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/ziputils.py` & `pex-2.3.1/pex/ziputils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/bin/pex.py` & `pex-2.3.1/pex/bin/pex.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/build_system/__init__.py` & `pex-2.3.1/pex/build_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/build_system/pep_517.py` & `pex-2.3.1/pex/build_system/pep_517.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/build_system/pep_518.py` & `pex-2.3.1/pex/build_system/pep_518.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/cli/command.py` & `pex-2.3.1/pex/cli/command.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/cli/pex.py` & `pex-2.3.1/pex/cli/pex.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/cli/commands/__init__.py` & `pex-2.3.1/pex/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/cli/commands/docs.py` & `pex-2.3.1/pex/cli/commands/docs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/cli/commands/interpreter.py` & `pex-2.3.1/pex/cli/commands/interpreter.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/cli/commands/lock.py` & `pex-2.3.1/pex/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/cli/commands/venv.py` & `pex-2.3.1/pex/cli/commands/venv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/commands/command.py` & `pex-2.3.1/pex/commands/command.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/distutils/commands/bdist_pex.py` & `pex-2.3.1/pex/distutils/commands/bdist_pex.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/docs/command.py` & `pex-2.3.1/pex/docs/command.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/docs/server.py` & `pex-2.3.1/pex/docs/server.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/download_observer.py` & `pex-2.3.1/pex/pip/download_observer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/installation.py` & `pex-2.3.1/pex/pip/installation.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/local_project.py` & `pex-2.3.1/pex/pip/local_project.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/log_analyzer.py` & `pex-2.3.1/pex/pip/log_analyzer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/tailer.py` & `pex-2.3.1/pex/pip/tailer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/tool.py` & `pex-2.3.1/pex/pip/tool.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/vcs.py` & `pex-2.3.1/pex/pip/vcs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/version.py` & `pex-2.3.1/pex/pip/version.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/foreign_platform/__init__.py` & `pex-2.3.1/pex/pip/foreign_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/foreign_platform/markers.py` & `pex-2.3.1/pex/pip/foreign_platform/markers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/foreign_platform/requires_python.py` & `pex-2.3.1/pex/pip/foreign_platform/requires_python.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/pip/foreign_platform/tags.py` & `pex-2.3.1/pex/pip/foreign_platform/tags.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/config.py` & `pex-2.3.1/pex/resolve/config.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/configured_resolve.py` & `pex-2.3.1/pex/resolve/configured_resolve.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/configured_resolver.py` & `pex-2.3.1/pex/resolve/configured_resolver.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/downloads.py` & `pex-2.3.1/pex/resolve/downloads.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pex.common import safe_mkdir, safe_mkdtemp
 from pex.hashing import Sha256
 from pex.jobs import Job, Raise, SpawnedJob, execute_parallel
 from pex.pip.download_observer import DownloadObserver
 from pex.pip.installation import get_pip
 from pex.pip.tool import PackageIndexConfiguration, Pip
 from pex.resolve import locker
-from pex.resolve.locked_resolve import Artifact, FileArtifact, LockConfiguration, LockStyle
+from pex.resolve.locked_resolve import Artifact, FileArtifact, LockConfiguration
 from pex.resolve.resolved_requirement import ArtifactURL, Fingerprint, PartialArtifact
 from pex.resolve.resolvers import Resolver
 from pex.result import Error
 from pex.targets import LocalInterpreter, Target
 from pex.typing import TYPE_CHECKING
 from pex.variables import ENV
 
@@ -46,14 +46,15 @@
         _DOWNLOADS_DIRS[root_dir] = downloads_dir
     return downloads_dir
 
 
 @attr.s(frozen=True)
 class ArtifactDownloader(object):
     resolver = attr.ib()  # type: Resolver
+    lock_configuration = attr.ib()  # type: LockConfiguration
     target = attr.ib(factory=LocalInterpreter.create)  # type: Target
     package_index_configuration = attr.ib(
         factory=PackageIndexConfiguration.create
     )  # type: PackageIndexConfiguration
     max_parallel_jobs = attr.ib(default=None)  # type: Optional[int]
     pip = attr.ib(init=False)  # type: Pip
 
@@ -109,15 +110,15 @@
 
         # Although we don't actually need to observe the download, we do need to patch Pip to not
         # care about wheel tags, environment markers or Requires-Python. The locker's download
         # observer does just this for universal locks with no target system or requires python
         # restrictions.
         download_observer = DownloadObserver(
             analyzer=None,
-            patch_set=locker.patch(lock_configuration=LockConfiguration(style=LockStyle.UNIVERSAL)),
+            patch_set=locker.patch(lock_configuration=self.lock_configuration),
         )
         return self.pip.spawn_download_distributions(
             download_dir=download_dir,
             requirements=[download_url],
             transitive=False,
             package_index_configuration=self.package_index_configuration,
             observer=download_observer,
```

### Comparing `pex-2.3.0/pex/resolve/lock_resolver.py` & `pex-2.3.1/pex/resolve/lock_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from pex.pip.vcs import digest_vcs_archive
 from pex.pip.version import PipVersionValue
 from pex.resolve.downloads import ArtifactDownloader
 from pex.resolve.locked_resolve import (
     DownloadableArtifact,
     FileArtifact,
     LocalProjectArtifact,
+    LockConfiguration,
     VCSArtifact,
 )
 from pex.resolve.lockfile.download_manager import DownloadedArtifact, DownloadManager
 from pex.resolve.lockfile.model import Lockfile
 from pex.resolve.lockfile.subset import subset
 from pex.resolve.requirement_configuration import RequirementConfiguration
 from pex.resolve.resolver_configuration import BuildConfiguration, ResolverVersion
@@ -277,14 +278,19 @@
     file_lock_style = FileLockStyle.BSD
 
     file_download_managers_by_target = {
         resolved_subset.target: FileArtifactDownloadManager(
             file_lock_style=file_lock_style,
             downloader=ArtifactDownloader(
                 resolver=resolver,
+                lock_configuration=LockConfiguration(
+                    style=lock.style,
+                    requires_python=lock.requires_python,
+                    target_systems=lock.target_systems,
+                ),
                 target=resolved_subset.target,
                 package_index_configuration=PackageIndexConfiguration.create(
                     pip_version=pip_version,
                     resolver_version=resolver_version,
                     indexes=indexes,
                     find_links=find_links,
                     network_configuration=network_configuration,
```

### Comparing `pex-2.3.0/pex/resolve/locked_resolve.py` & `pex-2.3.1/pex/resolve/locked_resolve.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/locker.py` & `pex-2.3.1/pex/resolve/locker.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/locker_patches.py` & `pex-2.3.1/pex/resolve/locker_patches.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/path_mappings.py` & `pex-2.3.1/pex/resolve/path_mappings.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/pex_repository_resolver.py` & `pex-2.3.1/pex/resolve/pex_repository_resolver.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/requirement_configuration.py` & `pex-2.3.1/pex/resolve/requirement_configuration.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/requirement_options.py` & `pex-2.3.1/pex/resolve/requirement_options.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/resolved_requirement.py` & `pex-2.3.1/pex/resolve/resolved_requirement.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/resolver_configuration.py` & `pex-2.3.1/pex/resolve/resolver_configuration.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/resolver_options.py` & `pex-2.3.1/pex/resolve/resolver_options.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/resolvers.py` & `pex-2.3.1/pex/resolve/resolvers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/target_configuration.py` & `pex-2.3.1/pex/resolve/target_configuration.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/target_options.py` & `pex-2.3.1/pex/resolve/target_options.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/lockfile/create.py` & `pex-2.3.1/pex/resolve/lockfile/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,14 +327,15 @@
 
         return tuple(
             LockedResolve.create(
                 resolved_requirements=resolved_requirements,
                 dist_metadatas=dist_metadatas_by_target[target],
                 fingerprinter=ArtifactDownloader(
                     resolver=self.resolver,
+                    lock_configuration=self.lock_configuration,
                     target=target,
                     package_index_configuration=self.package_index_configuration,
                     max_parallel_jobs=self.max_parallel_jobs,
                 ),
                 platform_tag=None
                 if self.lock_configuration.style == LockStyle.UNIVERSAL
                 else target.platform.tag,
```

### Comparing `pex-2.3.0/pex/resolve/lockfile/download_manager.py` & `pex-2.3.1/pex/resolve/lockfile/download_manager.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/lockfile/json_codec.py` & `pex-2.3.1/pex/resolve/lockfile/json_codec.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/lockfile/model.py` & `pex-2.3.1/pex/resolve/lockfile/model.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/lockfile/subset.py` & `pex-2.3.1/pex/resolve/lockfile/subset.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/lockfile/updater.py` & `pex-2.3.1/pex/resolve/lockfile/updater.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/pep_691/api.py` & `pex-2.3.1/pex/resolve/pep_691/api.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/pep_691/fingerprint_service.py` & `pex-2.3.1/pex/resolve/pep_691/fingerprint_service.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/resolve/pep_691/model.py` & `pex-2.3.1/pex/resolve/pep_691/model.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/third_party/__init__.py` & `pex-2.3.1/pex/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/tools/main.py` & `pex-2.3.1/pex/tools/main.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/tools/commands/__init__.py` & `pex-2.3.1/pex/tools/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/tools/commands/digraph.py` & `pex-2.3.1/pex/tools/commands/digraph.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/tools/commands/graph.py` & `pex-2.3.1/pex/tools/commands/graph.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/tools/commands/info.py` & `pex-2.3.1/pex/tools/commands/info.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/tools/commands/interpreter.py` & `pex-2.3.1/pex/tools/commands/interpreter.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/tools/commands/repository.py` & `pex-2.3.1/pex/tools/commands/repository.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/tools/commands/venv.py` & `pex-2.3.1/pex/tools/commands/venv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/README.md` & `pex-2.3.1/pex/vendor/README.md`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/__init__.py` & `pex-2.3.1/pex/vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/__main__.py` & `pex-2.3.1/pex/vendor/__main__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/__init__.pyi` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/_cmp.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/_cmp.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/_compat.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/_compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/_config.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/_config.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/_funcs.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/_funcs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/_make.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/_make.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/_next_gen.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/_next_gen.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/_version_info.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/_version_info.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/converters.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/converters.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/exceptions.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/exceptions.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/exceptions.pyi` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/filters.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/filters.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/setters.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/setters.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/setters.pyi` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/setters.pyi`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/validators.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/validators.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attr/validators.pyi` & `pex-2.3.1/pex/vendor/_vendored/attrs/attr/validators.pyi`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attrs/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/attrs/attrs/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attrs/__init__.pyi` & `pex-2.3.1/pex/vendor/_vendored/attrs/attrs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/AUTHORS.rst` & `pex-2.3.1/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/LICENSE` & `pex-2.3.1/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/METADATA` & `pex-2.3.1/pex/vendor/_vendored/attrs/attrs-21.5.0.dev0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/pyparsing.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/__about__.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/_compat.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/_structures.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/_typing.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/markers.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/requirements.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/specifiers.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/tags.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/utils.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging/version.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE.APACHE` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE.BSD` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/METADATA` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/packaging-20.9.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/LICENSE` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/METADATA` & `pex-2.3.1/pex/vendor/_vendored/packaging_20_9/pyparsing-2.4.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/pyparsing.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/__about__.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/_manylinux.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/_musllinux.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/_structures.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/markers.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/requirements.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/specifiers.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/tags.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/utils.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging/version.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE.APACHE` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE.BSD` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/METADATA` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/packaging-21.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/LICENSE` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/METADATA` & `pex-2.3.1/pex/vendor/_vendored/packaging_21_3/pyparsing-2.4.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_elffile.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_manylinux.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_musllinux.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_parser.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_structures.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/_tokenizer.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/markers.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/metadata.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/requirements.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/specifiers.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/tags.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/utils.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging/version.py` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE.APACHE` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE.BSD` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/METADATA` & `pex-2.3.1/pex/vendor/_vendored/packaging_23_1/packaging-23.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/__main__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/build_env.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cache.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/configuration.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/exceptions.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/locations.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/locations.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/pyproject.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/self_outdated_check.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/wheel_builder.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/autocompletion.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/base_command.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/cmdoptions.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/command_context.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/main.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/main_parser.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/parser.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/progress_bars.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/req_command.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/cli/spinners.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/cache.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/check.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/completion.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/configuration.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/debug.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/download.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/freeze.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/hash.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/help.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/install.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/list.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/search.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/show.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/uninstall.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/commands/wheel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/base.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/installed.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/sdist.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/distributions/wheel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/index/collector.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/index/package_finder.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/candidate.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/direct_url.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/format_control.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/index.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/link.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/scheme.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/search_scope.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/selection_prefs.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/target_python.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/models/wheel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/auth.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/cache.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/download.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/lazy_wheel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/session.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/utils.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/network/xmlrpc.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/check.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/freeze.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/prepare.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/build/metadata.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/build/metadata_legacy.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/build/wheel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/build/wheel_legacy.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/install/editable_legacy.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/install/legacy.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/operations/install/wheel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/constructors.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_file.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_install.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_set.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_tracker.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_tracker.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/req/req_uninstall.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/base.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/legacy/resolver.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/base.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/candidates.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/factory.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/found_candidates.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/provider.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/reporter.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/requirements.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/resolver.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/appdirs.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/compat.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/compatibility_tags.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/deprecation.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/direct_url_helpers.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/distutils_args.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/encoding.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/entrypoints.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/filesystem.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/filetypes.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/glibc.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/hashes.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/inject_securetransport.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/logging.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/misc.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/models.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/packaging.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/parallel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/pkg_resources.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/setuptools_build.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/subprocess.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/temp_dir.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/typing.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/typing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/unpacking.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/urls.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/virtualenv.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/utils/wheel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/bazaar.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/git.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/mercurial.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/subversion.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_internal/vcs/versioncontrol.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/appdirs.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/contextlib2.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/contextlib2.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distro.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distro.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/ipaddress.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/ipaddress.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pyparsing.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/retrying.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/retrying.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/six.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/_cmd.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/adapter.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/cache.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/compat.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/controller.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/filewrapper.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/heuristics.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/serialize.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/wrapper.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/file_cache.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/certifi/cacert.pem` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/certifi/core.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/big5freq.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/big5prober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/chardistribution.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/charsetgroupprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/charsetprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/codingstatemachine.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/compat.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/cp949prober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/enums.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/escprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/escsm.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/eucjpprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/euckrfreq.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/euckrprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/euctwfreq.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/euctwprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/gb2312freq.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/gb2312prober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/hebrewprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/jisfreq.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/jpcntx.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langbulgarianmodel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langcyrillicmodel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langgreekmodel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langhebrewmodel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langhungarianmodel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langthaimodel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/langturkishmodel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/latin1prober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcharsetprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcsgroupprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcssm.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/sbcharsetprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/sbcsgroupprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/sjisprober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/universaldetector.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/utf8prober.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/chardet/cli/chardetect.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/ansi.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/ansitowin32.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/initialise.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/win32.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/colorama/winterm.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/compat.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/database.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/index.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/locators.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/manifest.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/markers.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/metadata.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/resources.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/scripts.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/t32.exe` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/t64.exe` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/util.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/version.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/w32.exe` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/w64.exe` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/wheel.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/misc.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/misc.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/shutil.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/shutil.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/sysconfig.cfg` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/sysconfig.cfg`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/sysconfig.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/sysconfig.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/tarfile.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/distlib/_backport/tarfile.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_ihatexml.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_inputstream.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_tokenizer.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_utils.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/constants.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/html5parser.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/serializer.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/_base.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/py.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/alphabeticalattributes.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/inject_meta_charset.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/lint.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/optionaltags.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/sanitizer.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/whitespace.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/genshi.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/sax.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/base.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/dom.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/etree.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/etree_lxml.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/base.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/dom.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/etree.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/etree_lxml.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/genshi.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/codec.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/core.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/idnadata.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/intranges.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/idna/uts46data.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/msgpack/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/msgpack/exceptions.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/msgpack/ext.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/msgpack/fallback.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/__about__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/_compat.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/_structures.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/_typing.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/markers.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/requirements.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/specifiers.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/tags.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/utils.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/packaging/version.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/_in_process.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/_in_process.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/build.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/check.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/colorlog.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/compat.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/dirtools.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/envbuild.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/meta.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pep517/wrappers.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pkg_resources/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/pkg_resources/py31compat.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/progress/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/progress/bar.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/progress/bar.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/progress/counter.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/progress/counter.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/progress/spinner.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/_internal_utils.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/adapters.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/api.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/auth.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/compat.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/cookies.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/exceptions.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/help.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/hooks.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/models.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/packages.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/sessions.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/status_codes.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/structures.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/requests/utils.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/providers.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/reporters.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/resolvers.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/structs.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/toml/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/toml/decoder.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/toml/encoder.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/toml/tz.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/toml/tz.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/_collections.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/connection.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/connectionpool.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/exceptions.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/fields.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/filepost.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/poolmanager.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/request.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/response.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/appengine.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/ntlmpool.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/pyopenssl.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/securetransport.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/socks.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/six.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/backports/makefile.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/connection.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/proxy.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/request.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/response.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/retry.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/ssl_.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/ssltransport.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/timeout.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/url.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/wait.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/labels.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/mklabels.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/tests.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip/_vendor/webencodings/x_user_defined.py` & `pex-2.3.1/pex/vendor/_vendored/pip/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/LICENSE.txt` & `pex-2.3.1/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/METADATA` & `pex-2.3.1/pex/vendor/_vendored/pip/pip-20.3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/py31compat.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/appdirs.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/pyparsing.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/six.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/__about__.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/_compat.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/_structures.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/markers.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/requirements.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/specifiers.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/version.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/pkg_resources/extern/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_imp.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/archive_util.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/build_meta.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/cli-32.exe` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/cli-64.exe` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/cli.exe` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/config.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/config.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/dep_util.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/depends.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/dist.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/errors.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/extension.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/glob.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/gui-32.exe` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/gui-64.exe` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/gui.exe` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/installer.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/launch.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/lib2to3_ex.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/lib2to3_ex.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/monkey.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/msvc.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/namespaces.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/package_index.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/py27compat.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/py27compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/py31compat.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/py31compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/py33compat.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/py33compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/sandbox.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/site-patch.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/site-patch.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/ssl_support.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/ssl_support.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/unicode_utils.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/wheel.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/windows_support.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/ordered_set.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/pyparsing.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/six.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/__about__.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/_compat.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/_structures.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/markers.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/requirements.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/specifiers.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/tags.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/utils.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/version.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/alias.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/bdist_egg.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/bdist_rpm.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/bdist_wininst.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/bdist_wininst.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/build_clib.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/build_ext.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/build_py.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/develop.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/dist_info.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/easy_install.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/egg_info.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/install.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/install_egg_info.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/install_lib.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/install_scripts.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/launcher manifest.xml` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/py36compat.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/register.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/register.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/rotate.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/saveopts.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/sdist.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/setopt.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/test.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/upload.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/upload.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/command/upload_docs.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools/extern/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/LICENSE` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/METADATA` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/entry_points.txt` & `pex-2.3.1/pex/vendor/_vendored/setuptools/setuptools-44.0.0+3acb925dd708430aeaf197ea53ac8a752f7c1863.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/toml/toml/__init__.py` & `pex-2.3.1/pex/vendor/_vendored/toml/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/toml/toml/decoder.py` & `pex-2.3.1/pex/vendor/_vendored/toml/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/toml/toml/encoder.py` & `pex-2.3.1/pex/vendor/_vendored/toml/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/toml/toml/ordered.py` & `pex-2.3.1/pex/vendor/_vendored/toml/toml/ordered.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/toml/toml/tz.py` & `pex-2.3.1/pex/vendor/_vendored/toml/toml/tz.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/LICENSE` & `pex-2.3.1/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/METADATA` & `pex-2.3.1/pex/vendor/_vendored/toml/toml-0.10.2.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/venv/installer.py` & `pex-2.3.1/pex/venv/installer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/venv/installer_configuration.py` & `pex-2.3.1/pex/venv/installer_configuration.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/venv/installer_options.py` & `pex-2.3.1/pex/venv/installer_options.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/venv/virtualenv.py` & `pex-2.3.1/pex/venv/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pex/venv/virtualenv_16.7.12_py` & `pex-2.3.1/pex/venv/virtualenv_16.7.12_py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/scripts/build_cache_image.py` & `pex-2.3.1/scripts/build_cache_image.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/scripts/build_docs.py` & `pex-2.3.1/scripts/build_docs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/scripts/embed_virtualenv.py` & `pex-2.3.1/scripts/embed_virtualenv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/scripts/format.py` & `pex-2.3.1/scripts/format.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/scripts/lint.py` & `pex-2.3.1/scripts/lint.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/scripts/package.py` & `pex-2.3.1/scripts/package.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/scripts/typecheck.py` & `pex-2.3.1/scripts/typecheck.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/__init__.py` & `pex-2.3.1/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/build_system.py` & `pex-2.3.1/testing/build_system.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/cli.py` & `pex-2.3.1/testing/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # Copyright 2022 Pex project contributors.
 # Licensed under the Apache License, Version 2.0 (see LICENSE).
 
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import
 
 import subprocess
 import sys
 
-from pex.typing import TYPE_CHECKING
+from pex.compatibility import to_unicode
+from pex.typing import TYPE_CHECKING, cast
 from testing import IntegResults
 
 if TYPE_CHECKING:
+    from typing import Text  # noqa
     from typing import Any
 
 
 def run_pex3(
     *args,  # type: str
-    **popen_kwargs  # type: Any
+    **kwargs  # type: Any
 ):
     # type: (...) -> IntegResults
+
+    python = cast("Text", kwargs.pop("python", to_unicode(sys.executable)))
     process = subprocess.Popen(
-        args=[sys.executable, "-mpex.cli"] + list(args),
+        args=[python, "-mpex.cli"] + list(args),
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
-        **popen_kwargs
+        **kwargs
     )
     stdout, stderr = process.communicate()
     return IntegResults(
         output=stdout.decode("utf-8"), error=stderr.decode("utf-8"), return_code=process.returncode
     )
```

### Comparing `pex-2.3.0/testing/devpi-server.lock` & `pex-2.3.1/testing/devpi-server.lock`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/devpi.py` & `pex-2.3.1/testing/devpi.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/dist_metadata.py` & `pex-2.3.1/testing/dist_metadata.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/docker.py` & `pex-2.3.1/testing/docker.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/find_links.py` & `pex-2.3.1/testing/find_links.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/resolve.py` & `pex-2.3.1/testing/resolve.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/bin/run_tests.py` & `pex-2.3.1/testing/bin/run_tests.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/data/__init__.py` & `pex-2.3.1/testing/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/data/locks/mitmproxy.lock.json` & `pex-2.3.1/testing/data/locks/mitmproxy.lock.json`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/data/locks/requests.lock.json` & `pex-2.3.1/testing/data/locks/requests.lock.json`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/testing/data/platforms/macosx_10_13_x86_64-cp-36-m.tags.txt` & `pex-2.3.1/testing/data/platforms/macosx_10_13_x86_64-cp-36-m.tags.txt`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/conftest.py` & `pex-2.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_atomic_directory.py` & `pex-2.3.1/tests/test_atomic_directory.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_bdist_pex.py` & `pex-2.3.1/tests/test_bdist_pex.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_common.py` & `pex-2.3.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_compatibility.py` & `pex-2.3.1/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_compiler.py` & `pex-2.3.1/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_dependency_manager.py` & `pex-2.3.1/tests/test_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_dist_metadata.py` & `pex-2.3.1/tests/test_dist_metadata.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_enum.py` & `pex-2.3.1/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_environment.py` & `pex-2.3.1/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_execution_mode.py` & `pex-2.3.1/tests/test_execution_mode.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_executor.py` & `pex-2.3.1/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_fetcher.py` & `pex-2.3.1/tests/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_finders.py` & `pex-2.3.1/tests/test_finders.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_hashing.py` & `pex-2.3.1/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_inherits_path_option.py` & `pex-2.3.1/tests/test_inherits_path_option.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_interpreter.py` & `pex-2.3.1/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_interpreter_constraints.py` & `pex-2.3.1/tests/test_interpreter_constraints.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_jobs.py` & `pex-2.3.1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_packaging.py` & `pex-2.3.1/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pep_376.py` & `pex-2.3.1/tests/test_pep_376.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pep_425.py` & `pex-2.3.1/tests/test_pep_425.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pep_508.py` & `pex-2.3.1/tests/test_pep_508.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pex.py` & `pex-2.3.1/tests/test_pex.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pex_binary.py` & `pex-2.3.1/tests/test_pex_binary.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pex_bootstrapper.py` & `pex-2.3.1/tests/test_pex_bootstrapper.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pex_builder.py` & `pex-2.3.1/tests/test_pex_builder.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pex_info.py` & `pex-2.3.1/tests/test_pex_info.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pex_warnings.py` & `pex-2.3.1/tests/test_pex_warnings.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pip.py` & `pex-2.3.1/tests/test_pip.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_platform.py` & `pex-2.3.1/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pth.py` & `pex-2.3.1/tests/test_pth.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_pyvenv_cfg.py` & `pex-2.3.1/tests/test_pyvenv_cfg.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_requirements.py` & `pex-2.3.1/tests/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_resolver.py` & `pex-2.3.1/tests/test_resolver.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_sorted_tuple.py` & `pex-2.3.1/tests/test_sorted_tuple.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_targets.py` & `pex-2.3.1/tests/test_targets.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_third_party.py` & `pex-2.3.1/tests/test_third_party.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_util.py` & `pex-2.3.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_variables.py` & `pex-2.3.1/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_vendor.py` & `pex-2.3.1/tests/test_vendor.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/test_zip_utils.py` & `pex-2.3.1/tests/test_zip_utils.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/bin/test_sh_boot.py` & `pex-2.3.1/tests/bin/test_sh_boot.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/build_system/test_issue_2125.py` & `pex-2.3.1/tests/build_system/test_issue_2125.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/build_system/test_pep_517.py` & `pex-2.3.1/tests/build_system/test_pep_517.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/build_system/test_pep_518.py` & `pex-2.3.1/tests/build_system/test_pep_518.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/commands/test_command.py` & `pex-2.3.1/tests/commands/test_command.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/example_packages/MarkupSafe-1.0-cp27-cp27mu-linux_x86_64.whl` & `pex-2.3.1/tests/example_packages/MarkupSafe-1.0-cp27-cp27mu-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/example_packages/PyAthena-1.11.5-py2.py3-none-any.whl` & `pex-2.3.1/tests/example_packages/PyAthena-1.11.5-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/example_packages/PyAthena-1.9.0-py2.py3-none-any.whl` & `pex-2.3.1/tests/example_packages/PyAthena-1.9.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/example_packages/aws_cfn_bootstrap-1.4-py2-none-any.whl` & `pex-2.3.1/tests/example_packages/aws_cfn_bootstrap-1.4-py2-none-any.whl`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/example_packages/pyparsing-2.1.10-py2.py3-none-any.whl` & `pex-2.3.1/tests/example_packages/pyparsing-2.1.10-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/conftest.py` & `pex-2.3.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_downloads.py` & `pex-2.3.1/tests/integration/test_downloads.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import hashlib
 import os.path
 
 import pytest
 
 from pex.resolve.configured_resolver import ConfiguredResolver
 from pex.resolve.downloads import ArtifactDownloader
-from pex.resolve.locked_resolve import Artifact, FileArtifact
+from pex.resolve.locked_resolve import Artifact, FileArtifact, LockConfiguration, LockStyle
 from pex.resolve.resolved_requirement import Fingerprint, PartialArtifact
 from pex.typing import TYPE_CHECKING
 from testing import IS_LINUX
 
 if TYPE_CHECKING:
     pass
 
@@ -50,15 +50,18 @@
     sha256="c7be9d7f5b0d206f0bbc3794b8e16fb7dbc53ec9e40bbe8787c6f2d38efcf6c9",
 )
 
 
 @pytest.fixture
 def downloader():
     # type: () -> ArtifactDownloader
-    return ArtifactDownloader(ConfiguredResolver.default())
+    return ArtifactDownloader(
+        resolver=ConfiguredResolver.default(),
+        lock_configuration=LockConfiguration(style=LockStyle.UNIVERSAL),
+    )
 
 
 def test_issue_1849_download_foreign_artifact(
     tmpdir,  # type: str
     downloader,  # type: ArtifactDownloader
 ):
     # type: (...) -> None
```

### Comparing `pex-2.3.0/tests/integration/test_excludes.py` & `pex-2.3.1/tests/integration/test_excludes.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_executuon_mode_venv.py` & `pex-2.3.1/tests/integration/test_executuon_mode_venv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_inject_env_and_args.py` & `pex-2.3.1/tests/integration/test_inject_env_and_args.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_integration.py` & `pex-2.3.1/tests/integration/test_integration.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_interpreter.py` & `pex-2.3.1/tests/integration/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_interpreter_selection.py` & `pex-2.3.1/tests/integration/test_interpreter_selection.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1017.py` & `pex-2.3.1/tests/integration/test_issue_1017.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1018.py` & `pex-2.3.1/tests/integration/test_issue_1018.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1025.py` & `pex-2.3.1/tests/integration/test_issue_1025.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1031.py` & `pex-2.3.1/tests/integration/test_issue_1031.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1179.py` & `pex-2.3.1/tests/integration/test_issue_1179.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1201.py` & `pex-2.3.1/tests/integration/test_issue_1201.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1202.py` & `pex-2.3.1/tests/integration/test_issue_1202.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1218.py` & `pex-2.3.1/tests/integration/test_issue_1218.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1225.py` & `pex-2.3.1/tests/integration/test_issue_1225.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1232.py` & `pex-2.3.1/tests/integration/test_issue_1232.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1302.py` & `pex-2.3.1/tests/integration/test_issue_1302.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1316.py` & `pex-2.3.1/tests/integration/test_issue_1316.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1336.py` & `pex-2.3.1/tests/integration/test_issue_1336.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1422.py` & `pex-2.3.1/tests/integration/test_issue_1422.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1447.py` & `pex-2.3.1/tests/integration/test_issue_1447.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1479.py` & `pex-2.3.1/tests/integration/test_issue_1479.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1520.py` & `pex-2.3.1/tests/integration/test_issue_1520.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1537.py` & `pex-2.3.1/tests/integration/test_issue_1537.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1540.py` & `pex-2.3.1/tests/integration/test_issue_1540.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1550.py` & `pex-2.3.1/tests/integration/test_issue_1550.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1560.py` & `pex-2.3.1/tests/integration/test_issue_1560.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1597.py` & `pex-2.3.1/tests/integration/test_issue_1597.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1598.py` & `pex-2.3.1/tests/integration/test_issue_1598.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1656.py` & `pex-2.3.1/tests/integration/test_issue_1656.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1683.py` & `pex-2.3.1/tests/integration/test_issue_1683.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1726.py` & `pex-2.3.1/tests/integration/test_issue_1726.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         "--pex-root",
         pex_root,
         "--runtime-pex-root",
         pex_root,
         src,
         "--constraints",
         constraints,
+        "--resolver-version",
+        "pip-2020-resolver",
         "--",
         "-c",
         "from jaraco import collections; print(collections.__file__)",
     ]
     old_result = run_pex_command(
         args=["pex==2.1.80", "-c", "pex", "--"] + pex_args,
         # N.B.: Pex 2.1.80 only works on CPython 3.10 and older and PyPy 3.7 and older.
```

### Comparing `pex-2.3.0/tests/integration/test_issue_1730.py` & `pex-2.3.1/tests/integration/test_issue_1730.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1802.py` & `pex-2.3.1/tests/integration/test_issue_1802.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1809.py` & `pex-2.3.1/tests/integration/test_issue_1809.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1817.py` & `pex-2.3.1/tests/integration/test_issue_1817.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1825.py` & `pex-2.3.1/tests/integration/test_issue_1825.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1856.py` & `pex-2.3.1/tests/integration/test_issue_1856.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1861.py` & `pex-2.3.1/tests/integration/test_issue_1861.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1870.py` & `pex-2.3.1/tests/integration/test_issue_1870.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1872.py` & `pex-2.3.1/tests/integration/test_issue_1872.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1879.py` & `pex-2.3.1/tests/integration/test_issue_1879.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1933.py` & `pex-2.3.1/tests/integration/test_issue_1933.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1936.py` & `pex-2.3.1/tests/integration/test_issue_1936.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1949.py` & `pex-2.3.1/tests/integration/test_issue_1949.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_1995.py` & `pex-2.3.1/tests/integration/test_issue_1995.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2001.py` & `pex-2.3.1/tests/integration/test_issue_2001.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2006.py` & `pex-2.3.1/tests/integration/test_issue_2006.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2023.py` & `pex-2.3.1/tests/integration/test_issue_2023.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2038.py` & `pex-2.3.1/tests/integration/test_issue_2038.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2073.py` & `pex-2.3.1/tests/integration/test_issue_2073.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2087.py` & `pex-2.3.1/tests/integration/test_issue_2087.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2088.py` & `pex-2.3.1/tests/integration/test_issue_2088.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2134.py` & `pex-2.3.1/tests/integration/test_issue_2134.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2183.py` & `pex-2.3.1/tests/integration/test_issue_2183.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2186.py` & `pex-2.3.1/tests/integration/test_issue_2186.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2203.py` & `pex-2.3.1/tests/integration/test_issue_2203.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2235.py` & `pex-2.3.1/tests/integration/test_issue_2235.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2324.py` & `pex-2.3.1/tests/integration/test_issue_2324.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2343.py` & `pex-2.3.1/tests/integration/test_issue_2343.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2348.py` & `pex-2.3.1/tests/integration/test_issue_2348.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2355.py` & `pex-2.3.1/tests/integration/test_issue_2355.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2389.py` & `pex-2.3.1/tests/integration/test_issue_2389.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_2391.py` & `pex-2.3.1/tests/integration/test_issue_2391.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2014 Pex project contributors.
+# Copyright 2024 Pex project contributors.
 # Licensed under the Apache License, Version 2.0 (see LICENSE).
 
 import os.path
 import re
 import subprocess
 import sys
```

### Comparing `pex-2.3.0/tests/integration/test_issue_2739.py` & `pex-2.3.1/tests/integration/test_issue_2739.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_434.py` & `pex-2.3.1/tests/integration/test_issue_434.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_539.py` & `pex-2.3.1/tests/integration/test_issue_539.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_598.py` & `pex-2.3.1/tests/integration/test_issue_598.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_661.py` & `pex-2.3.1/tests/integration/test_issue_661.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_729.py` & `pex-2.3.1/tests/integration/test_issue_729.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_736.py` & `pex-2.3.1/tests/integration/test_issue_736.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_745.py` & `pex-2.3.1/tests/integration/test_issue_745.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_749.py` & `pex-2.3.1/tests/integration/test_issue_749.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_898.py` & `pex-2.3.1/tests/integration/test_issue_898.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_899.py` & `pex-2.3.1/tests/integration/test_issue_899.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_940.py` & `pex-2.3.1/tests/integration/test_issue_940.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_issue_996.py` & `pex-2.3.1/tests/integration/test_issue_996.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_layout.py` & `pex-2.3.1/tests/integration/test_layout.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_lock_resolver.py` & `pex-2.3.1/tests/integration/test_lock_resolver.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_locked_resolve.py` & `pex-2.3.1/tests/integration/test_locked_resolve.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_no_pre_install_wheels.py` & `pex-2.3.1/tests/integration/test_no_pre_install_wheels.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_pep_427.py` & `pex-2.3.1/tests/integration/test_pep_427.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_pex_bootstrapper.py` & `pex-2.3.1/tests/integration/test_pex_bootstrapper.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_pex_entry_points.py` & `pex-2.3.1/tests/integration/test_pex_entry_points.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_pex_import.py` & `pex-2.3.1/tests/integration/test_pex_import.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_reexec.py` & `pex-2.3.1/tests/integration/test_reexec.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_reproducible.py` & `pex-2.3.1/tests/integration/test_reproducible.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_setproctitle.py` & `pex-2.3.1/tests/integration/test_setproctitle.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_sh_boot.py` & `pex-2.3.1/tests/integration/test_sh_boot.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_shebang_length_limit.py` & `pex-2.3.1/tests/integration/test_shebang_length_limit.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/test_variables.py` & `pex-2.3.1/tests/integration/test_variables.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/build_system/test_issue_2063.py` & `pex-2.3.1/tests/integration/build_system/test_issue_2063.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/build_system/test_issue_2125.py` & `pex-2.3.1/tests/integration/build_system/test_issue_2125.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/build_system/test_pep_517.py` & `pex-2.3.1/tests/integration/build_system/test_pep_517.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/build_system/test_pep_518.py` & `pex-2.3.1/tests/integration/build_system/test_pep_518.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_export.py` & `pex-2.3.1/tests/integration/cli/commands/test_export.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_export_subset.lock.json` & `pex-2.3.1/tests/integration/cli/commands/test_export_subset.lock.json`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_export_subset.py` & `pex-2.3.1/tests/integration/cli/commands/test_export_subset.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_interpreter_inspect.py` & `pex-2.3.1/tests/integration/cli/commands/test_interpreter_inspect.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_1413.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_1413.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_1665.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_1665.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_1667.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_1667.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_1688.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_1688.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_1711.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_1711.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_1734.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_1734.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_1741.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_1741.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_1801.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_1801.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_1821.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_1821.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_2050.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_2050.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_2057.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_2057.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_2059.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_2059.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_2098.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_2098.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_2211.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_2211.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_issue_2268.py` & `pex-2.3.1/tests/integration/cli/commands/test_issue_2268.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_local_project_lock.py` & `pex-2.3.1/tests/integration/cli/commands/test_local_project_lock.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_lock.py` & `pex-2.3.1/tests/integration/cli/commands/test_lock.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_lock_resolve_auth.py` & `pex-2.3.1/tests/integration/cli/commands/test_lock_resolve_auth.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_lock_sync.py` & `pex-2.3.1/tests/integration/cli/commands/test_lock_sync.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_lock_update.py` & `pex-2.3.1/tests/integration/cli/commands/test_lock_update.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_lock_update_issues_2332_2334.py` & `pex-2.3.1/tests/integration/cli/commands/test_lock_update_issues_2332_2334.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_vcs_lock.py` & `pex-2.3.1/tests/integration/cli/commands/test_vcs_lock.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_venv_create.py` & `pex-2.3.1/tests/integration/cli/commands/test_venv_create.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/cli/commands/test_venv_inspect.py` & `pex-2.3.1/tests/integration/cli/commands/test_venv_inspect.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/resolve/test_issue_1918.py` & `pex-2.3.1/tests/integration/resolve/test_issue_1918.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/resolve/test_issue_2092.py` & `pex-2.3.1/tests/integration/resolve/test_issue_2092.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/resolve/pep_691/test_api.py` & `pex-2.3.1/tests/integration/resolve/pep_691/test_api.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/tools/commands/test_issue_2105.py` & `pex-2.3.1/tests/integration/tools/commands/test_issue_2105.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/tools/commands/test_venv.py` & `pex-2.3.1/tests/integration/tools/commands/test_venv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/conftest.py` & `pex-2.3.1/tests/integration/venv_ITs/conftest.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_install_wheel_multiple_site_packages_dirs.py` & `pex-2.3.1/tests/integration/venv_ITs/test_install_wheel_multiple_site_packages_dirs.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_issue_1630.py` & `pex-2.3.1/tests/integration/venv_ITs/test_issue_1630.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_issue_1637.py` & `pex-2.3.1/tests/integration/venv_ITs/test_issue_1637.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_issue_1641.py` & `pex-2.3.1/tests/integration/venv_ITs/test_issue_1641.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_issue_1668.py` & `pex-2.3.1/tests/integration/venv_ITs/test_issue_1668.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_issue_1745.py` & `pex-2.3.1/tests/integration/venv_ITs/test_issue_1745.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_issue_2065.py` & `pex-2.3.1/tests/integration/venv_ITs/test_issue_2065.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_issue_2160.py` & `pex-2.3.1/tests/integration/venv_ITs/test_issue_2160.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_issue_2248.py` & `pex-2.3.1/tests/integration/venv_ITs/test_issue_2248.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/integration/venv_ITs/test_virtualenv.py` & `pex-2.3.1/tests/integration/venv_ITs/test_virtualenv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/pip/test_tailer.py` & `pex-2.3.1/tests/pip/test_tailer.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/test_locked_resolve.py` & `pex-2.3.1/tests/resolve/test_locked_resolve.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/test_locker.py` & `pex-2.3.1/tests/resolve/test_locker.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/test_path_mappings.py` & `pex-2.3.1/tests/resolve/test_path_mappings.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/test_pex_repository_resolver.py` & `pex-2.3.1/tests/resolve/test_pex_repository_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,16 @@
         # The 2.25.1 release of requests constrains urllib3 to <1.27,>=1.21.1 and picks 1.26.2 on
         # its own as of this writing.
         "urllib3==1.26.1",
         # The 22.0.0 release of pyOpenSSL drops support for Python 2.7; so we pin lower.
         "pyOpenSSL<22",
         # The 2022 and later releases only support Python>=3.6; so we pin lower.
         "certifi<2022",
+        # The 2.22 release of pycparser drops support for Python 2.7.
+        "pycparser<2.22",
     )
 
     return create_pex_repository(
         interpreters=[py27, py310],
         platforms=[foreign_platform],
         requirements=["requests[security,socks]==2.25.1"],
         constraint_files=[constraints_file],
```

### Comparing `pex-2.3.0/tests/resolve/test_resolved_requirement.py` & `pex-2.3.1/tests/resolve/test_resolved_requirement.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/test_resolver_options.py` & `pex-2.3.1/tests/resolve/test_resolver_options.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/test_target_options.py` & `pex-2.3.1/tests/resolve/test_target_options.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/lockfile/test_download_manager.py` & `pex-2.3.1/tests/resolve/lockfile/test_download_manager.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/lockfile/test_json_codec.py` & `pex-2.3.1/tests/resolve/lockfile/test_json_codec.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/lockfile/test_lockfile.py` & `pex-2.3.1/tests/resolve/lockfile/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/pep_691/test_api.py` & `pex-2.3.1/tests/resolve/pep_691/test_api.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/pep_691/test_fingerprint_service.py` & `pex-2.3.1/tests/resolve/pep_691/test_fingerprint_service.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/resolve/pep_691/test_model.py` & `pex-2.3.1/tests/resolve/pep_691/test_model.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/tools/commands/test_interpreter_command.py` & `pex-2.3.1/tests/tools/commands/test_interpreter_command.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/tools/commands/test_repository.py` & `pex-2.3.1/tests/tools/commands/test_repository.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/tests/tools/commands/test_venv.py` & `pex-2.3.1/tests/tools/commands/test_venv.py`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/LICENSE` & `pex-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/README.rst` & `pex-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/pyproject.toml` & `pex-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pex-2.3.0/PKG-INFO` & `pex-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pex
-Version: 2.3.0
+Version: 2.3.1
 Summary: The PEX packaging toolchain.
-Project-URL: Changelog, https://github.com/pex-tool/pex/blob/v2.3.0/CHANGES.md
+Project-URL: Changelog, https://github.com/pex-tool/pex/blob/v2.3.1/CHANGES.md
 Project-URL: Documentation, https://docs.pex-tool.org/
-Project-URL: Download, https://github.com/pex-tool/pex/releases/download/v2.3.0/pex
+Project-URL: Download, https://github.com/pex-tool/pex/releases/download/v2.3.1/pex
 Project-URL: Homepage, https://github.com/pex-tool/pex
-Project-URL: Source, https://github.com/pex-tool/pex/tree/v2.3.0
+Project-URL: Source, https://github.com/pex-tool/pex/tree/v2.3.1
 Author-email: The PEX developers <developers@pex-tool.org>
 License-File: LICENSE
 Keywords: executable,freeze,lock,package,virtualenv
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
```

