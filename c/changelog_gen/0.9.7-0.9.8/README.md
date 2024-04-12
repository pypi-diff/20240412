# Comparing `tmp/changelog_gen-0.9.7.tar.gz` & `tmp/changelog_gen-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog_gen-0.9.7.tar", max compression
+gzip compressed data, was "changelog_gen-0.9.8.tar", max compression
```

## Comparing `changelog_gen-0.9.7.tar` & `changelog_gen-0.9.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11307 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/LICENSE
--rw-r--r--   0        0        0    12368 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/README.md
--rw-r--r--   0        0        0        0 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/changelog_gen/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/changelog_gen/cli/__init__.py
--rw-r--r--   0        0        0     9411 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/changelog_gen/cli/command.py
--rw-r--r--   0        0        0      314 2024-04-08 12:33:08.213795 changelog_gen-0.9.7/changelog_gen/cli/util.py
--rw-r--r--   0        0        0    12447 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/config.py
--rw-r--r--   0        0        0      528 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/errors.py
--rw-r--r--   0        0        0     8567 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/extractor.py
--rw-r--r--   0        0        0     2898 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/post_processor.py
--rw-r--r--   0        0        0     4225 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/vcs.py
--rw-r--r--   0        0        0     4366 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/version.py
--rw-r--r--   0        0        0     7316 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/changelog_gen/writer.py
--rw-r--r--   0        0        0     2846 2024-04-08 12:33:08.217795 changelog_gen-0.9.7/pyproject.toml
--rw-r--r--   0        0        0    13402 1970-01-01 00:00:00.000000 changelog_gen-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/LICENSE
+-rw-r--r--   0        0        0    12368 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/cli/__init__.py
+-rw-r--r--   0        0        0    11459 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/cli/command.py
+-rw-r--r--   0        0        0      551 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/cli/util.py
+-rw-r--r--   0        0        0    12529 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/config.py
+-rw-r--r--   0        0        0      528 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/errors.py
+-rw-r--r--   0        0        0     8569 2024-04-12 14:27:32.179276 changelog_gen-0.9.8/changelog_gen/extractor.py
+-rw-r--r--   0        0        0     2898 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/changelog_gen/post_processor.py
+-rw-r--r--   0        0        0     6013 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/changelog_gen/vcs.py
+-rw-r--r--   0        0        0     4366 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/changelog_gen/version.py
+-rw-r--r--   0        0        0     7316 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/changelog_gen/writer.py
+-rw-r--r--   0        0        0     2846 2024-04-12 14:27:32.183276 changelog_gen-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0    13402 1970-01-01 00:00:00.000000 changelog_gen-0.9.8/PKG-INFO
```

### Comparing `changelog_gen-0.9.7/LICENSE` & `changelog_gen-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.7/README.md` & `changelog_gen-0.9.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Changelog Generator - v0.9.7
+# Changelog Generator - v0.9.8
 [![image](https://img.shields.io/pypi/v/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/l/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/pyversions/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 ![style](https://github.com/NRWLDev/changelog-gen/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/changelog-gen/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/changelog-gen/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/changelog-gen)
```

### Comparing `changelog_gen-0.9.7/changelog_gen/cli/command.py` & `changelog_gen-0.9.8/changelog_gen/cli/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from __future__ import annotations
 
+import contextlib
 import importlib.metadata
 import json
 import logging
 import logging.config
+import shlex
+import subprocess
 from datetime import datetime, timezone
 from pathlib import Path
+from tempfile import NamedTemporaryFile
 from typing import Optional
 from warnings import warn
 
 import click
 import rtoml
 import typer
 from rich.logging import RichHandler
@@ -31,14 +35,15 @@
 VERBOSITY = {
     0: logging.ERROR,
     1: logging.WARNING,
     2: logging.INFO,
     3: logging.DEBUG,
 }
 
+tempfile_prefix = "_tmp_changelog"
 
 def setup_logging(verbose: int = 0) -> None:
     """Configure the logging."""
     logging.basicConfig(
         level=VERBOSITY.get(verbose, logging.DEBUG),
         format="%(message)s",
         datefmt="[%X]",
@@ -87,14 +92,28 @@
     if dry_run:
         return
 
     if info["dirty"] and not cfg.allow_dirty:
         logger.error("Working directory is not clean. Use `allow_dirty` configuration to ignore.")
         raise typer.Exit(code=1)
 
+    if info["missing_local"] and not cfg.allow_missing:
+        logger.error(
+            "Current local branch is missing commits from remote %s. Use `allow_missing` configuration to ignore.",
+            info["branch"],
+        )
+        raise typer.Exit(code=1)
+
+    if info["missing_remote"] and not cfg.allow_missing:
+        logger.error(
+            "Current remote branch is missing commits from local %s. Use `allow_missing` configuration to ignore.",
+            info["branch"],
+        )
+        raise typer.Exit(code=1)
+
     allowed_branches = cfg.allowed_branches
     if allowed_branches and info["branch"] not in allowed_branches:
         logger.error("Current branch not in allowed generation branches.")
         raise typer.Exit(code=1)
 
 
 @init_app.command("changelog-init")
@@ -156,19 +175,21 @@
     ),
     post_process_auth_env: Optional[str] = typer.Option(
         None,
         help="Name of the ENV variable that contains the rest API basic auth content.",
     ),
     date_format: Optional[str] = typer.Option(None, help="The date format for strftime - empty string allowed."),
     *,
-    dry_run: bool = typer.Option(False, help="Don't write release notes, check for errors."),  # noqa: FBT003
+    dry_run: bool = typer.Option(default=False, help="Don't write release notes, check for errors."),
     allow_dirty: Optional[bool] = typer.Option(None, help="Don't abort if branch contains uncommitted changes."),
+    allow_missing: Optional[bool] = typer.Option(None, help="Don't abort if branch missing commits on origin."),
     release: Optional[bool] = typer.Option(None, help="Use bumpversion to tag the release."),
     commit: Optional[bool] = typer.Option(None, help="Commit changes made to changelog after writing."),
     reject_empty: Optional[bool] = typer.Option(None, help="Don't accept changes if there are no release notes."),
+    interactive: Optional[bool] = typer.Option(default=True, help="Open changes in an editor before confirmation."),
     verbose: int = typer.Option(0, "-v", "--verbose", help="Set output verbosity.", count=True, max=3),
     _version: Optional[bool] = typer.Option(
         None,
         "--version",
         callback=_version_callback,
         help="Print version and exit.",
     ),
@@ -183,35 +204,71 @@
             FutureWarning,
             stacklevel=2,
         )
     setup_logging(verbose)
     cfg = config.read(
         release=release,
         allow_dirty=allow_dirty,
+        allow_missing=allow_missing,
         commit=commit,
         reject_empty=reject_empty,
         date_format=date_format,
         post_process_url=post_process_url,
         post_process_auth_env=post_process_auth_env,
         verbose=verbose,
     )
 
     try:
-        _gen(cfg, version_part, version_tag, dry_run=dry_run)
+        _gen(cfg, version_part, version_tag, dry_run=dry_run, interactive=interactive)
     except errors.ChangelogException as ex:
         logger.error("%s", ex)  # noqa: TRY400
         raise typer.Exit(code=1) from ex
 
 
+def create_with_editor(content: str, extension: writer.Extension) -> str:
+    """Open temporary file in editor to allow modifications."""
+    editor = util.get_editor()
+    tmpfile = NamedTemporaryFile(
+        mode="w",
+        encoding="UTF-8",
+        prefix=tempfile_prefix,
+        suffix=f".{extension.value}",
+        delete=False,
+    )
+    try:
+        with tmpfile as f:
+            f.write(content)
+
+        editor = [part.format(tmpfile.name) for part in shlex.split(editor)]
+        if not any(tmpfile.name in part for part in editor):
+            editor.append(tmpfile.name)
+
+        try:
+            subprocess.call(editor)  # noqa: S603
+        except OSError as e:
+            logger.error("Error: could not open editor!")  # noqa: TRY400
+            raise typer.Exit(code=1) from e
+
+        with Path(tmpfile.name).open() as f:
+            content = f.read()
+
+    finally:
+        with contextlib.suppress(OSError):
+            Path(tmpfile.name).unlink()
+
+    return content
+
+
 def _gen(
     cfg: config.Config,
     version_part: str | None = None,
     version_tag: str | None = None,
     *,
     dry_run: bool = False,
+    interactive: bool = True,
 ) -> None:
     bv = BumpVersion(verbose=cfg.verbose, dry_run=dry_run)
     git = Git(dry_run=dry_run)
 
     extension = util.detect_extension()
 
     if extension is None:
@@ -243,15 +300,17 @@
         version_string += f" {datetime.now(timezone.utc).strftime(date_fmt)}"
 
     w = writer.new_writer(extension, cfg, dry_run=dry_run)
 
     w.add_version(version_string)
     w.consume(cfg.type_headers, sections)
 
-    logger.error(str(w))
+    changes = create_with_editor(str(w), extension) if interactive else str(w)
+
+    logger.error(changes)
 
     processed = _finalise(w, e, version_tag, extension, cfg, dry_run=dry_run)
 
     post_process = cfg.post_process
     if post_process and processed:
         unique_issues = [r for r in unique_issues if not r.startswith("__")]
         per_issue_post_process(post_process, sorted(unique_issues), version_tag, dry_run=dry_run)
```

### Comparing `changelog_gen-0.9.7/changelog_gen/config.py` & `changelog_gen-0.9.8/changelog_gen/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,15 @@
 
     allowed_branches: list[str] = dataclasses.field(default_factory=list)
     commit_types: dict[str, CommitType] = dataclasses.field(default_factory=lambda: SUPPORTED_TYPES)
 
     release: bool = False
     commit: bool = False
     allow_dirty: bool = False
+    allow_missing: bool = False
     reject_empty: bool = False
 
     post_process: PostProcessConfig | None = None
 
     @property
     def semver_mappings(self: typing.Self) -> dict[str, str]:
         """Generate `type: semver` mapping from commit types."""
@@ -267,14 +268,15 @@
         ("commit_types", extract_dict_value),
         ("sections", extract_dict_value),
         ("section_mapping", extract_dict_value),
         ("post_process", extract_dict_value),
         ("release", extract_boolean_value),
         ("commit", extract_boolean_value),
         ("allow_dirty", extract_boolean_value),
+        ("allow_missing", extract_boolean_value),
         ("reject_empty", extract_boolean_value),
     ]:
         value = extract_func(parser, valuename)
         if value:
             cfg[valuename] = value
 
     if cfg != {}:
```

### Comparing `changelog_gen-0.9.7/changelog_gen/errors.py` & `changelog_gen-0.9.8/changelog_gen/errors.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.7/changelog_gen/extractor.py` & `changelog_gen-0.9.8/changelog_gen/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         # find tag from current version
         tag = self.git.find_tag(current_version)
         logs = self.git.get_logs(tag)
 
         # Build a conventional commit regex based on configured sections
         #   ^(build|chore|ci|docs|feat|fix|perf|refactor|revert|style|test){1}(\([\w\-\.]+\))?(!)?: ([\w ])+([\s\S]*)
         types = "|".join(self.type_headers.keys())
-        reg = re.compile(rf"^({types}){{1}}(\([\w\-\.]+\))?(!)?: ([\w .,`\-\/]+)+([\s\S]*)")
+        reg = re.compile(rf"^({types}){{1}}(\([\w\-\.]+\))?(!)?: ([\w .,\?`\-\/]+)+([\s\S]*)")
         logger.warning("Extracting commit log changes.")
 
         for i, (short_hash, commit_hash, log) in enumerate(logs):
             m = reg.match(log)
             if m is None:
                 logger.debug("  Skipping commit log (not conventional): %s", log.strip())
             if m:
```

### Comparing `changelog_gen-0.9.7/changelog_gen/post_processor.py` & `changelog_gen-0.9.8/changelog_gen/post_processor.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.7/changelog_gen/vcs.py` & `changelog_gen-0.9.8/changelog_gen/vcs.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,60 @@
 class Git:
     """VCS implementation for git repositories."""
 
     def __init__(self: T, *, commit: bool = True, dry_run: bool = False) -> None:
         self._commit = commit
         self.dry_run = dry_run
 
+    def _get_missing_local(self: T, branch: list[str]) -> list[str]:
+        try:
+            return (
+                subprocess.check_output(
+                    [  # noqa: S603, S607
+                        "git",
+                        "rev-list",
+                        f"HEAD..origin/{branch[0]}",
+                    ],
+                    stderr=subprocess.STDOUT,
+                )
+                .decode()
+                .strip()
+                .split("\n")
+            )
+        except subprocess.CalledProcessError as e:
+            msg = (
+                f"Unable to get remote status: {e.output.decode().strip()}"
+                if e.output
+                else "Unable to get current remote status."
+            )
+            raise errors.VcsError(msg) from e
+
+    def _get_missing_remote(self: T, branch: list[str]) -> list[str]:
+        try:
+            return (
+                subprocess.check_output(
+                    [  # noqa: S603, S607
+                        "git",
+                        "rev-list",
+                        f"origin/{branch[0]}..HEAD",
+                    ],
+                    stderr=subprocess.STDOUT,
+                )
+                .decode()
+                .strip()
+                .split("\n")
+            )
+        except subprocess.CalledProcessError as e:
+            msg = (
+                f"Unable to get remote status: {e.output.decode().strip()}"
+                if e.output
+                else "Unable to get current remote status."
+            )
+            raise errors.VcsError(msg) from e
+
     def get_current_info(self: T) -> dict[str, str]:
         """Get current state info from git."""
         changed_files = (
             subprocess.check_output(
                 ["git", "status", "-s"],  # noqa: S603, S607
                 stderr=subprocess.STDOUT,
             )
@@ -49,15 +95,20 @@
             msg = (
                 f"Unable to get current git branch: {e.output.decode().strip()}"
                 if e.output
                 else "Unable to get current git branch."
             )
             raise errors.VcsError(msg) from e
 
+        missing_local = self._get_missing_local(branch)
+        missing_remote = self._get_missing_remote(branch)
+
         return {
+            "missing_local": missing_local != [""],
+            "missing_remote": missing_remote != [""],
             "dirty": changed_files != [""],  # Any changed files == dirty
             "branch": branch[0],
         }
 
     def find_tag(self: T, version_string: str) -> str | None:
         """Find a version tag given the version string.
```

### Comparing `changelog_gen-0.9.7/changelog_gen/version.py` & `changelog_gen-0.9.8/changelog_gen/version.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.7/changelog_gen/writer.py` & `changelog_gen-0.9.8/changelog_gen/writer.py`

 * *Files identical despite different names*

### Comparing `changelog_gen-0.9.7/pyproject.toml` & `changelog_gen-0.9.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changelog_gen"
-version = "0.9.7"
+version = "0.9.8"
 description = "Changelog generation tool"
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/EdgyEdgemond/changelog-gen/"
 homepage="https://github.com/EdgyEdgemond/changelog-gen/"
 readme = "README.md"
 
@@ -33,15 +33,15 @@
 pytest-git = "^1.7.0"
 
 # Style
 ruff = "^0.3.0"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.9.7"
+current_version = "0.9.8"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "README.md"
 
 [[tool.bumpversion.files]]
```

### Comparing `changelog_gen-0.9.7/PKG-INFO` & `changelog_gen-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog_gen
-Version: 0.9.7
+Version: 0.9.8
 Summary: Changelog generation tool
 Home-page: https://github.com/EdgyEdgemond/changelog-gen/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: edgy.edgemond@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,15 +20,15 @@
 Requires-Dist: httpx (>=0.25,<0.26)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: rtoml (>=0.9)
 Requires-Dist: typer (>=0,<1)
 Project-URL: Repository, https://github.com/EdgyEdgemond/changelog-gen/
 Description-Content-Type: text/markdown
 
-# Changelog Generator - v0.9.7
+# Changelog Generator - v0.9.8
 [![image](https://img.shields.io/pypi/v/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/l/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 [![image](https://img.shields.io/pypi/pyversions/changelog_gen.svg)](https://pypi.org/project/changelog_gen/)
 ![style](https://github.com/NRWLDev/changelog-gen/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/changelog-gen/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/changelog-gen/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/changelog-gen)
```

