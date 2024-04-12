# Comparing `tmp/bearclaw-0.0.3.tar.gz` & `tmp/bearclaw-0.0.4.tar.gz`

## Comparing `bearclaw-0.0.3.tar` & `bearclaw-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,40 @@
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bearclaw-0.0.3/.dockerignore
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 bearclaw-0.0.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 bearclaw-0.0.3/Dockerfile
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 bearclaw-0.0.3/Dockerfile.GRCh37
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bearclaw-0.0.3/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bearclaw-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/_version.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/feature_extraction.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/preprocessing.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/transforms.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/io/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/io/tso.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/io/vcf.py
--rw-r--r--   0        0        0    18940 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_CN_GRCh37.txt
--rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_DBS_GRCh37.txt
--rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_ID_GRCh37.txt
--rw-r--r--   0        0        0   149327 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_SBS_GRCh37.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/__init__.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/test_feature_extraction.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/test_io.py
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/test_transforms.py
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/test_vcf.py
--rw-r--r--   0        0        0    14741 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh37/sample1.vcf
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh37/sample1.vcf.gz
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh37/sample2.vcf
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh37/tso500.example.vcf
--rw-r--r--   0        0        0    13758 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/GRCh38/sample1.vcf
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 bearclaw-0.0.3/src/test/resources/tso500/example_TMB_Trace.tsv
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 bearclaw-0.0.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bearclaw-0.0.3/LICENSE
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bearclaw-0.0.3/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 bearclaw-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 bearclaw-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bearclaw-0.0.4/.dockerignore
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 bearclaw-0.0.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bearclaw-0.0.4/Dockerfile
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 bearclaw-0.0.4/Dockerfile.GRCh37
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bearclaw-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bearclaw-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/_version.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/feature_extraction.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/preprocessing.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/transforms.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/io/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/io/tso.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/io/vcf.py
+-rw-r--r--   0        0        0    18940 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.3_CN_GRCh37.txt
+-rw-r--r--   0        0        0    17759 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.3_DBS_GRCh37.txt
+-rw-r--r--   0        0        0    29808 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.3_ID_GRCh37.txt
+-rw-r--r--   0        0        0   149327 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.3_SBS_GRCh37.txt
+-rw-r--r--   0        0        0    13831 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.4_CN_GRCh37.txt
+-rw-r--r--   0        0        0    18328 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.4_DBS_GRCh37.txt
+-rw-r--r--   0        0        0    22118 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.4_ID_GRCh37.txt
+-rw-r--r--   0        0        0    12145 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.4_RNA-SBS_GRCh37.txt
+-rw-r--r--   0        0        0    96398 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.4_SBS_GRCh37.txt
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.4_SV_GRCh38.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/__init__.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/test_feature_extraction.py
+-rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/test_io.py
+-rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/test_transforms.py
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/test_vcf.py
+-rw-r--r--   0        0        0    14741 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/resources/GRCh37/sample1.vcf
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/resources/GRCh37/sample1.vcf.gz
+-rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/resources/GRCh37/sample2.vcf
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/resources/GRCh37/tso500.example.vcf
+-rw-r--r--   0        0        0    13758 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/resources/GRCh38/sample1.vcf
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 bearclaw-0.0.4/src/test/resources/tso500/example_TMB_Trace.tsv
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 bearclaw-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bearclaw-0.0.4/LICENSE
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 bearclaw-0.0.4/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 bearclaw-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 bearclaw-0.0.4/PKG-INFO
```

### Comparing `bearclaw-0.0.3/.gitlab-ci.yml` & `bearclaw-0.0.4/.gitlab-ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 test:
   image: registry.gitlab.com/hylkedonker/bearclaw/grch37
   stage: test
   tags:
     - deployment
   script:
     - export DEBIAN_FRONTEND="noninteractive"
-    - pip3 install coverage
-    - cd src
-    - coverage run -m --source=bearclaw unittest discover test
-    - coverage report -m
-    - coverage xml
+    # - pip3 install coverage
+    # - cd src
+    # - coverage run -m --source=bearclaw unittest discover test
+    # - coverage report -m
+    # - coverage xml
   coverage: '/(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/'
   artifacts:
     reports:
       coverage_report:
         coverage_format: cobertura
         path: src/coverage.xml
 
@@ -29,37 +29,37 @@
     - name: arm64v8/docker:dind
       alias: docker
   variables:
     DOCKER_HOST: tcp://docker:2375
   tags:
     - deployment
   script:
-    - docker login -u gitlab-ci-token -p $CI_BUILD_TOKEN $CI_REGISTRY
+    - docker login -u $CI_REGISTRY_USER -p $CI_REGISTRY_PASSWORD $CI_REGISTRY
     # Install dependencies to build multi-architecture Dockerfile.
     - docker run --privileged --rm tonistiigi/binfmt --install all
     - docker buildx create --use
-    - docker buildx build
-      --push
-      --platform linux/amd64,linux/arm64,linux/arm/v7
-      -f Dockerfile.GRCh37
-      -t registry.gitlab.com/hylkedonker/bearclaw/grch37:${CI_COMMIT_SHORT_SHA}
-      -t registry.gitlab.com/hylkedonker/bearclaw/grch37:latest
-      .
+    # - docker buildx build
+    #   --push
+    #   --platform linux/amd64,linux/arm64,linux/arm/v7
+    #   -f Dockerfile.GRCh37
+    #   -t registry.gitlab.com/hylkedonker/bearclaw/grch37:${CI_COMMIT_SHORT_SHA}
+    #   -t registry.gitlab.com/hylkedonker/bearclaw/grch37:latest
+    #   .
     - docker buildx build
       --push
       --platform linux/amd64,linux/arm64,linux/arm/v7
       -f Dockerfile
       -t registry.gitlab.com/hylkedonker/bearclaw:${CI_COMMIT_SHORT_SHA}
       -t registry.gitlab.com/hylkedonker/bearclaw:latest
       .
   only:
   - main
 
 pages:
-  image: python:3.10
+  image: python:3.11
   stage: deploy
   tags:
     - deployment
   script:
   - pip3 install -r requirements.txt
   - pip3 install pdoc3
   - mkdir public
```

### Comparing `bearclaw-0.0.3/Dockerfile.GRCh37` & `bearclaw-0.0.4/Dockerfile.GRCh37`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM ubuntu:22.10
+FROM ubuntu:24.04
 
 ARG DEBIAN_FRONTEND=noninteractive
 
 RUN apt clean && apt update && \
     apt install --no-install-recommends --assume-yes \
     wget \
     python3-pip \
@@ -10,16 +10,16 @@
     python3-pandas \
     python3-statsmodels \
     python3-sklearn \
     python3-pysam
 
 WORKDIR /opt/
 
-RUN pip3 install --no-dependencies SigProfilerPlotting
-RUN pip3 install --no-dependencies SigProfilerMatrixGenerator
+RUN pip3 install --break-system-packages --no-dependencies SigProfilerPlotting
+RUN pip3 install --break-system-packages --no-dependencies SigProfilerMatrixGenerator
 
 
 # Install `GRCh37`, may take a long time!
 RUN python3 -c 'from SigProfilerMatrixGenerator import install; install.install("GRCh37", rsync=False, bash=True)'
 
 
 RUN pip3 install vcfpy
```

### Comparing `bearclaw-0.0.3/src/bearclaw/preprocessing.py` & `bearclaw-0.0.4/src/bearclaw/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         elif coverage_size in dataframe.columns:
             normalisation = dataframe[coverage_size]
         else:
             raise KeyError(f"Unknown column {coverage_size}.")
 
         X = []
         # Loop trough all label directories.
-        for index, filename in dataframe[x_col].iteritems():
+        for index, filename in dataframe[x_col].items():
             x_i = self._transform_x(Path(filename))
             # Normalise estimate by exome size.
             x_i /= normalisation[index]
 
             # Concatenate other columns.
             if keep_columns:
                 if x_i.index.nlevels > 1:
```

### Comparing `bearclaw-0.0.3/src/bearclaw/transforms.py` & `bearclaw-0.0.4/src/bearclaw/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from pathlib import Path
 
 from pandas import DataFrame, concat
 
-from bearclaw.feature_extraction import CosmicNMF, POSSIBLE_SBS_SEQUENCING_ARTEFACTS
+from bearclaw.feature_extraction import (
+    CosmicNMF,
+    POSSIBLE_SBS_SEQUENCING_ARTEFACTS,
+    POSSIBLE_DB_SEQUENCING_ARTEFACTS,
+)
 from bearclaw.io import extract_mutation_spectra, from_tso500_trace, vcf
 
 
 def spectrum(vcf_file: Path, exome: bool = False) -> DataFrame:
     """Extract single + doublet base substitutions and indel spectra from VCF file."""
     mutation_matrices = extract_mutation_spectra(vcf_file, exome=exome)
     spectra = list(mutation_matrices.values())
@@ -52,15 +56,17 @@
         "indel",
     ]:
         decomposer = CosmicNMF(cosmic_signature=spectrum)  # type: ignore
         signatures.append(decomposer.transform(mutation_matrices[spectrum]))
 
     result = concat(signatures, axis="columns")
     if filter_seq_artefact_signatures:
-        return result.drop(columns=POSSIBLE_SBS_SEQUENCING_ARTEFACTS)
+        return result.drop(columns=POSSIBLE_SBS_SEQUENCING_ARTEFACTS).drop(
+            columns=POSSIBLE_DB_SEQUENCING_ARTEFACTS
+        )
     return result
 
 
 @from_tso500_trace
 def mutational_signature_from_trace(
     trace_file: Path, filter_seq_artefact_signatures: bool = True
 ) -> DataFrame:
```

### Comparing `bearclaw-0.0.3/src/bearclaw/io/__init__.py` & `bearclaw-0.0.4/src/bearclaw/io/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,16 +58,16 @@
             target_vcf = Path(tmp_dir) / input_vcf.name
             copyfile(str(input_vcf), str(target_vcf))
 
         # Unique project name.
         name = "mutation-class"
         matrices = matGen.SigProfilerMatrixGeneratorFunc(
             project=name,
-            genome="GRCh37",
-            vcfFiles=tmp_dir,
+            reference_genome="GRCh37",
+            path_to_input_files=tmp_dir,
             plot=False,
             exome=exome,
             seqInfo=False,
         )
 
     index = input_vcf.name.split(".")[0]
```

### Comparing `bearclaw-0.0.3/src/bearclaw/io/tso.py` & `bearclaw-0.0.4/src/bearclaw/io/tso.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/bearclaw/io/vcf.py` & `bearclaw-0.0.4/src/bearclaw/io/vcf.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_CN_GRCh37.txt` & `bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.3_CN_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_DBS_GRCh37.txt` & `bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.3_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_ID_GRCh37.txt` & `bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.3_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/bearclaw/resources/COSMIC_v3.3_SBS_GRCh37.txt` & `bearclaw-0.0.4/src/bearclaw/resources/COSMIC_v3.3_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/test/test_feature_extraction.py` & `bearclaw-0.0.4/src/test/test_feature_extraction.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,46 +18,50 @@
 
     def setUp(self):
         # Fix seed for reproducibility.
         random.seed(1234)
 
     def test_single_base_substitution(self):
         """Test identity transformation for single base substitutions."""
-        signature_file = _COSMIC_MUTATIONAL_SIGNATURES["single_base_substitutions"]
-        # signature_file = "COSMIC_v3_SBS_GRCh37_noSBS84-85.txt"
-        H = read_csv(signature_file, sep="\t", index_col=0)
+        signature_file = _COSMIC_MUTATIONAL_SIGNATURES["3.4"][
+            "single_base_substitutions"
+        ]
+        weights = read_csv(signature_file, sep="\t", index_col=0).T
 
         # Test very specific activation functions.
-        W_true = DataFrame(0, index=range(2), columns=H.columns)
-        W_true.loc[0, "SBS3"] = 2600
-        W_true.loc[1, "SBS3"] = 3757
-        W_true.loc[0, "SBS5"] = 1240
-        W_true.loc[1, "SBS5"] = 277
-        W_true.loc[0, "SBS40"] = 2952
-        W_true.loc[1, "SBS40"] = 1245
+        H_true = DataFrame(0, index=range(2), columns=weights.index)
+        H_true.loc[0, "SBS3"] = 2600
+        H_true.loc[1, "SBS3"] = 3757
+        H_true.loc[0, "SBS5"] = 1240
+        H_true.loc[1, "SBS5"] = 277
+        H_true.loc[0, "SBS40a"] = 2952
+        H_true.loc[1, "SBS40a"] = 1245
 
         # Construct mutational spectrum from random W.
-        X = H @ W_true.transpose()
+        X = H_true @ weights
 
         decomposer = CosmicNMF(cosmic_signature="single_base_substitutions")
-        W_reconstr = decomposer.transform(X.T)
+        H_reconstr = decomposer.transform(X)
 
         # They should be (nearly) identical.
-        error = abs(W_reconstr - W_true)
-        relative_error = linalg.norm(error) / linalg.norm(W_true)
-        assert_array_almost_equal(relative_error, zeros_like(relative_error), decimal=3)
+        error = abs(H_reconstr - H_true)
+        relative_error = linalg.norm(error) / linalg.norm(H_true)
+        assert_array_almost_equal(relative_error, zeros_like(relative_error), decimal=2)
 
     def test_random_single_base_substitution(self):
         """Test identity transformation for single base substitutions."""
-        signature_file = _COSMIC_MUTATIONAL_SIGNATURES["single_base_substitutions"]
+        signature_file = _COSMIC_MUTATIONAL_SIGNATURES["3.4"][
+            "single_base_substitutions"
+        ]
         H = read_csv(signature_file, sep="\t", index_col=0).T
 
         m_samples = 3
         n_components = H.shape[0]
-        activations = random.randint(0, 2, size=(m_samples, n_components))
+        # We require >50 observations per sample.
+        activations = random.randint(0, 2, size=(m_samples, n_components)) * 5
         W_true = DataFrame(activations, columns=H.index)
 
         # Construct mutational spectrum from random W.
         X = W_true @ H
 
         decomposer = CosmicNMF(cosmic_signature="single_base_substitutions")
         W_reconstr = decomposer.transform(X)
@@ -65,46 +69,50 @@
         # They should be (nearly) identical.
         error = abs(W_reconstr - W_true)
         relative_error = linalg.norm(error) / linalg.norm(W_true)
         assert_array_almost_equal(relative_error, zeros_like(relative_error), decimal=1)
 
     def test_doublet_base_substitution(self):
         """Test identity transformation for doublet base substitutions."""
-        signature_file = _COSMIC_MUTATIONAL_SIGNATURES["doublet_base_substitutions"]
+        signature_file = _COSMIC_MUTATIONAL_SIGNATURES["3.4"][
+            "doublet_base_substitutions"
+        ]
         H = read_csv(signature_file, sep="\t", index_col=0).T
 
         m_samples = 3
         n_components = H.shape[0]
-        activations = random.randint(0, 2, size=(m_samples, n_components))
+        # We require >50 observations per sample.
+        activations = random.randint(0, 2, size=(m_samples, n_components)) * 5
         W_true = DataFrame(activations, columns=H.index)
 
         # Construct mutational spectrum from random W.
         X = W_true @ H
 
         decomposer = CosmicNMF(cosmic_signature="doublet_base_substitutions")
         W_reconstr = decomposer.transform(X)
 
         # They should be (nearly) identical.
         error = abs(W_reconstr - W_true)
         relative_error = linalg.norm(error) / linalg.norm(W_true)
-        assert_array_almost_equal(relative_error, zeros_like(relative_error), decimal=4)
+        assert_array_almost_equal(relative_error, zeros_like(relative_error), decimal=3)
 
     def test_indel(self):
         """Test identity transformation for indels."""
-        signature_file = _COSMIC_MUTATIONAL_SIGNATURES["indel"]
+        signature_file = _COSMIC_MUTATIONAL_SIGNATURES["3.4"]["indel"]
         H = read_csv(signature_file, sep="\t", index_col=0).T
 
         m_samples = 3
         n_components = H.shape[0]
-        activations = random.randint(0, 2, size=(m_samples, n_components))
+        # We require >50 observations per sample.
+        activations = random.randint(0, 2, size=(m_samples, n_components)) * 5
         W_true = DataFrame(activations, columns=H.index)
 
         # Construct mutational spectrum from random W.
         X = W_true @ H
 
         decomposer = CosmicNMF(cosmic_signature="indel")
         W_reconstr = decomposer.transform(X)
 
         # They should be (nearly) identical.
         error = abs(W_reconstr - W_true)
         relative_error = linalg.norm(error) / linalg.norm(W_true)
-        assert_array_almost_equal(relative_error, zeros_like(relative_error), decimal=4)
+        assert_array_almost_equal(relative_error, zeros_like(relative_error), decimal=3)
```

### Comparing `bearclaw-0.0.3/src/test/test_io.py` & `bearclaw-0.0.4/src/test/test_io.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/test/test_transforms.py` & `bearclaw-0.0.4/src/test/test_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from numpy.linalg import norm
 from numpy.testing import assert_almost_equal, assert_array_almost_equal
 from pandas import DataFrame, read_csv
 
 from bearclaw.feature_extraction import (
     _get_cosmic_feature_names,
     POSSIBLE_SBS_SEQUENCING_ARTEFACTS,
+    POSSIBLE_DB_SEQUENCING_ARTEFACTS,
     _COSMIC_MUTATIONAL_SIGNATURES,
     CosmicNMF,
 )
 from bearclaw.preprocessing import VariantDataGenerator
 from bearclaw.transforms import mutational_signature, non_synonymous_spectrum, spectrum
 
 TEST_RESOURCES = Path(__file__).parent.resolve() / "resources"
@@ -98,15 +99,19 @@
     def test_sbs_filter_sequencing_artefacts(self):
         """Verify that all SBS sequencing artefacts are removed."""
         dg = VariantDataGenerator(transform=mutational_signature)
         X, _ = dg.flow_from_dataframe(self.dataframe, keep_columns=False, x_col="vcf")
 
         self.assertEqual(
             len(X.columns),
-            11 + 78 + 18 - len(POSSIBLE_SBS_SEQUENCING_ARTEFACTS),
+            23
+            + 86
+            + 20
+            - len(POSSIBLE_SBS_SEQUENCING_ARTEFACTS)
+            - len(POSSIBLE_DB_SEQUENCING_ARTEFACTS),
         )
 
     def test_sbs_mutational_signature(self):
         """Test non-synonymous single base substitution mutational signature."""
         dg = VariantDataGenerator(
             transform=lambda x: mutational_signature(
                 x, filter_seq_artefact_signatures=False
@@ -128,15 +133,15 @@
         # mutation in the approximate ratios. So we expect almost complete
         # SBS48 activation. Lets validate.
         W_reconstr, _ = dg.flow_from_dataframe(
             self.dataframe, decimals=None, x_col="vcf", keep_columns=False
         )
 
         H = read_csv(
-            _COSMIC_MUTATIONAL_SIGNATURES["single_base_substitutions"],
+            _COSMIC_MUTATIONAL_SIGNATURES["3.4"]["single_base_substitutions"],
             sep="\t",
             index_col=0,
         ).T
 
         # Verify that SBS48 is the most activated state.
         sample2 = "dummy2"
         self.assertEqual(W_reconstr.loc[sample2].idxmax(), "SBS48")
```

### Comparing `bearclaw-0.0.3/src/test/test_vcf.py` & `bearclaw-0.0.4/src/test/test_vcf.py`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/test/resources/GRCh37/sample1.vcf` & `bearclaw-0.0.4/src/test/resources/GRCh37/sample1.vcf`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/test/resources/GRCh37/sample1.vcf.gz` & `bearclaw-0.0.4/src/test/resources/GRCh37/sample1.vcf.gz`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/test/resources/GRCh37/sample2.vcf` & `bearclaw-0.0.4/src/test/resources/GRCh37/sample2.vcf`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/test/resources/GRCh37/tso500.example.vcf` & `bearclaw-0.0.4/src/test/resources/GRCh37/tso500.example.vcf`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/test/resources/GRCh38/sample1.vcf` & `bearclaw-0.0.4/src/test/resources/GRCh38/sample1.vcf`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/src/test/resources/tso500/example_TMB_Trace.tsv` & `bearclaw-0.0.4/src/test/resources/tso500/example_TMB_Trace.tsv`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/.gitignore` & `bearclaw-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bearclaw-0.0.3/LICENSE` & `bearclaw-0.0.4/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Hylke C. Donker
+Copyright (c) 2024 Hylke C. Donker
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bearclaw-0.0.3/pyproject.toml` & `bearclaw-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bearclaw"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Hylke C. Donker", email="h.c.donker@umcg.nl" },
 ]
 description = "Pipeline components to extract features from variants."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `bearclaw-0.0.3/PKG-INFO` & `bearclaw-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: bearclaw
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pipeline components to extract features from variants.
 Project-URL: Homepage, https://gitlab.com/hylkedonker/bearclaw
 Project-URL: Bug Tracker, https://gitlab.com/hylkedonker/bearclaw/-/issues
 Author-email: "Hylke C. Donker" <h.c.donker@umcg.nl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,8 +42,8 @@
 ```
 
 ## Reference documentation
 https://hylkedonker.gitlab.io/bearclaw/
 
 
 ## License
-For open source projects, say how it is licensed.
+The code in this repository is licensed under the  [MIT License](LICENSE).
```

