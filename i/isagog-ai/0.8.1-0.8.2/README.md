# Comparing `tmp/isagog_ai-0.8.1.tar.gz` & `tmp/isagog_ai-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isagog_ai-0.8.1.tar", max compression
+gzip compressed data, was "isagog_ai-0.8.2.tar", max compression
```

## Comparing `isagog_ai-0.8.1.tar` & `isagog_ai-0.8.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.1/isagog/__init__.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.1/isagog/client/__init__.py
--rw-r--r--   0        0        0     9032 2024-04-10 13:38:15.982049 isagog_ai-0.8.1/isagog/client/kg_client.py
--rw-r--r--   0        0        0     5971 2024-04-09 14:40:57.250758 isagog_ai-0.8.1/isagog/client/nlp_client.py
--rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.1/isagog/generator/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.1/isagog/generator/sparql_generator.py
--rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.1/isagog/model/__init__.py
--rw-r--r--   0        0        0    14592 2024-04-10 14:14:03.090951 isagog_ai-0.8.1/isagog/model/kg_model.py
--rw-r--r--   0        0        0    27390 2024-04-10 09:06:24.629297 isagog_ai-0.8.1/isagog/model/kg_query.py
--rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.1/isagog/model/nlp_model.py
--rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.1/LICENSE
--rw-r--r--   0        0        0      588 2024-04-09 14:31:16.952983 isagog_ai-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.1/README.md
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.454784 isagog_ai-0.8.2/isagog/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.455784 isagog_ai-0.8.2/isagog/client/__init__.py
+-rw-r--r--   0        0        0     9306 2024-04-12 14:54:45.671149 isagog_ai-0.8.2/isagog/client/kg_client.py
+-rw-r--r--   0        0        0     5971 2024-04-09 14:40:57.250758 isagog_ai-0.8.2/isagog/client/nlp_client.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:28:01.370228 isagog_ai-0.8.2/isagog/generator/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-10 08:27:28.933122 isagog_ai-0.8.2/isagog/generator/sparql_generator.py
+-rw-r--r--   0        0        0        0 2023-11-09 14:36:49.456784 isagog_ai-0.8.2/isagog/model/__init__.py
+-rw-r--r--   0        0        0    16266 2024-04-12 15:51:09.197547 isagog_ai-0.8.2/isagog/model/kg_model.py
+-rw-r--r--   0        0        0    27390 2024-04-10 09:06:24.629297 isagog_ai-0.8.2/isagog/model/kg_query.py
+-rw-r--r--   0        0        0      443 2024-04-03 11:27:43.045375 isagog_ai-0.8.2/isagog/model/nlp_model.py
+-rw-r--r--   0        0        0      577 2023-12-16 19:08:20.361655 isagog_ai-0.8.2/LICENSE
+-rw-r--r--   0        0        0      588 2024-04-11 15:27:47.069933 isagog_ai-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-11-28 11:06:21.183153 isagog_ai-0.8.2/README.md
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 isagog_ai-0.8.2/PKG-INFO
```

### Comparing `isagog_ai-0.8.1/isagog/client/kg_client.py` & `isagog_ai-0.8.2/isagog/client/kg_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,47 +216,53 @@
             return [kind(r.get('id'), **r) for r in res.json()]
         elif res.status_code < 500:
             self.logger.warning("query individuals return code %d, reason %s", res.status_code, res.text)
         else:
             self.logger.error("query individuals return code code %d, reason %s", res.status_code, res.text)
         return []
 
-    def upsert_individual(self, individual: ID, assetions: list[Assertion], auth_token=None) -> bool:
+    def upsert_individual(self, individual: Individual, auth_token=None) -> bool:
         """
         Updates an individual or insert it if not present; existing properties are preserved
 
         :param individual: the individual
         :param assetions: assertions to be updated
         :param auth_token:
         :return:
         """
-        self.logger.debug("Updating individual %s", individual)
+        if individual.need_update():
+
+            self.logger.debug("Updating individual %s", individual.id)
+
+            params = {'id': individual.id}
+            if self.dataset:
+                params['dataset'] = self.dataset
+
+            req = [ass.to_dict() for ass in individual.get_assertions()]
+
+            headers = {"Accept": "application/json"}
+
+            if auth_token:
+                headers["Authorization"] = f'Bearer {auth_token}'
+
+            try:
+                res = httpx.patch(
+                    url=self.route,
+                    params=params,
+                    json=req,
+                    headers=headers
+                )
+
+                if res.status_code == 200:
+                    individual.updated()
+                    return True
+                else:
+                    print(f"upsert failed {res.status_code}")
+                    return False
+            except Exception as e:
+                raise e
+        else:
+            self.logger.debug("Individual %s doesn't need update", individual.id)
 
-        params = {'id': individual}
-        if self.dataset:
-            params['dataset'] = self.dataset
-
-        req = [ass.to_dict() for ass in assetions]
-
-        headers = {"Accept": "application/json"}
-
-        if auth_token:
-            headers["Authorization"] = f'Bearer {auth_token}'
-
-        try:
-            res = httpx.patch(
-                url=self.route,
-                params=params,
-                json=req,
-                headers=headers
-            )
-
-            if res.status_code == 200:
-                return True
-            else:
-                print(f"upsert failed {res.status_code}")
-                return False
-        except Exception as e:
-            raise e
 
     def delete_individual(self, _id: ID, auth_key=None):
         pass
```

### Comparing `isagog_ai-0.8.1/isagog/client/nlp_client.py` & `isagog_ai-0.8.2/isagog/client/nlp_client.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.1/isagog/generator/sparql_generator.py` & `isagog_ai-0.8.2/isagog/generator/sparql_generator.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.1/isagog/model/kg_model.py` & `isagog_ai-0.8.2/isagog/model/kg_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
     A model for Knowledge Graph entities and relations
     (c) Isagog S.r.l. 2024, MIT License
 """
-
-from typing import IO, TextIO, Any
+import datetime
+import logging
+from typing import IO, TextIO, Any, Optional
 
 from rdflib import OWL, Graph, RDF, URIRef, RDFS
 
 # Type definitions
 
 ID = URIRef | str  # Identifier type
 
-ALLOWED_TYPES = [OWL.Axiom, OWL.NamedIndividual, OWL.ObjectProperty, OWL.DatatypeProperty, OWL.Class]
+OWL_ENTITY_TYPES = [OWL.Class, OWL.NamedIndividual, OWL.ObjectProperty, OWL.DatatypeProperty, OWL.AnnotationProperty]
+
+PROFILE_ATTRIBUTE = "https://isagog.com/ontology#profile"
 
 
 def _uri_label(uri: str) -> str:
     """
     Extracts a label from a URI
     :param uri:
     :return:
@@ -57,19 +60,23 @@
 class Entity(object):
     """
     Any identified knowledge entity, either predicative (property) or individual
     """
 
     def __init__(self, _id: ID, **kwargs):
         assert _id
-        self.id = str(_id).strip("<>") if isinstance(_id, URIRef) else _id
+        self.id = str(_id).strip("<>")
         owl_type = kwargs.get('owl')
-        self.__owl__ = owl_type if owl_type and owl_type in ALLOWED_TYPES else None
+        if owl_type:
+            if owl_type in OWL_ENTITY_TYPES:
+                self.__owl__ = owl_type
+            else:
+                logging.warning("bad owl type %s", owl_type)
 
-    def n3(self) -> str:
+    def n3(self, namespace_manager: Optional["NamespaceManager"] = None) -> str:
         """Convert to n3"""
         return f"<{self.id}>"
 
     def __eq__(self, other):
         return (
                 (isinstance(other, Entity) and self.id == other.id)
                 or (isinstance(other, URIRef) and self.id == str(other).strip("<>"))
@@ -84,31 +91,30 @@
 
 
 class Annotation(Entity):
     """
     References to owl:AnnotationProperty
     """
 
-    def __init__(self, _id: ID):
-        super().__init__(self, _id=_id)
+    def __init__(self, _id: ID, **kwargs):
+        super().__init__(self, _id=_id, owl=OWL.AnnotationProperty, **kwargs)
 
 
 class Concept(Entity):
     """
     Unary predicate
     """
 
     def __init__(self, _id: ID, **kwargs):
         """
 
         :param _id: the concept identifier
         :param kwargs:
         """
-        kwargs['owl'] = OWL.Class
-        super().__init__(_id, **kwargs)
+        super().__init__(_id, owl=OWL.Class, **kwargs)
         self.comment = kwargs.get('comment', "")
         self.ontology = kwargs.get('ontology', "")
         self.parents = kwargs.get('parents', [OWL.Thing])
 
 
 class Attribute(Entity):
     """
@@ -118,64 +124,73 @@
 
     def __init__(self, _id: ID, **kwargs):
         """
 
         :param _id:
         :param kwargs: domain
         """
-        kwargs['owl'] = OWL.DatatypeProperty
-        super().__init__(_id, **kwargs)
+
+        super().__init__(_id, owl=OWL.DatatypeProperty)
         self.domain = kwargs.get('domain', OWL.Thing)
+        self.parents = kwargs.get('parents', [OWL.topDataProperty])
+        self.type = kwargs.get('type', "string")
 
 
 class Relation(Entity):
     """
     Assertions ranging on individuals
     owl:ObjectProperty
     """
 
     def __init__(
             self,
             _id: ID,
             **kwargs
     ):
         """
-
         :param _id:
         :param kwargs: inverse, domain, range, label
         """
-        kwargs['owl'] = OWL.ObjectProperty
-        super().__init__(_id, **kwargs)
+
+        super().__init__(_id, owl=OWL.ObjectProperty)
         self.inverse = kwargs.get('inverse')
         self.domain = kwargs.get('domain', Concept(OWL.Thing))
         self.range = kwargs.get('range', Concept(OWL.Thing))
         self.label = kwargs.get('label', _uri_label(_id))
+        self.parents = kwargs.get('parents', [OWL.topObjectProperty])
 
 
 class Assertion(object):
     """
-    Logical assertion of the form: property(subject, values)
+    Assertion axiom of the form: property(subject, values)
     """
 
     def __init__(self,
-                 predicate: ID,
+                 predicate: ID = None,
                  subject: ID = None,
-                 values: list = None):
+                 values: list = None,
+                 **kwargs):
         """
 
         :param predicate:
         :param subject:
         :param values:
         """
-        assert predicate
+        if predicate is None:
+            predicate = kwargs.get('property', kwargs.get('id', None))
+            if predicate is None:
+                raise ValueError("missing predicate")
+        if values is None:
+            values = kwargs.get('values', [])
+
         self.predicate = str(predicate).strip("<>")
         self.subject = str(subject).strip("<>") if subject else None
         self.values = values if values else []
 
-    def n3(self) -> list[str]:
+    def n3(self, namespace_manager: Optional["NamespaceManager"] = None) -> list[str]:
         """Convert to n3"""
         rt = []
         for value in self.values:
             rt.append(f"<{self.subject}> <{self.predicate}> {value}")
         return rt
 
     def to_dict(self) -> dict:
@@ -195,14 +210,15 @@
     """
 
     def __init__(
             self,
             source: IO[bytes] | TextIO | str,
             publicIRI: str,
             source_format="turtle",
+            **kwargs
     ):
         """
         :param source:  Path to the ontology source file.
         :param publicIRI:  Base IRI for the ontology.
         :param source_format:  Format of the ontology.
 
         """
@@ -274,28 +290,27 @@
 class AttributeInstance(Assertion):
     """
     Attributive assertion
     """
 
     def __init__(self, predicate: ID = None,
                  subject: ID = None,
-                 values: list = None, **kwargs):
+                 values: list = None,
+                 **kwargs):
         """
         :param subject: the asserted subject
         :param predicate: the asserted property
         :param values: the asserted values
         :param kwargs:
         """
-        if predicate is None:
-            predicate = kwargs.get('property', kwargs.get('id', KeyError("missing relation property")))
-        if values is None:
-            values = kwargs.get('values', [])
+
         super().__init__(predicate=predicate,
                          subject=subject,
-                         values=values)
+                         values=values,
+                         **kwargs)
         self.value_type = kwargs.get('type', "string")
 
     def all_values_as_string(self) -> str:
         match len(self.values):
             case 0:
                 return ""
             case 1:
@@ -328,30 +343,27 @@
         """
 
         :param property: the asserted property
         :param subject: the assertion's subject
         :param values: the asserted values
         :param kwargs:
         """
-        if predicate is None:
-            predicate = kwargs.get('property', kwargs.get('id', KeyError("missing relation property")))
-        if values is None:
-            values = kwargs.get('values', [])
         if values:
             specimen = values[0]
             if isinstance(specimen, Individual):
                 pass
             elif isinstance(specimen, dict):
                 inst_values = [Individual(_id=r_data.get('id'), **r_data) for r_data in values]
                 values = inst_values
             else:
                 raise ValueError("bad values for relation instance")
         super().__init__(predicate=predicate,
                          subject=subject,
-                         values=values)
+                         values=values,
+                         **kwargs)
 
     def all_values(self, only_id=True) -> list:
         """
         Returns all values of the relation instance
         :param only_id:
         :return:
         """
@@ -397,31 +409,42 @@
 
     def __init__(self, _id: ID, **kwargs):
         """
 
         :param _id: the individual identifier
         :param kwargs:
         """
-        super().__init__(_id, **kwargs)
-        self.__owl__ = OWL.NamedIndividual
+        super().__init__(_id, owl=OWL.NamedIndividual, **kwargs)
+        self.attributes = []
+        self.relations = []
         self.label = kwargs.get('label', _uri_label(self.id))
+        self.add_attribute(AttributeInstance(predicate=RDFS.label, values=[self.label]))
+
         self.kind = kwargs.get('kind', kwargs.get('kinds', [OWL.Thing]))  # back compatibility w 0.7
+        if not all(x == OWL.Thing for x in self.kind):
+            self.add_attribute(AttributeInstance(predicate=RDF.type, values=self.kind))
+
         self.comment = kwargs.get('comment', '')
-        self.attributes = [AttributeInstance(**a_data) for a_data in
-                           kwargs.get('attributes', list[AttributeInstance]())]
-        self.relations = [RelationInstance(**r_data) for r_data in kwargs.get('relations', list[RelationInstance]())]
+        if self.comment:
+            self.add_attribute(AttributeInstance(predicate=RDFS.comment, values=[self.comment]))
+
+        self.attributes.extend([AttributeInstance(**a_data) for a_data in
+                                kwargs.get('attributes', list[AttributeInstance]())])
+        self.relations.extend(
+            [RelationInstance(**r_data) for r_data in kwargs.get('relations', list[RelationInstance]())])
         if 'score' in kwargs:
             self.score = float(kwargs.get('score'))
-        if self.has_attribute("https://isagog.com/ontology#profile"):
+        if self.has_attribute(PROFILE_ATTRIBUTE):
             self.profile = {
                 profile_value.split("=")[0]: int(profile_value.split("=")[1])
-                for profile_value in self.get_attribute("https://isagog.com/ontology#profile").values
+                for profile_value in self.get_attribute(PROFILE_ATTRIBUTE).values
             }
         else:
             self.profile = {}
+        self._refresh = True
 
     def has_attribute(self, attribute_id: ID) -> bool:
         """
         Checks if the individual has a given ontology defined attribute
         :param attribute_id:
         :return:
         """
@@ -457,18 +480,50 @@
         """
         found = next(filter(lambda x: x.predicate == relation_id, self.relations), None)
         if found and not found.is_empty():
             return found
         else:
             return VOID_RELATION
 
+    def get_assertions(self) -> list[Assertion]:
+        """
+        Gets all assertions about the individual
+        :return:
+        """
+        return self.attributes + self.relations
+
     def set_score(self, score: float):
         self.score = score
 
     def get_score(self) -> float | None:
         if hasattr(self, 'score'):
             return self.score
         else:
             return None
 
     def has_score(self) -> bool:
         return hasattr(self, 'score')
+
+    def add_attribute(self, attribute: AttributeInstance):
+        """
+        Adds an attribute to the individual
+        :param attribute:
+        """
+        attribute.subject = self.id
+        self.attributes.append(attribute)
+        self._refresh = True
+
+    def add_relation(self, relation: RelationInstance):
+        """
+
+        :param relation:
+        :return:
+        """
+        relation.subject = self.id
+        self.relations.append(relation)
+        self._refresh = True
+
+    def need_update(self):
+        return self._refresh
+
+    def updated(self):
+        self._refresh = False
```

### Comparing `isagog_ai-0.8.1/isagog/model/kg_query.py` & `isagog_ai-0.8.2/isagog/model/kg_query.py`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.1/LICENSE` & `isagog_ai-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isagog_ai-0.8.1/pyproject.toml` & `isagog_ai-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2269 7361 676f 672d 6169  ame = "isagog-ai
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 302e  "..version = "0.
-00000030: 382e 3122 0d0a 6465 7363 7269 7074 696f  8.1"..descriptio
+00000030: 382e 3222 0d0a 6465 7363 7269 7074 696f  8.2"..descriptio
 00000040: 6e20 3d20 2263 6c69 656e 7420 666f 7220  n = "client for 
 00000050: 6973 6167 6f67 2061 6920 7365 7276 6963  isagog ai servic
 00000060: 6573 220d 0a61 7574 686f 7273 203d 205b  es"..authors = [
 00000070: 2247 7569 646f 2056 6574 6572 6520 3c67  "Guido Vetere <g
 00000080: 2e76 6574 6572 6540 6973 6167 6f67 2e63  .vetere@isagog.c
 00000090: 6f6d 3e22 5d0d 0a72 6561 646d 6520 3d20  om>"]..readme = 
 000000a0: 2252 4541 444d 452e 6d64 220d 0a70 6163  "README.md"..pac
```

### Comparing `isagog_ai-0.8.1/PKG-INFO` & `isagog_ai-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isagog-ai
-Version: 0.8.1
+Version: 0.8.2
 Summary: client for isagog ai services
 Author: Guido Vetere
 Author-email: g.vetere@isagog.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

