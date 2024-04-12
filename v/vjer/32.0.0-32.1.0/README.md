# Comparing `tmp/vjer-32.0.0.tar.gz` & `tmp/vjer-32.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vjer-32.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vjer-32.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vjer-32.0.0.tar` & `vjer-32.1.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0     6148 2024-04-11 01:07:45.534438 vjer-32.0.0/.DS_Store
--rw-r--r--   0        0        0     1788 2024-04-11 01:07:45.534438 vjer-32.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2134 2024-04-11 01:07:45.534438 vjer-32.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     4755 2024-04-11 01:07:45.534438 vjer-32.0.0/.gitignore
--rw-r--r--   0        0        0     4999 2024-04-11 01:07:45.534438 vjer-32.0.0/.p4ignore
--rw-r--r--   0        0        0       42 2024-04-11 01:07:45.534438 vjer-32.0.0/.readthedocs.yml
--rw-r--r--   0        0        0    39819 2024-04-11 01:07:45.534438 vjer-32.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       64 2024-04-11 01:07:45.534438 vjer-32.0.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-04-11 01:07:45.534438 vjer-32.0.0/LICENSE
--rw-r--r--   0        0        0       90 2024-04-11 01:07:45.534438 vjer-32.0.0/MANIFEST.in
--rw-r--r--   0        0        0     1499 2024-04-11 01:07:45.534438 vjer-32.0.0/README.md
--rwxr-xr-x   0        0        0      878 2024-04-11 01:07:45.538438 vjer-32.0.0/cicd-support/cicd.sh
--rw-r--r--   0        0        0      634 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/Makefile
--rw-r--r--   0        0        0     9167 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2103 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/conf.py
--rw-r--r--   0        0        0      795 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/make.bat
--rw-r--r--   0        0        0       59 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     2180 2024-04-11 01:08:31.398089 vjer-32.0.0/pyproject.toml
--rw-r--r--   0        0        0      476 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer.yml
--rw-r--r--   0        0        0      654 2024-04-11 01:08:31.398089 vjer-32.0.0/vjer/__init__.py
--rw-r--r--   0        0        0      205 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/__main__.py
--rw-r--r--   0        0        0     5208 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/build.py
--rw-r--r--   0        0        0     1185 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/deploy.py
--rw-r--r--   0        0        0     2875 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/freeze.py
--rw-r--r--   0        0        0     1501 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/pre_release.py
--rw-r--r--   0        0        0        0 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/py.typed
--rw-r--r--   0        0        0     3519 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/release.py
--rw-r--r--   0        0        0      769 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/rollback.py
--rw-r--r--   0        0        0     3457 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/test.py
--rw-r--r--   0        0        0     2946 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/tool_reporter.py
--rw-r--r--   0        0        0    25133 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/utils.py
--rwxr-xr-x   0        0        0     2445 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/vjer.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 vjer-32.0.0/setup.py
--rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 vjer-32.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1788 2024-04-12 02:21:43.862315 vjer-32.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2134 2024-04-12 02:21:43.862315 vjer-32.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     5245 2024-04-12 02:21:43.862315 vjer-32.1.0/.gitignore
+-rw-r--r--   0        0        0     4999 2024-04-12 02:21:43.862315 vjer-32.1.0/.p4ignore
+-rw-r--r--   0        0        0       42 2024-04-12 02:21:43.862315 vjer-32.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0    39968 2024-04-12 02:21:43.862315 vjer-32.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       64 2024-04-12 02:21:43.862315 vjer-32.1.0/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-04-12 02:21:43.862315 vjer-32.1.0/LICENSE
+-rw-r--r--   0        0        0       90 2024-04-12 02:21:43.862315 vjer-32.1.0/MANIFEST.in
+-rw-r--r--   0        0        0      973 2024-04-12 02:21:43.862315 vjer-32.1.0/README.md
+-rwxr-xr-x   0        0        0      878 2024-04-12 02:21:43.862315 vjer-32.1.0/cicd-support/cicd.sh
+-rw-r--r--   0        0        0      634 2024-04-12 02:21:43.862315 vjer-32.1.0/docs/Makefile
+-rw-r--r--   0        0        0     9167 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/coding_standards.py
+-rw-r--r--   0        0        0     2103 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/conf.py
+-rw-r--r--   0        0        0      795 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/make.bat
+-rw-r--r--   0        0        0       59 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-04-12 02:21:43.866315 vjer-32.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2180 2024-04-12 02:22:13.610476 vjer-32.1.0/pyproject.toml
+-rw-r--r--   0        0        0      305 2024-04-12 02:21:43.866315 vjer-32.1.0/util/New-Env.ps1
+-rw-r--r--   0        0        0      259 2024-04-12 02:21:43.866315 vjer-32.1.0/util/Update-Env.ps1
+-rw-r--r--   0        0        0      271 2024-04-12 02:21:43.866315 vjer-32.1.0/util/new-env.sh
+-rw-r--r--   0        0        0      241 2024-04-12 02:21:43.866315 vjer-32.1.0/util/update-env.sh
+-rw-r--r--   0        0        0      476 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer.yml
+-rw-r--r--   0        0        0      654 2024-04-12 02:22:13.610476 vjer-32.1.0/vjer/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/__main__.py
+-rw-r--r--   0        0        0     5208 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/build.py
+-rw-r--r--   0        0        0     1185 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/deploy.py
+-rw-r--r--   0        0        0     2875 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/freeze.py
+-rw-r--r--   0        0        0     1501 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/pre_release.py
+-rw-r--r--   0        0        0        0 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/py.typed
+-rw-r--r--   0        0        0     3525 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/release.py
+-rw-r--r--   0        0        0      769 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/rollback.py
+-rw-r--r--   0        0        0     3457 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/test.py
+-rw-r--r--   0        0        0     2946 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/tool_reporter.py
+-rw-r--r--   0        0        0    24942 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/utils.py
+-rwxr-xr-x   0        0        0     2825 2024-04-12 02:21:43.866315 vjer-32.1.0/vjer/vjer.py
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 vjer-32.1.0/setup.py
+-rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 vjer-32.1.0/PKG-INFO
```

### Comparing `vjer-32.0.0/.github/workflows/build.yml` & `vjer-32.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/.github/workflows/publish.yml` & `vjer-32.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/.gitignore` & `vjer-32.1.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # File created using '.gitignore Generator' for Visual Studio Code: https://bit.ly/vscode-gig
-# Created by https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python,git
-# Edit at https://www.toptal.com/developers/gitignore?templates=windows,visualstudiocode,python,git
+# Created by https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python,git,macos
+# Edit at https://www.toptal.com/developers/gitignore?templates=windows,visualstudiocode,python,git,macos
 
 ### Git ###
 # Created by git for backups. To disable backups in Git:
 # $ git config --global mergetool.keepBackup false
 *.orig
 
 # Created by git when using merge tools for conflicts
@@ -13,14 +13,46 @@
 *.LOCAL.*
 *.REMOTE.*
 *_BACKUP_*.txt
 *_BASE_*.txt
 *_LOCAL_*.txt
 *_REMOTE_*.txt
 
+### macOS ###
+# General
+.DS_Store
+.AppleDouble
+.LSOverride
+
+# Icon must end with two \r
+Icon
+
+# Thumbnails
+._*
+
+# Files that might appear in the root of a volume
+.DocumentRevisions-V100
+.fseventsd
+.Spotlight-V100
+.TemporaryItems
+.Trashes
+.VolumeIcon.icns
+.com.apple.timemachine.donotpresent
+
+# Directories potentially created on remote AFP share
+.AppleDB
+.AppleDesktop
+Network Trash Folder
+Temporary Items
+.apdisk
+
+### macOS Patch ###
+# iCloud generated files
+*.icloud
+
 ### Python ###
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
@@ -230,15 +262,15 @@
 *.msix
 *.msm
 *.msp
 
 # Windows shortcuts
 *.lnk
 
-# End of https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python,git
+# End of https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python,git,macos
 
 # Custom rules (everything added below won't be overriden by 'Generate .gitignore File' if you use 'Update' option)
 
 .git/
 .p4cfg
 artifacts/
 unit_test_results/
```

### Comparing `vjer-32.0.0/.p4ignore` & `vjer-32.1.0/.p4ignore`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/CHANGELOG.md` & `vjer-32.1.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,30 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## Current Release
 
+### [32.1.0] - 2024-04-11
+
+- Changed
+  - Cleanup version output and add --version option. (GitHub #8)
+  - Fix tagging on release. (GitHub #7)
+
+## Release History
+
 ### [32.0.0] - 2024-04-10
 
 - Added
   - Added flit and bumpver support. (GitHub #2)
 
 - Removed
   - Removed implicit release steps. (GitHub #6)
 
-## Release History
-
 ### [31.0.0] - 2024-03-21
 
 - Added
   - Added bumpver version service. (GitHub #3)
   - Added python test types: flake8, pylint, and mypy. (GitHub #3)
   - Added __main__.py to enable module execution. (GitHub #4)
```

### Comparing `vjer-32.0.0/LICENSE` & `vjer-32.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/cicd-support/cicd.sh` & `vjer-32.1.0/cicd-support/cicd.sh`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/docs/Makefile` & `vjer-32.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/docs/coding_standards.py` & `vjer-32.1.0/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/docs/conf.py` & `vjer-32.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/docs/make.bat` & `vjer-32.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/pyproject.toml` & `vjer-32.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "xmlrunner.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "v32.0.0"
+current_version = "v32.1.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip ci]"
 commit = true
 tag = false
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `vjer-32.0.0/vjer/__init__.py` & `vjer-32.1.0/vjer/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
            '__author__', '__email__',
            '__license__', '__copyright__')
 
 __title__ = 'Vjer'
 __summary__ = 'CI/CD Toolkit'
 __uri__ = 'https://github.com/tardis4500/vjer/'
 
-__version__ = '32.0.0'
+__version__ = '32.1.0'
 __build_name__ = '{var:build_name}'
 __build_date__ = '{var:build_date}'
 
 __author__ = 'Jeffery G. Smith'
 __email__ = 'web@pobox.com'
 
 __license__ = 'MIT'
```

### Comparing `vjer-32.0.0/vjer/build.py` & `vjer-32.1.0/vjer/build.py`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/vjer/deploy.py` & `vjer-32.1.0/vjer/deploy.py`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/vjer/freeze.py` & `vjer-32.1.0/vjer/freeze.py`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/vjer/pre_release.py` & `vjer-32.1.0/vjer/pre_release.py`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/vjer/release.py` & `vjer-32.1.0/vjer/release.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     def release_flit_build(self) -> None:
         """Run a Python flit build."""
         self.flit_build()
 
     def release_github(self) -> None:
         """Create a GitHub release."""
-        SysCmdRunner('gh', 'release', 'create', self.version, title=f'Release {self.version}', latest=True, generate_notes=True).run()
+        SysCmdRunner('gh', 'release', 'create', f'v{self.version}', title=f'Release {self.version}', latest=True, generate_notes=True).run()
 
     def release_helm(self) -> None:
         """Perform a release of a Helm chart."""
         helm('push', self.helm_package, self.helm_repo.name, **self.helm_repo.push_args)
 
     def release_increment_release(self) -> None:
         """Increment the project release version."""
```

### Comparing `vjer-32.0.0/vjer/rollback.py` & `vjer-32.1.0/vjer/rollback.py`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/vjer/test.py` & `vjer-32.1.0/vjer/test.py`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/vjer/tool_reporter.py` & `vjer-32.1.0/vjer/tool_reporter.py`

 * *Files identical despite different names*

### Comparing `vjer-32.0.0/vjer/utils.py` & `vjer-32.1.0/vjer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from batcave.sysutil import CMDError, SysCmdRunner, syscmd
 from bumpver.config import init as bumpver_config
 from dotmap import DotMap
 from flit.build import main as flit_builder
 from yaml import safe_dump as yaml_dump, safe_load as yaml_load
 
 # Import project modules
-from . import __title__, __version__, __build_name__, __build_date__
 from .tool_reporter import tool_reporter
 
 _CONFIG_SECTIONS = ('project', 'test', 'build', 'deploy', 'rollback', 'release')
 _PROJECT_DEFAULTS = DotMap(build_artifacts='artifacts',
                            build_num_var='VJER_BUILD_NUM',
                            chart_root='helm-chart',
                            container_registry=DotMap(type='local', name=''),
@@ -536,15 +535,14 @@
         """
         self.config = ProjectConfig()
         self.action_type = action_type
         self.action_step_class = action_step_class
 
     def execute(self) -> None:
         """Run the action."""
-        VjerStep().log_message(f'Starting {__title__} version {__version__} ({__build_name__}) [{__build_date__}]', True)
         for (category, info) in (yaml_to_dotmap(TOOL_REPORT) if TOOL_REPORT.exists() else tool_reporter()).items():
             VjerStep().log_message(category.replace('_', ' ').title(), True)
             for (name, data) in info.items():
                 VjerStep().log_message(f'  {name}: {data}')
         if not hasattr(action_def := getattr(self.config, self.action_type), 'steps'):
             return
```

### Comparing `vjer-32.0.0/vjer/vjer.py` & `vjer-32.1.0/vjer/vjer.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,26 +8,31 @@
 import os
 from os import getenv
 from platform import platform
 from sys import exit as sys_exit, stderr, version as python_version
 
 # Import third-party modules
 from batcave.commander import Argument, Commander
+from batcave.version import AppVersion, VersionStyle
 
 # Import local modules
-from .utils import apt, apt_install, VJER_ENV, pip_install, ProjectConfig, ConfigurationError, PROJECT_CFG_FILE
+from . import __title__, __version__, __build_name__, __build_date__
+from .utils import apt, apt_install, VJER_ENV, pip_install, ProjectConfig, ConfigurationError, PROJECT_CFG_FILE, VjerStep
 
 ACTIONS = ['test', 'build', 'deploy', 'rollback', 'pre_release', 'release', 'freeze']
 
 
 def main() -> None:
     """The main entrypoint."""
-    args = Commander('Vjer CI/CD Automation Tool', [Argument('actions', choices=ACTIONS, nargs='+')]).parse_args()
+    version = AppVersion(__title__, __version__, __build_date__, __build_name__)
+    args = Commander('Vjer CI/CD Automation Tool', [Argument('actions', choices=ACTIONS, nargs='+')], version=version).parse_args()
+    VjerStep().log_message(version.get_info(VersionStyle.one_line), True)
     _setup_environment()
-    print(f'OS: {platform()}\nPython version: {python_version}')
+    VjerStep().log_message(f'OS: {platform()}')
+    VjerStep().log_message(f'Python version: {python_version}')
 
     _sys_initialize()
     for action in args.actions:
         action_module = import_module(f'vjer.{action}')
         action_module.__dict__[action]()
 
 
@@ -38,22 +43,22 @@
 
 def _setup_environment() -> None:
     try:
         config = ProjectConfig()
     except ConfigurationError as err:
         if err.code != ConfigurationError.CONFIG_FILE_NOT_FOUND.code:
             raise
-        print('The Vjer configuration file was not found:', PROJECT_CFG_FILE, file=stderr)
+        print('ERROR The Vjer configuration file was not found:', PROJECT_CFG_FILE, file=stderr)
         sys_exit(1)
     if (VJER_ENV == 'local') and not getenv('VIRTUAL_ENV', ''):
-        print('Vjer must be run from a virtual environment.', file=stderr)
+        print('ERROR Vjer must be run from a virtual environment.', file=stderr)
         sys_exit(1)
     if hasattr((config := ProjectConfig()).project, 'environment'):
         for (var, val) in config.project.environment.items():
-            print(f'setting {var}={val}')
+            VjerStep().log_message(f'setting {var}={val}')
             os.environ[var] = val  # putenv doesn't work because the values are needed for this process.
 
 
 def _sys_initialize() -> None:
     if pkg_installs := getenv('VJER_PKG_INSTALLS', ''):
         apt('update')
         apt_install(pkg_installs)
```

### Comparing `vjer-32.0.0/setup.py` & `vjer-32.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 extras_require = \
 {'dev': ['flit', 'twine'], 'test': ['types-PyYAML', 'types-requests']}
 
 entry_points = \
 {'console_scripts': ['vjer = vjer.vjer:main']}
 
 setup(name='vjer',
-      version='32.0.0',
+      version='32.1.0',
       description='Vjer CI/CD module.',
       author=None,
       author_email='"Jeffery G. Smith" <web@pobox.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `vjer-32.0.0/PKG-INFO` & `vjer-32.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vjer
-Version: 32.0.0
+Version: 32.1.0
 Summary: Vjer CI/CD module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

