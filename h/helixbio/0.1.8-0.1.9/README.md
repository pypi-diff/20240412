# Comparing `tmp/helixbio-0.1.8.tar.gz` & `tmp/helixbio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helixbio-0.1.8.tar", max compression
+gzip compressed data, was "helixbio-0.1.9.tar", max compression
```

## Comparing `helixbio-0.1.8.tar` & `helixbio-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-09-26 10:30:15.779501 helixbio-0.1.8/LICENSE
--rw-r--r--   0        0        0     2158 2024-01-10 20:28:24.047717 helixbio-0.1.8/README.md
--rw-r--r--   0        0        0       20 2023-10-18 23:09:39.426116 helixbio-0.1.8/helix/__init__.py
--rw-r--r--   0        0        0     9038 2024-01-10 21:27:13.749156 helixbio-0.1.8/helix/esm.py
--rw-r--r--   0        0        0     4701 2024-01-08 13:47:14.560084 helixbio-0.1.8/helix/evoprotgrad.py
--rw-r--r--   0        0        0     5355 2024-01-05 13:07:56.608698 helixbio-0.1.8/helix/flows.py
--rw-r--r--   0        0        0     1340 2023-10-29 11:38:21.566375 helixbio-0.1.8/helix/main.py
--rw-r--r--   0        0        0    40436 2023-10-21 17:15:22.575362 helixbio-0.1.8/helix/proteinmpnn.py
--rw-r--r--   0        0        0     2630 2023-10-18 23:07:13.437080 helixbio-0.1.8/helix/synthesis.py
--rw-r--r--   0        0        0     3194 2023-12-22 16:24:19.124234 helixbio-0.1.8/helix/utils.py
--rw-r--r--   0        0        0      888 2024-01-10 21:28:20.343028 helixbio-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2833 1970-01-01 00:00:00.000000 helixbio-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-09-26 10:30:15.779501 helixbio-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2158 2024-01-10 20:28:24.047717 helixbio-0.1.9/README.md
+-rw-r--r--   0        0        0       20 2023-10-18 23:09:39.426116 helixbio-0.1.9/helix/__init__.py
+-rw-r--r--   0        0        0      811 2024-01-18 16:41:11.010475 helixbio-0.1.9/helix/ai.py
+-rw-r--r--   0        0        0    14262 2024-03-21 22:50:34.863778 helixbio-0.1.9/helix/esm.py
+-rw-r--r--   0        0        0     5081 2024-03-22 00:11:47.714069 helixbio-0.1.9/helix/evoprotgrad.py
+-rw-r--r--   0        0        0     1480 2024-04-07 18:28:53.850817 helixbio-0.1.9/helix/finetuning/common.py
+-rw-r--r--   0        0        0     6022 2024-04-09 18:17:19.199949 helixbio-0.1.9/helix/finetuning/inference.py
+-rw-r--r--   0        0        0     1489 2024-04-07 18:26:37.657015 helixbio-0.1.9/helix/finetuning/train.py
+-rw-r--r--   0        0        0     8416 2024-04-07 16:43:25.394063 helixbio-0.1.9/helix/finetuning/train_old.py
+-rw-r--r--   0        0        0      181 2024-04-07 20:06:48.028995 helixbio-0.1.9/helix/finetuning/training_config.yaml
+-rw-r--r--   0        0        0     6286 2024-04-09 12:24:32.915605 helixbio-0.1.9/helix/finetuning/utils.py
+-rw-r--r--   0        0        0     8243 2024-03-21 23:04:23.628728 helixbio-0.1.9/helix/flows.py
+-rw-r--r--   0        0        0     1340 2024-04-07 18:29:13.290407 helixbio-0.1.9/helix/main.py
+-rw-r--r--   0        0        0    40436 2023-10-21 17:15:22.575362 helixbio-0.1.9/helix/proteinmpnn.py
+-rw-r--r--   0        0        0     9659 2024-04-06 23:50:22.897782 helixbio-0.1.9/helix/synthesis.py
+-rw-r--r--   0        0        0     3194 2023-12-22 16:24:19.124234 helixbio-0.1.9/helix/utils.py
+-rw-r--r--   0        0        0      926 2024-04-12 13:30:06.749573 helixbio-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 helixbio-0.1.9/PKG-INFO
```

### Comparing `helixbio-0.1.8/LICENSE` & `helixbio-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `helixbio-0.1.8/README.md` & `helixbio-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `helixbio-0.1.8/helix/esm.py` & `helixbio-0.1.9/helix/esm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,103 @@
 from io import StringIO
-from modal import Image, method, Mount
+from modal import Image, method, gpu
 from .main import CACHE_DIR, volume, stub
-from Bio.SeqRecord import SeqRecord
+import modal
 from Bio.PDB.Structure import Structure
 from Bio import SeqIO
+from Bio.Seq import Seq
+from Bio.SeqRecord import SeqRecord
 from Bio.PDB.PDBIO import PDBIO
 import os
 import transformers
 
 
 def download_models():
-    from transformers import EsmModel, EsmForProteinFolding
+    from transformers import EsmModel, EsmForProteinFolding, AutoTokenizer
+
     EsmForProteinFolding.from_pretrained(
         "facebook/esmfold_v1")
+    AutoTokenizer.from_pretrained(
+        "facebook/esmfold_v1")
+
     EsmModel.from_pretrained(
         "facebook/esm2_t36_3B_UR50D")
-    # tokenizers
-    transformers.AutoTokenizer.from_pretrained(
-        "facebook/esmfold_v1")
-    transformers.AutoTokenizer.from_pretrained(
+    AutoTokenizer.from_pretrained(
         "facebook/esm2_t36_3B_UR50D")
 
+    EsmModel.from_pretrained(
+        "facebook/esm2_t48_15B_UR50D")
+    AutoTokenizer.from_pretrained(
+        "facebook/esm2_t48_15B_UR50D")
+
 
 image = Image.debian_slim().apt_install("git").pip_install(
     "torch",
     "biopython",
     "matplotlib",
     "transformers",
-    "pandas").run_function(download_models, mounts=[Mount.from_local_python_packages("helix")])
+    "pandas"
+).run_function(download_models)
 
 
-@stub.cls(gpu='A10G', timeout=2000, network_file_systems={CACHE_DIR: volume}, image=image, allow_cross_region_volumes=True, concurrency_limit=9)
+@stub.cls(gpu=gpu.A10G(), timeout=2000, network_file_systems={CACHE_DIR: volume}, image=image, allow_cross_region_volumes=True, concurrency_limit=9)
 class EsmModel():
     def __init__(self, device: str = "cuda", model_name: str = "facebook/esm2_t36_3B_UR50D"):
         import transformers
         self.tokenizer = transformers.AutoTokenizer.from_pretrained(
             model_name)
         self.model = transformers.AutoModel.from_pretrained(
             model_name)
         self.device = device
         if device == "cuda":
             self.model = self.model.cuda()
         self.model.eval()
 
     @method()
-    def infer(self, sequences, output_hidden_states: bool = False, output_attentions: bool = False) -> transformers.modeling_outputs.BaseModelOutputWithPoolingAndCrossAttentions:
+    def infer(self, sequences, output_hidden_states: bool = False, output_attentions: bool = False, return_logits: bool = False) -> transformers.modeling_outputs.BaseModelOutputWithPoolingAndCrossAttentions:
         import torch
         if not torch.cuda.is_available():
             raise Exception("CUDA is not available")
         print(f"Running inference on {sequences} sequences")
-        sequences = [str(sequence.seq) for sequence in sequences]
         tokenized = self.tokenizer(
             sequences, return_tensors="pt", add_special_tokens=False)['input_ids']
         tokenized = tokenized.to(self.device)
         with torch.inference_mode():
             outputs = self.model(tokenized, output_hidden_states=output_hidden_states,
                                  output_attentions=output_attentions)
         return outputs
 
     def __exit__(self, exc_type, exc_value, traceback):
         import torch
         torch.cuda.empty_cache()
 
 
-@stub.cls(gpu='A10G', timeout=2000, network_file_systems={CACHE_DIR: volume}, image=image, allow_cross_region_volumes=True, concurrency_limit=9)
+@stub.cls(gpu=gpu.A100(memory=80), timeout=2000, network_file_systems={CACHE_DIR: volume}, image=image, allow_cross_region_volumes=True, concurrency_limit=9)
 class EsmForMaskedLM():
     def __init__(self, device: str = "cuda", model_name: str = "facebook/esm2_t36_3B_UR50D"):
         import transformers
         self.tokenizer = transformers.AutoTokenizer.from_pretrained(
             model_name)
         self.model = transformers.AutoModelForMaskedLM.from_pretrained(
             model_name)
         self.device = device
         if device == "cuda":
             self.model = self.model.cuda()
         self.model.eval()
 
     @method()
+    def infer(self, sequence: str) -> transformers.modeling_outputs.MaskedLMOutput:
+        import torch
+        tokenized = self.tokenizer.encode(sequence, return_tensors='pt')
+        tokenized = tokenized.to(self.device)
+        with torch.inference_mode():
+            outputs = self.model(tokenized, return_dict=True)
+        return outputs
+
+    @method()
     def score(self, sequence: str, batch_size: int = 32) -> float:
         # Reference: Masked Language Model Scoring
         # https://arxiv.org/abs/1910.14659
         import torch
         import numpy as np
         tokenized = self.tokenizer.encode(sequence, return_tensors='pt')
         repeat_input = tokenized.repeat(tokenized.size(-1)-2, 1)
@@ -107,15 +124,69 @@
                 total_loss += loss.item() * batch_masked_input.size(0)
 
         # Calculate average loss
         avg_loss = total_loss / masked_input.size(0)
 
         return np.exp(avg_loss)
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    @method()
+    def entropies(self, sequence: str, batch_size: int = 32) -> list[float]:
+        """
+        Calculate the entropy for each residue position in a protein sequence by masking each residue and calculating the entropy of the masked position.
+        """
+        import torch
+        tokenized = self.tokenizer.encode(sequence, return_tensors='pt')
+        repeat_input = tokenized.repeat(tokenized.size(-1)-2, 1)
+
+        # mask one by one except [CLS] and [SEP]
+        mask = torch.ones(tokenized.size(-1) - 1).diag(1)[:-2]
+        masked_input = repeat_input.masked_fill(
+            mask == 1, self.tokenizer.mask_token_id)
+
+        labels = repeat_input.masked_fill(
+            masked_input != self.tokenizer.mask_token_id, -100)
+
+        # Initialize entropy list with zeros for each position in the sequence
+        # Subtract 2 for [CLS] and [SEP] tokens
+        entropies = [0.0] * len(sequence)
+        distributions = [torch.zeros(
+            self.model.config.vocab_size)] * len(sequence)
+        # Process in batches
+        for i in range(0, masked_input.size(0), batch_size):
+            batch_masked_input = masked_input[i:i+batch_size].to(self.device)
+            batch_labels = labels[i:i+batch_size].to(self.device)
+
+            with torch.inference_mode():
+                outputs = self.model(batch_masked_input, labels=batch_labels)
+                logits = outputs.logits
+                probabilities = torch.softmax(logits, dim=-1)
+                log_probabilities = torch.log(probabilities)
+                batch_entropy = - \
+                    torch.sum(probabilities * log_probabilities, dim=-1)
+                # Round to 4 decimal places
+                batch_entropy = torch.round(batch_entropy, decimals=4)
+                probabilities = torch.round(probabilities, decimals=4)
+                # check that probabilities sum to 1 roughly
+
+                # Update the corresponding positions in the entropies list
+                for j, entropy_value in enumerate(batch_entropy.cpu().tolist()):
+                    position = i+j
+                    entropies[position] = entropy_value[position+1]
+                    prob_distribution = probabilities[j,
+                                                      position + 1].cpu().numpy()
+                    distributions[position] = {
+                        self.tokenizer.decode([token_id]): prob
+                        for token_id, prob in enumerate(prob_distribution)
+                        if self.tokenizer.decode([token_id]).isalpha() and len(self.tokenizer.decode([token_id])) == 1
+                    }
+
+        return entropies, distributions
+
+    @modal.exit()
+    def empty_cache(self):
         import torch
         torch.cuda.empty_cache()
 
 
 @stub.cls(gpu="A10G", timeout=6000, network_file_systems={CACHE_DIR: volume}, image=image)
 class ESMFold():
     def __init__(self, device: str = "cuda"):
@@ -216,7 +287,57 @@
     sequences = list(SeqIO.parse(fasta_file, "fasta"))
     result = predict_structures.remote(sequences, batch_size=batch_size)
     os.makedirs(output_dir, exist_ok=True)
     for struct in result:
         io = PDBIO()
         io.set_structure(struct)
         io.save(f"{output_dir}/{struct.id}.pdb")
+
+
+@stub.local_entrypoint()
+def predict_structures_from_csv(csv_file: str, id_column: str, sequence_column: str, output_dir: str, batch_size: int = 1):
+    """
+    Predicts protein structures from a given CSV file and saves them as PDB files in the specified output directory.
+
+    Args:
+        csv_file (str): Path to the CSV file containing protein sequences with their IDs.
+        id_column (str): The name of the column in the CSV file that contains the sequence IDs.
+        sequence_column (str): The name of the column in the CSV file that contains the protein sequences.
+        output_dir (str): Directory where the PDB files will be saved.
+        batch_size (int): Number of sequences to process in a batch. Default is 1 due to high memory usage of the model.
+                            For shorter sequences, the batch size can be increased.
+    """
+    import pandas as pd
+    df = pd.read_csv(csv_file)
+    if id_column not in df.columns or sequence_column not in df.columns:
+        raise ValueError(
+            f"CSV file must contain '{id_column}' and '{sequence_column}' columns.")
+
+    sequences = []
+    for _, row in df.iterrows():
+        sequences.append(
+            SeqRecord(Seq(row[sequence_column]), id=str(row[id_column])))
+
+    result = predict_structures.remote(
+        sequences, batch_size=batch_size)
+    os.makedirs(output_dir, exist_ok=True)
+    for struct in result:
+        io = PDBIO()
+        io.set_structure(struct)
+        io.save(f"{output_dir}/{struct.id}.pdb")
+
+
+@stub.local_entrypoint()
+def calculate_entropy(sequence: str, model_name: str = "facebook/esm2_t36_3B_UR50D") -> list[float]:
+    """
+    Calculate the entropy for each residue position in a protein sequence.
+
+    Args:
+        sequence (str): A single protein sequence.
+        model_name (str): Name of the model to use for entropy calculation. Default is 'facebook/esm2_t36_3B_UR50D'.
+
+    Returns:
+        list[float]: A list of entropy values for each residue position in the sequence.
+    """
+    model = EsmModel(model_name=model_name)
+    entropy = model.get_entropy.remote(sequence)
+    return entropy.tolist()
```

### Comparing `helixbio-0.1.8/helix/evoprotgrad.py` & `helixbio-0.1.9/helix/evoprotgrad.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import hashlib
 from pprint import pprint
 from modal import Image, method
 import pandas as pd
 from .main import stub
 
+
+def download_esm_models(slugs: list[str] = ["facebook/esm1b_t33_650M_UR50S", "facebook/esm2_t33_650M_UR50D", "facebook/esm2_t36_3B_UR50D", "facebook/esm2_t48_15B_UR50D"]):
+    from transformers import EsmForMaskedLM, AutoTokenizer
+    for slug in slugs:
+        EsmForMaskedLM.from_pretrained(slug)
+        AutoTokenizer.from_pretrained(slug)
+
+
 image = Image.debian_slim().pip_install(
     "transformers[torch]==4.30.0",
     "torch",
     "evo_prot_grad",
-    "pandas")
+    "pandas").run_function(download_esm_models)
 
 
-@stub.cls(gpu='A10G', timeout=2000, image=image, allow_cross_region_volumes=True, concurrency_limit=9)
+@stub.cls(gpu='A100', timeout=2000, image=image, allow_cross_region_volumes=True, concurrency_limit=9)
 class EvoProtGrad:
     def __init__(self, experts: list[str] = ["esm"], device: str = "cuda"):
         from evo_prot_grad import get_expert
         from transformers import EsmForMaskedLM, AutoTokenizer
         self.experts = []
         for expert in experts:
             model = None
```

### Comparing `helixbio-0.1.8/helix/main.py` & `helixbio-0.1.9/helix/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 VOLUME_NAME = "job-storage-vol"
 
 CACHE_DIR = "/cache"
 
 RESULTS_DIR = pathlib.Path(CACHE_DIR, "results")
 
-volume = NetworkFileSystem.persisted(VOLUME_NAME)
+volume = NetworkFileSystem.from_name(VOLUME_NAME)
 
 
 web_app = FastAPI()
 stub = Stub(name="helix", mounts=[Mount.from_local_python_packages("helix")])
 image = Image.debian_slim()
```

### Comparing `helixbio-0.1.8/helix/proteinmpnn.py` & `helixbio-0.1.9/helix/proteinmpnn.py`

 * *Files identical despite different names*

### Comparing `helixbio-0.1.8/helix/utils.py` & `helixbio-0.1.9/helix/utils.py`

 * *Files identical despite different names*

### Comparing `helixbio-0.1.8/pyproject.toml` & `helixbio-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "helixbio"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Ragnor Comerford <hello@ragnor.co>"]
 readme = "README.md"
 packages = [
     { include = "helix", from = "./" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 biopython = "^1.81"
-modal = "^0.55.4127"
+modal = "^0.62.43"
 dnachisel = "^3.2.11"
 torch = "^2.0.1"
 transformers = "^4.30.0"
 matplotlib = "^3.8.0"
 evo-prot-grad = "^0.1.4"
 pandas = "^2.1.4"
+litellm = "^1.18.1"
+openpyxl = "^3.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.291"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `helixbio-0.1.8/PKG-INFO` & `helixbio-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: helixbio
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Ragnor Comerford
 Author-email: hello@ragnor.co
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: biopython (>=1.81,<2.0)
 Requires-Dist: dnachisel (>=3.2.11,<4.0.0)
 Requires-Dist: evo-prot-grad (>=0.1.4,<0.2.0)
+Requires-Dist: litellm (>=1.18.1,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
-Requires-Dist: modal (>=0.55.4127,<0.56.0)
+Requires-Dist: modal (>=0.62.43,<0.63.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: transformers (>=4.30.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 logo
```

