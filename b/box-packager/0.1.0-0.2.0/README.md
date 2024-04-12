# Comparing `tmp/box_packager-0.1.0.tar.gz` & `tmp/box_packager-0.2.0.tar.gz`

## Comparing `box_packager-0.1.0.tar` & `box_packager-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,55 @@
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 box_packager-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 box_packager-0.1.0/.python-version
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 box_packager-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 box_packager-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 box_packager-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 box_packager-0.1.0/requirements.lock
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 box_packager-0.1.0/.github/workflows/integration_tests.yml
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 box_packager-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 box_packager-0.1.0/docs/changelog.md
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 box_packager-0.1.0/docs/cli.md
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 box_packager-0.1.0/docs/examples.md
--rw-r--r--   0        0        0    10099 2020-02-02 00:00:00.000000 box_packager-0.1.0/docs/guide.md
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 box_packager-0.1.0/docs/index.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 box_packager-0.1.0/docs/.includes/build.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 box_packager-0.1.0/docs/.includes/install.md
--rw-r--r--   0        0        0  2090452 2020-02-02 00:00:00.000000 box_packager-0.1.0/docs/assets/ex_qtcowsay.gif
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 box_packager-0.1.0/src/box/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 box_packager-0.1.0/src/box/__main__.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 box_packager-0.1.0/src/box/cleaner.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 box_packager-0.1.0/src/box/cli.py
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 box_packager-0.1.0/src/box/config.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 box_packager-0.1.0/src/box/formatters.py
--rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 box_packager-0.1.0/src/box/initialization.py
--rw-r--r--   0        0        0    11648 2020-02-02 00:00:00.000000 box_packager-0.1.0/src/box/packager.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 box_packager-0.1.0/src/box/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/cli/test_box.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/cli/test_cli_clean.py
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/cli/test_cli_initialization.py
--rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/cli/test_cli_packager.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/cli/test_cli_uninitialize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/data/__init__.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/data/pyapp-source.tar.gz
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/data/pyapp-v0.14.0/source.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/func/__init__.py
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/func/test_config.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/func/test_initialization.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/func/test_packager.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 box_packager-0.1.0/tests/func/test_utils.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 box_packager-0.1.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 box_packager-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 box_packager-0.1.0/README.md
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 box_packager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 box_packager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 box_packager-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 box_packager-0.2.0/.python-version
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 box_packager-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 box_packager-0.2.0/mkdocs.yml
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 box_packager-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 box_packager-0.2.0/requirements.lock
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 box_packager-0.2.0/.github/workflows/integration_tests.yml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 box_packager-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 box_packager-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/changelog.md
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/cli.md
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/examples.md
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/guide.md
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/index.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/.includes/build.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/.includes/install.md
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/.includes/installer_cli.md
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/.includes/installer_gui.md
+-rw-r--r--   0        0        0  2090452 2020-02-02 00:00:00.000000 box_packager-0.2.0/docs/assets/ex_qtcowsay.gif
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/__main__.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/cleaner.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/cli.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/config.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/formatters.py
+-rw-r--r--   0        0        0     9224 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/initialization.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/installer.py
+-rw-r--r--   0        0        0    11766 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/packager.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/installer_utils/__init__.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/installer_utils/linux_hlp.py
+-rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 box_packager-0.2.0/src/box/installer_utils/windows_hlp.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/cli/test_box.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/cli/test_cli_clean.py
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/cli/test_cli_initialization.py
+-rw-r--r--   0        0        0     7771 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/cli/test_cli_installer.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/cli/test_cli_packager.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/cli/test_cli_uninitialize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/data/__init__.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/data/pyapp-source.tar.gz
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/data/pyapp-v0.14.0/source.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/unit/test_config.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/unit/test_initialization.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/unit/test_installer.py
+-rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/unit/test_packager.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 box_packager-0.2.0/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 box_packager-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 box_packager-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 box_packager-0.2.0/README.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 box_packager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 box_packager-0.2.0/PKG-INFO
```

### Comparing `box_packager-0.1.0/mkdocs.yml` & `box_packager-0.2.0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 site_name: "box"
 
 theme:
   name: material
   features:
     - content.code.copy
     - content.code.select
+    - content.tabs.link
     - navigation.footer
   palette:
     # Palette toggle for dark mode
     - scheme: slate
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
```

### Comparing `box_packager-0.1.0/requirements-dev.lock` & `box_packager-0.2.0/requirements-dev.lock`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: true
 #   with-sources: false
 
 -e file:.
+    # via file:///-
 babel==2.14.0
     # via mkdocs-material
 bracex==2.4
     # via wcmatch
-build==1.0.3
+build==1.2.1
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via box-packager
     # via mkdocs
     # via mkdocs-click
     # via rich-click
 colorama==0.4.6
     # via box-packager
     # via mkdocs-material
 coverage==7.4.3
+    # via coverage
     # via pytest-cov
 ghp-import==2.1.0
     # via mkdocs
 gitdb==4.0.11
     # via gitpython
 gitpython==3.1.42
 idna==3.6
```

### Comparing `box_packager-0.1.0/requirements.lock` & `box_packager-0.2.0/requirements.lock`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: true
 #   with-sources: false
 
 -e file:.
+    # via file:///-
 babel==2.14.0
     # via mkdocs-material
 bracex==2.4
     # via wcmatch
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
```

### Comparing `box_packager-0.1.0/.github/workflows/integration_tests.yml` & `box_packager-0.2.0/.github/workflows/integration_tests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -32,18 +32,20 @@
         repository: trappitsch/qtcowsay
         path: "qtcowsay"
     - name: Test build qtcowsay (GUI)
       run: |
         cd qtcowsay
         box init -q -b build
         box package
+        box installer
     - name: Checkout cowsay-python
       uses: actions/checkout@v4
       with:
           repository: VaasuDevanS/cowsay-python
           path: "cowsay"
     - name: Test build cowsay-python (CLI)
       run: |
         cd cowsay
         git checkout 3db622cefd8b11620ece7386d4151b5e734b078b
         box init -q -b build
         box package
+        box installer
```

### Comparing `box_packager-0.1.0/.github/workflows/tests.yml` & `box_packager-0.2.0/.github/workflows/tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -16,15 +16,20 @@
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - name: Checkout repo
       uses: actions/checkout@v4
     - name: Install the latest version of rye
-      uses: eifinger/setup-rye@v1
+      uses: eifinger/setup-rye@v2
+      with:
+        github-token: ${{ secrets.GITHUB_TOKEN }}
+    - name: Setup rye config - required for tests
+      run: |
+        rye config --set default.author="Firstname Lastname <email@domain.com>"
     - name: Sync Rye
       run: |
         rye pin ${{ matrix.python-version }}
         rye sync
     - name: Run Tests for python interface
       run: rye run test
     - name: Run Lint on one python
```

### Comparing `box_packager-0.1.0/docs/examples.md` & `box_packager-0.2.0/docs/examples.md`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/docs/guide.md` & `box_packager-0.2.0/docs/guide.md`

 * *Files 8% similar despite different names*

```diff
@@ -91,14 +91,58 @@
 An information about this will be printed.
 
 To re-copy the local source into the `build` folder,
 the `box` project needs to be cleaned first.
 Then run `box package -p LOCAL_SOURCE` again,
 where `LOCAL_SOURCE` is the path to the local source as described above.
 
+
+## Installer
+
+Your packaged project is simply a file.
+However, you might want to distribute an installer to your users.
+Installers can be created simply in box by typing:
+
+```
+box installer
+```
+
+Optionally, you can run the installer with the `-v`/`--verbose` flag.
+This will provide you with more information on the process, if available.
+
+This will create an installer based on the platform and type of project for you
+in the `target/release` folder.
+
+!!! note
+    A packaged binary must already be present in the `target/release` folder.
+    If it isn't, you will be prompted to package the project first.
+
+### CLIs
+
+{% include-markdown ".includes/installer_cli.md" %}
+
+### GUIs
+
+In order to package a GUI,
+you should have an icon file in the `assets` folder in your project.
+For Linux, the icon file should be a `svg`, `png`, `jpg`, or `jpeg` file.
+For Windows, the icon file should be a `ico` file.
+In either case, the icon file(s) must be named `icon.<ext>`,
+where `<ext>` is the file extension.
+If multiple icons are available,
+order of preference is `svg`, `png`, `jpg`, `jpeg`.
+
+!!! note
+    Creating an installer will associate the GUI with the PyApp executable, not with the actual Python process.
+    Please read up on what you need to do in order to have the icon show up in the taskbar or dock.
+    For `PyQt`, some information can, e.g., be found
+    [here](https://www.geeksforgeeks.org/how-to-set-icon-to-a-window-in-pyqt5/).
+
+{% include-markdown ".includes/installer_gui.md" %}
+
 ## Cleaning your project
 
 If you want to clean the project, run:
 
 ```
 box clean
 ```
```

### Comparing `box_packager-0.1.0/docs/index.md` & `box_packager-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/docs/.includes/install.md` & `box_packager-0.2.0/docs/.includes/install.md`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/docs/assets/ex_qtcowsay.gif` & `box_packager-0.2.0/docs/assets/ex_qtcowsay.gif`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/src/box/cleaner.py` & `box_packager-0.2.0/src/box/cleaner.py`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/src/box/cli.py` & `box_packager-0.2.0/src/box/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+"""CLI for box-packager."""
+
+from pathlib import Path
+
 import rich_click as click
 
+import box
 from box.cleaner import CleanProject
 from box.config import uninitialize
 from box.initialization import InitializeProject
+from box.installer import CreateInstaller
 import box.formatters as fmt
 from box.packager import PackageApp
 import box.utils as ut
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
@@ -128,14 +134,42 @@
     fmt.success(
         f"Project successfully packaged.\n"
         f"You can find the executable file {binary_file.name} "
         f"in the `target/release` folder."
     )
 
 
+@cli.command(name="installer")
+@click.option(
+    "-v",
+    "--verbose",
+    default=False,
+    is_flag=True,
+    help="Flag to enable verbose mode.",
+)
+def installer(verbose):
+    """Create an installer for the project."""
+    ut.check_boxproject()
+    my_installer = CreateInstaller(verbose=verbose)
+    my_installer.create_installer()
+    inst_name = my_installer.installer_name
+    if inst_name is not None:
+        if Path(box.RELEASE_DIR_NAME).joinpath(inst_name).exists():
+            fmt.success(
+                f"Installer successfully created.\n"
+                f"You can find the installer file {inst_name} "
+                f"in the `target/release` folder."
+            )
+        else:
+            raise click.ClickException(
+                "Installer was not created. "
+                "Run with `box installer -v` to get verbose feedback."
+            )
+
+
 @cli.command(name="clean")
 @click.option(
     "-d",
     "--dist",
     default=False,
     is_flag=True,
     help="Flag to clean the `dist` folder where the python build lives.",
```

### Comparing `box_packager-0.1.0/src/box/config.py` & `box_packager-0.2.0/src/box/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 
     @property
     def app_entry_type(self):
         """Return the entry type of the project for PyApp."""
         return self._pyproject["tool"]["box"]["entry_type"]
 
     @property
+    def author(self) -> str:
+        """Return the (first) author of the project."""
+        return self._project["authors"][0]["name"]
+
+    @property
     def builder(self) -> str:
         """Return the builder of the project."""
         return self._pyproject["tool"]["box"]["builder"]
 
     @property
     def is_box_project(self):
         """Return if this folder is a box project or not."""
```

### Comparing `box_packager-0.1.0/src/box/formatters.py` & `box_packager-0.2.0/src/box/formatters.py`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/src/box/initialization.py` & `box_packager-0.2.0/src/box/initialization.py`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/src/box/packager.py` & `box_packager-0.2.0/src/box/packager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Build the project with PyApp
 
 import os
+import sys
 from pathlib import Path
 import shutil
 import subprocess
 import tarfile
 from typing import List, Union
 import urllib.request
 
@@ -230,21 +231,25 @@
         )
 
         # create release folder if it does not exist
         self._release_dir.mkdir(exist_ok=True, parents=True)
 
         # move package to dev folder and rename it to module_name
         binary_path = self._pyapp_path.joinpath("target/release/pyapp")
-        suffix = ""
+        if sys.platform == "win32":
+            binary_path = binary_path.with_suffix(".exe")
+
         if not binary_path.is_file():
-            binary_path = binary_path.with_suffix(".exe")  # we are probably on windows!
-            suffix = ".exe"
-        self._binary_name = self._release_dir.joinpath(
-            self.config.name_pkg
-        ).with_suffix(suffix)
+            raise click.ClickException(
+                "No binary created. Please check build process with `box package -v`."
+            )
+
+        self._binary_name = self._release_dir.joinpath(self.config.name).with_suffix(
+            binary_path.suffix
+        )
         shutil.move(binary_path, self._binary_name)
 
     def _set_env(self):
         """Set the environment for packaging the project with PyApp."""
         # clean all variables startying with `PYAPP` from environment
         for var in list(os.environ):
             if var.startswith("PYAPP"):
@@ -267,15 +272,15 @@
         # set variables
         os.environ["PYAPP_PROJECT_NAME"] = self.config.name_pkg
         os.environ["PYAPP_PROJECT_VERSION"] = self.config.version
         os.environ["PYAPP_PROJECT_PATH"] = str(dist_file)
         os.environ[var_app_entry] = self.config.app_entry
         os.environ["PYAPP_PYTHON_VERSION"] = py_version
         if value := self.config.optional_dependencies:
-            os.environ["PYAPP_PIP_OPTIONAL_DEPS"] = value
+            os.environ["PYAPP_PROJECT_FEATURES"] = value
         optional_pyapp_vars = self.config.optional_pyapp_variables
         for key, value in optional_pyapp_vars.items():
             os.environ[key] = value
         if self.config.is_gui:
             os.environ["PYAPP_IS_GUI"] = "1"
 
     # STATIC METHODS #
```

### Comparing `box_packager-0.1.0/src/box/utils.py` & `box_packager-0.2.0/src/box/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Utility and helper functions
 
 from contextlib import contextmanager
 import os
 from pathlib import Path
+import subprocess
 
 from rich_click import ClickException
 
 from box.config import PyProjectParser
 
 # available app entry types that are used in box
 PYAPP_APP_ENTRY_TYPES = ["spec", "module", "script", "notebook"]
 
-
 # supported Python versions. Default will be set to last entry (latest).
 PYAPP_PYTHON_VERSIONS = (
     "pypy2.7",
     "pypy3.9",
     "pypy3.10",
     "3.7",
     "3.8",
@@ -41,15 +41,25 @@
 
 
 def cmd_python() -> str:
     """Get the command to run Python on the current operating system.
 
     :return: Command to run Python
     """
-    return "py" if is_windows() else "python"
+    if is_windows():
+        try:
+            subprocess.run(
+                ["py", "--version"],
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+            )
+            return "py"
+        except FileNotFoundError:
+            pass
+    return "python"
 
 
 def is_windows() -> bool:
     """Check if the operating system is Windows.
 
     :return: True if Windows, False otherwise
     """
```

### Comparing `box_packager-0.1.0/tests/conftest.py` & `box_packager-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/tests/cli/test_cli_clean.py` & `box_packager-0.2.0/tests/cli/test_cli_clean.py`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/tests/cli/test_cli_initialization.py` & `box_packager-0.2.0/tests/cli/test_cli_initialization.py`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/tests/cli/test_cli_packager.py` & `box_packager-0.2.0/tests/cli/test_cli_packager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Test builder with CLI - system calls mostly mocked, full build in unit tests
 
 import os
 import shutil
+import sys
 from pathlib import Path
 import urllib.request
 
 from click.testing import CliRunner
 import pytest
 
 from box.cli import cli
@@ -43,15 +44,16 @@
     pyapp_dir = build_dir.joinpath("pyapp-v1.2.3")
     pyapp_dir.mkdir(parents=True)
     build_dir.joinpath("pyapp-source.tar.gz").touch()
 
     # create fake binary
     cargo_target = build_dir.joinpath("pyapp-v1.2.3/target/release")
     cargo_target.mkdir(parents=True)
-    cargo_target.joinpath("pyapp").touch()
+    exename = "pyapp.exe" if sys.platform == "win32" else "pyapp"
+    cargo_target.joinpath(exename).touch()
 
     runner = CliRunner()
     result = runner.invoke(cli, cmd)
     assert result.exit_code == 0
     assert "Project successfully packaged." in result.output
 
     # assert system calls
```

### Comparing `box_packager-0.1.0/tests/cli/test_cli_uninitialize.py` & `box_packager-0.2.0/tests/cli/test_cli_uninitialize.py`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/tests/func/test_config.py` & `box_packager-0.2.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/tests/func/test_initialization.py` & `box_packager-0.2.0/tests/unit/test_initialization.py`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/tests/func/test_packager.py` & `box_packager-0.2.0/tests/unit/test_packager.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,14 +236,17 @@
     with pytest.raises(click.ClickException):
         packager._get_pyapp(local_source="wrong_source.tar.gz")
 
 
 @pytest.mark.parametrize("binary_extensions", [".exe", ""])
 def test_package_pyapp_cargo_and_move(rye_project, mocker, binary_extensions):
     """Ensure cargo is called correctly and final binary moved to the right folder."""
+    # mock sys.platform based on binary extension
+    mocker.patch("sys.platform", "win32" if binary_extensions == ".exe" else "linux")
+
     pyapp_path = rye_project.joinpath("build/pyapp-vx.y.z")
     cargo_binary_folder = pyapp_path.joinpath("target/release")
     cargo_binary_folder.mkdir(parents=True)
 
     pyapp_binary = cargo_binary_folder.joinpath("pyapp").with_suffix(binary_extensions)
     pyapp_binary.write_text("not really a binary")
 
@@ -257,21 +260,37 @@
 
     sp_run_mock.assert_called_with(
         ["cargo", "build", "--release"],
         cwd=pyapp_path,
         stdout=sp_devnull_mock,
         stderr=sp_devnull_mock,
     )
-    exp_binary = rye_project.joinpath(
-        f"target/release/{rye_project.name}{binary_extensions}"
-    )
+    conf = PyProjectParser()
+    exp_binary = rye_project.joinpath(f"target/release/{conf.name}{binary_extensions}")
     assert exp_binary.is_file()
     assert exp_binary.read_text() == "not really a binary"
 
 
+def test_package_pyapp_no_binary_created(rye_project, mocker):
+    """Raise click exception if no binary was created by cargo."""
+    pyapp_path = rye_project.joinpath("build/pyapp-vx.y.z")
+    cargo_binary_folder = pyapp_path.joinpath("target/release")
+    cargo_binary_folder.mkdir(parents=True)
+
+    # mock subprocess.run
+    mocker.patch("subprocess.run")
+    mocker.patch("subprocess.DEVNULL")
+
+    packager = PackageApp()
+    packager._pyapp_path = pyapp_path
+    with pytest.raises(click.ClickException) as e:
+        packager._package_pyapp()
+    assert "box package -v" in e.value.args[0]  # some useful help on error
+
+
 @pytest.mark.parametrize("app_entry_type", ut.PYAPP_APP_ENTRY_TYPES)
 @pytest.mark.parametrize("opt_deps", ["gui", None])
 @pytest.mark.parametrize("opt_pyapp_vars", ["PYAPP_SOMETHING 2", None])
 @pytest.mark.parametrize("gui", [True, False])
 def test_set_env(rye_project, mocker, app_entry_type, opt_deps, opt_pyapp_vars, gui):
     """Set environment for `PyApp` packaging."""
     config = PyProjectParser()
@@ -300,15 +319,15 @@
     package_name = rye_project.name.replace("-", "_").lower()
     assert os.environ["PYAPP_PROJECT_NAME"] == package_name
     assert os.environ["PYAPP_PROJECT_VERSION"] == "0.1.0"
     assert os.environ["PYAPP_PROJECT_PATH"] == str(dist_file)
     assert os.environ[f"PYAPP_EXEC_{app_entry_type.upper()}"] == exec_spec
     assert os.environ["PYAPP_PYTHON_VERSION"] == ut.PYAPP_PYTHON_VERSIONS[-1]
     if opt_deps:
-        assert os.environ["PYAPP_PIP_OPTIONAL_DEPS"] == opt_deps
+        assert os.environ["PYAPP_PROJECT_FEATURES"] == opt_deps
     if opt_pyapp_vars:
         assert os.environ["PYAPP_SOMETHING"] == "2"
     if gui:
         assert os.environ["PYAPP_IS_GUI"] == "1"
     else:  # no such variable should be set!
         with pytest.raises(KeyError):
             _ = os.environ["PYAPP_IS_GUI"]
```

### Comparing `box_packager-0.1.0/tests/func/test_utils.py` & `box_packager-0.2.0/tests/unit/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,17 +12,25 @@
     "os_python",
     [["nt", "py"], ["posix", "python"]],
 )
 def test_cmd_python(mocker, os_python):
     """Get python on mulitple operating systems."""
     # mock os.name
     mocker.patch("os.name", os_python[0])
+    mocker.patch("subprocess.run")
     assert ut.cmd_python() == os_python[1]
 
 
+def test_cmd_python_py_not_found(mocker):
+    """Default to python on windows if py not found."""
+    mocker.patch("os.name", "nt")
+    mocker.patch("subprocess.run", side_effect=FileNotFoundError)
+    assert ut.cmd_python() == "python"
+
+
 def test_check_boxproject(rye_project):
     """Check if the box project is already initialized."""
     ut.check_boxproject()
 
 
 def test_check_boxproject_error(rye_project_no_box):
     """Raise a click exception if the box project is not found."""
```

### Comparing `box_packager-0.1.0/.gitignore` & `box_packager-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/LICENSE.txt` & `box_packager-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/README.md` & `box_packager-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `box_packager-0.1.0/pyproject.toml` & `box_packager-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "box-packager"
-version = "0.1.0"
+version = "0.2.0"
 description = "Automatic packaging and installers of your GUI with PyApp"
 readme = "README.md"
 authors = [
     { name = "Reto Trappitsch", email = "reto@galactic-forensics.space" }
 ]
 dependencies = [
     "click>=8.1.7",
     "tomlkit>=0.12.3",
     "rich-click>=1.7.3",
     "rich>=13.7.0",
     "colorama>=0.4.6",
+    "box-packager>=0.1.0",
 ]
 requires-python = ">= 3.8"
 license = { text = "MIT" }
 
 [project.scripts]
 box = "box.cli:cli"
 
@@ -42,15 +43,15 @@
 managed = true
 dev-dependencies = [
     "pytest>=8.0.0",
     "ruff>=0.1.15",
     "pytest-cov>=4.1.0",
     "pytest-mock>=3.12.0",
     "gitpython>=3.1.42",
-    "build>=1.0.3",
+    "build>=1.2.1",
 ]
 
 [tool.rye.scripts]
 test = "pytest -m 'not unit'"
 test_cov = "pytest -m 'not unit' --cov --cov-report xml"
 
 [tool.hatch.metadata]
@@ -64,11 +65,7 @@
 testpaths = "tests"
 
 [tool.pytest.ini_options]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "unit: marks unit tests, which build a full PyApp with cargo (deselect with '-m \"not unit\"')",
 ]
-
-[tool.box]
-builder = "rye"
-app_entry = "box.cli:cli"
```

### Comparing `box_packager-0.1.0/PKG-INFO` & `box_packager-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: box-packager
-Version: 0.1.0
+Version: 0.2.0
 Summary: Automatic packaging and installers of your GUI with PyApp
 Project-URL: Homepage, https://github.com/trappitsc/box
 Project-URL: Documentation, https://box.readthedocs.io/
 Project-URL: Changelog, https://github.com/trappitsc/box/releases
 Project-URL: Issues, https://github.com/trappitsc/box/issues
 Project-URL: CI, https://github.com/trappitsc/box/actions
 Author-email: Reto Trappitsch <reto@galactic-forensics.space>
 License: MIT
 License-File: LICENSE.txt
 Requires-Python: >=3.8
+Requires-Dist: box-packager>=0.1.0
 Requires-Dist: click>=8.1.7
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: rich-click>=1.7.3
 Requires-Dist: rich>=13.7.0
 Requires-Dist: tomlkit>=0.12.3
 Provides-Extra: docs
 Requires-Dist: mkdocs-click>=0.8.1; extra == 'docs'
```

