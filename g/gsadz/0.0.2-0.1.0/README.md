# Comparing `tmp/gsadz-0.0.2.tar.gz` & `tmp/gsadz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsadz-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gsadz-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gsadz-0.0.2.tar` & `gsadz-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2032 2024-04-08 17:08:29.322151 gsadz-0.0.2/README.md
--rw-r--r--   0        0        0    11473 2024-04-09 12:17:30.646080 gsadz-0.0.2/gsadz/__init__.py
--rw-r--r--   0        0        0     3551 2024-04-05 13:39:31.000000 gsadz-0.0.2/gsadz/parse_data.py
--rw-r--r--   0        0        0  6936203 2024-03-27 22:51:54.000000 gsadz-0.0.2/gsadz/pt/SentiLex-flex-PT02.txt
--rw-r--r--   0        0        0   344162 2024-03-27 14:41:18.000000 gsadz-0.0.2/gsadz/pt/SentiLex-lem-PT02.txt
--rw-r--r--   0        0        0      983 2024-03-29 16:05:38.000000 gsadz-0.0.2/gsadz/pt/booster.txt
--rw-r--r--   0        0        0      512 2024-04-04 14:56:17.000000 gsadz-0.0.2/gsadz/pt/negate.txt
--rw-r--r--   0        0        0      606 2024-04-09 12:50:10.130066 gsadz-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 gsadz-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2861 2024-04-12 13:42:18.314789 gsadz-0.1.0/README.md
+-rw-r--r--   0        0        0    10895 2024-04-12 13:40:53.163794 gsadz-0.1.0/gsadz/__init__.py
+-rw-r--r--   0        0        0     3551 2024-04-05 13:39:31.000000 gsadz-0.1.0/gsadz/parse_data.py
+-rw-r--r--   0        0        0  6936203 2024-03-27 22:51:54.000000 gsadz-0.1.0/gsadz/pt/SentiLex-flex-PT02.txt
+-rw-r--r--   0        0        0   344162 2024-03-27 14:41:18.000000 gsadz-0.1.0/gsadz/pt/SentiLex-lem-PT02.txt
+-rw-r--r--   0        0        0      983 2024-03-29 16:05:38.000000 gsadz-0.1.0/gsadz/pt/booster.txt
+-rw-r--r--   0        0        0      512 2024-04-04 14:56:17.000000 gsadz-0.1.0/gsadz/pt/negate.txt
+-rw-r--r--   0        0        0      681 2024-04-12 14:18:56.602189 gsadz-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 gsadz-0.1.0/PKG-INFO
```

### Comparing `gsadz-0.0.2/README.md` & `gsadz-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,72 @@
 # GSADZ - Ferramenta de Análise de Sentimento para a língua portuguesa
 
-O **gsadz** apresenta-se como um módulo de análise de sentimento para a língua portuguesa, baseado num léxico de sentimentos denominado [```SentiLex-PT 02```](https://b2find.eudat.eu/dataset/b6bd16c2-a8ab-598f-be41-1e7aeecd60d3), e um conjunto de negadores e boosters recolhidos através da ferramenta [```LeIA```](https://github.com/rafjaa/LeIA).
+O **gsadz** apresenta-se como um módulo de análise de sentimento para a língua portuguesa, baseado num léxico de sentimentos denominado [```SentiLex-PT 02```](https://b2find.eudat.eu/dataset/b6bd16c2-a8ab-598f-be41-1e7aeecd60d3), e um conjunto de negadores e boosters adaptados a partir da recolha através da ferramenta [```LeIA```](https://github.com/rafjaa/LeIA).
 
-### Modo de Utilização
+### Exemplo de Utilização
 
-- Como módulo:
+#### Como módulo:
+O módulo SentimentAnalysis apresenta dois parâmetros relativos à calibração das polaridades, conferindo a possibilidade de atribuição de diferentes pesos entre elas.
 
 ```py
 from gsadz import SentimentAnalysis
 
-text = """
-
-"""
+text = "Nesta bela manhã, encontro-me feliz."
+```
 
+- Sem calibração de polaridades
+```py
 sa = SentimentAnalysis()
 
 print(sa.polarity_result(text))
+# {'Polarity': 1.0, 'Words': 5, 'Puncts': 2, 'Boosters': 0, 'Deniers': 0, 'Positives': 2, 'Negatives': 0, 'Neutrals': 0}
+```
+
+- Com calibração de polaridades
+```py
+# A polaridade positiva apresenta um peso de 1.75 e a negativa de 0.75
+sa = SentimentAnalysis(1.75, 0.75)
 
+print(sa.polarity_result(text))
+# {'Polarity': 1.75, 'Words': 5, 'Puncts': 2, 'Boosters': 0, 'Deniers': 0, 'Positives': 2, 'Negatives': 0, 'Neutrals': 0}
 ```
 
-- Como script:
+#### Como script:
 ```
-gsadz -f "texto_exemplo.txt"        ## Recebe o input através 
+gsadz [Opção].. [Ficheiro]...
+
+Sem Ficheiro, o input é recebido através do stdin.
+
+Opções
+
+    -n NUM     Calibração de polaridade negativa
+
+    -p NUM     Calibração de polaridade positiva
 
-gsadz                               ## Recebe o input através do stdin
+    -v         Output em modo non-verbose
 ```
 
 
 ### Features
 
 - Negadores
 ```py
 print(sa.polarity_result("Não gosto nada de ti."))
-{'Polarity': -1.0, 'Words': 5, 'Puncts': 1, 'Boosters': 0, 'Deniers': 1, 'Positives': 1, 'Negatives': 0, 'Neutrals': 0}
+# {'Polarity': -1.0, 'Words': 5, 'Puncts': 1, 'Boosters': 0, 'Deniers': 1, 'Positives': 1, 'Negatives': 0, 'Neutrals': 0}
 ```
 - Boosters
 ```py
 print(sa.polarity_result("És incrivelmente inteligente."))
-{'Polarity': 1.25, 'Words': 3, 'Puncts': 1, 'Boosters': 1, 'Deniers': 0, 'Positives': 1, 'Negatives': 0, 'Neutrals': 0}
+# {'Polarity': 1.25, 'Words': 3, 'Puncts': 1, 'Boosters': 1, 'Deniers': 0, 'Positives': 1, 'Negatives': 0, 'Neutrals': 0}
 ```
 
 - Expressões idiomáticas 
 ```py
 print(sa.polarity_result("O João dá de frosques."))
-{'Polarity': -1.0, 'Words': 5, 'Puncts': 1, 'Boosters': 0, 'Deniers': 0, 'Positives': 0, 'Negatives': 0}
+# {'Polarity': -1.0, 'Words': 5, 'Puncts': 1, 'Boosters': 0, 'Deniers': 0, 'Positives': 0, 'Negatives': 1, 'Neutrals': 0}
 ```
 
 ### Output
 
 * ```Polarity```: Valor final da polaridade do input
     + ```Polarity > 0``` : Sentimento positivo
     + ```Polarity == 0```: Sentimento neutro
```

### Comparing `gsadz-0.0.2/gsadz/__init__.py` & `gsadz-0.1.0/gsadz/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #!/usr/bin/python3
 '''
 NAME
     gsadz - Portuguese Sentiment Analysis module
 
 SYNOPSIS
-    gsadz [OPTION]...
+    gsadz [OPTION].. [FILE]...
 
 DESCRIPTION
     Module of Portuguese Sentiment Analysis that calculates the sentiment polarity and the frequency of words, punctuation, boosters, deniers, positive tokens, negative tokens and neutral tokens of a given input.
-    
-    SentiLex-PT is a sentiment lexicon for Portuguese, LeIA
 
-    With no OPTION, reads from standard input.
+    With no FILE, reads from standard input.
+
+    -n NUM     Negative lexicons polarities weight
+
+    -p NUM     Positive lexicons polarities weight
 
-    -f file     Analyzes the file's content
+    -v         Non-verbose output, just polarity value
 
-    --help      Display this help and exit
+    --help     Display this help and exit
 '''
 
 from .parse_data import SentilexData
 from jjcli import *
 import spacy, os
 
 
@@ -133,15 +135,24 @@
     
 
     def find_special(self, ind_types, index):
         for i in range (0, len(ind_types)):
             if index in ind_types[i][0]:
                 return ind_types[i][1], ind_types[i][0].index(index)
 
-        return None 
+        return None
+    
+    def update_counters(self, counters, polarity):
+        if polarity > 0:
+            res = (counters['n_positives'] + 1, counters['n_negatives'], counters['n_neutrals'], polarity * self.p_weight)
+        elif polarity < 0:
+            res = (counters['n_positives'], counters['n_negatives'] + 1, counters['n_neutrals'], polarity * self.n_weight)
+        else:
+            res = (counters['n_positives'], counters['n_negatives'], counters['n_neutrals'] + 1, polarity)
+        return res
             
  
     def polarity_result(self, input):
         doc = self.nlp(input)
 
         counters = {
             'n_tokens': 0,
@@ -188,16 +199,17 @@
 
                         elif special[0] == 'neg':
                             self.negate = -1
                             counters['n_negates'] += 1
                             continue
 
                         else:
-                            score = int(special[0]) * self.booster * self.negate
-                            sentence_scores.append(score)
+                            polarity = int(special[0])
+                            counters['n_positives'], counters['n_negatives'], counters['n_neutrals'], polarity = self.update_counters(counters, polarity)
+                            sentence_scores.append(polarity * self.booster * self.negate) 
                             self.reset_scores()
                             continue
 
 
                 if str(token).lower() in self.sentilexdata.flex:
                     entry = self.sentilexdata.flex[str(token).lower()]
 
@@ -207,31 +219,25 @@
                 if entry != None:
 
                     for elem in entry:
                         if elem['PoS'] == POS.get(token.pos_, ""):  
 
                             if len(list(elem['POL'].values())) == 1:
                                 polarity = int(list(elem['POL'].values())[0])
-                                counters['n_positives'], counters['n_negatives'], counters['n_neutrals'], polarity = (counters['n_positives'] + 1, counters['n_negatives'], counters['n_neutrals'], polarity * self.p_weight) if polarity > 0 \
-                                                                                                      else (counters['n_positives'], counters['n_negatives'] + 1, counters['n_neutrals'], polarity * self.n_weight) if polarity < 0 \
-                                                                                                      else (counters['n_positives'], counters['n_negatives'], counters['n_neutrals'] + 1, polarity)
+                                counters['n_positives'], counters['n_negatives'], counters['n_neutrals'], polarity = self.update_counters(counters, polarity)
                                 sentence_scores.append(polarity * self.booster * self.negate)
 
                             else:
                                 if token.dep_ in OBJECT_DEP or token.head.dep_ in OBJECT_DEP:
                                     polarity = int(elem['POL']["N1"])
-                                    counters['n_positives'], counters['n_negatives'], counters['n_neutrals'], polarity = (counters['n_positives'] + 1, counters['n_negatives'], counters['n_neutrals'], polarity * self.p_weight) if polarity > 0 \
-                                                                                                      else (counters['n_positives'], counters['n_negatives'] + 1, counters['n_neutrals'], polarity * self.n_weight) if polarity < 0 \
-                                                                                                      else (counters['n_positives'], counters['n_negatives'], counters['n_neutrals'] + 1, polarity)
+                                    counters['n_positives'], counters['n_negatives'], counters['n_neutrals'], polarity = self.update_counters(counters, polarity)
                                     sentence_scores.append(polarity * self.booster * self.negate)
                                 elif token.dep_ in SUBJECT_DEP or token.head.dep_ in SUBJECT_DEP:
                                     polarity = int(elem['POL']["N1"])
-                                    counters['n_positives'], counters['n_negatives'], counters['n_neutrals'], polarity = (counters['n_positives'] + 1, counters['n_negatives'], counters['n_neutrals'], polarity * self.p_weight) if polarity > 0 \
-                                                                                                      else (counters['n_positives'], counters['n_negatives'] + 1, counters['n_neutrals'], polarity * self.n_weight) if polarity < 0 \
-                                                                                                      else (counters['n_positives'], counters['n_negatives'], counters['n_neutrals'] + 1, polarity)
+                                    counters['n_positives'], counters['n_negatives'], counters['n_neutrals'], polarity = self.update_counters(counters, polarity)
                                     sentence_scores.append(polarity * self.booster * self.negate)           
                                 else:
                                     token_scores = [int(value) * self.booster * self.negate for value in list(elem['POL'].values())]
                                     token_scores += [sum(token_scores) / len(token_scores)]
                                     pending_scores.append((token_scores, self.negate))
 
                             break
@@ -267,22 +273,32 @@
         }   
 
         return result
 
 
 
 def main():
-    sa = SentimentAnalysis()
+    p_weight = 1
+    n_weight = 1
+
+    cl = clfilter("p:n:v", doc=__doc__)
 
-    cl = clfilter("f:", doc=__doc__)
-    if '-f' in cl.opt:
-        with open(cl.opt.get('-f')) as file:
-            content = file.read()
-    else:
-        content = input()
+    if '-p' in cl.opt:
+        p_weight = float(cl.opt.get("-p"))
+    elif '-n'in cl.opt:
+        n_weight = float(cl.opt.get("-n"))
     
-    analysis = sa.polarity_result(content)
-    print(analysis)
+    sa = SentimentAnalysis(p_weight, n_weight)
+
+    keeper = cl.text()
+    if len(cl.args) == 0:
+        keeper = cl.input()
+
+    for content in keeper:
+        analysis = sa.polarity_result(content)
+        if '-v' in cl.opt:
+            analysis = analysis['Polarity']
+        print(analysis)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gsadz-0.0.2/gsadz/parse_data.py` & `gsadz-0.1.0/gsadz/parse_data.py`

 * *Files identical despite different names*

### Comparing `gsadz-0.0.2/gsadz/pt/SentiLex-flex-PT02.txt` & `gsadz-0.1.0/gsadz/pt/SentiLex-flex-PT02.txt`

 * *Files identical despite different names*

### Comparing `gsadz-0.0.2/gsadz/pt/SentiLex-lem-PT02.txt` & `gsadz-0.1.0/gsadz/pt/SentiLex-lem-PT02.txt`

 * *Files identical despite different names*

### Comparing `gsadz-0.0.2/gsadz/pt/booster.txt` & `gsadz-0.1.0/gsadz/pt/booster.txt`

 * *Files identical despite different names*

### Comparing `gsadz-0.0.2/gsadz/pt/negate.txt` & `gsadz-0.1.0/gsadz/pt/negate.txt`

 * *Files identical despite different names*

### Comparing `gsadz-0.0.2/pyproject.toml` & `gsadz-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "gsadz"
 readme = "README.md"
-keywords = ['gsadz', 'sentiment analysis', 'SentiLex-PT']
+keywords = ['gsadz', 'sentiment analysis', 'SentiLex-PT', 'spacy']
 authors = [
     { name = "duarte", email="duarte.g.parente@gmail.com" },
     { name = "goncalo", email="goncalocp02@gmail.com" },
     { name = "topzN", email="jose.moreira.um@gmail.com" }
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
 ]
 requires-python = ">=3.8"
 dynamic = ["description"]
-version = "0.0.2"
+version = "0.1.0"
 
 dependencies = [
     "spacy>=3.7.4",
     "jjcli"
 ]
 
+[project.urls]
+Source = "https://github.com/duarteparente/gsadz"
+
 [project.scripts]
 gsadz = "gsadz:main"
```

