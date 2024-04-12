# Comparing `tmp/omuplugin_emoji-0.2.3.tar.gz` & `tmp/omuplugin_emoji-0.2.4.tar.gz`

## Comparing `omuplugin_emoji-0.2.3.tar` & `omuplugin_emoji-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.3/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.3/src/omuplugin_emoji/__init__.py
--rw-r--r--   0        0        0     5194 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.3/src/omuplugin_emoji/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.3/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.3/README.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.4/.python-version
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.4/src/omuplugin_emoji/__init__.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.4/src/omuplugin_emoji/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.4/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.4/README.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 omuplugin_emoji-0.2.4/PKG-INFO
```

### Comparing `omuplugin_emoji-0.2.3/src/omuplugin_emoji/plugin.py` & `omuplugin_emoji-0.2.4/src/omuplugin_emoji/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,97 +15,97 @@
 APP = App(
     IDENTIFIER,
     version="0.1.0",
 )
 client = Client(APP)
 
 
-class TextPettern(TypedDict):
+class TextPattern(TypedDict):
     type: Literal["text"]
     text: str
 
 
-class ImagePettern(TypedDict):
+class ImagePattern(TypedDict):
     type: Literal["image"]
     id: str
 
 
-class RegexPettern(TypedDict):
+class RegexPattern(TypedDict):
     type: Literal["regex"]
     regex: str
 
 
-type Pettern = TextPettern | ImagePettern | RegexPettern
+type Pattern = TextPattern | ImagePattern | RegexPattern
 
 
 class EmojiData(TypedDict):
     id: str
     asset: str
-    petterns: List[Pettern]
+    patterns: List[Pattern]
 
 
 class Emoji(Model[EmojiData], Keyable):
     def __init__(
         self,
         id: str,
         asset: Identifier,
-        petterns: List[Pettern],
+        patterns: List[Pattern],
     ) -> None:
         self.id = id
         self.asset = asset
-        self.petterns = petterns
+        self.patterns = patterns
 
     def key(self) -> str:
         return self.id
 
     @classmethod
     def from_json(cls, json: EmojiData):
         return cls(
             json["id"],
             Identifier.from_key(json["asset"]),
-            json["petterns"],
+            json["patterns"],
         )
 
     def to_json(self) -> EmojiData:
         return {
             "id": self.id,
             "asset": self.asset.key(),
-            "petterns": self.petterns,
+            "patterns": self.patterns,
         }
 
 
 EMOJI_TABLE_TYPE = TableType.create_model(
     IDENTIFIER,
     name="emoji",
-    model=Emoji,
+    model_type=Emoji,
 )
 emoji_table = client.tables.get(EMOJI_TABLE_TYPE)
 emoji_table.set_cache_size(1000)
 
 
-class petterns:
-    text: List[Tuple[TextPettern, Emoji]] = []
-    image: List[Tuple[ImagePettern, Emoji]] = []
-    regex: List[Tuple[RegexPettern, Emoji]] = []
+class Patterns:
+    text: List[Tuple[TextPattern, Emoji]] = []
+    image: List[Tuple[ImagePattern, Emoji]] = []
+    regex: List[Tuple[RegexPattern, Emoji]] = []
 
 
 @emoji_table.listen
 async def update_emoji_table(items: Mapping[str, Emoji]):
-    petterns.text.clear()
-    petterns.image.clear()
-    petterns.regex.clear()
+    Patterns.text.clear()
+    Patterns.image.clear()
+    Patterns.regex.clear()
 
     for emoji in items.values():
-        for pettern in emoji.petterns:
-            if pettern["type"] == "text":
-                petterns.text.append((pettern, emoji))
-            elif pettern["type"] == "image":
-                petterns.image.append((pettern, emoji))
-            elif pettern["type"] == "regex":
-                petterns.regex.append((pettern, emoji))
+        for pattern in emoji.patterns:
+            if pattern["type"] == "text":
+                Patterns.text.append((pattern, emoji))
+            elif pattern["type"] == "image":
+                Patterns.image.append((pattern, emoji))
+            elif pattern["type"] == "regex":
+                Patterns.regex.append((pattern, emoji))
 
 
 @dataclass
 class EmojiMatch:
     start: int
     end: int
     emoji: Emoji
@@ -114,16 +114,16 @@
 def transform(component: content.Component) -> content.Component:
     if isinstance(component, content.Text):
         parts = transform_text_content(component)
         if len(parts) == 1:
             return parts[0]
         return content.Root(parts)
     if isinstance(component, content.Image):
-        for pettern, emoji in petterns.image:
-            if component.id == pettern["id"]:
+        for pattern, emoji in Patterns.image:
+            if component.id == pattern["id"]:
                 return content.Image.of(
                     url=client.assets.url(emoji.asset),
                     id=emoji.id,
                 )
     if isinstance(component, content.Parent):
         component.set_children(
             [transform(sibling) for sibling in component.get_children()]
@@ -151,35 +151,35 @@
         )
         text = text[match.end :]
     return parts
 
 
 def find_matching_emoji(text: str) -> EmojiMatch | None:
     match: EmojiMatch | None = None
-    for pettern, asset in petterns.text:
+    for pattern, asset in Patterns.text:
         if match:
-            search_end = match.end + len(pettern["text"])
-            start = text.find(pettern["text"], None, search_end)
+            search_end = match.end + len(pattern["text"])
+            start = text.find(pattern["text"], None, search_end)
         else:
-            start = text.find(pettern["text"])
+            start = text.find(pattern["text"])
         if start == -1:
             continue
         if not match or start < match.start:
-            end = start + len(pettern["text"])
+            end = start + len(pattern["text"])
             match = EmojiMatch(start, end, asset)
         if match.start == 0:
             break
     if match:
         if match.start == 0:
             return match
         text = text[: match.start]
-    for pettern, asset in petterns.regex:
-        if len(pettern["regex"]) == 0:
+    for pattern, asset in Patterns.regex:
+        if len(pattern["regex"]) == 0:
             continue
-        result = re.search(pettern["regex"], text)
+        result = re.search(pattern["regex"], text)
         if not result:
             continue
         if not match or result.start() < match.start:
             match = EmojiMatch(result.start(), result.end(), asset)
         if match.start == 0:
             break
     return match
```

### Comparing `omuplugin_emoji-0.2.3/pyproject.toml` & `omuplugin_emoji-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_emoji"
-version = "0.2.3"
+version = "0.2.4"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

