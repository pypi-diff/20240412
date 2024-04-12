# Comparing `tmp/medroom_ai_dataengineer-0.0.2.tar.gz` & `tmp/medroom_ai_dataengineer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medroom_ai_dataengineer-0.0.2.tar", last modified: Fri Apr 12 18:04:33 2024, max compression
+gzip compressed data, was "medroom_ai_dataengineer-0.0.3.tar", last modified: Fri Apr 12 20:32:03 2024, max compression
```

## Comparing `medroom_ai_dataengineer-0.0.2.tar` & `medroom_ai_dataengineer-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.533494 medroom_ai_dataengineer-0.0.2/
--rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.531494 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/
--rw-rw-rw-   0        0        0    13724 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      115 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      124 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 18:04:33.000000 medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13724 2024-04-12 18:04:33.532493 medroom_ai_dataengineer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5758 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.497490 medroom_ai_dataengineer-0.0.2/medroom/
-drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.498490 medroom_ai_dataengineer-0.0.2/medroom/dna/
-drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.528497 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/__init__.py
--rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/config.py
--rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/main.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:04:33.530493 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/__init__.py
--rw-rw-rw-   0        0        0     2211 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/evalmetrics.py
--rw-rw-rw-   0        0        0     1889 2024-04-12 17:16:27.000000 medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/textclean.py
--rw-rw-rw-   0        0        0       42 2024-04-12 18:04:33.533494 medroom_ai_dataengineer-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:32:03.575700 medroom_ai_dataengineer-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-12 20:32:03.573701 medroom_ai_dataengineer-0.0.3/MedRoom.AI.DataEngineer.egg-info/
+-rw-rw-rw-   0        0        0    13724 2024-04-12 20:32:03.000000 medroom_ai_dataengineer-0.0.3/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-04-12 20:32:03.000000 medroom_ai_dataengineer-0.0.3/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      115 2024-04-12 20:32:03.000000 medroom_ai_dataengineer-0.0.3/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.3/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      124 2024-04-12 20:32:03.000000 medroom_ai_dataengineer-0.0.3/MedRoom.AI.DataEngineer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 20:32:03.000000 medroom_ai_dataengineer-0.0.3/MedRoom.AI.DataEngineer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13724 2024-04-12 20:32:03.574699 medroom_ai_dataengineer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5758 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 20:32:03.488719 medroom_ai_dataengineer-0.0.3/medroom/
+drwxrwxrwx   0        0        0        0 2024-04-12 20:32:03.488719 medroom_ai_dataengineer-0.0.3/medroom/dna/
+drwxrwxrwx   0        0        0        0 2024-04-12 20:32:03.558701 medroom_ai_dataengineer-0.0.3/medroom/dna/processors/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.3/medroom/dna/processors/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.3/medroom/dna/processors/config.py
+-rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.3/medroom/dna/processors/main.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:32:03.572704 medroom_ai_dataengineer-0.0.3/medroom/dna/processors/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.3/medroom/dna/processors/utils/__init__.py
+-rw-rw-rw-   0        0        0     2860 2024-04-12 20:29:03.000000 medroom_ai_dataengineer-0.0.3/medroom/dna/processors/utils/evalmetrics.py
+-rw-rw-rw-   0        0        0     1889 2024-04-12 17:16:27.000000 medroom_ai_dataengineer-0.0.3/medroom/dna/processors/utils/textclean.py
+-rw-rw-rw-   0        0        0       42 2024-04-12 20:32:03.575700 medroom_ai_dataengineer-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1298 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.3/setup.py
```

### Comparing `medroom_ai_dataengineer-0.0.2/LICENSE` & `medroom_ai_dataengineer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/PKG-INFO` & `medroom_ai_dataengineer-0.0.3/MedRoom.AI.DataEngineer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `medroom_ai_dataengineer-0.0.2/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt` & `medroom_ai_dataengineer-0.0.3/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.2/PKG-INFO` & `medroom_ai_dataengineer-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `medroom_ai_dataengineer-0.0.2/README.md` & `medroom_ai_dataengineer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.2/medroom/dna/processors/config.py` & `medroom_ai_dataengineer-0.0.3/medroom/dna/processors/config.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.2/medroom/dna/processors/main.py` & `medroom_ai_dataengineer-0.0.3/medroom/dna/processors/main.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/evalmetrics.py` & `medroom_ai_dataengineer-0.0.3/medroom/dna/processors/utils/evalmetrics.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from sklearn import preprocessing
 from sklearn.metrics import accuracy_score, classification_report, confusion_matrix, roc_auc_score
-
+from sklearn.preprocessing import LabelBinarizer
+from io import BytesIO
 
 class ModelEvaluator:
     @staticmethod
     def accuracy(y_true, y_pred):
         acc = accuracy_score(y_true, y_pred)
-        print("Acurácia do modelo = %2.f%%" % (acc * 100.00))
+        print(f"Acurácia do modelo = {acc * 100.0:.2f}%")
+        return acc
 
     @staticmethod
-    def classification_report(y_true, y_pred):
-        report_df = pd.DataFrame(classification_report(y_true, y_pred, output_dict=True)).T
-        report_df = report_df.drop(columns=["support"])
-        plt.subplots(figsize=(4, 3))
-        sns.heatmap(report_df, cmap="Greens", linewidths=0.5, annot=True)
-        plt.title("Classification Report")
-        plt.show()
+    def flatten_classification_report(report, prefix="", suffix=""):
+        flat_report = {}
+        for key, value in report.items():
+            if isinstance(value, dict):
+                for metric, metric_value in value.items():
+                    new_key = f"{prefix} {key} {metric} {suffix}".strip()
+                    flat_report[new_key] = metric_value
+            else:
+                new_key = f"{prefix} {key} {suffix}".strip()
+                flat_report[new_key] = value
+        return flat_report
 
     @staticmethod
-    def confusion_matrix(y_true, y_pred):
-        # Criando a matriz de confusão
-        report_df = pd.DataFrame(classification_report(y_true, y_pred, output_dict=True)).T
+    def classification_report_img_generator(y_true, y_pred):
+        report = classification_report(y_true, y_pred, output_dict=True)
+        report_df = pd.DataFrame(report).transpose()
         report_df = report_df.drop(columns=["support"])
+        
+        fig, ax = plt.subplots(figsize=(4, 3))
+        sns.heatmap(report_df, cmap="Greens", linewidths=0.5, annot=True, ax=ax)
+        ax.set_title("Classification Report")
+
+        img = BytesIO()
+        plt.savefig(img, format='png', bbox_inches='tight')
+        plt.close(fig)
+        img.seek(0)
+        return img, report
 
-        cnf_report_df = report_df.index[:-3]
+    @staticmethod
+    def confusion_matrix_img_generator(y_true, y_pred):
         cnf_matrix = confusion_matrix(y_true, y_pred)
-        cnf_matrix = pd.DataFrame(cnf_matrix, index=cnf_report_df.values, columns=cnf_report_df.values)
-        cnf_matrix = cnf_matrix / cnf_matrix.sum(axis=1).values[:, np.newaxis]  # Normalização em linha (recall)
-
-        # Plotagem da matriz de confusão
-        sns.heatmap(
-            cnf_matrix,
-            cmap="Greens",
-            linecolor="white",
-            linewidths=0.5,
-            annot=True,
-            fmt=".0%",
-            cbar=False,
-            square=True,
-        )
-        plt.title("Confusion Matrix")
-        plt.show()
+        report_df = pd.DataFrame(classification_report(y_true, y_pred, output_dict=True)).transpose()
+        cnf_matrix_df = pd.DataFrame(cnf_matrix, index=report_df.index[:-3].values, columns=report_df.index[:-3].values)
+        cnf_matrix_normalized = cnf_matrix_df / cnf_matrix_df.sum(axis=1).values[:, np.newaxis]
+
+        fig, ax = plt.subplots()
+        sns.heatmap(cnf_matrix_normalized, cmap="Greens", linecolor="white", linewidths=0.5, annot=True, fmt=".0%", cbar=False, square=True, ax=ax)
+        ax.set_title("Confusion Matrix")
+
+        img = BytesIO()
+        plt.savefig(img, format='png', bbox_inches='tight')
+        plt.close(fig)
+        img.seek(0)
+        return img, cnf_matrix_normalized
 
     @staticmethod
     def roc_auc(y_true, y_pred):
-        # Converter rótulos para formato binário
-        lb = preprocessing.LabelBinarizer()
+        lb = LabelBinarizer()
         lb.fit(y_true)
-
         y_test = lb.transform(y_true)
         y_pred = lb.transform(y_pred)
-
-        # Calcular a área sob a curva (AUC-ROC)
         auc_roc = roc_auc_score(y_test, y_pred, average="weighted", multi_class="ovr")
-        print("ROC_AUC do modelo = %2.f%%" % (auc_roc * 100.00))
+        print(f"ROC_AUC do modelo = {auc_roc * 100.0:.2f}%")
+        return auc_roc
```

### Comparing `medroom_ai_dataengineer-0.0.2/medroom/dna/processors/utils/textclean.py` & `medroom_ai_dataengineer-0.0.3/medroom/dna/processors/utils/textclean.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.2/setup.py` & `medroom_ai_dataengineer-0.0.3/setup.py`

 * *Files identical despite different names*

