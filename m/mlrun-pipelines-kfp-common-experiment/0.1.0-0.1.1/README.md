# Comparing `tmp/mlrun_pipelines_kfp_common_experiment-0.1.0-py3-none-any.whl.zip` & `tmp/mlrun_pipelines_kfp_common_experiment-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13080 bytes, number of entries: 9
--rw-r--r--  2.0 unx      571 b- defN 24-Feb-27 20:19 mlrun_pipelines/common/__init__.py
--rw-r--r--  2.0 unx     4552 b- defN 24-Apr-07 17:43 mlrun_pipelines/common/helpers.py
--rw-r--r--  2.0 unx     2946 b- defN 24-Mar-11 23:09 mlrun_pipelines/common/models.py
--rw-r--r--  2.0 unx     1747 b- defN 24-Mar-14 15:38 mlrun_pipelines/common/mounts.py
--rw-r--r--  2.0 unx    23141 b- defN 24-Mar-31 22:28 mlrun_pipelines/common/ops.py
--rw-r--r--  2.0 unx      324 b- defN 24-Apr-10 00:48 mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 00:48 mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-10 00:48 mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      862 b- defN 24-Apr-10 00:48 mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/RECORD
-9 files, 34251 bytes uncompressed, 11558 bytes compressed:  66.3%
+Zip file size: 13450 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      571 b- defN 24-Apr-10 22:12 mlrun_pipelines/common/__init__.py
+-rw-r--r--  2.0 unx     4552 b- defN 24-Apr-10 22:12 mlrun_pipelines/common/helpers.py
+-rw-r--r--  2.0 unx     3518 b- defN 24-Apr-11 00:14 mlrun_pipelines/common/models.py
+-rw-r--r--  2.0 unx     1747 b- defN 24-Apr-10 22:12 mlrun_pipelines/common/mounts.py
+-rw-r--r--  2.0 unx    23368 b- defN 24-Apr-10 23:38 mlrun_pipelines/common/ops.py
+-rw-r--r--  2.0 unx      324 b- defN 24-Apr-12 20:55 mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 20:55 mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-12 20:55 mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      862 b- defN 24-Apr-12 20:55 mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/RECORD
+9 files, 35050 bytes uncompressed, 11928 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mlrun_pipelines/common/mounts.py
 Comment: 
 
 Filename: mlrun_pipelines/common/ops.py
 Comment: 
 
-Filename: mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/METADATA
+Filename: mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/WHEEL
+Filename: mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/top_level.txt
+Filename: mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/RECORD
+Filename: mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlrun_pipelines/common/models.py

```diff
@@ -1,7 +1,22 @@
+# Copyright 2024 Iguazio
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
 from enum import Enum
 
 
 class RunStatuses(Enum):
     """
     Class for different types of statuses a 'PipelineRun' can have using an enum type.
     Beyond enumerating all possible statuses, this class ensures comparisons are case-insensitive.
```

## mlrun_pipelines/common/ops.py

```diff
@@ -35,16 +35,16 @@
     logger,
     run_keys,
     version,
 )
 
 # default KFP artifacts and output (ui metadata, metrics etc.)
 # directories to /tmp to allow running with security context
-KFPMETA_DIR = os.environ.get("KFPMETA_OUT_DIR", "/tmp")
-KFP_ARTIFACTS_DIR = os.environ.get("KFP_ARTIFACTS_DIR", "/tmp")
+KFPMETA_DIR = "/tmp"
+KFP_ARTIFACTS_DIR = "/tmp"
 
 
 class PipelineRunType:
     run = "run"
     build = "build"
     deploy = "deploy"
 
@@ -281,17 +281,17 @@
             "--returns",
             json.dumps(log_hint) if isinstance(log_hint, dict) else log_hint,
         ]
     for label, val in labels.items():
         cmd += ["--label", f"{label}={val}"]
     for output in outputs:
         cmd += ["-o", str(output)]
-        file_outputs[
-            output.replace(".", "_")
-        ] = f"/tmp/{output}"  # not using path.join to avoid windows "\"
+        file_outputs[output.replace(".", "_")] = (
+            f"/tmp/{output}"  # not using path.join to avoid windows "\"
+        )
     if project:
         cmd += ["--project", project]
     if handler:
         cmd += ["--handler", handler]
     if runtime:
         cmd += ["--runtime", runtime]
     if in_path:
@@ -554,15 +554,15 @@
 
     results = struct["status"].get("results", {})
     metrics = {
         "metrics": [
             {"name": k, "numberValue": v} for k, v in results.items() if is_num(v)
         ],
     }
-    with open(KFPMETA_DIR + "/mlpipeline-metrics.json", "w") as f:
+    with open(os.path.join(KFPMETA_DIR, "mlpipeline-metrics.json"), "w") as f:
         json.dump(metrics, f)
 
     struct = deepcopy(struct)
     uid = struct["metadata"].get("uid")
     project = struct["metadata"].get("project", config.default_project)
     output_artifacts, out_dict = get_kfp_outputs(
         struct["status"].get(run_keys.artifacts, []),
@@ -575,35 +575,37 @@
     for key in struct["spec"].get(run_keys.outputs, []):
         val = "None"
         if key in out_dict:
             val = out_dict[key]
         elif key in results:
             val = results[key]
         try:
-            path = "/".join([KFP_ARTIFACTS_DIR, key])
+            # NOTE: if key has "../x", it would fail on path traversal
+            path = os.path.join(KFP_ARTIFACTS_DIR, key)
+            if not mlrun.utils.helpers.is_safe_path(KFP_ARTIFACTS_DIR, path):
+                logger.warning(
+                    "Path traversal is not allowed ignoring", path=path, key=key
+                )
+                continue
+            path = os.path.abspath(path)
             logger.info("Writing artifact output", path=path, val=val)
             with open(path, "w") as fp:
                 fp.write(str(val))
         except Exception as exc:
-            logger.warning("Failed writing to temp file. Ignoring", exc=repr(exc))
+            logger.warning("Failed writing to temp file. Ignoring", exc=err_to_str(exc))
             pass
 
     text = "# Run Report\n"
     if "iterations" in struct["status"]:
         del struct["status"]["iterations"]
 
     text += "## Metadata\n```yaml\n" + dict_to_yaml(struct) + "```\n"
 
-    metadata = {
-        "outputs": output_artifacts
-        + [{"type": "markdown", "storage": "inline", "source": text}]
-    }
-
-    # saar is working on removing this
-    with open(KFPMETA_DIR + "/mlpipeline-ui-metadata.json", "w") as f:
+    metadata = {"outputs": [{"type": "markdown", "storage": "inline", "source": text}]}
+    with open(os.path.join(KFPMETA_DIR, "mlpipeline-ui-metadata.json"), "w") as f:
         json.dump(metadata, f)
 
 
 def get_kfp_outputs(artifacts, labels, project):
     outputs = []
     out_dict = {}
     for output in artifacts:
```

## Comparing `mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/RECORD` & `mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlrun_pipelines/common/__init__.py,sha256=sOBwPJ0KuM6LMolYEwR4tPiJhlgFsla5_0gIdyxONlw,571
 mlrun_pipelines/common/helpers.py,sha256=zz1LwF-iqhC12X-QP4xo5zyAI93RUxIYpi6UxPDUtMk,4552
-mlrun_pipelines/common/models.py,sha256=FCA7MmDQzE7-8h5QOpmV6RPBSNBBahPsb-gCbXKW0QI,2946
+mlrun_pipelines/common/models.py,sha256=822LGUNR5B50MUBTzBCylkJJbcjgKg29KOwv6L1qe5s,3518
 mlrun_pipelines/common/mounts.py,sha256=Ayu0FWCT3d0nuL7tBx5EbeBt3ediKq4tnWOQKyCOn_I,1747
-mlrun_pipelines/common/ops.py,sha256=fwMdKOnk-UN1gH37CK-ERYWca15O-S9SKMxpdOfhRCY,23141
-mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/METADATA,sha256=FkcC7-4KQtsKIhz_Grar3tPbnBaWzCZaTOHKhxg_3hU,324
-mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/top_level.txt,sha256=nLog7d6Z7sH90lLPiJHgM1Q2hqwiKlkc8MtKtltFJvE,16
-mlrun_pipelines_kfp_common_experiment-0.1.0.dist-info/RECORD,,
+mlrun_pipelines/common/ops.py,sha256=FTgFmSb9U-w6PoVC1DUfiFMRBguYiFja7Yi4L5BB2Y8,23368
+mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/METADATA,sha256=9MPjs22atmdoiigfkOes0cWe6fv1FvAoVzLKQC9og-4,324
+mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/top_level.txt,sha256=nLog7d6Z7sH90lLPiJHgM1Q2hqwiKlkc8MtKtltFJvE,16
+mlrun_pipelines_kfp_common_experiment-0.1.1.dist-info/RECORD,,
```

