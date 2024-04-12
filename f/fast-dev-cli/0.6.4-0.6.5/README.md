# Comparing `tmp/fast_dev_cli-0.6.4.tar.gz` & `tmp/fast_dev_cli-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_dev_cli-0.6.4.tar", max compression
+gzip compressed data, was "fast_dev_cli-0.6.5.tar", max compression
```

## Comparing `fast_dev_cli-0.6.4.tar` & `fast_dev_cli-0.6.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.6.4/LICENSE
--rw-r--r--   0        0        0     1663 2024-03-07 02:13:22.157917 fast_dev_cli-0.6.4/README.md
--rw-r--r--   0        0        0       76 2024-03-06 06:08:37.265993 fast_dev_cli-0.6.4/fast_dev_cli/__init__.py
--rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.6.4/fast_dev_cli/__main__.py
--rw-r--r--   0        0        0    19833 2024-03-12 14:15:24.546794 fast_dev_cli-0.6.4/fast_dev_cli/cli.py
--rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.6.4/fast_dev_cli/py.typed
--rw-r--r--   0        0        0     1357 2024-04-03 14:29:18.885217 fast_dev_cli-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     2463 1970-01-01 00:00:00.000000 fast_dev_cli-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-06 06:08:37.265617 fast_dev_cli-0.6.5/LICENSE
+-rw-r--r--   0        0        0     1755 2024-04-07 08:42:22.439293 fast_dev_cli-0.6.5/README.md
+-rw-r--r--   0        0        0       76 2024-03-06 06:08:37.265993 fast_dev_cli-0.6.5/fast_dev_cli/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-06 06:08:37.266125 fast_dev_cli-0.6.5/fast_dev_cli/__main__.py
+-rw-r--r--   0        0        0    20941 2024-04-12 03:36:40.730435 fast_dev_cli-0.6.5/fast_dev_cli/cli.py
+-rw-r--r--   0        0        0        0 2024-03-06 06:08:37.266469 fast_dev_cli-0.6.5/fast_dev_cli/py.typed
+-rw-r--r--   0        0        0     1357 2024-04-12 04:18:58.312545 fast_dev_cli-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     2555 1970-01-01 00:00:00.000000 fast_dev_cli-0.6.5/PKG-INFO
```

### Comparing `fast_dev_cli-0.6.4/LICENSE` & `fast_dev_cli-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_dev_cli-0.6.4/README.md` & `fast_dev_cli-0.6.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -30,25 +30,29 @@
 ## Installation
 
 <div class="termy">
 
 ```console
 $ pip install "fast-dev-cli[all]"
 ---> 100%
-Successfully installed fast-dev-cli
+Successfully installed fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage
 ```
 
 </div>
 
 ## Usage
 
 - Lint py code:
 ```bash
 fast lint /path/to/file-or-directory
 ```
+- Check only
+```bash
+fast check
+```
 - Bump up version in pyproject.toml
 ```bash
 fast bump
 ```
 - Run unittest and report coverage
 ```bash
 fast test
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                                  [FastDevCli]
                   TToooollkkiitt ffoorr ppyytthhoonn ccooddee lliinntt//tteesstt//bbuummpp ......
    _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_G_i_t_h_u_b_A_c_t_i_o_n_R_e_s_u_l_t_]_[_C_o_v_e_r_a_g_e
                                     _S_t_a_t_u_s_]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_a_k_e_t_z_h_e_n_g_/_f_a_s_t_-_d_e_v_-_c_l_i ## Requirements
 Python 3.11+ ## Installation
 ```console $ pip install "fast-dev-cli[all]" ---> 100% Successfully installed
-fast-dev-cli ```
+fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage ```
 ## Usage - Lint py code: ```bash fast lint /path/to/file-or-directory ``` -
-Bump up version in pyproject.toml ```bash fast bump ``` - Run unittest and
-report coverage ```bash fast test ``` - Export requirement file and install
-`pip install -r ` ```bash fast sync ``` - Upgrade main/dev dependencies to
-latest version ```bash fast upgrade ```
+Check only ```bash fast check ``` - Bump up version in pyproject.toml ```bash
+fast bump ``` - Run unittest and report coverage ```bash fast test ``` - Export
+requirement file and install `pip install -r ` ```bash fast sync ``` - Upgrade
+main/dev dependencies to latest version ```bash fast upgrade ```
```

### Comparing `fast_dev_cli-0.6.4/fast_dev_cli/cli.py` & `fast_dev_cli-0.6.5/fast_dev_cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 import subprocess
 import sys
 from enum import StrEnum
 from functools import cached_property
 from pathlib import Path
 from subprocess import CompletedProcess
+from typing import Self, Type
 
 __version__ = importlib.metadata.version(Path(__file__).parent.name)
 
 
 def parse_files(args: list[str] | tuple[str, ...]) -> list[str]:
     return [i for i in args if not i.startswith("-")]
 
@@ -125,32 +126,34 @@
         if _exit:
             sys.exit(rc)
         raise Exit(rc)
     return r
 
 
 class DryRun:
-    def __init__(self, _exit=False, dry=False):
+    def __init__(self: Self, _exit=False, dry=False) -> None:
         self.dry = dry
         self._exit = _exit
 
-    def gen(self) -> str:
+    def gen(self: Self) -> str:
         raise NotImplementedError
 
-    def run(self) -> None:
+    def run(self: Self) -> None:
         exit_if_run_failed(self.gen(), _exit=self._exit, dry=self.dry)
 
 
 class BumpUp(DryRun):
     class PartChoices(StrEnum):
         patch = "patch"
         minor = "minor"
         major = "major"
 
-    def __init__(self, commit: bool, part: str, filename=TOML_FILE, dry=False):
+    def __init__(
+        self: Self, commit: bool, part: str, filename=TOML_FILE, dry=False
+    ) -> None:
         self.commit = commit
         self.part = part
         self.filename = filename
         super().__init__(dry=dry)
 
     def get_part(self, s: str) -> str:
         choices: dict[str, str] = {}
@@ -159,15 +162,15 @@
             choices.update({str(i): v, v: v})
         try:
             return choices[s]
         except KeyError as e:
             echo(f"Invalid part: {s!r}")
             raise Exit(1) from e
 
-    def gen(self) -> str:
+    def gen(self: Self) -> str:
         _version = get_current_version()
         filename = self.filename
         echo(f"Current version(@{filename}): {_version}")
         if self.part:
             part = self.get_part(self.part)
         else:
             tip = "Which one?"
@@ -182,41 +185,42 @@
             if part != "patch":
                 cmd += " --tag"
             cmd += " --commit && git push && git push --tags && git log -1"
         else:
             cmd += " --allow-dirty"
         return cmd
 
-    def run(self) -> None:
+    def run(self: Self) -> None:
         super().run()
         if not self.commit and not self.dry:
             new_version = get_current_version(True)
             echo(new_version)
             if self.part != "patch":
                 echo("You may want to pin tag by `fast tag`")
 
 
 @cli.command()
-def version():
+def version() -> None:
     """Show the version of this tool"""
     echo(__version__)
 
 
 @cli.command(name="bump")
 def bump_version(
     part: BumpUp.PartChoices,
     commit: bool = Option(
         False, "--commit", "-c", help="Whether run `git commit` after version changed"
     ),
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
-):
+) -> None:
+    """Bump up version string in pyproject.toml"""
     return BumpUp(commit, part.value, dry=dry).run()
 
 
-def bump():
+def bump() -> None:
     part, commit = "", False
     if args := sys.argv[2:]:
         if "-c" in args or "--commit" in args:
             commit = True
         for a in args:
             if not a.startswith("-"):
                 part = a
@@ -235,30 +239,34 @@
         for _ in range(depth):
             if parent.joinpath(name).exists():
                 return parent
             parent = parent.parent
         return None
 
     @classmethod
-    def get_work_dir(cls, name=TOML_FILE, cwd: Path | None = None) -> Path:
+    def get_work_dir(
+        cls: Type[Self], name=TOML_FILE, cwd: Path | None = None, allow_cwd=False
+    ) -> Path:
         if d := cls.work_dir(name, cwd or Path.cwd(), cls.path_depth):
             return d
+        if allow_cwd:
+            return cls.get_root_dir(cwd)
         raise EnvError(f"{name} not found! Make sure this is a poetry project.")
 
     @classmethod
-    def load_toml_text(cls):
+    def load_toml_text(cls: Type[Self]) -> str:
         toml_file = cls.get_work_dir().resolve() / TOML_FILE  # to be optimize
         return toml_file.read_text("utf8")
 
     @staticmethod
     def python_exec_dir() -> Path:
         return Path(sys.executable).parent
 
     @classmethod
-    def get_root_dir(cls, cwd: Path | None = None) -> Path:
+    def get_root_dir(cls: Type[Self], cwd: Path | None = None) -> Path:
         root = cwd or Path.cwd()
         venv_parent = cls.python_exec_dir().parent.parent
         if root.is_relative_to(venv_parent):
             root = venv_parent
         return root
 
 
@@ -309,15 +317,15 @@
         elif v.startswith(">") or v.startswith("<") or v[0].isdigit():
             echo(f"Ignore bigger/smaller/equal: {line}")
             return True
         return False
 
     @classmethod
     def build_args(
-        cls, package_lines: list[str]
+        cls: Type[Self], package_lines: list[str]
     ) -> tuple[list[str], dict[str, list[str]]]:
         args: list[str] = []  # ['typer[all]', 'fastapi']
         specials: dict[str, list[str]] = {}  # {'--platform linux': ['gunicorn']}
         for line in package_lines:
             if not (m := line.strip()) or m.startswith("#"):
                 continue
             try:
@@ -343,15 +351,15 @@
             if key is not None:
                 specials[key] = specials.get(key, []) + [item]
             else:
                 args.append(item)
         return args, specials
 
     @classmethod
-    def should_with_dev(cls):
+    def should_with_dev(cls: Type[Self]) -> bool:
         text = cls.load_toml_text()
         return cls.DevFlag.new in text or cls.DevFlag.old in text
 
     @staticmethod
     def parse_item(toml_str) -> list[str]:
         lines: list[str] = []
         for line in toml_str.splitlines():
@@ -360,15 +368,15 @@
                     break
             elif line:
                 lines.append(line)
         return lines
 
     @classmethod
     def get_args(
-        cls, toml_text: str | None = None
+        cls: Type[Self], toml_text: str | None = None
     ) -> tuple[list[str], list[str], list[list[str]], str]:
         if toml_text is None:
             toml_text = cls.load_toml_text()
         main_title = "[tool.poetry.dependencies]"
         text = toml_text.split(main_title)[-1]
         dev_flag = "--group dev"
         if (dev_title := cls.DevFlag.new.value) not in text:
@@ -386,15 +394,15 @@
             others.extend([[k] + v for k, v in specials.items()])
         dev_packs, specials = cls.build_args(devs)
         if specials:
             others.extend([[k] + v + [dev_flag] for k, v in specials.items()])
         return prod_packs, dev_packs, others, dev_flag
 
     @classmethod
-    def gen_cmd(cls) -> str:
+    def gen_cmd(cls: Type[Self]) -> str:
         main_args, dev_args, others, dev_flags = cls.get_args()
         return cls.to_cmd(main_args, dev_args, others, dev_flags)
 
     @staticmethod
     def to_cmd(
         main_args: list[str],
         dev_args: list[str],
@@ -409,100 +417,97 @@
             if _upgrade:
                 _upgrade += " && "
             _upgrade += command + dev_flags + " " + " ".join(dev_args)
         for single in others:
             _upgrade += f" && poetry add {' '.join(single)}"
         return _upgrade
 
-    def gen(self) -> str:
+    def gen(self: Self) -> str:
         return self.gen_cmd()
 
 
 @cli.command()
 def upgrade(
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
-):
+) -> None:
     """Upgrade dependencies in pyproject.toml to latest versions"""
     UpgradeDependencies(dry=dry).run()
 
 
 class GitTag(DryRun):
-    def __init__(self, message, dry):
+    def __init__(self: Self, message: str, dry: bool) -> None:
         self.message = message
         super().__init__(dry=dry)
 
-    def has_v_prefix(self) -> bool:
+    def has_v_prefix(self: Self) -> bool:
         return "v" in capture_cmd_output("git tag")
 
-    def should_push(self) -> bool:
+    def should_push(self: Self) -> bool:
         return "git push" in self.git_status
 
-    def gen(self):
+    def gen(self: Self) -> str:
         _version = get_current_version(verbose=False)
         if self.has_v_prefix():
             # Add `v` at prefix to compare with bumpversion tool
             _version = "v" + _version
         cmd = f"git tag -a {_version} -m {self.message!r} && git push --tags"
         if self.should_push():
             cmd += " && git push"
         return cmd
 
     @cached_property
-    def git_status(self) -> str:
+    def git_status(self: Self) -> str:
         return capture_cmd_output("git status")
 
-    def mark_tag(self) -> bool:
+    def mark_tag(self: Self) -> bool:
         if not re.search(r"working (tree|directory) clean", self.git_status):
             run_and_echo("git status")
             echo("ERROR: Please run git commit to make sure working tree is clean!")
             return False
         return bool(super().run())
 
-    def run(self):
+    def run(self: Self) -> None:
         if self.mark_tag() and not self.dry:
             echo("You may want to publish package:\n poetry publish --build")
 
 
 @cli.command()
 def tag(
     message: str = Option("", "-m", "--message"),
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
-):
+) -> None:
     """Run shell command: git tag -a <current-version-in-pyproject.toml> -m {message}"""
     GitTag(message, dry=dry).run()
 
 
 class LintCode(DryRun):
-    def __init__(self, args, check_only=False, _exit=False, dry=False):
+    def __init__(self: Self, args, check_only=False, _exit=False, dry=False) -> None:
         self.args = args
         self.check_only = check_only
         super().__init__(_exit, dry)
 
     @staticmethod
     def check_lint_tool_installed() -> bool:
         return check_call("black --version")
 
     @classmethod
-    def to_cmd(cls, paths=".", check_only=False):
+    def to_cmd(cls: Type[Self], paths=".", check_only=False) -> str:
         cmd = ""
         tools = ["isort --profile=black", "black", "ruff check --fix", "mypy"]
         if check_only:
             tools[0] += " --check-only"
             tools[1] += " --check --fast"
         if check_only or load_bool("NO_FIX"):
             tools[2] = tools[2].replace(" --fix", "")
         if load_bool("SKIP_MYPY"):
             # Sometimes mypy is too slow
             tools = tools[:-1]
         lint_them = " && ".join("{0}{%d} {1}" % i for i in range(2, len(tools) + 2))
         current_path = Path.cwd()
-        try:
-            root = Project.get_work_dir(cwd=current_path)
-        except EnvError:
-            root = Project.get_root_dir(cwd=current_path)
+        root = Project.get_work_dir(cwd=current_path, allow_cwd=True)
         app_name = root.name.replace("-", "_")
         if (app_dir := root / app_name).exists() or (app_dir := root / "app").exists():
             if current_path == app_dir:
                 tools[0] += " --src=."
             elif current_path == root:
                 tools[0] += f" --src={app_dir.name}"
             else:
@@ -520,54 +525,54 @@
                 if check_call("python -c 'import fast_dev_cli'"):
                     command = 'python -m pip install -U "fast_dev_cli[all]"'
                     tip = "You may need to run the following command to install lint tools"
                     secho(f"{tip}:\n\n  {command}\n", fg="yellow")
         cmd += lint_them.format(prefix, paths, *tools)
         return cmd
 
-    def gen(self) -> str:
+    def gen(self: Self) -> str:
         paths = " ".join(self.args) if self.args else "."
         return self.to_cmd(paths, self.check_only)
 
 
-def lint(files=None, dry=False):
+def lint(files=None, dry=False) -> None:
     if files is None:
         files = parse_files(sys.argv[1:])
     LintCode(files, dry=dry).run()
 
 
-def check(files=None, dry=False):
+def check(files=None, dry=False) -> None:
     LintCode(files, check_only=True, _exit=True, dry=dry).run()
 
 
 @cli.command(name="lint")
 def make_style(
     files: list[str],
     check_only: bool = Option(False, "--check-only", "-c"),
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
-):
+) -> None:
     """Run: isort+black+ruff to reformat code and then mypy to check"""
     if isinstance(files, str):
         files = [files]
     if check_only:
         check(files, dry=dry)
     else:
         lint(files, dry=dry)
 
 
 @cli.command(name="check")
 def only_check(
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
-):
+) -> None:
     """Check code style without reformat"""
     check(dry=dry)
 
 
 class Sync(DryRun):
-    def __init__(self, filename: str, extras: str, save: bool, dry=False):
+    def __init__(self: Self, filename: str, extras: str, save: bool, dry=False) -> None:
         self.filename = filename
         self.extras = extras
         self._save = save
         super().__init__(dry=dry)
 
     def gen(self) -> str:
         extras, save = self.extras, self._save
@@ -590,26 +595,47 @@
 def sync(
     filename="dev_requirements.txt",
     extras: str = Option("", "--extras", "-E"),
     save: bool = Option(
         False, "--save", "-s", help="Whether save the requirement file"
     ),
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
-):
+) -> None:
     """Export dependencies by poetry to a txt file then install by pip."""
     Sync(filename, extras, save, dry=dry).run()
 
 
+def _should_run_test_script(path: Path) -> bool:
+    return path.exists()
+
+
 @cli.command()
 def test(
     dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
-):
+) -> None:
     """Run unittest by pytest and report coverage"""
-    cmd = 'coverage run -m pytest -s && coverage report --omit="tests/*" -m'
-    if not is_venv() or not check_call("coverage --version"):
-        sep = " && "
-        cmd = sep.join("poetry run " + i for i in cmd.split(sep))
+    cwd = Path.cwd()
+    root = Project.get_work_dir(cwd=cwd, allow_cwd=True)
+    test_script = root / "scripts" / "test.sh"
+    if _should_run_test_script(test_script):
+        cmd = f"sh {test_script.relative_to(root)}"
+        if cwd != root:
+            cmd = f"cd {root} && " + cmd
+    else:
+        cmd = 'coverage run -m pytest -s && coverage report --omit="tests/*" -m'
+        if not is_venv() or not check_call("coverage --version"):
+            sep = " && "
+            cmd = sep.join("poetry run " + i for i in cmd.split(sep))
+    exit_if_run_failed(cmd, dry=dry)
+
+
+@cli.command()
+def upload(
+    dry: bool = Option(False, "--dry", help="Only print, not really run shell command"),
+) -> None:
+    """Shortcut for package publish"""
+    cmd = "poetry publish --build"
     exit_if_run_failed(cmd, dry=dry)
 
 
 if __name__ == "__main__":
     cli()  # pragma: no cover
```

### Comparing `fast_dev_cli-0.6.4/pyproject.toml` & `fast_dev_cli-0.6.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-dev-cli"
-version = "0.6.4"
+version = "0.6.5"
 description = ""
 authors = ["Waket Zheng <waketzheng@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fast_dev_cli"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `fast_dev_cli-0.6.4/PKG-INFO` & `fast_dev_cli-0.6.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-dev-cli
-Version: 0.6.4
+Version: 0.6.5
 Summary: 
 Author: Waket Zheng
 Author-email: waketzheng@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -52,25 +52,29 @@
 ## Installation
 
 <div class="termy">
 
 ```console
 $ pip install "fast-dev-cli[all]"
 ---> 100%
-Successfully installed fast-dev-cli
+Successfully installed fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage
 ```
 
 </div>
 
 ## Usage
 
 - Lint py code:
 ```bash
 fast lint /path/to/file-or-directory
 ```
+- Check only
+```bash
+fast check
+```
 - Bump up version in pyproject.toml
 ```bash
 fast bump
 ```
 - Run unittest and report coverage
 ```bash
 fast test
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.6.4 Summary: Author: Waket
+Metadata-Version: 2.1 Name: fast-dev-cli Version: 0.6.5 Summary: Author: Waket
 Zheng Author-email: waketzheng@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all Requires-Dist: black (>=23.9.1) ; extra == "all" Requires-
 Dist: bumpversion (>=0.6.0,<0.7.0) ; extra == "all" Requires-Dist: click
 (>=7.1.1) Requires-Dist: coverage (>=6.5.0) ; extra == "all" Requires-Dist:
 isort (>=5.12.0) ; extra == "all" Requires-Dist: mypy (>=1.5.0) ; extra ==
@@ -12,13 +12,13 @@
                                  [FastDevCli]
                   TToooollkkiitt ffoorr ppyytthhoonn ccooddee lliinntt//tteesstt//bbuummpp ......
    _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_G_i_t_h_u_b_A_c_t_i_o_n_R_e_s_u_l_t_]_[_C_o_v_e_r_a_g_e
                                     _S_t_a_t_u_s_]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_w_a_k_e_t_z_h_e_n_g_/_f_a_s_t_-_d_e_v_-_c_l_i ## Requirements
 Python 3.11+ ## Installation
 ```console $ pip install "fast-dev-cli[all]" ---> 100% Successfully installed
-fast-dev-cli ```
+fast-dev-cli isort black ruff mypy typer bumpversion pytest coverage ```
 ## Usage - Lint py code: ```bash fast lint /path/to/file-or-directory ``` -
-Bump up version in pyproject.toml ```bash fast bump ``` - Run unittest and
-report coverage ```bash fast test ``` - Export requirement file and install
-`pip install -r ` ```bash fast sync ``` - Upgrade main/dev dependencies to
-latest version ```bash fast upgrade ```
+Check only ```bash fast check ``` - Bump up version in pyproject.toml ```bash
+fast bump ``` - Run unittest and report coverage ```bash fast test ``` - Export
+requirement file and install `pip install -r ` ```bash fast sync ``` - Upgrade
+main/dev dependencies to latest version ```bash fast upgrade ```
```

