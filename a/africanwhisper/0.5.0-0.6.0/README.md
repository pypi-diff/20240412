# Comparing `tmp/africanwhisper-0.5.0.tar.gz` & `tmp/africanwhisper-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "africanwhisper-0.5.0.tar", last modified: Thu Apr 11 12:32:53 2024, max compression
+gzip compressed data, was "africanwhisper-0.6.0.tar", last modified: Thu Apr 11 12:46:39 2024, max compression
```

## Comparing `africanwhisper-0.5.0.tar` & `africanwhisper-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.581253 africanwhisper-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/src/africanwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 12:32:53.000000 africanwhisper-0.5.0/src/africanwhisper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.581253 africanwhisper-0.5.0/src/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/deployment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/deployment/speech_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.581253 africanwhisper-0.5.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/tests/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:53.585253 africanwhisper-0.5.0/src/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/audio_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/collator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/gradio_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/gradio_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/wandb_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-11 12:32:50.000000 africanwhisper-0.5.0/src/training/whisper_model_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:46:39.685396 africanwhisper-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-11 12:46:39.685396 africanwhisper-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-11 12:46:39.685396 africanwhisper-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:46:39.677396 africanwhisper-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:46:39.681396 africanwhisper-0.6.0/src/africanwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-04-11 12:46:39.000000 africanwhisper-0.6.0/src/africanwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-11 12:46:39.000000 africanwhisper-0.6.0/src/africanwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:46:39.000000 africanwhisper-0.6.0/src/africanwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-11 12:46:39.000000 africanwhisper-0.6.0/src/africanwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 12:46:39.000000 africanwhisper-0.6.0/src/africanwhisper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:46:39.681396 africanwhisper-0.6.0/src/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/deployment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/deployment/speech_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:46:39.681396 africanwhisper-0.6.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/tests/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:46:39.681396 africanwhisper-0.6.0/src/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/audio_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/collator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/gradio_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/gradio_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/wandb_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-11 12:46:28.000000 africanwhisper-0.6.0/src/training/whisper_model_prep.py
```

### Comparing `africanwhisper-0.5.0/LICENSE` & `africanwhisper-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/PKG-INFO` & `africanwhisper-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -103,15 +103,15 @@
 ## Step 2: Set Parameters
 
 ```python
 # Set the parameters (refer to the 'Usage on VM' section for more details)
 huggingface_read_token = " "
 huggingface_write_token = " "
 dataset_name = "mozilla-foundation/common_voice_16_1" 
-language_abbr= " "                                    # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
+language_abbr= [ ]                                    # Example `["ti", "yi"]`. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
                                                       # Note: choose a small dataset so as to not run out of memory,
 model_id= "model-id"                                  # Example openai/whisper-small, openai/whisper-medium
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
 use_peft = True                                       # Note: PEFT only works on a notebook with GPU-support.
 
 ```
@@ -153,15 +153,14 @@
     huggingface_write_token,
     model_id,
     processed_dataset,
     model,
     feature_processor,
     feature_extractor,
     tokenizer,
-    language_abbr,
     wandb_api_key,
     use_peft
 )
 trainer.train(
     max_steps=100,
     learning_rate=1e-3,
     per_device_train_batch_size=96,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.5.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.6.0 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
@@ -45,42 +45,43 @@
 //colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/16r4cxP-dSFplRTfgPLbzGXYRzBIUqpx9?usp=sharing)
 ## Step 1: Installation ```python !pip install africanwhisper # If you're on
 Colab, restart the session due to issue with numpy installation on colab. ```
 ## Step 2: Set Parameters ```python # Set the parameters (refer to the 'Usage
 on VM' section for more details) huggingface_read_token = " "
 huggingface_write_token = " " dataset_name = "mozilla-foundation/
-common_voice_16_1" language_abbr= " " # Example 'af', 'sw'. see abbreviations
-here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. #
-Note: choose a small dataset so as to not run out of memory, model_id= "model-
-id" # Example openai/whisper-small, openai/whisper-medium processing_task=
-"automatic-speech-recognition" wandb_api_key = " " use_peft = True # Note: PEFT
-only works on a notebook with GPU-support. ``` ## Step 3: Prepare the Model
-```python from training.data_prep import DataPrep # Initialize the DataPrep
-class and prepare the model process = DataPrep( huggingface_read_token,
-dataset_name, language_abbr, model_id, processing_task, use_peft ) tokenizer,
-feature_extractor, feature_processor, model = process.prepare_model() ``` ##
-Step 4: Preprocess the Dataset ```python # Load and preprocess the dataset
-processed_dataset = process.load_dataset( feature_extractor=feature_extractor,
-tokenizer=tokenizer, processor=feature_processor ) ``` ## Step 5: Train the
-Model ```python from training.model_trainer import Trainer # Initialize the
-Trainer class and train the model trainer = Trainer( huggingface_write_token,
-model_id, processed_dataset, model, feature_processor, feature_extractor,
-tokenizer, language_abbr, wandb_api_key, use_peft ) trainer.train
-( max_steps=100, learning_rate=1e-3, per_device_train_batch_size=96,
-per_device_eval_batch_size=64, optim="adamw_bnb_8bit" ) # Optional parameters
-for training: # max_steps (int): The maximum number of training steps (default
-is 100). # learning_rate (float): The learning rate for training (default is
-1e-5). # per_device_train_batch_size (int): The batch size per GPU for training
-(default is 96). # per_device_eval_batch_size (int): The batch size per GPU for
-evaluation (default is 64). # optim (str): The optimizer used for training
-(default is "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI
-```python from training.gradio_inference import WhisperDemo # Generate a demo
-model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/
-whisper-small-af" demo = WhisperDemo(model_name, huggingface_read_token)
+common_voice_16_1" language_abbr= [ ] # Example `["ti", "yi"]`. see
+abbreviations here https://huggingface.co/datasets/mozilla-foundation/
+common_voice_16_1. # Note: choose a small dataset so as to not run out of
+memory, model_id= "model-id" # Example openai/whisper-small, openai/whisper-
+medium processing_task= "automatic-speech-recognition" wandb_api_key = " "
+use_peft = True # Note: PEFT only works on a notebook with GPU-support. ``` ##
+Step 3: Prepare the Model ```python from training.data_prep import DataPrep #
+Initialize the DataPrep class and prepare the model process = DataPrep
+( huggingface_read_token, dataset_name, language_abbr, model_id,
+processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
+model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
+# Load and preprocess the dataset processed_dataset = process.load_dataset
+( feature_extractor=feature_extractor, tokenizer=tokenizer,
+processor=feature_processor ) ``` ## Step 5: Train the Model ```python from
+training.model_trainer import Trainer # Initialize the Trainer class and train
+the model trainer = Trainer( huggingface_write_token, model_id,
+processed_dataset, model, feature_processor, feature_extractor, tokenizer,
+wandb_api_key, use_peft ) trainer.train( max_steps=100, learning_rate=1e-3,
+per_device_train_batch_size=96, per_device_eval_batch_size=64,
+optim="adamw_bnb_8bit" ) # Optional parameters for training: # max_steps (int):
+The maximum number of training steps (default is 100). # learning_rate (float):
+The learning rate for training (default is 1e-5). # per_device_train_batch_size
+(int): The batch size per GPU for training (default is 96). #
+per_device_eval_batch_size (int): The batch size per GPU for evaluation
+(default is 64). # optim (str): The optimizer used for training (default is
+"adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI ```python from
+training.gradio_inference import WhisperDemo # Generate a demo model_name =
+"your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-
+small-af" demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python from
 deployment.speech_inference import SpeechInference model_name = "your-
 finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " " task = "desired-task" # either 'translate' or
 'transcribe' audiofile_dir = "location-of-audio-file" # filetype should be .mp3
 or .wav # Initialize the SpeechInference class and run inference inference =
 SpeechInference(model_name, huggingface_read_token) pipeline =
```

### Comparing `africanwhisper-0.5.0/README.md` & `africanwhisper-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 ## Step 2: Set Parameters
 
 ```python
 # Set the parameters (refer to the 'Usage on VM' section for more details)
 huggingface_read_token = " "
 huggingface_write_token = " "
 dataset_name = "mozilla-foundation/common_voice_16_1" 
-language_abbr= " "                                    # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
+language_abbr= [ ]                                    # Example `["ti", "yi"]`. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
                                                       # Note: choose a small dataset so as to not run out of memory,
 model_id= "model-id"                                  # Example openai/whisper-small, openai/whisper-medium
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
 use_peft = True                                       # Note: PEFT only works on a notebook with GPU-support.
 
 ```
@@ -119,15 +119,14 @@
     huggingface_write_token,
     model_id,
     processed_dataset,
     model,
     feature_processor,
     feature_extractor,
     tokenizer,
-    language_abbr,
     wandb_api_key,
     use_peft
 )
 trainer.train(
     max_steps=100,
     learning_rate=1e-3,
     per_device_train_batch_size=96,
```

#### html2text {}

```diff
@@ -29,42 +29,43 @@
 //colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/16r4cxP-dSFplRTfgPLbzGXYRzBIUqpx9?usp=sharing)
 ## Step 1: Installation ```python !pip install africanwhisper # If you're on
 Colab, restart the session due to issue with numpy installation on colab. ```
 ## Step 2: Set Parameters ```python # Set the parameters (refer to the 'Usage
 on VM' section for more details) huggingface_read_token = " "
 huggingface_write_token = " " dataset_name = "mozilla-foundation/
-common_voice_16_1" language_abbr= " " # Example 'af', 'sw'. see abbreviations
-here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. #
-Note: choose a small dataset so as to not run out of memory, model_id= "model-
-id" # Example openai/whisper-small, openai/whisper-medium processing_task=
-"automatic-speech-recognition" wandb_api_key = " " use_peft = True # Note: PEFT
-only works on a notebook with GPU-support. ``` ## Step 3: Prepare the Model
-```python from training.data_prep import DataPrep # Initialize the DataPrep
-class and prepare the model process = DataPrep( huggingface_read_token,
-dataset_name, language_abbr, model_id, processing_task, use_peft ) tokenizer,
-feature_extractor, feature_processor, model = process.prepare_model() ``` ##
-Step 4: Preprocess the Dataset ```python # Load and preprocess the dataset
-processed_dataset = process.load_dataset( feature_extractor=feature_extractor,
-tokenizer=tokenizer, processor=feature_processor ) ``` ## Step 5: Train the
-Model ```python from training.model_trainer import Trainer # Initialize the
-Trainer class and train the model trainer = Trainer( huggingface_write_token,
-model_id, processed_dataset, model, feature_processor, feature_extractor,
-tokenizer, language_abbr, wandb_api_key, use_peft ) trainer.train
-( max_steps=100, learning_rate=1e-3, per_device_train_batch_size=96,
-per_device_eval_batch_size=64, optim="adamw_bnb_8bit" ) # Optional parameters
-for training: # max_steps (int): The maximum number of training steps (default
-is 100). # learning_rate (float): The learning rate for training (default is
-1e-5). # per_device_train_batch_size (int): The batch size per GPU for training
-(default is 96). # per_device_eval_batch_size (int): The batch size per GPU for
-evaluation (default is 64). # optim (str): The optimizer used for training
-(default is "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI
-```python from training.gradio_inference import WhisperDemo # Generate a demo
-model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/
-whisper-small-af" demo = WhisperDemo(model_name, huggingface_read_token)
+common_voice_16_1" language_abbr= [ ] # Example `["ti", "yi"]`. see
+abbreviations here https://huggingface.co/datasets/mozilla-foundation/
+common_voice_16_1. # Note: choose a small dataset so as to not run out of
+memory, model_id= "model-id" # Example openai/whisper-small, openai/whisper-
+medium processing_task= "automatic-speech-recognition" wandb_api_key = " "
+use_peft = True # Note: PEFT only works on a notebook with GPU-support. ``` ##
+Step 3: Prepare the Model ```python from training.data_prep import DataPrep #
+Initialize the DataPrep class and prepare the model process = DataPrep
+( huggingface_read_token, dataset_name, language_abbr, model_id,
+processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
+model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
+# Load and preprocess the dataset processed_dataset = process.load_dataset
+( feature_extractor=feature_extractor, tokenizer=tokenizer,
+processor=feature_processor ) ``` ## Step 5: Train the Model ```python from
+training.model_trainer import Trainer # Initialize the Trainer class and train
+the model trainer = Trainer( huggingface_write_token, model_id,
+processed_dataset, model, feature_processor, feature_extractor, tokenizer,
+wandb_api_key, use_peft ) trainer.train( max_steps=100, learning_rate=1e-3,
+per_device_train_batch_size=96, per_device_eval_batch_size=64,
+optim="adamw_bnb_8bit" ) # Optional parameters for training: # max_steps (int):
+The maximum number of training steps (default is 100). # learning_rate (float):
+The learning rate for training (default is 1e-5). # per_device_train_batch_size
+(int): The batch size per GPU for training (default is 96). #
+per_device_eval_batch_size (int): The batch size per GPU for evaluation
+(default is 64). # optim (str): The optimizer used for training (default is
+"adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI ```python from
+training.gradio_inference import WhisperDemo # Generate a demo model_name =
+"your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-
+small-af" demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python from
 deployment.speech_inference import SpeechInference model_name = "your-
 finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " " task = "desired-task" # either 'translate' or
 'transcribe' audiofile_dir = "location-of-audio-file" # filetype should be .mp3
 or .wav # Initialize the SpeechInference class and run inference inference =
 SpeechInference(model_name, huggingface_read_token) pipeline =
```

### Comparing `africanwhisper-0.5.0/setup.cfg` & `africanwhisper-0.6.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = africanwhisper
 author = Kevin Kibe
-version = 0.5.0
+version = 0.6.0
 author_email = keviinkibe@gmail.com
 description = A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/African-Whisper
 license = MIT
```

### Comparing `africanwhisper-0.5.0/src/africanwhisper.egg-info/PKG-INFO` & `africanwhisper-0.6.0/src/africanwhisper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: africanwhisper
-Version: 0.5.0
+Version: 0.6.0
 Summary: A package for fast fine-tuning and API endpoint deployment of Whisper model specifically developed to accelerate Automatic Speech Recognition(ASR) for African Languages.
 Home-page: https://github.com/KevKibe/African-Whisper
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -103,15 +103,15 @@
 ## Step 2: Set Parameters
 
 ```python
 # Set the parameters (refer to the 'Usage on VM' section for more details)
 huggingface_read_token = " "
 huggingface_write_token = " "
 dataset_name = "mozilla-foundation/common_voice_16_1" 
-language_abbr= " "                                    # Example 'af', 'sw'. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
+language_abbr= [ ]                                    # Example `["ti", "yi"]`. see abbreviations here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. 
                                                       # Note: choose a small dataset so as to not run out of memory,
 model_id= "model-id"                                  # Example openai/whisper-small, openai/whisper-medium
 processing_task= "automatic-speech-recognition" 
 wandb_api_key = " "
 use_peft = True                                       # Note: PEFT only works on a notebook with GPU-support.
 
 ```
@@ -153,15 +153,14 @@
     huggingface_write_token,
     model_id,
     processed_dataset,
     model,
     feature_processor,
     feature_extractor,
     tokenizer,
-    language_abbr,
     wandb_api_key,
     use_peft
 )
 trainer.train(
     max_steps=100,
     learning_rate=1e-3,
     per_device_train_batch_size=96,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: africanwhisper Version: 0.5.0 Summary: A package
+Metadata-Version: 2.1 Name: africanwhisper Version: 0.6.0 Summary: A package
 for fast fine-tuning and API endpoint deployment of Whisper model specifically
 developed to accelerate Automatic Speech Recognition(ASR) for African
 Languages. Home-page: https://github.com/KevKibe/African-Whisper Author: Kevin
 Kibe Author-email: keviinkibe@gmail.com License: MIT Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pip==24.0 Requires-Dist: transformers==4.39.2 Requires-Dist: datasets==2.17.0
 Requires-Dist: librosa==0.10.1 Requires-Dist: evaluate==0.4.1 Requires-Dist:
@@ -45,42 +45,43 @@
 //colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/16r4cxP-dSFplRTfgPLbzGXYRzBIUqpx9?usp=sharing)
 ## Step 1: Installation ```python !pip install africanwhisper # If you're on
 Colab, restart the session due to issue with numpy installation on colab. ```
 ## Step 2: Set Parameters ```python # Set the parameters (refer to the 'Usage
 on VM' section for more details) huggingface_read_token = " "
 huggingface_write_token = " " dataset_name = "mozilla-foundation/
-common_voice_16_1" language_abbr= " " # Example 'af', 'sw'. see abbreviations
-here https://huggingface.co/datasets/mozilla-foundation/common_voice_16_1. #
-Note: choose a small dataset so as to not run out of memory, model_id= "model-
-id" # Example openai/whisper-small, openai/whisper-medium processing_task=
-"automatic-speech-recognition" wandb_api_key = " " use_peft = True # Note: PEFT
-only works on a notebook with GPU-support. ``` ## Step 3: Prepare the Model
-```python from training.data_prep import DataPrep # Initialize the DataPrep
-class and prepare the model process = DataPrep( huggingface_read_token,
-dataset_name, language_abbr, model_id, processing_task, use_peft ) tokenizer,
-feature_extractor, feature_processor, model = process.prepare_model() ``` ##
-Step 4: Preprocess the Dataset ```python # Load and preprocess the dataset
-processed_dataset = process.load_dataset( feature_extractor=feature_extractor,
-tokenizer=tokenizer, processor=feature_processor ) ``` ## Step 5: Train the
-Model ```python from training.model_trainer import Trainer # Initialize the
-Trainer class and train the model trainer = Trainer( huggingface_write_token,
-model_id, processed_dataset, model, feature_processor, feature_extractor,
-tokenizer, language_abbr, wandb_api_key, use_peft ) trainer.train
-( max_steps=100, learning_rate=1e-3, per_device_train_batch_size=96,
-per_device_eval_batch_size=64, optim="adamw_bnb_8bit" ) # Optional parameters
-for training: # max_steps (int): The maximum number of training steps (default
-is 100). # learning_rate (float): The learning rate for training (default is
-1e-5). # per_device_train_batch_size (int): The batch size per GPU for training
-(default is 96). # per_device_eval_batch_size (int): The batch size per GPU for
-evaluation (default is 64). # optim (str): The optimizer used for training
-(default is "adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI
-```python from training.gradio_inference import WhisperDemo # Generate a demo
-model_name = "your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/
-whisper-small-af" demo = WhisperDemo(model_name, huggingface_read_token)
+common_voice_16_1" language_abbr= [ ] # Example `["ti", "yi"]`. see
+abbreviations here https://huggingface.co/datasets/mozilla-foundation/
+common_voice_16_1. # Note: choose a small dataset so as to not run out of
+memory, model_id= "model-id" # Example openai/whisper-small, openai/whisper-
+medium processing_task= "automatic-speech-recognition" wandb_api_key = " "
+use_peft = True # Note: PEFT only works on a notebook with GPU-support. ``` ##
+Step 3: Prepare the Model ```python from training.data_prep import DataPrep #
+Initialize the DataPrep class and prepare the model process = DataPrep
+( huggingface_read_token, dataset_name, language_abbr, model_id,
+processing_task, use_peft ) tokenizer, feature_extractor, feature_processor,
+model = process.prepare_model() ``` ## Step 4: Preprocess the Dataset ```python
+# Load and preprocess the dataset processed_dataset = process.load_dataset
+( feature_extractor=feature_extractor, tokenizer=tokenizer,
+processor=feature_processor ) ``` ## Step 5: Train the Model ```python from
+training.model_trainer import Trainer # Initialize the Trainer class and train
+the model trainer = Trainer( huggingface_write_token, model_id,
+processed_dataset, model, feature_processor, feature_extractor, tokenizer,
+wandb_api_key, use_peft ) trainer.train( max_steps=100, learning_rate=1e-3,
+per_device_train_batch_size=96, per_device_eval_batch_size=64,
+optim="adamw_bnb_8bit" ) # Optional parameters for training: # max_steps (int):
+The maximum number of training steps (default is 100). # learning_rate (float):
+The learning rate for training (default is 1e-5). # per_device_train_batch_size
+(int): The batch size per GPU for training (default is 96). #
+per_device_eval_batch_size (int): The batch size per GPU for evaluation
+(default is 64). # optim (str): The optimizer used for training (default is
+"adamw_bnb_8bit") ``` ## Step 6: Generate a Demo using GradioUI ```python from
+training.gradio_inference import WhisperDemo # Generate a demo model_name =
+"your-finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-
+small-af" demo = WhisperDemo(model_name, huggingface_read_token)
 demo.generate_demo() ``` ## Step 7: Test Model using Audio File ```python from
 deployment.speech_inference import SpeechInference model_name = "your-
 finetuned-model-name-on-huggingface-hub" # e.g., "KevinKibe/whisper-small-af"
 huggingface_read_token = " " task = "desired-task" # either 'translate' or
 'transcribe' audiofile_dir = "location-of-audio-file" # filetype should be .mp3
 or .wav # Initialize the SpeechInference class and run inference inference =
 SpeechInference(model_name, huggingface_read_token) pipeline =
```

### Comparing `africanwhisper-0.5.0/src/africanwhisper.egg-info/SOURCES.txt` & `africanwhisper-0.6.0/src/africanwhisper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/deployment/main.py` & `africanwhisper-0.6.0/src/deployment/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/deployment/speech_inference.py` & `africanwhisper-0.6.0/src/deployment/speech_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/tests/test_dataset.py` & `africanwhisper-0.6.0/src/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/audio_data_processor.py` & `africanwhisper-0.6.0/src/training/audio_data_processor.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/collator.py` & `africanwhisper-0.6.0/src/training/collator.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/data_prep.py` & `africanwhisper-0.6.0/src/training/data_prep.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/evaluation.py` & `africanwhisper-0.6.0/src/training/evaluation.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/gradio_demo.py` & `africanwhisper-0.6.0/src/training/gradio_demo.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/gradio_inference.py` & `africanwhisper-0.6.0/src/training/gradio_inference.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/load_data.py` & `africanwhisper-0.6.0/src/training/load_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         """Load datasets for each language abbreviation and concatenate train/test splits.
 
         Returns:
             dict: A dictionary containing concatenated train and test splits for each language.
         """
         data = {}
         for lang in self.language_abbr:
-            dataset = load_dataset(self.dataset_name, lang, streaming=True, token=self.huggingface_token, trust_remote_code=True, disable_progress_bar=True, disable_metadata=True)
+            dataset = load_dataset(self.dataset_name, lang, streaming=True, token=self.huggingface_token, trust_remote_code=True)
             train_split = dataset['train']
             test_split = dataset['test']
             if "train" in data:
                 data["train"] = concatenate_datasets([data["train"], train_split])
             else:
                 data["train"] = train_split
             if "test" in data:
```

### Comparing `africanwhisper-0.5.0/src/training/main.py` & `africanwhisper-0.6.0/src/training/main.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/model_trainer.py` & `africanwhisper-0.6.0/src/training/model_trainer.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/wandb_callback.py` & `africanwhisper-0.6.0/src/training/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `africanwhisper-0.5.0/src/training/whisper_model_prep.py` & `africanwhisper-0.6.0/src/training/whisper_model_prep.py`

 * *Files identical despite different names*

