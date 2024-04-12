# Comparing `tmp/fizz_cli-0.1.0.tar.gz` & `tmp/fizz_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fizz_cli-0.1.0.tar", max compression
+gzip compressed data, was "fizz_cli-0.1.1.tar", max compression
```

## Comparing `fizz_cli-0.1.0.tar` & `fizz_cli-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-11 12:01:32.805176 fizz_cli-0.1.0/fizz_cli/__init__.py
--rw-r--r--   0        0        0     7677 2024-04-11 12:01:32.806180 fizz_cli-0.1.0/fizz_cli/main.py
--rw-r--r--   0        0        0        0 2024-04-11 12:01:32.806180 fizz_cli-0.1.0/fizz_cli/templates/__init__.py
--rw-r--r--   0        0        0       40 2024-04-11 12:01:32.807181 fizz_cli-0.1.0/fizz_cli/templates/main.py
--rw-r--r--   0        0        0      415 2024-04-11 12:01:32.807181 fizz_cli-0.1.0/fizz_cli/templates/route.yaml
--rw-r--r--   0        0        0    14745 2024-04-11 12:01:32.807181 fizz_cli-0.1.0/fizz_cli/utils.py
--rw-r--r--   0        0        0      531 2024-04-11 12:20:00.489454 fizz_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4837 2024-04-11 12:01:32.804180 fizz_cli-0.1.0/README.md
--rw-r--r--   0        0        0     5038 1970-01-01 00:00:00.000000 fizz_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-11 12:01:32.805176 fizz_cli-0.1.1/fizz_cli/__init__.py
+-rw-r--r--   0        0        0     8606 2024-04-12 08:15:47.708227 fizz_cli-0.1.1/fizz_cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:01:32.806180 fizz_cli-0.1.1/fizz_cli/templates/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-11 12:01:32.807181 fizz_cli-0.1.1/fizz_cli/templates/main.py
+-rw-r--r--   0        0        0      415 2024-04-11 12:01:32.807181 fizz_cli-0.1.1/fizz_cli/templates/route.yaml
+-rw-r--r--   0        0        0    16914 2024-04-12 08:15:47.709227 fizz_cli-0.1.1/fizz_cli/utils.py
+-rw-r--r--   0        0        0      531 2024-04-12 08:16:05.864062 fizz_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4837 2024-04-11 12:01:32.804180 fizz_cli-0.1.1/README.md
+-rw-r--r--   0        0        0     5038 1970-01-01 00:00:00.000000 fizz_cli-0.1.1/PKG-INFO
```

### Comparing `fizz_cli-0.1.0/fizz_cli/main.py` & `fizz_cli-0.1.1/fizz_cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import subprocess
 import time
 
 import typer
 from click import clear
 from rich import print
+from rich.console import Console
+from rich.table import Table
 
 from .utils import bold_blue
 from .utils import check_fission_directory
 from .utils import create_new_fn_spec_and_boilerplate
 from .utils import delete_file_if_exists
 from .utils import delete_function
+from .utils import destroy
 from .utils import ensure_leading_slash
 from .utils import enumerate_functions
 from .utils import exec_package_script
+from .utils import get_current_environment
 from .utils import get_fn_route_path
 from .utils import id_generator
 from .utils import init_fission
+from .utils import modify_package_yaml_to_init_containers
 from .utils import read_yaml_file
 from .utils import rename_fn_in_specs
 from .utils import rename_folder
 from .utils import replace_route
 from .utils import save_yaml_file
+from .utils import specs_apply
 from .utils import update_shell_scripts
-from .utils import get_current_environment
 
 app = typer.Typer()
 route_app = typer.Typer(help=f"Manage {bold_blue('routes')} for functions.")
 fn_app = typer.Typer(
     help=f"Manage {bold_blue('functions')}. fn is not mandatory, all commands pertaining to functions also work without fn keyword ."
 )
 
@@ -36,28 +41,31 @@
 
 @app.command()
 @fn_app.command()
 def new(function_name: str):
     """
     Creates a new function with the given name.
     """
-    print(f"Creating new function: {function_name} \n")
+    print(f"Creating new function name: {function_name} \n")
     created = create_new_fn_spec_and_boilerplate(function_name)
     env = get_current_environment()
     if created:
         executed = exec_package_script()
         if executed:
             subprocess.run(
                 f'fission package create --sourcearchive {function_name}.zip --env {env} --buildcmd "./build.sh"  --name {function_name} --spec',
                 shell=True,
                 text=False,
                 capture_output=False,
             )
+
+            modify_package_yaml_to_init_containers(function_name)
+
             subprocess.run(
-                f'fission fn create --name {function_name} --pkg {function_name} --entrypoint "main.main" --env=ipl-2024 --spec',
+                f'fission fn create --name {function_name} --pkg {function_name} --entrypoint "main.main" --env={env} --spec',
                 shell=True,
                 text=False,
                 capture_output=False,
             )
             subprocess.run(
                 f"fission route create --name {function_name} --method GET --method POST --url /{function_name} --function {function_name} --spec",
                 shell=True,
@@ -68,15 +76,15 @@
 
 @app.command()
 def init():
     """
     Initialise fission in the current directory so that fission development can be started
     """
     print(
-        "[bold green]:white_heavy_check_mark:Fission Spec Initialisation Completed.[/bold green]"
+        "[bold green]:white_heavy_check_mark:  Fission Spec Initialisation Completed.[/bold green]"
     )
     init_fission()
 
 
 @app.command()
 @fn_app.command()
 def delete(function_name: str):
@@ -166,18 +174,20 @@
     """
     Interactive Mode
     """
     exit_cli = False
     while exit_cli is False:
         clear()
         print(
-            "[:toolbox:] What would you like to do? \n"
-            "[:wrench:]\t1) Modify Existing Function \n"
-            "[:new:]\t2) Create New Function \n"
-            "[:green_square:]\t0) Initialise Fission"
+            ":toolbox:  What would you like to do? \n"
+            ":wrench:\t1) Modify Existing Function \n"
+            ":new:\t2) Create New Function \n"
+            ":grinning_face:\t3) Create Deployment \n"
+            ":grimacing_face:\t4) Destroy Deployment\n"
+            ":bulb:\t0) Initialise Fission\n"
         )
         choice = typer.prompt("Choice", type=int)
 
         if choice == 1:
             exists = check_fission_directory()
             if not exists:
                 print(
@@ -188,50 +198,61 @@
                     "Navigate to the level where the specs folder exists."
                     "[/yellow]"
                 )
                 time.sleep(2)
                 continue
 
             func_list = enumerate_functions()
-            fn_name = typer.prompt(
-                f"Existing Functions: {func_list}\nChoose a function to modify:",
-                type=str,
+            console = Console()
+            table = Table(title="Function List")
+            table.add_column("Index", justify="center", style="cyan")
+            table.add_column("Function Name", justify="center", style="magenta")
+            for index, func in enumerate(func_list):
+                table.add_row(str(index), func)
+            console.print(table)
+            fn_index = typer.prompt(
+                f"Existing Functions: {func_list}\nChoose a index to modify function:",
+                type=int,
             )
 
             print(
-                f"[bold green][:hammer_and_wrench:] {fn_name}[/bold green] "
+                f"[bold green]:hammer_and_wrench:      {func_list[fn_index]}[/bold green] "
                 f"[bold blue]Modification Options:[/bold blue]"
             )
 
             print(
-                "[:toolbox:] What would you like to do? \n"
-                ":pencil:\t1) Rename Route\n"
-                ":skull:\t2) Delete Route\n"
-                ":spiral_notepad:\t3) Rename Function\n"
-                ":cross_mark:\t4) Delete Function"
+                ":toolbox:      What would you like to do? \n"
+                ":pencil:\t1)Rename Route\n"
+                ":skull:\t2)Delete Route\n"
+                ":spiral_notepad:     3)Rename Function\n"
+                ":negative_squared_cross_mark:       4)Delete Function"
             )
             choice = typer.prompt("Choice", type=int)
 
             if choice == 1:
                 new_route = typer.prompt(
                     bold_blue("Enter the new route name"),
                     show_default=False,
                 )
-                route_rename(fn_name, new_route)
+                route_rename(func_list[fn_index], new_route)
 
             elif choice == 2:
-                route_delete(fn_name)
+                route_delete(func_list[fn_index])
             elif choice == 3:
-                rename(fn_name)
+                rename(func_list[fn_index])
             elif choice == 4:
-                delete(fn_name)
+                delete(func_list[fn_index])
         elif choice == 2:
             folder_name = typer.prompt(bold_blue("Enter the new function name"))
             new(folder_name)
         elif choice == 0:
             init()
+        elif choice == 3:
+            specs_apply()
+        elif choice == 4:
+            destroy()
         else:
             print(":boom::skull:[bold red]Invalid Choice![/bold red]")
             time.sleep(1)
             continue
 
         time.sleep(5)
```

### Comparing `fizz_cli-0.1.0/fizz_cli/utils.py` & `fizz_cli-0.1.1/fizz_cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,44 @@
         with open(f"{SPECS_DIR}/{prefix}-{fn_name}.yaml", "r") as file:
             data = yaml.safe_load(file)
             return True, data
     except Exception:
         return False, None
 
 
+def read_all_yaml_files(prefix: str, fn_name: str):
+    try:
+        with open(f"{SPECS_DIR}/{prefix}-{fn_name}.yaml", "r") as file:
+            yaml_files = yaml.safe_load_all(file)
+            return True, yaml_files
+    except Exception:
+        return False, None
+
+
+def modify_package_yaml_to_init_containers(fn_name):
+    try:
+        success, data = read_all_yaml_files("package", fn_name)
+
+        if not success:
+            return
+
+        for document in data:
+            if "spec" in document:
+                spec = document["spec"]
+                if "buildcmd" in spec:
+                    spec["initContainers"] = [
+                        {"command": ["chmod +x build.sh", "./build.sh"]}
+                    ]
+                    del spec["buildcmd"]
+
+        save_yaml_file_multi("package", fn_name, data)
+    except Exception as e:
+        print(f"Error modifying YAML file: {e}")
+
+
 def save_yaml_file(prefix: str, fn_name: str, data):
     try:
         with open(f"{SPECS_DIR}/{prefix}-{fn_name}.yaml", "w") as file:
             yaml.safe_dump(data, file, default_flow_style=False, sort_keys=False)
         return True
     except Exception:
         return False
@@ -137,24 +167,19 @@
             print(f"[bold green]The file {file_path} has been deleted.[/bold green]")
         else:
             print(f"[bold red]The file {file_path} does not exist.[/bold red]")
     except OSError as e:
         print(f"[bold red]Error: {e.strerror}, filename: {e.filename}[/bold red]")
 
 
-def rename_folder(current_fn, new_fn):
+def rename_folder(current_fn: str, new_fn: str) -> bool:
     """
-    Renames a folder from current_folder_path to new_folder_path.
-
-    Parameters:
-        current_fn (str): Name of the function (corresponding to which a folder is expected).
-        new_fn (str): The new name of the function folder.
-
-    Returns:
-        bool: True if the folder was successfully renamed, False otherwise.
+    @param current_fn: Name of the function (corresponding to which a folder is expected).
+    @param new_fn: The new name of the function folder.
+    @return: True if the folder was successfully renamed, False otherwise.
     """
     try:
         # Rename the folder
         shutil.move(f"./{current_fn}", f"./{new_fn}")
         return True
     except OSError as e:
         print(f"Error: {e}")
@@ -362,49 +387,70 @@
     if env exists
     """
     if os.path.exists(f"{os.getcwd()}/specs"):
         files = os.listdir(f"{os.getcwd()}/specs")
         env_file = [
             file for file in files if file.endswith(".yaml") and file.startswith("env")
         ]
+        print("env_file", env_file[0])
         with open(f"{os.getcwd()}/specs/{env_file[0]}", "r") as file:
             yaml_content = yaml.safe_load(file)
 
         environment_name = yaml_content["metadata"]["name"]
         return environment_name
     else:
         return False
 
 
 def init_fission():
-    current_environment = get_current_environment()
-    if current_environment:
-        print(
-            f"[bold red]environment already exists\n"
-            "spec folder already exists\n[/bold red]"
-        )
+    try:
+        current_environment = get_current_environment()
+        if current_environment:
+            print(
+                f"[bold red]environment already exists\n"
+                "spec folder already exists\n[/bold red]"
+            )
+        else:
+            subprocess.run(
+                f"fission spec init",
+                shell=True,
+                text=False,
+                capture_output=False,
+                check=True,
+            )
+            new_environment = typer.prompt(
+                "Enter New Environment Name", default=f"env-{id_generator()}"
+            )
+            subprocess.run(
+                f"fission env create --name {new_environment} --image fission/python-env-3.10:latest --builder fission/python-builder-3.10:latest --spec",
+                shell=True,
+                text=False,
+                capture_output=False,
+                check=True,
+            )
+            print(f"[bold green][Environment created {new_environment}]")
+    except Exception as e:
+        print(f"Error occurred: {e}")
+
+
+def ensure_specs_directory():
+    """
+    Ensure that the 'specs' directory exists.
+    If it doesn't exist, create it.
+    """
+    directory_path = os.path.join(os.getcwd(), "specs")
+    if not os.path.exists(directory_path):
+        os.makedirs(directory_path)
+        print("specs directory created!")
     else:
-        subprocess.run(
-            f"fission spec init",
-            shell=True,
-            text=False,
-            capture_output=False,
-            check=True,
-        )
-        new_environment = typer.prompt(
-            "Enter New Environment Name", default=f"env-{id_generator()}"
-        )
-        subprocess.run(
-            f"fission env create --name {new_environment} --image fission/python-env-3.10:latest --builder fission/python-builder-3.10:latest --spec",
-            shell=True,
-            text=False,
-            capture_output=False,
-            check=True,
-        )
-        print(f"[Environment created {new_environment}]")
+        print("specs directory already exists!")
+
+
+def modify_package_yaml_file():
+    print("Modifying yaml file...")
 
 
 def create_new_fn_spec_and_boilerplate(folder_name):
     new_folder_path = os.path.join(os.getcwd(), folder_name)
     os.makedirs(new_folder_path, exist_ok=True)
     files_to_create = ["main.py", "build.sh", "__init__.py", "requirements.txt"]
 
@@ -452,7 +498,36 @@
             file.write(
                 f"@echo off\n\n"
                 f"pushd {folder_name}\n"
                 f'powershell -Command "Compress-Archive -Path * -DestinationPath ..\\{folder_name}.zip" -Force\n'
                 "popd\n"
             )
     return True
+
+
+def specs_apply():
+    subprocess.run(
+        f"fission spec apply",
+        shell=True,
+        text=False,
+        capture_output=False,
+        check=True,
+    )
+    print(f"[bold green]specs applied successfully[/bold green]")
+
+
+def destroy():
+    subprocess.run(
+        f"fission spec destroy",
+        shell=True,
+        text=False,
+        capture_output=False,
+        check=True,
+    )
+    subprocess.run(
+        f"fission spec destroy --force",
+        shell=True,
+        text=False,
+        capture_output=False,
+        check=True,
+    )
+    print(f"[bold green]Destroy Successfully[/bold green]")
```

### Comparing `fizz_cli-0.1.0/pyproject.toml` & `fizz_cli-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fizz-cli"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Kaustubh Kishore <KaustubhKishorem@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `fizz_cli-0.1.0/README.md` & `fizz_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fizz_cli-0.1.0/PKG-INFO` & `fizz_cli-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fizz-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Kaustubh Kishore
 Author-email: KaustubhKishorem@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

