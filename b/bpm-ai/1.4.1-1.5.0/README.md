# Comparing `tmp/bpm_ai-1.4.1.tar.gz` & `tmp/bpm_ai-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.4.1.tar", max compression
+gzip compressed data, was "bpm_ai-1.5.0.tar", max compression
```

## Comparing `bpm_ai-1.4.1.tar` & `bpm_ai-1.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      932 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/README.md
--rw-r--r--   0        0        0        0 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0      143 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/common/errors.py
--rw-r--r--   0        0        0     1034 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1509 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/compose/compose.anthropic.prompt
--rw-r--r--   0        0        0     1369 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     3575 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0      738 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     3316 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/decide/decide.anthropic.prompt
--rw-r--r--   0        0        0     3385 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     4082 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     1986 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/extract/extract.anthropic.prompt
--rw-r--r--   0        0        0     1286 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     7294 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0     2578 2024-04-04 21:31:57.807533 bpm_ai-1.4.1/bpm_ai/extract/util.py
--rw-r--r--   0        0        0        0 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      616 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/bpm_ai/generic/generic.anthropic.prompt
--rw-r--r--   0        0        0      544 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0     1486 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      576 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/bpm_ai/translate/translate.anthropic.prompt
--rw-r--r--   0        0        0      611 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0     2902 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0      680 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/bpm_ai/translate/util.py
--rw-r--r--   0        0        0     1369 2024-04-04 21:31:57.811533 bpm_ai-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1980 1970-01-01 00:00:00.000000 bpm_ai-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      932 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1034 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     3575 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      738 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     3543 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     3405 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     4164 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     2322 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     7294 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0     2578 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/extract/util.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0     1486 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0     2902 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0      680 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/bpm_ai/translate/util.py
+-rw-r--r--   0        0        0     1391 2024-04-11 22:02:58.749891 bpm_ai-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 bpm_ai-1.5.0/PKG-INFO
```

### Comparing `bpm_ai-1.4.1/README.md` & `bpm_ai-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/common/multimodal.py` & `bpm_ai-1.5.0/bpm_ai/common/multimodal.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/compose/compose.anthropic.prompt` & `bpm_ai-1.5.0/bpm_ai/compose/compose.anthropic.prompt`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 <role>
 You are a brilliant creative writing AI that loves to compose {{style}} {{type}} that have a {{tone}} tone. You are an expert for writing in {{lang}}.
 </role>
 
 <task>
 Your task is to compose text parts for variables (in curly braces) in a text template (in <text_template></text_template> tags), based on given context information (in <context></context> tags) and desired text properties (in <text_properties></text_properties> tags).
 Only use information from the given template, properties and context, do not make something up.
+Use `store_text` to store your text parts.
 
 <important>
 Do *NOT* use any template variables in your generated text parts, the text you generate *must* be directly usable!
 Be mindful of the relative position, whitespaces, and punctuation (or lack thereof) between template variables. When the template is formatted with your generated variables, it must have correct spacing and a coherent content!
 </important>
 </task>
 
@@ -29,8 +30,9 @@
 {{template}}
 </text_template>
 
 <reminder>
 Remember to respect the text properties specified above and write in {{lang}}!
 Remember to *NOT* use template variables in your generated text parts and to mind the position, spacing, and punctuation of template variable texts!
 Generate text for *all* template variables in curly braces, do not forget anything!
+Use `store_text` to store your text parts.
 </reminder>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 [# system #] You are a brilliant creative writing AI that loves to compose {
 {style}} {{type}} that have a {{tone}} tone. You are an expert for writing in {
 {lang}}. Your task is to compose text parts for variables (in curly braces) in
 a text template (in tags), based on given context information (in tags) and
 desired text properties (in tags). Only use information from the given
-template, properties and context, do not make something up. Do *NOT* use any
-template variables in your generated text parts, the text you generate *must*
-be directly usable! Be mindful of the relative position, whitespaces, and
-punctuation (or lack thereof) between template variables. When the template is
-formatted with your generated variables, it must have correct spacing and a
-coherent content!
+template, properties and context, do not make something up. Use `store_text` to
+store your text parts. Do *NOT* use any template variables in your generated
+text parts, the text you generate *must* be directly usable! Be mindful of the
+relative position, whitespaces, and punctuation (or lack thereof) between
+template variables. When the template is formatted with your generated
+variables, it must have correct spacing and a coherent content!
 {{tone}} {{length}} {{lang}} [# user #] {{context | markdown}} {{template}}
 Remember to respect the text properties specified above and write in {{lang}}!
 Remember to *NOT* use template variables in your generated text parts and to
 mind the position, spacing, and punctuation of template variable texts!
 Generate text for *all* template variables in curly braces, do not forget
-anything!
+anything! Use `store_text` to store your text parts.
```

### Comparing `bpm_ai-1.4.1/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.5.0/bpm_ai/compose/compose.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/compose/compose.py` & `bpm_ai-1.5.0/bpm_ai/compose/compose.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/compose/util.py` & `bpm_ai-1.5.0/bpm_ai/compose/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/decide/decide.anthropic.prompt` & `bpm_ai-1.5.0/bpm_ai/decide/decide.anthropic.prompt`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 <role>
 You are an extremely clever business AI that loves to make smart decisions and give correct results. Your job is to help users execute their business processes in a smart and efficient way by making smart decisions.
 </role>
 
 <task>
 You will receive a decision question or task description and context information to base your decision on.
 Make a decision based on the question or decision task description and given context data.
+Use `store_decision` to store your reasoning and final decision.
 {% if possible_values %}Respect the enum of possible values for the decision!{% endif %}
 Always try to make a decision as best as you can given the provided information. If you absolutely can't make a decision, output null as decision value.
 
 <important>{% if strategy == 'cot' %}
-You will first list *all* relevant facts you know for the decision (relevantFacts).
-Then you will try to deduce new helpful information based on the relevantFacts (deducedInformation).
-Then you will think and reason step-by-step before coming to a conclusion (reasoningSteps).
-Finally, write a summary of your final reasoning (finalReasoning), given the facts and reasoning steps.
+You will first list *all* relevant facts you know for the decision (0_relevantFacts).
+Then you will try to deduce new helpful information based on the relevantFacts (1_deducedInformation).
+Then you will think and reason step-by-step before coming to a conclusion (2_reasoningSteps).
+Finally, write a summary of your final reasoning (3_finalReasoning), given the facts and reasoning steps.
 Be detailed and precise.
 {% else %}
-Describe the reasoning behind your decision step-by-step (only make the conclusion in the end), mentioning supporting information and arguments.
+Fill the `0_reasoning` field first by thinking and reasoning step-by-step - mentioning supporting information and arguments - before finally coming to a conclusion and filling the `1_decision` field.
 Be concise in length but thorough in the points and information you consider.
 {% endif %}</important>
 </task>
 
 {% if strategy == 'cot' %}
 <example>
 <context>
@@ -30,40 +31,40 @@
 note: I want to throw a house party.
 </context>
 
 <decision_task>
 What is the best dish?
 </decision_task>
 
-<result>
+<example_tool_call>
 {
-  "reasoning": {
-    "relevantFacts": [
+  "0_reasoning": {
+    "0_relevantFacts": [
       "The season is Fall",
       "The number of guests is 26",
       "The occasion is a House Party",
       "The budget is low"
     ],
-    "deducedInformation": [
+    "1_deducedInformation": [
       "Fall season usually calls for warm, hearty meals",
       "A low budget means we need to choose a dish that is cost-effective",
       "The number of guests suggests we need a dish that can be easily prepared in large quantities",
       "The occasion of a house party does not call for a special or extravagant dish."
     ],
-    "reasoningSteps": [
+    "2_reasoningSteps": [
       "1. Given the Fall season, a warm, hearty meal like Spareribs, Roastbeef, Dry Aged Gourmet Steak or Stew would be appropriate",
       "2. Considering the low budget, Stew would be more cost-effective than Spareribs, Roastbeef or Dry Aged Gourmet Steak.",
       "3. Given the number of guests, a dish that can be easily prepared in large quantities like a Stew would be suitable",
       "4. Considering all factors (warm and hearty for Fall, cost-effective for a low budget, and easily prepared in large quantities for a house party) Stew seems to be the best choice"
     ],
-    "finalReasoning": "Stew is the best choice as it meets all the requirements: it's a warm, hearty meal suitable for Fall, it's cost-effective, and it can be easily prepared in large quantities for a house party."
+    "3_finalReasoning": "Stew is the best choice as it meets all the requirements: it's a warm, hearty meal suitable for Fall, it's cost-effective, and it can be easily prepared in large quantities for a house party."
   },
-  "decision": "Stew"
+  "1_decision": "Stew"
 }
-</result>
+</example_tool_call>
 </example>
 {% endif %}
 
 [# user #]
 <context>
 {{context | markdown}}
 </context>
@@ -71,8 +72,9 @@
 <decision_task>
 {{task}}
 </decision_task>
 
 <reminder>
 {% if possible_values %}Remember to respect the enum of possible decision values!{% endif %}
 Remember that the type of the final decision value must be `{{output_type}}`.
+Use `store_decision` to store your reasoning and final decision.
 </reminder>
```

### Comparing `bpm_ai-1.4.1/bpm_ai/decide/decide.openai.prompt` & `bpm_ai-1.5.0/bpm_ai/decide/decide.openai.prompt`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 Your job is to help users execute their business processes in a smart and efficient way by making smart decisions.
 
 You will receive a decision task description and context information to base your decision on.
 Make a decision based on the decision task description and context data and store it by calling the function.
 Respect the enum of possible values for the decision, if any is given.
 Always try to make a decision as best as you can given the provided information. If you absolutely can't make a decision, your decision value will be null.
 {% if strategy == 'cot' %}
-You will first list *all* relevant facts you know for the decision (relevantFacts).
-Then you will try to deduce new helpful information based on the relevantFacts (deducedInformation).
-Then you will think and reason step-by-step before coming to a conclusion (reasoningSteps).
-Finally, store a summary of your final reasoning (finalReasoning), given the facts and reasoning steps.
+You will first list *all* relevant facts you know for the decision (0_relevantFacts).
+Then you will try to deduce new helpful information based on the relevantFacts (1_deducedInformation).
+Then you will think and reason step-by-step before coming to a conclusion (2_reasoningSteps).
+Finally, store a summary of your final reasoning (3_finalReasoning), given the facts and reasoning steps.
 Be detailed and precise.
 {% else %}
 Describe the reasoning behind your decision step-by-step (only make the conclusion in the end), mentioning supporting information and arguments.
 Be concise in length but thorough in the points and information you consider.
 {% endif %}
 
 {% if strategy == 'cot' %}
@@ -28,15 +28,15 @@
 # DECISION TASK DESCRIPTION
 What is the best dish?
 
 Remember to respect the enum of possible decision values, if given!
 
 [# assistant #]
 [# tool_call: store_decision (call_kufP7dqLA3OmtHJD10cZ5Jt1) #]
-{"reasoning": {"relevantFacts": ["The season is Fall", "The number of guests is 26", "The occasion is a House Party", "The budget is low"], "deducedInformation": ["Fall season usually calls for warm, hearty meals", "A low budget means we need to choose a dish that is cost-effective", "The number of guests suggests we need a dish that can be easily prepared in large quantities", "The occasion of a house party does not call for a special or extravagant dish."], "reasoningSteps": ["1. Given the Fall season, a warm, hearty meal like Spareribs, Roastbeef, Dry Aged Gourmet Steak or Stew would be appropriate", "2. Considering the low budget, Stew would be more cost-effective than Spareribs, Roastbeef or Dry Aged Gourmet Steak.", "3. Given the number of guests, a dish that can be easily prepared in large quantities like a Stew would be suitable", "4. Considering all factors (warm and hearty for Fall, cost-effective for a low budget, and easily prepared in large quantities for a house party) Stew seems to be the best choice"], "finalReasoning": "Stew is the best choice as it meets all the requirements: it\'s a warm, hearty meal suitable for Fall, it\'s cost-effective, and it can be easily prepared in large quantities for a house party."}, "decision": "Stew"}
+{"0_reasoning": {"0_relevantFacts": ["The season is Fall", "The number of guests is 26", "The occasion is a House Party", "The budget is low"], "1_deducedInformation": ["Fall season usually calls for warm, hearty meals", "A low budget means we need to choose a dish that is cost-effective", "The number of guests suggests we need a dish that can be easily prepared in large quantities", "The occasion of a house party does not call for a special or extravagant dish."], "2_reasoningSteps": ["1. Given the Fall season, a warm, hearty meal like Spareribs, Roastbeef, Dry Aged Gourmet Steak or Stew would be appropriate", "2. Considering the low budget, Stew would be more cost-effective than Spareribs, Roastbeef or Dry Aged Gourmet Steak.", "3. Given the number of guests, a dish that can be easily prepared in large quantities like a Stew would be suitable", "4. Considering all factors (warm and hearty for Fall, cost-effective for a low budget, and easily prepared in large quantities for a house party) Stew seems to be the best choice"], "3_finalReasoning": "Stew is the best choice as it meets all the requirements: it\'s a warm, hearty meal suitable for Fall, it\'s cost-effective, and it can be easily prepared in large quantities for a house party."}, "1_decision": "Stew"}
 [# tool_result: call_kufP7dqLA3OmtHJD10cZ5Jt1 #]
 Decision stored, continue with next task.
 {% endif %}
 
 [# user #]
 # CONTEXT
 {{context | markdown}}
```

### Comparing `bpm_ai-1.4.1/bpm_ai/decide/decide.py` & `bpm_ai-1.5.0/bpm_ai/decide/decide.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from bpm_ai_core.prompt.prompt import Prompt
 from bpm_ai_core.speech_recognition.asr import ASRModel
 from bpm_ai_core.tracing.decorators import trace
 from bpm_ai_core.util.markdown import dict_to_md
 
 from bpm_ai.common.errors import MissingParameterError
 from bpm_ai.common.multimodal import transcribe_audio, prepare_images_for_llm_prompt, ocr_documents
-from bpm_ai.decide.schema import get_cot_decision_output_schema, get_decision_output_schema
+from bpm_ai.decide.schema import get_cot_decision_output_schema, get_decision_output_schema, remove_order_prefix_from_keys
 
 
 @trace("bpm-ai-decide", ["llm"])
 async def decide_llm(
     llm: LLM,
     input_data: dict[str, str | dict | None],
     instructions: str,
@@ -57,15 +57,15 @@
         "description": "Stores the final decision value and corresponding reasoning.",
         "type": "object",
         "properties": output_schema
     }
 
     message = await llm.generate_message(prompt, output_schema=decide_schema)
 
-    return message.content or {}
+    return remove_order_prefix_from_keys(message.content) if message.content else{}
 
 
 @trace("bpm-ai-decide", ["classifier"])
 async def decide_classifier(
     classifier: ZeroShotClassifier,
     input_data: dict[str, str | dict | None],
     output_type: str,
```

### Comparing `bpm_ai-1.4.1/bpm_ai/decide/schema.py` & `bpm_ai-1.5.0/bpm_ai/decide/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 
 def get_decision_output_schema(
     output_type: str,
     possible_values: list | None = None
 ):
     return {
-        "reasoning": "concise description of the reasoning behind the decision",
-        "decision": {
+        "0_reasoning": "concise description of the reasoning behind the decision",
+        "1_decision": {
             "description": "the final decision value, may be null if no decision was possible",
             "type": output_type,
             **({"enum": possible_values} if possible_values is not None else {})
         }
     }
 
 
 def get_cot_decision_output_schema(
     output_type: str,
     possible_values: list | None = None
 ):
     return {
-        "reasoning": {
+        "0_reasoning": {
             "type": "object",
             "properties": {
-                "relevantFacts": {
+                "0_relevantFacts": {
                     "type": "array",
                     "items": {
                         "type": "string",
                         "description": "A discrete fact"
                     }
                 },
-                "deducedInformation": {
+                "1_deducedInformation": {
                     "type": "array",
                     "items": {
                         "type": "string",
                         "description": "Additional information that can be deduced from the relevantFacts"
                     }
                 },
-                "reasoningSteps": {
+                "2_reasoningSteps": {
                     "type": "array",
                     "items": {
                         "type": "string",
                         "description": "A discrete reasoning step. Do not perform multiple steps in one. Be very fine-grained and use discrete steps/items."
                     }
                 },
-                "finalReasoning": {
+                "3_finalReasoning": {
                     "type": "string",
                     "description": "Concise description of the final reasoning behind the decision"
                 }
             }
         },
-        "decision": {
+        "1_decision": {
             "description": "The final decision value, may be null if no decision was possible",
             "type": output_type,
             **({"enum": possible_values} if possible_values is not None else {})
         }
-    }
+    }
+
+
+def remove_order_prefix_from_keys(data):
+    if isinstance(data, dict):
+        return {key.lstrip('0123456789_'): remove_order_prefix_from_keys(value) for key, value in data.items()}
+    elif isinstance(data, list):
+        return [remove_order_prefix_from_keys(item) for item in data]
+    else:
+        return data
```

### Comparing `bpm_ai-1.4.1/bpm_ai/extract/extract.anthropic.prompt` & `bpm_ai-1.5.0/bpm_ai/extract/extract.anthropic.prompt`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [# system #]
 <role>
 You are a brilliant information extraction AI. You love to extract data and information from user-provided context and output correct and complete results.
 </role>
 
 <task>{% if repeated %}
-Extract and output a list of objects (as specified in the schema in <schema></schema> tags below) contained in the following context by the user (in <context></context> tags). There may be one, multiple, or no objects present.
+Extract and output a list of objects (as specified in the schema for `information_extraction`) contained in the following context by the user (in <context></context> tags). There may be one, multiple, or no objects present.
 {% else %}
-Extract and output the desired information (as specified in the schema in <schema></schema> tags below) from the following context by the user (in <context></context> tags).
+Extract and output the desired information (as specified in the schema for `information_extraction`) from the following context by the user (in <context></context> tags).
 {% endif %}
 <important>
 Pay close attention to the type and description of each requested property. Just the name of a property may be too general or misleading in order to determine what to extract. Strictly follow the description of the property!
 Only extract information that is completely contained in the context either directly or indirectly.
 NEVER make anything up or assume information that isn't contained in or can't be deduced from the context.
 If any property or information is not contained in or can't be deduced from the context, set the property to null. NEVER make up a value!
 </important>
@@ -19,8 +19,9 @@
 [# user #]
 <context>
 {{input | markdown}}
 </context>
 
 <reminder>
 Set properties to null if they are not present in or can't be deduced from the context!
+Use `information_extraction` to record the extracted information as well-structured JSON.
 </reminder>
```

### Comparing `bpm_ai-1.4.1/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.5.0/bpm_ai/extract/extract.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/extract/extract.py` & `bpm_ai-1.5.0/bpm_ai/extract/extract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/extract/util.py` & `bpm_ai-1.5.0/bpm_ai/extract/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/generic/generic.anthropic.prompt` & `bpm_ai-1.5.0/bpm_ai/generic/generic.anthropic.prompt`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 You are a genius business AI that loves to make smart decisions, give correct results and follow instructions to the word.
 </role>
 
 <task>
 Your task is to help users execute their business processes by performing a given task.
 
 You will receive a task description (in <task_description></task_description> tags) and context information (in <context></context> tags) that may help with the task.
-Perform the task based on the description and context information and output the result.
+Perform the task based on the description and context information and record the result using `store_task_result`.
 </task>
 
 [# user #]
 <context>
 {{context | markdown}}
 </context>
 
 <task_description>
 {{task}}
-</task_description>
+</task_description>
+
+Use `store_task_result` to record your result.
```

### Comparing `bpm_ai-1.4.1/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.5.0/bpm_ai/generic/generic.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/generic/generic.py` & `bpm_ai-1.5.0/bpm_ai/generic/generic.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/translate/translate.anthropic.prompt` & `bpm_ai-1.5.0/bpm_ai/translate/translate.anthropic.prompt`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 <role>
 You are a highly skilled translator with profound expertise in many languages and you are native in {{lang}}.
 </role>
 
 <task>
 You will be given a JSON object with text in one or more languages.
 Your task is to identify the language of the texts in the JSON object the user provides and accurately translate them into {{lang}} while preserving the meaning, tone, and nuance of the original text. Please maintain proper grammar, spelling, and punctuation in the translated version.
+Use `store_translation` to record the translated texts.
 </task>
 
 <target_language>
 {{lang}}
 </target_language>
 
 [# user #]
```

### Comparing `bpm_ai-1.4.1/bpm_ai/translate/translate.openai.prompt` & `bpm_ai-1.5.0/bpm_ai/translate/translate.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/translate/translate.py` & `bpm_ai-1.5.0/bpm_ai/translate/translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/bpm_ai/translate/util.py` & `bpm_ai-1.5.0/bpm_ai/translate/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.4.1/pyproject.toml` & `bpm_ai-1.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "bpm-ai"
-version = "1.4.1"
+version = "1.5.0"
 description = "AI task automation for BPM engines."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
-bpm-ai-core = "2.2.0"
+python = "~3.11"
+bpm-ai-core = "2.3.2"
 openai = "^1.11.0"
-anthropic = "^0.21.3"
+anthropic = "^0.23.1"
 langfuse = "^2.13.3"
 amazon-textract-prettyprinter = "^0.1.9"
 aiobotocore = "^2.12.1"
 azure-storage-blob = "^12.19.1"
 azure-ai-translation-text = "^1.0.0b1"
 azure-ai-documentintelligence = "^1.0.0b2"
 av = "^11.0.0"
 
 [tool.poetry.group.dev.dependencies]
-bpm-ai-inference = "0.2.2"
+bpm-ai-inference = "0.2.5"
+ctranslate2 = "4.1.0"
 torch = [
     { version = "=2.2.2", source="pypi", markers = "sys_platform == 'darwin'" },
     { version = "=2.2.2+cpu", source = "torch-cpu", markers = "sys_platform != 'darwin'" },
 ]
 spacy = [
     { version = "=3.7.4", markers = "sys_platform != 'darwin'" },
     { version = "=3.7.4", extras = ["apple"], markers = "sys_platform == 'darwin' and platform_machine == 'arm64'" },
```

### Comparing `bpm_ai-1.4.1/PKG-INFO` & `bpm_ai-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.4.1
+Version: 1.5.0
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiobotocore (>=2.12.1,<3.0.0)
 Requires-Dist: amazon-textract-prettyprinter (>=0.1.9,<0.2.0)
-Requires-Dist: anthropic (>=0.21.3,<0.22.0)
+Requires-Dist: anthropic (>=0.23.1,<0.24.0)
 Requires-Dist: av (>=11.0.0,<12.0.0)
 Requires-Dist: azure-ai-documentintelligence (>=1.0.0b2,<2.0.0)
 Requires-Dist: azure-ai-translation-text (>=1.0.0b1,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
-Requires-Dist: bpm-ai-core (==2.2.0)
+Requires-Dist: bpm-ai-core (==2.3.2)
 Requires-Dist: langfuse (>=2.13.3,<3.0.0)
 Requires-Dist: openai (>=1.11.0,<2.0.0)
 Project-URL: Repository, https://github.com/holunda-io/bpm-ai
 Description-Content-Type: text/markdown
 
 # bpm-ai
 _AI task automation for BPM engines._
```

