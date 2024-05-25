# Comparing `tmp/jk_smallgraph-0.2023.10.8.tar.gz` & `tmp/jk_smallgraph-0.2024.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jk_smallgraph-0.2023.10.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jk_smallgraph-0.2024.5.25.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jk_smallgraph-0.2023.10.8.tar` & `jk_smallgraph-0.2024.5.25.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1167 2022-07-30 09:31:02.654721 jk_smallgraph-0.2023.10.8/README.md
--rw-r--r--   0        0        0     7869 2024-04-12 12:57:01.528391 jk_smallgraph-0.2023.10.8/jk_smallgraph/DirectedGraph.py
--rw-r--r--   0        0        0     1429 2022-07-30 14:26:27.062924 jk_smallgraph-0.2023.10.8/jk_smallgraph/ILink.py
--rw-r--r--   0        0        0     1475 2022-07-30 14:26:31.886887 jk_smallgraph-0.2023.10.8/jk_smallgraph/INode.py
--rw-r--r--   0        0        0     2010 2022-07-30 14:26:15.211014 jk_smallgraph-0.2023.10.8/jk_smallgraph/Link.py
--rw-r--r--   0        0        0     2142 2022-07-30 14:26:09.299059 jk_smallgraph-0.2023.10.8/jk_smallgraph/Node.py
--rw-r--r--   0        0        0      204 2024-04-12 12:56:53.596553 jk_smallgraph-0.2023.10.8/jk_smallgraph/__init__.py
--rw-r--r--   0        0        0     1783 2022-07-30 14:26:52.042734 jk_smallgraph-0.2023.10.8/jk_smallgraph/io/GraphvizIO.py
--rw-r--r--   0        0        0     2203 2022-07-30 14:26:44.954788 jk_smallgraph-0.2023.10.8/jk_smallgraph/io/SimpleEdgeListIO.py
--rw-r--r--   0        0        0       87 2022-07-30 09:28:53.703974 jk_smallgraph-0.2023.10.8/jk_smallgraph/io/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-12 13:02:48.257305 jk_smallgraph-0.2023.10.8/pyproject.toml
--rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 jk_smallgraph-0.2023.10.8/PKG-INFO
+-rw-r--r--   0        0        0     1167 2022-07-30 09:31:02.654721 jk_smallgraph-0.2024.5.25/README.md
+-rw-r--r--   0        0        0     7949 2024-05-25 10:06:26.822850 jk_smallgraph-0.2024.5.25/jk_smallgraph/DirectedGraph.py
+-rw-r--r--   0        0        0     1583 2024-05-25 10:05:04.235543 jk_smallgraph-0.2024.5.25/jk_smallgraph/ILink.py
+-rw-r--r--   0        0        0     1629 2024-05-25 10:04:59.335584 jk_smallgraph-0.2024.5.25/jk_smallgraph/INode.py
+-rw-r--r--   0        0        0     2177 2024-05-25 10:04:44.775707 jk_smallgraph-0.2024.5.25/jk_smallgraph/Link.py
+-rw-r--r--   0        0        0     2308 2024-05-25 10:04:48.711674 jk_smallgraph-0.2024.5.25/jk_smallgraph/Node.py
+-rw-r--r--   0        0        0      204 2024-05-25 10:09:19.009427 jk_smallgraph-0.2024.5.25/jk_smallgraph/__init__.py
+-rw-r--r--   0        0        0     1783 2022-07-30 14:26:52.042734 jk_smallgraph-0.2024.5.25/jk_smallgraph/io/GraphvizIO.py
+-rw-r--r--   0        0        0     2299 2024-05-25 10:08:30.721824 jk_smallgraph-0.2024.5.25/jk_smallgraph/io/SimpleEdgeListIO.py
+-rw-r--r--   0        0        0       87 2022-07-30 09:28:53.703974 jk_smallgraph-0.2024.5.25/jk_smallgraph/io/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-12 13:02:48.257305 jk_smallgraph-0.2024.5.25/pyproject.toml
+-rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 jk_smallgraph-0.2024.5.25/PKG-INFO
```

### Comparing `jk_smallgraph-0.2023.10.8/README.md` & `jk_smallgraph-0.2024.5.25/README.md`

 * *Files identical despite different names*

### Comparing `jk_smallgraph-0.2023.10.8/jk_smallgraph/DirectedGraph.py` & `jk_smallgraph-0.2024.5.25/jk_smallgraph/DirectedGraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 		self.__nodesByID[nodeID] = node
 		self.__nodesByName[name] = node
 
 		return node
 	#
 
 	@jk_typing.checkFunctionSignature()
-	def getNode(self, nodeIdentifier:typing.Union[str,int]) -> Node:
+	def getNode(self, nodeIdentifier:typing.Union[str,int]) -> typing.Union[Node,None]:
 		if isinstance(nodeIdentifier, str):
 			return self.__nodesByName.get(nodeIdentifier)
 		else:
 			return self.__nodesByID.get(nodeIdentifier)
 	#
 
 	@jk_typing.checkFunctionSignature()
@@ -204,14 +204,17 @@
 		fromNode._outgoingLinks[linkID] = link
 		toNode._incomingLinks[linkID] = link
 		self.__linksByID[linkID] = link
 
 		return link
 	#
 
+	#
+	# Iterate over all nodes connected by outgoing links.
+	#
 	def iterateConnectedNodes(self,
 			nodeIdentifiers:typing.Union[str,int,Node,typing.Iterable[typing.Union[int,str,Node]]],
 			bIncludedStart:bool = False,
 		) -> typing.Iterable[Node]:
 
 		startNodes = self.__getNodeOrNodesE(nodeIdentifiers)
```

### Comparing `jk_smallgraph-0.2023.10.8/jk_smallgraph/ILink.py` & `jk_smallgraph-0.2024.5.25/jk_smallgraph/ILink.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,14 +32,24 @@
 	#
 
 	@property
 	def toNode(self) -> INode:
 		raise NotImplementedError()
 	#
 
+	@property
+	def tag(self) -> typing.Any:
+		raise NotImplementedError()
+	#
+
+	@tag.setter
+	def tag(self, tag:typing.Any):
+		raise NotImplementedError()
+	#
+
 	################################################################################################################################
 	## Helper Methods
 	################################################################################################################################
 
 	################################################################################################################################
 	## Public Methods
 	################################################################################################################################
```

### Comparing `jk_smallgraph-0.2023.10.8/jk_smallgraph/INode.py` & `jk_smallgraph-0.2024.5.25/jk_smallgraph/INode.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,24 @@
 	#
 
 	@property
 	def isEndNode(self) -> bool:
 		raise NotImplementedError()
 	#
 
+	@property
+	def tag(self) -> typing.Any:
+		raise NotImplementedError()
+	#
+
+	@tag.setter
+	def tag(self, tag:typing.Any):
+		raise NotImplementedError()
+	#
+
 	################################################################################################################################
 	## Helper Methods
 	################################################################################################################################
 
 	################################################################################################################################
 	## Public Methods
 	################################################################################################################################
```

### Comparing `jk_smallgraph-0.2023.10.8/jk_smallgraph/Link.py` & `jk_smallgraph-0.2024.5.25/jk_smallgraph/Link.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,57 +21,68 @@
 	################################################################################################################################
 
 	#
 	# Constructor method.
 	#
 	@jk_typing.checkFunctionSignature()
 	def __init__(self, graph, linkID:int, fromNode:INode, toNode:INode):
-		self._graph = graph
-		self._linkID = linkID
-		self._fromNode = fromNode
-		self._toNode = toNode
+		self.__graph = graph
+		self.__linkID = linkID
+		self.__fromNode = fromNode
+		self.__toNode = toNode
+		self.__tag = None
 	#
 
 	################################################################################################################################
 	## Public Properties
 	################################################################################################################################
 
 	@property
 	def linkID(self) -> int:
-		return self._linkID
+		return self.__linkID
 	#
 
 	@property
 	def fromNode(self) -> INode:
-		return self._fromNode
+		return self.__fromNode
 	#
 
 	@property
 	def toNode(self) -> INode:
-		return self._toNode
+		return self.__toNode
+	#
+
+	@property
+	def tag(self) -> typing.Any:
+		return self.__tag
+	#
+
+	@tag.setter
+	def tag(self, tag:typing.Any):
+		self.__tag = tag
 	#
 
 	################################################################################################################################
 	## Helper Methods
 	################################################################################################################################
 
 	################################################################################################################################
 	## Public Methods
 	################################################################################################################################
 
 	def __str__(self):
-		return "Link<({}, {}->{})>".format(self._linkID, repr(self._fromNode._name), repr(self._toNode._name))
+		return "Link<({}, {}->{})>".format(self.__linkID, repr(self.__fromNode._name), repr(self.__toNode._name))
 	#
 
 	def __repr__(self):
-		return "Link<({}, {}->{})>".format(self._linkID, repr(self._fromNode._name), repr(self._toNode._name))
+		return "Link<({}, {}->{})>".format(self.__linkID, repr(self.__fromNode._name), repr(self.__toNode._name))
 	#
 
 	def __hash__(self) -> int:
-		return self._linkID.__hash__()
+		return self.__linkID.__hash__()
 	#
 
 #
```

### Comparing `jk_smallgraph-0.2023.10.8/jk_smallgraph/Node.py` & `jk_smallgraph-0.2024.5.25/jk_smallgraph/Node.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,68 +20,80 @@
 	################################################################################################################################
 
 	#
 	# Constructor method.
 	#
 	@jk_typing.checkFunctionSignature()
 	def __init__(self, graph, nodeID:int, name:str):
-		self._graph = graph
-		self._nodeID = nodeID
-		self._name = name
+		self.__graph = graph
+		self.__nodeID = nodeID
+		self.__name = name
+		self.__tag = None
+
 		self._incomingLinks = {}
 		self._outgoingLinks = {}
 	#
 
 	################################################################################################################################
 	## Public Properties
 	################################################################################################################################
 
 	@property
 	def name(self) -> str:
-		return self._name
+		return self.__name
 	#
 
 	@property
 	def nodeID(self) -> int:
-		return self._nodeID
+		return self.__nodeID
 	#
 
 	@property
 	def isStartNode(self) -> bool:
 		return len(self._incomingLinks) == 0
 	#
 
 	@property
 	def isEndNode(self) -> bool:
 		return len(self._outgoingLinks) == 0
 	#
 
+	@property
+	def tag(self) -> typing.Any:
+		return self.__tag
+	#
+
+	@tag.setter
+	def tag(self, tag:typing.Any):
+		self.__tag = tag
+	#
+
 	################################################################################################################################
 	## Helper Methods
 	################################################################################################################################
 
 	################################################################################################################################
 	## Public Methods
 	################################################################################################################################
 
 	def __str__(self):
-		return "Node<({}, {})>".format(self._nodeID, repr(self._name))
+		return "Node<({}, {})>".format(self.__nodeID, repr(self.__name))
 	#
 
 	def __repr__(self):
-		return "Node<({}, {})>".format(self._nodeID, repr(self._name))
+		return "Node<({}, {})>".format(self.__nodeID, repr(self.__name))
 	#
 
 	def __hash__(self) -> int:
-		return self._nodeID.__hash__()
+		return self.__nodeID.__hash__()
 	#
 
 	def __eq__(self, other: object) -> bool:
 		if isinstance(other, Node):
-			return other._nodeID == self._nodeID
+			return other.__nodeID == self.__nodeID
 		else:
 			return False
 	#
 
 #
```

### Comparing `jk_smallgraph-0.2023.10.8/jk_smallgraph/io/GraphvizIO.py` & `jk_smallgraph-0.2024.5.25/jk_smallgraph/io/GraphvizIO.py`

 * *Files identical despite different names*

### Comparing `jk_smallgraph-0.2023.10.8/jk_smallgraph/io/SimpleEdgeListIO.py` & `jk_smallgraph-0.2024.5.25/jk_smallgraph/io/SimpleEdgeListIO.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,26 +47,28 @@
 
 	@staticmethod
 	def loadFromJSONDict(jData:dict) -> DirectedGraph:
 		return SimpleEdgeListIO.loadFromJSONList(jData["edges"])
 	#
 
 	@staticmethod
-	def loadFromJSONList(jEdgeList:list) -> DirectedGraph:
+	def loadFromJSONList(jEdgeList:typing.Union[tuple,list]) -> DirectedGraph:
 		g = DirectedGraph()
 
 		nodeIDs = set()
 		for jEdge in jEdgeList:
+			assert isinstance(jEdge, (tuple,list))
+			assert len(jEdge) == 2
 			nodeIDs.add(jEdge[0])
 			nodeIDs.add(jEdge[1])
 		for nodeID in sorted(nodeIDs):
 			g.createNode(str(nodeID))
 
 		for jEdge in jEdgeList:
-			assert isinstance(jEdge, list)
+			assert isinstance(jEdge, (tuple,list))
 			fromNode = g.getCreateNode(str(jEdge[0]))
 			toNode = g.getCreateNode(str(jEdge[1]))
 			g.createLink(fromNode, toNode)
 
 		return g
 	#
```

### Comparing `jk_smallgraph-0.2023.10.8/pyproject.toml` & `jk_smallgraph-0.2024.5.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jk_smallgraph-0.2023.10.8/PKG-INFO` & `jk_smallgraph-0.2024.5.25/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jk_smallgraph
-Version: 0.2023.10.8
+Version: 0.2024.5.25
 Summary: A directed graph implementation where each node and link is represented as an individual object.
 Keywords: graph
 Author-email: Jürgen Knauth <pubsrc@binary-overflow.de>
 Maintainer-email: Jürgen Knauth <pubsrc@binary-overflow.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

