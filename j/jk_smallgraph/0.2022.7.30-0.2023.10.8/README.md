# Comparing `tmp/jk_smallgraph-0.2022.7.30.tar.gz` & `tmp/jk_smallgraph-0.2023.10.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jk_smallgraph-0.2022.7.30.tar", last modified: Sat Jul 30 14:40:55 2022, max compression
+gzip compressed data, was "jk_smallgraph-0.2023.10.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jk_smallgraph-0.2022.7.30.tar` & `jk_smallgraph-0.2023.10.8.tar`

### file list

```diff
@@ -1,25 +1,12 @@
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-07-30 14:40:55.980726 jk_smallgraph-0.2022.7.30/
--rw-r-----   0 woodoo    (1000) woodoo    (1000)    10173 2022-07-30 09:32:50.000000 jk_smallgraph-0.2022.7.30/LICENSE.txt
--rw-rw----   0 woodoo    (1000) woodoo    (1000)       38 2022-07-30 07:05:00.000000 jk_smallgraph-0.2022.7.30/MANIFEST.in
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     2117 2022-07-30 14:40:55.980726 jk_smallgraph-0.2022.7.30/PKG-INFO
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     1167 2022-07-30 09:31:02.000000 jk_smallgraph-0.2022.7.30/README.md
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-07-30 14:40:55.980726 jk_smallgraph-0.2022.7.30/jk_smallgraph/
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     7408 2022-07-30 14:26:40.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph/DirectedGraph.py
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     1429 2022-07-30 14:26:27.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph/ILink.py
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     1475 2022-07-30 14:26:31.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph/INode.py
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     2010 2022-07-30 14:26:15.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph/Link.py
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     2142 2022-07-30 14:26:09.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph/Node.py
--rw-rw----   0 woodoo    (1000) woodoo    (1000)      204 2022-07-30 09:34:27.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph/__init__.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-07-30 14:40:55.980726 jk_smallgraph-0.2022.7.30/jk_smallgraph/io/
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     1783 2022-07-30 14:26:52.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph/io/GraphvizIO.py
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     2203 2022-07-30 14:26:44.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph/io/SimpleEdgeListIO.py
--rw-rw----   0 woodoo    (1000) woodoo    (1000)       87 2022-07-30 09:28:53.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph/io/__init__.py
-drwxrwx---   0 woodoo    (1000) woodoo    (1000)        0 2022-07-30 14:40:55.980726 jk_smallgraph-0.2022.7.30/jk_smallgraph.egg-info/
--rw-r-----   0 woodoo    (1000) woodoo    (1000)     2117 2022-07-30 14:40:55.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph.egg-info/PKG-INFO
--rw-r-----   0 woodoo    (1000) woodoo    (1000)      506 2022-07-30 14:40:55.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph.egg-info/SOURCES.txt
--rw-r-----   0 woodoo    (1000) woodoo    (1000)        1 2022-07-30 14:40:55.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph.egg-info/dependency_links.txt
--rw-r-----   0 woodoo    (1000) woodoo    (1000)        1 2022-07-30 09:31:18.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph.egg-info/not-zip-safe
--rw-r-----   0 woodoo    (1000) woodoo    (1000)       27 2022-07-30 14:40:55.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph.egg-info/requires.txt
--rw-r-----   0 woodoo    (1000) woodoo    (1000)       14 2022-07-30 14:40:55.000000 jk_smallgraph-0.2022.7.30/jk_smallgraph.egg-info/top_level.txt
--rw-rw----   0 woodoo    (1000) woodoo    (1000)       38 2022-07-30 14:40:55.980726 jk_smallgraph-0.2022.7.30/setup.cfg
--rw-rw----   0 woodoo    (1000) woodoo    (1000)     1427 2022-07-30 14:40:15.000000 jk_smallgraph-0.2022.7.30/setup.py
+-rw-r--r--   0        0        0     1167 2022-07-30 09:31:02.654721 jk_smallgraph-0.2023.10.8/README.md
+-rw-r--r--   0        0        0     7869 2024-04-12 12:57:01.528391 jk_smallgraph-0.2023.10.8/jk_smallgraph/DirectedGraph.py
+-rw-r--r--   0        0        0     1429 2022-07-30 14:26:27.062924 jk_smallgraph-0.2023.10.8/jk_smallgraph/ILink.py
+-rw-r--r--   0        0        0     1475 2022-07-30 14:26:31.886887 jk_smallgraph-0.2023.10.8/jk_smallgraph/INode.py
+-rw-r--r--   0        0        0     2010 2022-07-30 14:26:15.211014 jk_smallgraph-0.2023.10.8/jk_smallgraph/Link.py
+-rw-r--r--   0        0        0     2142 2022-07-30 14:26:09.299059 jk_smallgraph-0.2023.10.8/jk_smallgraph/Node.py
+-rw-r--r--   0        0        0      204 2024-04-12 12:56:53.596553 jk_smallgraph-0.2023.10.8/jk_smallgraph/__init__.py
+-rw-r--r--   0        0        0     1783 2022-07-30 14:26:52.042734 jk_smallgraph-0.2023.10.8/jk_smallgraph/io/GraphvizIO.py
+-rw-r--r--   0        0        0     2203 2022-07-30 14:26:44.954788 jk_smallgraph-0.2023.10.8/jk_smallgraph/io/SimpleEdgeListIO.py
+-rw-r--r--   0        0        0       87 2022-07-30 09:28:53.703974 jk_smallgraph-0.2023.10.8/jk_smallgraph/io/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-12 13:02:48.257305 jk_smallgraph-0.2023.10.8/pyproject.toml
+-rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 jk_smallgraph-0.2023.10.8/PKG-INFO
```

### Comparing `jk_smallgraph-0.2022.7.30/README.md` & `jk_smallgraph-0.2023.10.8/README.md`

 * *Files identical despite different names*

### Comparing `jk_smallgraph-0.2022.7.30/jk_smallgraph/DirectedGraph.py` & `jk_smallgraph-0.2023.10.8/jk_smallgraph/DirectedGraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 	################################################################################################################################
 	## Public Methods
 	################################################################################################################################
 
 	#
 	# Create a new node.
-	# 
+	#
 	# You need to provide a unique name for the node.
 	# If a node with this name already exists an exception is thrown.
 	#
 	@jk_typing.checkFunctionSignature()
 	def createNode(self, name:str) -> Node:
 		if name in self.__nodesByName:
 			raise Exception("Node name already in use: " + repr(name))
@@ -249,14 +249,34 @@
 		curNode = self.__getNodeE(nodeIdentifier)
 
 		for link in curNode._outgoingLinks.values():
 			assert isinstance(link, Link)
 			yield link.toNode
 	#
 
+	def iterateIncomingLinks(self,
+			nodeIdentifier:typing.Union[str,int,Node],
+		) -> typing.Iterable[Link]:
+
+		curNode = self.__getNodeE(nodeIdentifier)
+
+		yield from curNode._incomingLinks.values()
+	#
+
+	def iterateIncomingNodes(self,
+			nodeIdentifier:typing.Union[str,int,Node],
+		) -> typing.Iterable[Node]:
+
+		curNode = self.__getNodeE(nodeIdentifier)
+
+		for link in curNode._incomingLinks.values():
+			assert isinstance(link, Link)
+			yield link.toNode
+	#
+
 	def iterateStartNodes(self) -> typing.Iterable[Node]:
 		for node in self.__nodesByID.values():
 			if not node._incomingLinks:
 				yield node
 	#
 
 	def iterateEndNodes(self) -> typing.Iterable[Node]:
```

### Comparing `jk_smallgraph-0.2022.7.30/jk_smallgraph/ILink.py` & `jk_smallgraph-0.2023.10.8/jk_smallgraph/ILink.py`

 * *Files identical despite different names*

### Comparing `jk_smallgraph-0.2022.7.30/jk_smallgraph/INode.py` & `jk_smallgraph-0.2023.10.8/jk_smallgraph/INode.py`

 * *Files identical despite different names*

### Comparing `jk_smallgraph-0.2022.7.30/jk_smallgraph/Link.py` & `jk_smallgraph-0.2023.10.8/jk_smallgraph/Link.py`

 * *Files identical despite different names*

### Comparing `jk_smallgraph-0.2022.7.30/jk_smallgraph/Node.py` & `jk_smallgraph-0.2023.10.8/jk_smallgraph/Node.py`

 * *Files identical despite different names*

### Comparing `jk_smallgraph-0.2022.7.30/jk_smallgraph/io/GraphvizIO.py` & `jk_smallgraph-0.2023.10.8/jk_smallgraph/io/GraphvizIO.py`

 * *Files identical despite different names*

### Comparing `jk_smallgraph-0.2022.7.30/jk_smallgraph/io/SimpleEdgeListIO.py` & `jk_smallgraph-0.2023.10.8/jk_smallgraph/io/SimpleEdgeListIO.py`

 * *Files identical despite different names*

