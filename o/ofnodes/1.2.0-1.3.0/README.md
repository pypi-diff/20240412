# Comparing `tmp/ofnodes-1.2.0.tar.gz` & `tmp/ofnodes-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.2.0.tar", max compression
+gzip compressed data, was "ofnodes-1.3.0.tar", max compression
```

## Comparing `ofnodes-1.2.0.tar` & `ofnodes-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-11 14:48:58.616284 ofnodes-1.2.0/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-11 14:48:58.616284 ofnodes-1.2.0/README.md
--rw-r--r--   0        0        0      590 2024-04-11 17:13:23.250240 ofnodes-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      953 2024-04-11 14:48:58.620284 ofnodes-1.2.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 14:48:58.620284 ofnodes-1.2.0/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     2112 2024-04-11 17:04:01.503993 ofnodes-1.2.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-04-11 14:48:58.620284 ofnodes-1.2.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-11 14:48:58.620284 ofnodes-1.2.0/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0    21735 2024-04-11 16:51:02.879332 ofnodes-1.2.0/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.3.0/README.md
+-rw-r--r--   0        0        0      590 2024-04-12 21:27:53.635786 ofnodes-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      953 2024-04-05 16:17:48.873936 ofnodes-1.3.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.3.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     2112 2024-04-12 13:03:43.078945 ofnodes-1.3.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.3.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.3.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0    24357 2024-04-12 21:21:44.886271 ofnodes-1.3.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.3.0/PKG-INFO
```

### Comparing `ofnodes-1.2.0/LICENSE` & `ofnodes-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.2.0/README.md` & `ofnodes-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.2.0/pyproject.toml` & `ofnodes-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.2.0"
+version = "1.3.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.2.0/src/ofnodes/__init__.py` & `ofnodes-1.3.0/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.2.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.3.0/src/ofnodes/nodes/singlynode.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.2.0/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.3.0/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,16 +105,14 @@
             `SinglyLinkedList` has its data compared to the target data. The first
             node instance data that match the target data is assigned to the `.target`
             property. If a match is not found, the target data is stored as is in the
             `.target` attribute.
 
         Examples:
             >>> sllist = SinglyLinkedList()
-            >>> sllist.__dict__
-            {'_head': None, '_tail': None, '_target': None}
             >>> sllist.target = '5 node'
             Empty `SinglyLinkedList()`. Target data is assigned to SinglyLinkedList's target property.
             >>> type(sllist.target) != SinglyNode
             True
             >>> list(sllist.insert_tail(f"{i} node") for i in range(1, 5))
             [None, None, None, None]
             >>> sllist.target = '5 node'
@@ -140,26 +138,26 @@
         match target_data:
             case _:
                 #  TODO: data validation
                 validated_data = target_data
 
         match self._head:
             case None:
-                print(f"Empty `SinglyLinkedList()`. Target data is assigned to {type(self).__name__}'s target property.")
+                #print(f"Empty `SinglyLinkedList()`. Target data is assigned to {type(self).__name__}'s target property.")
                 self._target = validated_data
 
             case self._head:
                 current_node = self._head
                 while current_node:
                     if current_node.data == validated_data:
-                        print(f"""At least one target match. First target node instance is assigned to {type(self).__name__}'s target property.""")
+                        #print(f"""At least one target match. First target node instance is assigned to {type(self).__name__}'s target property.""")
                         setattr(self, '_target', current_node)
                         return
                     current_node = current_node.next
-                print(f"""No target matches. Target data assigned to {type(self).__name__}'s target property.""")
+                #print(f"""No target matches. Target data assigned to {type(self).__name__}'s target property.""")
                 setattr(self, '_target', validated_data)
                 return
 
 
     @target.deleter
     def target(self):
         """Deleter property for the target of the linked list.
@@ -188,16 +186,14 @@
             >>> assert llist.next is None
             >>> assert llist.head.next is None
             >>> llist.tail
             >>> llist.tail = "new tail"
             >>> assert llist.head.next is llist.tail
             >>> llist
             SinglyLinkedList(head=This node's data is 22 of type str., tail=This node's data is 8 of type str.)
-            >>> llist.__dict__
-            {'_head': SinglyNode(data='first node in the list'), '_tail': SinglyNode(data='new tail')}
             >>> llist.head, llist.tail
             (SinglyNode(data='first node in the list'), SinglyNode(data='new tail'))
         """
         return self._tail
 
     @tail.setter
     def tail(self, value: SinglyNode | Any) -> None:
@@ -292,16 +288,14 @@
             ...     linked_list.head.next is linked_list.tail
             ... )
             >>> linked_list.head, linked_list.tail
             (SinglyNode(data={'the second node': (42.0, True, SinglyNode(data='LGRW'))}), SinglyNode(data='the first node in the list'))
             >>> linked_list.head = "third node added as head via property"
             >>> linked_list.head, linked_list.tail
             (SinglyNode(data='third node added as head via property'), SinglyNode(data='the first node in the list'))
-            >>> linked_list.head.__dict__
-            {'_data': 'third node added as head via property', '_next': SinglyNode(data={'the second node': (42.0, True, SinglyNode(data='LGRW'))})}
             >>> llist = SinglyLinkedList()
             >>> list(llist.insert_head(f"{i} node") for i in range(1, 5))
             [None, None, None, None]
             >>> llist.head = "to be assigned to `SinglyNode.data` then `SinglyLinkedList.head`"
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='to be assigned to `SinglyNode.data` then `SinglyLinkedList.head`'), SinglyNode(data='4 node'), SinglyNode(data='1 node'))
         """
@@ -341,16 +335,14 @@
             >>> linked_list.tail
             SinglyNode(data={'the second node': (42.0, True, SinglyNode(data='LGRW'))})
             >>> linked_list.tail.data['the second node']
             (42.0, True, SinglyNode(data='LGRW'))
             >>> linked_list.tail.data['the second node'][2].data
             'LGRW'
             >>> linked_list.tail = "insert 3rd node via property"
-            >>> linked_list.tail.__dict__
-            {'_data': 'insert 3rd node via property', '_next': None}
             >>> linked_list.tail.data
             'insert 3rd node via property'
             >>> llist = SinglyLinkedList()
             >>> list(llist.insert_tail(f"{i} node") for i in range(1, 5))
             >>> llist.head, llist.head.next, llist.tail
             (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='4 node'))
             >>> llist.tail = "is passed to setter to become SinglyNode()"
@@ -399,14 +391,92 @@
                     if current_node.data == validated_data:
                         return True
                     current_node = current_node.next
                 return False
             raise ValueError("Cannot perform search: The list is empty.")
         raise ValueError("This data is unable to be target.")
 
+
+
+    def remove(self, target_data: Any | SinglyNode) -> None:
+        """Removes the first occurrence of a node with the specified target data from the linked list.
+
+        Args:
+            target_data (Any | SinglyNode): The data or node to be removed from the linked list.
+
+        Raises:
+            ValueError: If the linked list is empty.
+
+        Returns:
+            None: This method does not return any value.
+
+        Removes the first occurrence of a node with the specified target data from the linked list.
+        If the linked list is empty, a ValueError is raised.
+
+        If the target data is found in the linked list:
+        - If the target node is the head, the head of the linked list is updated to the next node.
+        - If the target node is the tail, the tail of the linked list is updated to the previous node.
+        - For any other node, the reference to the next node is adjusted to skip the target node.
+        Notes:
+            This method removes only the first occurrence of the target data if multiple nodes contain the same data.
+
+        Examples:
+            >>> sllist = SinglyLinkedList()
+            >>> list(sllist.insert_tail(f"{i} node") for i in range(1, 5))
+            [None, None, None, None]
+            >>> sllist.remove('0 node')
+            >>> sllist.target
+            '0 node'
+            >>> sllist.head, sllist.head.next, sllist.tail
+            (SinglyNode(data='1 node'), SinglyNode(data='2 node'), SinglyNode(data='4 node'))
+            >>> sllist.remove('1 node')
+            >>> sllist.target
+            SinglyNode(data='1 node')
+            >>> sllist.head, sllist.head.next, sllist.tail
+            (SinglyNode(data='2 node'), SinglyNode(data='3 node'), SinglyNode(data='4 node'))
+            >>> sllist.remove(sllist.tail)
+            >>> sllist.target
+            SinglyNode(data='4 node')
+            >>> sllist.head, sllist.head.next, sllist.tail
+            (SinglyNode(data='2 node'), SinglyNode(data='3 node'), SinglyNode(data='3 node'))
+            >>> sllist.head.next
+            SinglyNode(data='3 node')
+            >>> sllist.tail
+            SinglyNode(data='3 node')
+            >>> sllist.remove(sllist.tail)
+            >>> sllist.tail
+            SinglyNode(data='2 node')
+            >>> sllist.head.next
+            >>> sllist.head, sllist.head.next, sllist.tail
+            (SinglyNode(data='2 node'), None, SinglyNode(data='2 node'))
+        """
+
+        if not self._head:
+            raise ValueError("The linked list is empty.")
+
+        self.target = target_data  # trigger the setter
+
+        if self._head is self._target:
+            # node = self._head
+            self.remove_head()
+            return #node
+        if self._tail is self._target:
+            # node = self._tail
+            self.remove_tail()
+            return #node
+
+        current_node = self._head
+        while current_node.next:
+            if current_node.next is self._target:
+                #node = current_node.next
+                setattr(current_node, '_next', current_node.next.next)
+                return # node
+            current_node = current_node.next
+
+
     def remove_head(self) -> None:
         """Removes the head node from the linked list.
 
         Raises:
             ValueError: If the linked list is empty.
 
         Returns:
@@ -523,8 +593,7 @@
             3 node
             4 node
         """
         current_node = self._head
         while current_node:
             print(current_node.data)
             current_node = current_node.next
-
```

### Comparing `ofnodes-1.2.0/PKG-INFO` & `ofnodes-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.2.0
+Version: 1.3.0
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

