# Comparing `tmp/oteltest-0.5.0.tar.gz` & `tmp/oteltest-0.6.0.tar.gz`

## Comparing `oteltest-0.5.0.tar` & `oteltest-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 oteltest-0.5.0/_v/.gitignore
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.5.0/example_scripts/simple_loop.json
--rwxr-xr-x   0        0        0     1402 2020-02-02 00:00:00.000000 oteltest-0.5.0/example_scripts/simple_loop.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 oteltest-0.5.0/src/oteltest/__init__.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 oteltest-0.5.0/src/oteltest/main.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 oteltest-0.5.0/src/oteltest/private.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.5.0/src/oteltest/version.py
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 oteltest-0.5.0/src/oteltest/sink/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 oteltest-0.5.0/src/oteltest/sink/private.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.5.0/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 oteltest-0.5.0/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 oteltest-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 oteltest-0.6.0/example_scripts/simple_loop.json
+-rwxr-xr-x   0        0        0     1484 2020-02-02 00:00:00.000000 oteltest-0.6.0/example_scripts/simple_loop.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 oteltest-0.6.0/src/oteltest/__init__.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 oteltest-0.6.0/src/oteltest/main.py
+-rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 oteltest-0.6.0/src/oteltest/private.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.6.0/src/oteltest/version.py
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 oteltest-0.6.0/src/oteltest/sink/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 oteltest-0.6.0/src/oteltest/sink/private.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.6.0/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 oteltest-0.6.0/README.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 oteltest-0.6.0/PKG-INFO
```

### Comparing `oteltest-0.5.0/example_scripts/simple_loop.json` & `oteltest-0.6.0/example_scripts/simple_loop.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996279761904763%*

 * *Differences: {"'trace_reqs'": "{0: {'request': {'resourceSpans': {0: {'scopeSpans': {0: {'spans': {0: "*

 * *                 "{'traceId': 'wKn+9uYSu732Bvp/d6soig==', 'spanId': 'GFQ0Y/1usHw=', "*

 * *                 "'startTimeUnixNano': '1712759490850426000', 'endTimeUnixNano': "*

 * *                 "'1712759491354281000'}, 1: {'traceId': 'TlfIBrx/au+g7z9/g8c6JA==', 'spanId': "*

 * *                 "'9g/OJxA/XS4=', 'startTimeUnixNano': '1712759491354586000', 'endTimeUnixNano': "*

 * *                 "'1712759491857068000'}, 2: {'traceId': […]*

```diff
@@ -46,93 +46,93 @@
                         "scopeSpans": [
                             {
                                 "scope": {
                                     "name": "my-tracer"
                                 },
                                 "spans": [
                                     {
-                                        "endTimeUnixNano": "1712855472884344000",
+                                        "endTimeUnixNano": "1712759491354281000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "FYAuwBn2t6Q=",
-                                        "startTimeUnixNano": "1712855472382751000",
+                                        "spanId": "GFQ0Y/1usHw=",
+                                        "startTimeUnixNano": "1712759490850426000",
                                         "status": {},
-                                        "traceId": "/jTKD0zJzsEbKwptpQuJXQ=="
+                                        "traceId": "wKn+9uYSu732Bvp/d6soig=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855473388776000",
+                                        "endTimeUnixNano": "1712759491857068000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "qvFm87ysls4=",
-                                        "startTimeUnixNano": "1712855472884518000",
+                                        "spanId": "9g/OJxA/XS4=",
+                                        "startTimeUnixNano": "1712759491354586000",
                                         "status": {},
-                                        "traceId": "boxcW7YNIjRjzvqxXByTHg=="
+                                        "traceId": "TlfIBrx/au+g7z9/g8c6JA=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855473891075000",
+                                        "endTimeUnixNano": "1712759492359400000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "5a+3ecJ2gYo=",
-                                        "startTimeUnixNano": "1712855473388956000",
+                                        "spanId": "dkWwAUyNjO8=",
+                                        "startTimeUnixNano": "1712759491857207000",
                                         "status": {},
-                                        "traceId": "UNdTJXdJUV6oNhzXhuAoUQ=="
+                                        "traceId": "h+YaJ65EcB6Kf9qD1XLpYA=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855474395149000",
+                                        "endTimeUnixNano": "1712759492863414000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "JBreKRDYI0M=",
-                                        "startTimeUnixNano": "1712855473891334000",
+                                        "spanId": "4tqPOx4B+Eo=",
+                                        "startTimeUnixNano": "1712759492359552000",
                                         "status": {},
-                                        "traceId": "r6ksUlHS0yKTCBKq+jEzdw=="
+                                        "traceId": "x73Excz4sdxygBM+ID69+w=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855474896273000",
+                                        "endTimeUnixNano": "1712759493368265000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "M/HpiT9eR5w=",
-                                        "startTimeUnixNano": "1712855474395277000",
+                                        "spanId": "R2a/Swb/XBY=",
+                                        "startTimeUnixNano": "1712759492863667000",
                                         "status": {},
-                                        "traceId": "7NvJmJVhcos05uof+AutGA=="
+                                        "traceId": "kp7/+JXh/sDqCH6bsesshg=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855475399799000",
+                                        "endTimeUnixNano": "1712759493871011000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "ToCblhg4laI=",
-                                        "startTimeUnixNano": "1712855474896452000",
+                                        "spanId": "ei+dgcuqSRY=",
+                                        "startTimeUnixNano": "1712759493368418000",
                                         "status": {},
-                                        "traceId": "WhgYGJ2ab03R8+WIfcUH+g=="
+                                        "traceId": "rla9nswFh1ONlj3ktaaQVg=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855475903390000",
+                                        "endTimeUnixNano": "1712759494372957000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "DCI4pLk8hUc=",
-                                        "startTimeUnixNano": "1712855475399932000",
+                                        "spanId": "u1oBpdXkEsY=",
+                                        "startTimeUnixNano": "1712759493871273000",
                                         "status": {},
-                                        "traceId": "MJ/ihnngeUzx9zLkmQiuNw=="
+                                        "traceId": "aar/fPoP1SbWePlkuUAHlQ=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855476407598000",
+                                        "endTimeUnixNano": "1712759494873477000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "KStEi8P4x7w=",
-                                        "startTimeUnixNano": "1712855475903605000",
+                                        "spanId": "TnHUM/kRZt8=",
+                                        "startTimeUnixNano": "1712759494373152000",
                                         "status": {},
-                                        "traceId": "2eZo257Cxph2X8hJFBC3WA=="
+                                        "traceId": "lj5EHWo9ElfkBu/kSznVeg=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855476911519000",
+                                        "endTimeUnixNano": "1712759495373978000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "JpTZ+pcGOkk=",
-                                        "startTimeUnixNano": "1712855476407779000",
+                                        "spanId": "8e109dTowyk=",
+                                        "startTimeUnixNano": "1712759494873735000",
                                         "status": {},
-                                        "traceId": "exSzGQquUuV9QF3rHyJHMg=="
+                                        "traceId": "+vDpXIG67rjtv8lrS8SpEQ=="
                                     }
                                 ]
                             }
                         ]
                     }
                 ]
             }
@@ -181,39 +181,39 @@
                         "scopeSpans": [
                             {
                                 "scope": {
                                     "name": "my-tracer"
                                 },
                                 "spans": [
                                     {
-                                        "endTimeUnixNano": "1712855477416435000",
+                                        "endTimeUnixNano": "1712759495877969000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "PWsh8Ddvy2g=",
-                                        "startTimeUnixNano": "1712855476911665000",
+                                        "spanId": "ddV2pt1uCLE=",
+                                        "startTimeUnixNano": "1712759495374180000",
                                         "status": {},
-                                        "traceId": "j1c3r2bJwTLCO0Oy63xkDQ=="
+                                        "traceId": "+p/vEXWXA3e9pOP6k6EdhQ=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855477921437000",
+                                        "endTimeUnixNano": "1712759496381277000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "8O6d5G/wCwk=",
-                                        "startTimeUnixNano": "1712855477416709000",
+                                        "spanId": "IrKP3d5WENQ=",
+                                        "startTimeUnixNano": "1712759495878226000",
                                         "status": {},
-                                        "traceId": "0lfv9Q9TcCqBMZv52hBANw=="
+                                        "traceId": "TNr46zLbAWYZcwB5kmnJ8g=="
                                     },
                                     {
-                                        "endTimeUnixNano": "1712855478422798000",
+                                        "endTimeUnixNano": "1712759496884624000",
                                         "kind": "SPAN_KIND_INTERNAL",
                                         "name": "my-span",
-                                        "spanId": "orZAkq6kglQ=",
-                                        "startTimeUnixNano": "1712855477921582000",
+                                        "spanId": "fy0SEmyae3k=",
+                                        "startTimeUnixNano": "1712759496381403000",
                                         "status": {},
-                                        "traceId": "5aaMHWRyrqI3f739S1QtVg=="
+                                        "traceId": "3eEzf3zfr/vdfqRC9aaV7A=="
                                     }
                                 ]
                             }
                         ]
                     }
                 ]
             }
```

### Comparing `oteltest-0.5.0/example_scripts/simple_loop.py` & `oteltest-0.6.0/example_scripts/simple_loop.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,9 +37,12 @@
 
     def wrapper_script(self):
         return "opentelemetry-instrument"
 
     def on_script_start(self):
         return None
 
-    def validate(self, telemetry: Telemetry):
+    def on_script_end(self, stdout, stderr, returncode) -> None:
+        pass
+
+    def on_shutdown(self, telemetry: Telemetry):
         assert telemetry.num_spans() == NUM_ADDS
```

### Comparing `oteltest-0.5.0/src/oteltest/__init__.py` & `oteltest-0.6.0/src/oteltest/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,10 +129,13 @@
         pass
 
     @abc.abstractmethod
     def on_script_start(self) -> Optional[float]:
         pass
 
     @abc.abstractmethod
-    def validate(self, telemetry: Telemetry) -> None:
+    def on_script_end(self, stdout: str, stderr: str, returncode: int) -> None:
         pass
 
+    @abc.abstractmethod
+    def on_shutdown(self, telemetry: Telemetry) -> None:
+        pass
```

### Comparing `oteltest-0.5.0/src/oteltest/main.py` & `oteltest-0.6.0/src/oteltest/main.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.5.0/src/oteltest/private.py` & `oteltest-0.6.0/src/oteltest/private.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import importlib
 import inspect
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
+import typing
 import venv
 from pathlib import Path
 
 from google.protobuf.json_format import MessageToDict
 
 from opentelemetry.proto.collector.logs.v1.logs_service_pb2 import (
     ExportLogsServiceRequest,
@@ -22,15 +23,15 @@
 )
 from oteltest import OtelTest, Telemetry
 from oteltest.sink import GrpcSink, RequestHandler
 
 
 def run(script_dir: str, wheel_file: str, venv_parent_dir: str):
     temp_dir = venv_parent_dir or tempfile.mkdtemp()
-    print(f"using temp dir: {temp_dir}")
+    print(f"- Using temp dir: {temp_dir}")
 
     sys.path.append(script_dir)
 
     for script in ls_scripts(script_dir):
         setup_script_environment(temp_dir, script_dir, script, wheel_file)
 
 
@@ -65,15 +66,15 @@
 
     run_python_script(script, script_dir, oteltest_instance, v)
 
     v.rm()
 
     save_telemetry_json(script_dir, module_name, handler.telemetry_to_json())
 
-    oteltest_instance.validate(handler.telemetry)
+    oteltest_instance.on_shutdown(handler.telemetry)
     print(f"- {script} PASSED")
 
 
 def save_telemetry_json(script_dir, module_name, json_str):
     path_str = str(Path(script_dir) / f"{module_name}.json")
     with open(path_str, "w") as file:
         file.write(json_str)
@@ -85,64 +86,73 @@
         str(Path(script_dir) / script),
     ]
 
     wrapper_script = oteltest_instance.wrapper_script()
     if wrapper_script is not None:
         python_script_cmd.insert(0, v.path_to_executable(wrapper_script))
 
-    process = subprocess.Popen(
+    sprocess = subprocess.Popen(
         python_script_cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
+        text=True,
         env=oteltest_instance.environment_variables(),
     )
 
     timeout = oteltest_instance.on_script_start()
     if timeout is None:
         print(
             f"- Will wait indefinitely for {script} to finish (on_script_start() returned None)"
         )
     else:
         print(
             f"- Will wait for up to {timeout} seconds for {script} to finish"
         )
 
+    stdout, stderr, returncode = wait_for_subprocess(sprocess, script, timeout)
+    print_result(stdout, stderr, returncode)
+    oteltest_instance.on_script_end(stdout, stderr, returncode)
+
+
+def wait_for_subprocess(
+    process: subprocess.Popen, script, timeout
+) -> typing.Tuple[str, str, int]:
     try:
         stdout, stderr = process.communicate(timeout=timeout)
-        print_result(process.returncode, stderr, stdout)
+        return stdout, stderr, process.returncode
     except subprocess.TimeoutExpired as ex:
         print(f"- Script {script} was force quit")
-        print_result(process.returncode, ex.stderr, ex.stdout)
+        return decode(ex.stdout), decode(ex.stderr), process.returncode
+
+
+def print_result(stdout, stderr, returncode):
+    print(f"- Return Code: {returncode}")
+    print("- Standard Output:")
+    if stdout:
+        print(stdout)
+    print("- Standard Error:")
+    if stderr:
+        print(stderr)
+    print("- End Subprocess -\n")
 
 
 def run_subprocess(args):
     print(f"- Subprocess: {args}")
     result = subprocess.run(
         args,
         capture_output=True,
     )
     returncode = result.returncode
     stdout = result.stdout
     stderr = result.stderr
     print_result(returncode, stderr, stdout)
 
 
-def print_result(returncode, stderr, stdout):
-    print(f"- Return Code: {returncode}")
-    print("- Standard Output:")
-    if stdout:
-        print(decode(stdout))
-    print("- Standard Error:")
-    if stderr:
-        print(decode(stderr))
-    print("- End Subprocess -\n")
-
-
-def decode(stream):
-    return stream.decode("utf-8").strip()
+def decode(s):
+    return s.decode("utf-8")
 
 
 def load_test_class_for_script(module_name):
     module = importlib.import_module(module_name)
     for attr_name in dir(module):
         value = getattr(module, attr_name)
         if is_test_class(value):
```

### Comparing `oteltest-0.5.0/src/oteltest/version.py` & `oteltest-0.6.0/src/oteltest/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
```

### Comparing `oteltest-0.5.0/src/oteltest/sink/__init__.py` & `oteltest-0.6.0/src/oteltest/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.5.0/src/oteltest/sink/private.py` & `oteltest-0.6.0/src/oteltest/sink/private.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.5.0/tests/__init__.py` & `oteltest-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.5.0/.gitignore` & `oteltest-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oteltest-0.5.0/LICENSE.txt` & `oteltest-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oteltest-0.5.0/README.md` & `oteltest-0.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,87 +14,92 @@
 
 ```console
 pip install oteltest
 ```
 
 ## Overview
 
-The `oteltest` package contains utilities for testing OpenTelemetry Python.
+The `oteltest` package contains utilities for testing OpenTelemetry Python. The motivation for oteltest is to provide
+an easy way to test OpenTelemetry Python, which involves a Python environment with specific packages
 
 ### oteltest
 
-`oteltest` is a CLI command which you can use to run black box tests against OpenTelemetry Python scripts.
+The `oteltest` command runs black box tests against Python scripts that send telemetry.
 
-#### Execution
 
-You can run `oteltest` as a shell command and provide as an argument either a file:
+#### Motivation
 
-```shell
-oteltest my_script.py
-```
+The motivation for oteltest is to make it as easy as possible to run code that emits telemetry, with all of the
+information required to run a test co-located with the code being tested. With that in place, you should be able to
+point something at it that sets up the environment, runs the script, records the telemetry that the script sends, and
+sends that telemetry back to the script so that the validate can be co-located with the test configuration, and the test
+code.
 
-or a directory:
+#### Execution
+
+Run `oteltest` as a shell command and provide a directory as an argument:
 
 ```shell
 oteltest my_script_dir
 ```
 
-Given a directory, the `oteltest` command will attempt to run all `oteltest`-runnable scripts in `my_script_dir`,
-non-recursively.
+in which case it will attempt to run all `oteltest`-eligible scripts in `my_script_dir`, non-recursively.
 
 #### Operation
 
-Running `oteltest` against `my_script.py` 1) starts a Python OTLP listener, 2) creates a new Python virtual
-environment, 3) installs any `requirements()`, 4) starts a subprocess with any requested `wrapper_script()`
-and `environment_variables()`, 5) waits for `my_script.py` to complete, 6) stops the OTLP listener, and finally 7) sends
-the listener's telemetry received back to `my_script.py` in the form of a call to `validate(telemetry)`. It also writes
-a `.json` file with that telemetry next to the script (with the same name but `.json` extension).
+Running `oteltest` against a directory containing `my_script.py`
+
+1) Starts an [otelsink](#otelsink) instance
+2) Creates a new Python virtual environment with `requirements()`
+3) Using that new environment, starts running `my_script.py` in a subprocess
+4) Meanwhile, calls `OtelTest#on_script_start()` waiting until completion
+5) Depending on the return value from `on_script_start()`, waits for `my_script.py` to complete or interrupts
+6) Stops the OTLP listener
+7) Calls `validate(telemetry)` with otelsink's received telemetry
+8) Writes the telemetry to a `.json` file next to the script (script name but `.json`)
 
-#### Scripts
+#### Script Eligibility
 
-For a Python script to be runnable by `oteltest`, it must both be executable and define an implementation of
-`OtelTest`. The script below has an implementation called `MyTest`:
+For a Python script to be runnable by `oteltest`, it must both be executable and define an implementation of the
+[OtelTest]() abstract base class. The script below has an implementation called `MyTest`:
 
 ```python
 import time
+
 from opentelemetry import trace
-from oteltest.common import OtelTest, Telemetry
+from oteltest import OtelTest, Telemetry
 
-SERVICE_NAME = "my-test"
+SERVICE_NAME = "integration-test"
 NUM_ADDS = 12
 
 if __name__ == "__main__":
     tracer = trace.get_tracer("my-tracer")
     for i in range(NUM_ADDS):
         with tracer.start_as_current_span("my-span"):
-            print(f"{i + 1}/{NUM_ADDS}")
+            print(f"simple_loop.py: {i + 1}/{NUM_ADDS}")
             time.sleep(0.5)
 
 
 class MyTest(OtelTest):
     def requirements(self):
         return "opentelemetry-distro", "opentelemetry-exporter-otlp-proto-grpc"
 
+    def environment_variables(self):
+        return {"OTEL_SERVICE_NAME": SERVICE_NAME}
+
     def wrapper_script(self):
         return "opentelemetry-instrument"
 
-    def environment_variables(self):
-        return {"OTEL_SERVICE_NAME": SERVICE_NAME}
+    def on_script_start(self):
+        return None
 
     def validate(self, telemetry: Telemetry):
         assert telemetry.num_spans() == NUM_ADDS
 ```
 
-#### Usage with OTel Examples
-
-Runnable examples are a great way to get up to speed on OpenTelemetry but running them can be tedious.
-oteltest lets you run example scripts and potentially see the telemetry you just generated without starting Docker or
-setting up Python enviornments. Adding an `OtelTest` implementation (e.g. `MyTest` above) to an existing example script
-lets you run it without having to set up a Python environment with dependencies.
-
 ### otelsink
 
 `otelsink` is a gRPC server that listens for OTel metrics, traces, and logs.
 
 #### Operation
 
 You can run otelink either from the command line by using the `otelsink` command (installed when you
```

### Comparing `oteltest-0.5.0/pyproject.toml` & `oteltest-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteltest-0.5.0/PKG-INFO` & `oteltest-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oteltest
-Version: 0.5.0
+Version: 0.6.0
 Summary: OpenTelemetry Tester
 Project-URL: Documentation, https://github.com/open-telemetry/opentelemetry-python#readme
 Project-URL: Issues, https://github.com/open-telemetry/opentelemetry-python/issues
 Project-URL: Source, https://github.com/open-telemetry/opentelemetry-python/
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -41,87 +41,92 @@
 
 ```console
 pip install oteltest
 ```
 
 ## Overview
 
-The `oteltest` package contains utilities for testing OpenTelemetry Python.
+The `oteltest` package contains utilities for testing OpenTelemetry Python. The motivation for oteltest is to provide
+an easy way to test OpenTelemetry Python, which involves a Python environment with specific packages
 
 ### oteltest
 
-`oteltest` is a CLI command which you can use to run black box tests against OpenTelemetry Python scripts.
+The `oteltest` command runs black box tests against Python scripts that send telemetry.
 
-#### Execution
 
-You can run `oteltest` as a shell command and provide as an argument either a file:
+#### Motivation
 
-```shell
-oteltest my_script.py
-```
+The motivation for oteltest is to make it as easy as possible to run code that emits telemetry, with all of the
+information required to run a test co-located with the code being tested. With that in place, you should be able to
+point something at it that sets up the environment, runs the script, records the telemetry that the script sends, and
+sends that telemetry back to the script so that the validate can be co-located with the test configuration, and the test
+code.
 
-or a directory:
+#### Execution
+
+Run `oteltest` as a shell command and provide a directory as an argument:
 
 ```shell
 oteltest my_script_dir
 ```
 
-Given a directory, the `oteltest` command will attempt to run all `oteltest`-runnable scripts in `my_script_dir`,
-non-recursively.
+in which case it will attempt to run all `oteltest`-eligible scripts in `my_script_dir`, non-recursively.
 
 #### Operation
 
-Running `oteltest` against `my_script.py` 1) starts a Python OTLP listener, 2) creates a new Python virtual
-environment, 3) installs any `requirements()`, 4) starts a subprocess with any requested `wrapper_script()`
-and `environment_variables()`, 5) waits for `my_script.py` to complete, 6) stops the OTLP listener, and finally 7) sends
-the listener's telemetry received back to `my_script.py` in the form of a call to `validate(telemetry)`. It also writes
-a `.json` file with that telemetry next to the script (with the same name but `.json` extension).
+Running `oteltest` against a directory containing `my_script.py`
+
+1) Starts an [otelsink](#otelsink) instance
+2) Creates a new Python virtual environment with `requirements()`
+3) Using that new environment, starts running `my_script.py` in a subprocess
+4) Meanwhile, calls `OtelTest#on_script_start()` waiting until completion
+5) Depending on the return value from `on_script_start()`, waits for `my_script.py` to complete or interrupts
+6) Stops the OTLP listener
+7) Calls `validate(telemetry)` with otelsink's received telemetry
+8) Writes the telemetry to a `.json` file next to the script (script name but `.json`)
 
-#### Scripts
+#### Script Eligibility
 
-For a Python script to be runnable by `oteltest`, it must both be executable and define an implementation of
-`OtelTest`. The script below has an implementation called `MyTest`:
+For a Python script to be runnable by `oteltest`, it must both be executable and define an implementation of the
+[OtelTest]() abstract base class. The script below has an implementation called `MyTest`:
 
 ```python
 import time
+
 from opentelemetry import trace
-from oteltest.common import OtelTest, Telemetry
+from oteltest import OtelTest, Telemetry
 
-SERVICE_NAME = "my-test"
+SERVICE_NAME = "integration-test"
 NUM_ADDS = 12
 
 if __name__ == "__main__":
     tracer = trace.get_tracer("my-tracer")
     for i in range(NUM_ADDS):
         with tracer.start_as_current_span("my-span"):
-            print(f"{i + 1}/{NUM_ADDS}")
+            print(f"simple_loop.py: {i + 1}/{NUM_ADDS}")
             time.sleep(0.5)
 
 
 class MyTest(OtelTest):
     def requirements(self):
         return "opentelemetry-distro", "opentelemetry-exporter-otlp-proto-grpc"
 
+    def environment_variables(self):
+        return {"OTEL_SERVICE_NAME": SERVICE_NAME}
+
     def wrapper_script(self):
         return "opentelemetry-instrument"
 
-    def environment_variables(self):
-        return {"OTEL_SERVICE_NAME": SERVICE_NAME}
+    def on_script_start(self):
+        return None
 
     def validate(self, telemetry: Telemetry):
         assert telemetry.num_spans() == NUM_ADDS
 ```
 
-#### Usage with OTel Examples
-
-Runnable examples are a great way to get up to speed on OpenTelemetry but running them can be tedious.
-oteltest lets you run example scripts and potentially see the telemetry you just generated without starting Docker or
-setting up Python enviornments. Adding an `OtelTest` implementation (e.g. `MyTest` above) to an existing example script
-lets you run it without having to set up a Python environment with dependencies.
-
 ### otelsink
 
 `otelsink` is a gRPC server that listens for OTel metrics, traces, and logs.
 
 #### Operation
 
 You can run otelink either from the command line by using the `otelsink` command (installed when you
```

