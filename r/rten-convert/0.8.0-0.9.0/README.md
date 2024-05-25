# Comparing `tmp/rten_convert-0.8.0.tar.gz` & `tmp/rten_convert-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rten_convert-0.8.0.tar", last modified: Mon Apr 29 20:59:56 2024, max compression
+gzip compressed data, was "rten_convert-0.9.0.tar", last modified: Fri May 17 05:13:34 2024, max compression
```

## Comparing `rten_convert-0.8.0.tar` & `rten_convert-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-29 20:59:56.489125 rten_convert-0.8.0/
--rw-r--r--   0 robert     (501) staff       (20)     1070 2024-04-29 18:40:42.000000 rten_convert-0.8.0/LICENSE
--rw-r--r--   0 robert     (501) staff       (20)     1212 2024-04-29 20:59:56.488448 rten_convert-0.8.0/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)      780 2024-04-29 18:40:42.000000 rten_convert-0.8.0/README.md
--rw-r--r--   0 robert     (501) staff       (20)      533 2024-04-29 20:59:17.000000 rten_convert-0.8.0/pyproject.toml
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-29 20:59:56.481554 rten_convert-0.8.0/rten_convert/
--rw-r--r--   0 robert     (501) staff       (20)        0 2024-04-29 18:40:42.000000 rten_convert-0.8.0/rten_convert/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)    44649 2024-04-29 20:43:46.000000 rten_convert-0.8.0/rten_convert/converter.py
--rw-r--r--   0 robert     (501) staff       (20)   167524 2024-04-29 20:43:46.000000 rten_convert-0.8.0/rten_convert/schema_generated.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-29 20:59:56.487898 rten_convert-0.8.0/rten_convert.egg-info/
--rw-r--r--   0 robert     (501) staff       (20)     1212 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)      334 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/SOURCES.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/dependency_links.txt
--rw-r--r--   0 robert     (501) staff       (20)       61 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/entry_points.txt
--rw-r--r--   0 robert     (501) staff       (20)       23 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/requires.txt
--rw-r--r--   0 robert     (501) staff       (20)       13 2024-04-29 20:59:56.000000 rten_convert-0.8.0/rten_convert.egg-info/top_level.txt
--rw-r--r--   0 robert     (501) staff       (20)       38 2024-04-29 20:59:56.489299 rten_convert-0.8.0/setup.cfg
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-17 05:13:34.369779 rten_convert-0.9.0/
+-rw-r--r--   0 robert     (501) staff       (20)     1070 2024-04-29 18:40:42.000000 rten_convert-0.9.0/LICENSE
+-rw-r--r--   0 robert     (501) staff       (20)     1375 2024-05-17 05:13:34.369042 rten_convert-0.9.0/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)      943 2024-05-09 19:20:38.000000 rten_convert-0.9.0/README.md
+-rw-r--r--   0 robert     (501) staff       (20)      869 2024-05-17 05:11:37.000000 rten_convert-0.9.0/pyproject.toml
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-17 05:13:34.362233 rten_convert-0.9.0/rten_convert/
+-rw-r--r--   0 robert     (501) staff       (20)        0 2024-05-08 19:21:18.000000 rten_convert-0.9.0/rten_convert/__init__.py
+-rw-r--r--   0 robert     (501) staff       (20)    46168 2024-05-09 19:20:38.000000 rten_convert-0.9.0/rten_convert/converter.py
+-rw-r--r--   0 robert     (501) staff       (20)   185491 2024-05-09 19:20:38.000000 rten_convert-0.9.0/rten_convert/schema_generated.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-17 05:13:34.368168 rten_convert-0.9.0/rten_convert.egg-info/
+-rw-r--r--   0 robert     (501) staff       (20)     1375 2024-05-17 05:13:34.000000 rten_convert-0.9.0/rten_convert.egg-info/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)      334 2024-05-17 05:13:34.000000 rten_convert-0.9.0/rten_convert.egg-info/SOURCES.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2024-05-17 05:13:34.000000 rten_convert-0.9.0/rten_convert.egg-info/dependency_links.txt
+-rw-r--r--   0 robert     (501) staff       (20)       61 2024-05-17 05:13:34.000000 rten_convert-0.9.0/rten_convert.egg-info/entry_points.txt
+-rw-r--r--   0 robert     (501) staff       (20)       23 2024-05-17 05:13:34.000000 rten_convert-0.9.0/rten_convert.egg-info/requires.txt
+-rw-r--r--   0 robert     (501) staff       (20)       13 2024-05-17 05:13:34.000000 rten_convert-0.9.0/rten_convert.egg-info/top_level.txt
+-rw-r--r--   0 robert     (501) staff       (20)       38 2024-05-17 05:13:34.369963 rten_convert-0.9.0/setup.cfg
```

### Comparing `rten_convert-0.8.0/LICENSE` & `rten_convert-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rten_convert-0.8.0/PKG-INFO` & `rten_convert-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rten-convert
-Version: 0.8.0
+Version: 0.9.0
 Summary: Convert ONNX models to .rten format
 Project-URL: Homepage, https://github.com/robertknight/rten
 Project-URL: Issues, https://github.com/robertknight/rten/issues
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -43,7 +43,20 @@
 ## Development
 
 To install this tool from a checkout of the Git repository, run:
 
 ```sh
 pip install -e .
 ```
+
+After making changes, run the QA checks. First, install the development
+dependencies:
+
+```
+pip install -r requirements.dev.txt
+```
+
+Then run:
+
+```
+make check
+```
```

### Comparing `rten_convert-0.8.0/README.md` & `rten_convert-0.9.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -29,7 +29,20 @@
 ## Development
 
 To install this tool from a checkout of the Git repository, run:
 
 ```sh
 pip install -e .
 ```
+
+After making changes, run the QA checks. First, install the development
+dependencies:
+
+```
+pip install -r requirements.dev.txt
+```
+
+Then run:
+
+```
+make check
+```
```

### Comparing `rten_convert-0.8.0/rten_convert/converter.py` & `rten_convert-0.9.0/rten_convert/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from argparse import ArgumentParser
 from dataclasses import dataclass
 import hashlib
 import json
 from os.path import splitext
 import sys
-from typing import Any, Callable, Literal, Optional
+from typing import Any, Callable, Literal, Optional, cast
 
 import flatbuffers
 import numpy as np
 import onnx
 import onnx.numpy_helper as numpy_helper
 from onnx import TensorProto, ValueInfoProto
 
@@ -64,15 +64,15 @@
             )
 
         # Verify that this is a data type that we'll be able to serialize later.
         match data.dtype:
             case np.float32 | np.int32:
                 pass
             case _:
-                dtype_name = data.dtype.name
+                dtype_name: str = data.dtype.name  # type:ignore[union-attr]
                 raise ValueError(
                     f'Tried to construct ConstantNode "{name}" with unsupported data type {dtype_name}'
                 )
 
     def get_scalar(self):
         if self.shape != []:
             return None
@@ -332,14 +332,15 @@
             return
 
         if input_index < len(self.input_indexes):
             raise Exception(
                 f'Operator has both an attribute "{attr_name}" and corresponding input at index {input_index}'
             )
 
+        shape: list[int]
         match attr_type:
             case "int":
                 shape = []
                 data = np.array(attr_val).astype(np.int32)
 
             case "float":
                 shape = []
@@ -413,15 +414,14 @@
     if len(ints) != allowed_length:
         raise Exception(f'Attribute "{name}" must have {allowed_length} values')
 
 
 def constant_node_from_onnx_initializer(
     tensor: onnx.TensorProto, op_name: Optional[str]
 ) -> ConstantNode:
-
     dims = list(tensor.dims)
     data = numpy_helper.to_array(tensor)
 
     match data.dtype.name:
         # Types that don't need to change
         case "float32" | "int32":
             pass
@@ -480,20 +480,19 @@
     if value.type.tensor_type.shape.dim:
         dims = [d.dim_param or d.dim_value for d in value.type.tensor_type.shape.dim]
     else:
         dims = None
     return ValueNode(name=value.name, shape=dims)
 
 
-def read_pads(op_reader: ONNXOperatorReader) -> tuple[str, list[int] | None]:
+def read_pads(op_reader: ONNXOperatorReader) -> tuple[str, list[int]]:
     """
     Read a padding specification from an ONNX operator.
     """
 
-    pads = None
     auto_pad = op_reader.get_attr("auto_pad", "string", "NOTSET")
 
     match auto_pad:
         case "SAME_UPPER" | "SAME_LOWER":
             pad_mode = "same"
             pads = []
         case "NOTSET":
@@ -574,27 +573,27 @@
             raise Exception(
                 f'Unable to find output "{output_name}" for operator {onnx_op.name}'
             )
         output_indexes.append(index)
 
     # Operator attributes. This will be `None` for operators with no attributes,
     # or one of the `OperatorNameAttrsT` classes generated by flatc.
-    attrs = None
+    attrs: object | None = None
 
     # Operator type name in RTen models. By default assume this is the same as
     # the ONNX type.
     op_type = onnx_op.op_type
     op_reader = ONNXOperatorReader(onnx_op, input_indexes, add_node)
 
     # Check / convert operator attributes and operator name, if different than
     # ONNX.
     match op_type:
         case "ArgMax" | "ArgMin":
             attrs = sg.ArgMaxAttrsT()
-            attrs.axes = op_reader.get_attr("axis", "int", None)
+            attrs.axis = op_reader.get_attr("axis", "int", None)
             attrs.keepDims = bool(op_reader.get_attr("keepdims", "int", 1))
             op_reader.check_attr("select_last_index", "int", 0)
 
         case "AveragePool":
             kernel_shape = op_reader.require_attr("kernel_shape", "ints")
             check_ints_length("kernel_shape", kernel_shape, 2)
             pad_mode, pads = read_pads(op_reader)
@@ -618,22 +617,22 @@
 
             # Ignore attributes which are valid only if training_mode=1, which
             # is unsupported.
             op_reader.ignore_attr("momentum")
 
         case "Cast":
             attrs = sg.CastAttrsT()
-            to = op_reader.get_attr("to", "int", TensorProto.DataType.FLOAT)
+            to = op_reader.get_attr("to", "int", TensorProto.DataType.FLOAT)  # type:ignore[attr-defined]
             match to:
-                case TensorProto.DataType.FLOAT:
+                case TensorProto.DataType.FLOAT:  # type:ignore[attr-defined]
                     attrs.to = sg.DataType.Float
                 case (
-                    TensorProto.DataType.BOOL
-                    | TensorProto.DataType.INT32
-                    | TensorProto.DataType.INT64
+                    TensorProto.DataType.BOOL  # type:ignore[attr-defined]
+                    | TensorProto.DataType.INT32  # type:ignore[attr-defined]
+                    | TensorProto.DataType.INT64  # type:ignore[attr-defined]
                 ):
                     attrs.to = sg.DataType.Int32
                 case _:
                     raise Exception(f"Unsupported target type for cast {to}")
 
         case "Clip":
             op_reader.generate_input_from_attr(1, "min", "float")
@@ -648,14 +647,15 @@
             const_node = constant_node_from_onnx_initializer(tensor, onnx_op.name)
 
             if len(const_node.data) != 1:
                 raise Exception(
                     "Expected ConstantOfShape value to be a 1-element tensor"
                 )
 
+            scalar: sg.FloatScalarT | sg.IntScalarT
             if const_node.data.dtype == np.float32:
                 scalar_type = sg.Scalar.FloatScalar
                 scalar = sg.FloatScalarT()
                 scalar.value = const_node.data.item()
             elif const_node.data.dtype == np.int32:
                 scalar_type = sg.Scalar.IntScalar
                 scalar = sg.IntScalarT()
@@ -685,23 +685,28 @@
             # The kernel shape is inferred at runtime from the input weight tensor.
             op_reader.ignore_attr("kernel_shape")
 
         case "ConvTranspose":
             attrs = sg.ConvTransposeAttrsT()
             attrs.strides = read_strides(op_reader)
 
-            op_reader.check_attr("auto_pad", "string", "NOTSET")
             op_reader.check_attr("dilations", "ints", ([1], [1, 1]))
             op_reader.check_attr("group", "int", 1)
 
             # The kernel shape is inferred at runtime from the input weight tensor.
             op_reader.ignore_attr("kernel_shape")
 
             op_reader.check_attr("output_padding", "ints", [0, 0, 0, 0])
-            op_reader.check_attr("pads", "ints", [0, 0, 0, 0])
+
+            pad_mode, pads = read_pads(op_reader)
+            if pad_mode == "same":
+                attrs.padMode = sg.PadMode.Same
+            else:
+                attrs.padMode = sg.PadMode.Fixed
+                attrs.pads = pads
 
         case "CumSum":
             op_reader.check_attr("exclusive", "int", 0)
             op_reader.check_attr("reverse", "int", 0)
 
         case "Elu":
             attrs = sg.EluAttrsT()
@@ -711,14 +716,18 @@
             attrs = sg.FlattenAttrsT()
             attrs.axis = op_reader.get_attr("axis", "int", 1)
 
         case "Gather" | "GatherElements":
             attrs = sg.GatherAttrsT()
             attrs.axis = op_reader.get_attr("axis", "int", 0)
 
+        case "GatherND":
+            attrs = sg.GatherNDAttrsT()
+            attrs.batchDims = op_reader.get_attr("batch_dims", "int", 0)
+
         case "Gemm":
             attrs = sg.GemmAttrsT()
             attrs.alpha = op_reader.get_attr("alpha", "float", 1.0)
             attrs.beta = op_reader.get_attr("beta", "float", 1.0)
             attrs.transposeA = bool(op_reader.get_attr("transA", "int", 0))
             attrs.transposeB = bool(op_reader.get_attr("transB", "int", 0))
 
@@ -798,20 +807,37 @@
                 1: sg.NMSBoxOrder.CenterWidthHeight,
             }[center_point_box]
 
         case "OneHot":
             attrs = sg.OneHotAttrsT()
             attrs.axis = op_reader.get_attr("axis", "int", -1)
 
-        case "RandomUniform":
-            attrs = sg.RandomUniformAttrsT()
+        case "RandomNormal" | "RandomNormalLike":
+            match op_type:
+                case "RandomNormal":
+                    attrs = sg.RandomNormalAttrsT()
+                    attrs.shape = op_reader.require_attr("shape", "ints")
+                case "RandomNormalLike":
+                    attrs = sg.RandomNormalLikeAttrsT()
+
             op_reader.check_attr("dtype", "int", 1)
+            attrs.seed = op_reader.get_attr("seed", "float", None)
+            attrs.mean = op_reader.get_attr("mean", "float", 0.0)
+            attrs.scale = op_reader.get_attr("scale", "float", 1.0)
+
+        case "RandomUniform" | "RandomUniformLike":
+            match op_type:
+                case "RandomUniform":
+                    attrs = sg.RandomUniformAttrsT()
+                    attrs.shape = op_reader.require_attr("shape", "ints")
+                case "RandomUniformLike":
+                    attrs = sg.RandomUniformLikeAttrsT()
 
+            op_reader.check_attr("dtype", "int", 1)
             attrs.seed = op_reader.get_attr("seed", "float", None)
-            attrs.shape = op_reader.require_attr("shape", "ints")
             attrs.low = op_reader.get_attr("low", "float", 0.0)
             attrs.high = op_reader.get_attr("high", "float", 1.0)
 
         case (
             "ReduceL2"
             | "ReduceMax"
             | "ReduceMean"
@@ -914,15 +940,15 @@
         )
 
     return OperatorNode(
         name=onnx_op.name,
         op_type=op_type,
         attrs=attrs,
         inputs=op_reader.input_indexes,
-        outputs=output_indexes,
+        outputs=cast(list[int | None], output_indexes),
     )
 
 
 def duplicate_node_names(nodes: list[onnx.ValueInfoProto]) -> list[str]:
     """
     Check for node names which are duplicated in `nodes` and return the
     duplicates.
@@ -938,28 +964,32 @@
 def graph_from_onnx_graph(onnx_graph: onnx.GraphProto) -> Graph:
     """
     Parse an ONNX model into a graph representation compatible with this library.
     """
 
     nodes: list[Node] = []
 
-    # Map from tensor ID to node index
-    tensor_map: dict[str, int] = {}
+    # Map from name of constant or value node to index in `nodes`.
+    value_name_to_index: dict[str, int] = {}
 
-    # Map of constant/initializer name to node
+    # Map of constant/initializer name to node.
     constant_map: dict[str, ConstantNode] = {}
 
     def add_node(node: Node) -> int:
-        if node.name in tensor_map:
-            raise Exception(f'Node name "{node.name}" conflicts with another node')
-        if isinstance(node, ConstantNode):
-            constant_map[node.name] = node
         nodes.append(node)
         node_index = len(nodes) - 1
-        tensor_map[node.name] = node_index
+
+        if not isinstance(node, OperatorNode) and node.name:
+            if node.name in value_name_to_index:
+                raise Exception(f'Node name "{node.name}" conflicts with another node')
+            value_name_to_index[node.name] = node_index
+
+        if isinstance(node, ConstantNode):
+            constant_map[node.name] = node
+
         return node_index
 
     conversion_errors = 0
 
     for tensor in onnx_graph.initializer:
         try:
             const_node = constant_node_from_onnx_initializer(tensor, None)
@@ -989,15 +1019,15 @@
         # If the same node is referenced in at 2 or more of:
         #
         # - The initializer list
         # - The input list
         # - The output list
         #
         # Then we only keep the first definition seen.
-        if value.name in tensor_map:
+        if value.name in value_name_to_index:
             return
         value_node = value_node_from_onnx_value(value)
         add_node(value_node)
 
     for value_info in onnx_graph.input:
         add_value_node(value_info)
 
@@ -1007,22 +1037,22 @@
     for operator in onnx_graph.node:
         if operator.op_type == "Constant":
             continue
 
         for output_name in operator.output:
             # If this output is also a model output, it will have been
             # registered already.
-            if output_name in tensor_map:
+            if output_name in value_name_to_index:
                 continue
             value_node = ValueNode(output_name, shape=None)
             add_node(value_node)
 
         try:
             op_node = op_node_from_onnx_operator(
-                operator, tensor_map, constant_map, add_node=add_node
+                operator, value_name_to_index, constant_map, add_node=add_node
             )
             add_node(op_node)
         except Exception as ex:
             print(
                 f"Error converting {operator.op_type} operator {operator.name}: {ex}",
                 file=sys.stderr,
             )
@@ -1041,16 +1071,16 @@
 
     dup_outputs = duplicate_node_names(list(onnx_graph.output))
     if dup_outputs:
         raise ValueError(
             f"ONNX graph contains duplicate output names: {', '.join(dup_outputs)}"
         )
 
-    inputs = [tensor_map[info.name] for info in onnx_graph.input]
-    outputs = [tensor_map[info.name] for info in onnx_graph.output]
+    inputs = [value_name_to_index[info.name] for info in onnx_graph.input]
+    outputs = [value_name_to_index[info.name] for info in onnx_graph.output]
     return Graph(nodes=nodes, inputs=inputs, outputs=outputs)
 
 
 def build_constant_node(builder: flatbuffers.Builder, constant: ConstantNode):
     """
     Serialize a constant tensor value (eg. model weights) into a FlatBuffers model.
     """
@@ -1070,15 +1100,15 @@
             const_data_type = sg.ConstantData.FloatData
         case np.int32:
             sg.IntDataStart(builder)
             sg.IntDataAddData(builder, data_vec)
             const_data = sg.IntDataEnd(builder)
             const_data_type = sg.ConstantData.IntData
         case _:
-            raise ValueError(f"Unsupported data array type {constant.data.dtype.name}")
+            raise ValueError(f"Unsupported data array type {constant.data.dtype.name}")  # type:ignore[union-attr]
 
     sg.ConstantNodeStart(builder)
     sg.ConstantNodeAddShape(builder, shape_vec)
     sg.ConstantNodeAddDataType(builder, const_data_type)
     sg.ConstantNodeAddData(builder, const_data)
     return sg.ConstantNodeEnd(builder)
```

### Comparing `rten_convert-0.8.0/rten_convert/schema_generated.py` & `rten_convert-0.9.0/rten_convert/schema_generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,19 @@
     NonMaxSuppression = 90
     Sign = 91
     GatherElements = 92
     LayerNormalization = 93
     ReduceSumSquare = 94
     RandomUniform = 95
     Elu = 96
+    RandomUniformLike = 97
+    RandomNormal = 98
+    RandomNormalLike = 99
+    Softplus = 100
+    GatherND = 101
 
 
 class RNNDirection(object):
     Forward = 0
     Reverse = 1
     Bidirectional = 2
 
@@ -170,14 +175,18 @@
     HardSigmoidAttrs = 26
     TriluAttrs = 27
     ScatterNDAttrs = 28
     NonMaxSuppressionAttrs = 29
     LayerNormalizationAttrs = 30
     RandomUniformAttrs = 31
     EluAttrs = 32
+    RandomUniformLikeAttrs = 33
+    RandomNormalAttrs = 34
+    RandomNormalLikeAttrs = 35
+    GatherNDAttrs = 36
 
 def OperatorAttrsCreator(unionType, table):
     from flatbuffers.table import Table
     if not isinstance(table, Table):
         return None
     if unionType == OperatorAttrs().ArgMaxAttrs:
         return ArgMaxAttrsT.InitFromBuf(table.Bytes, table.Pos)
@@ -239,14 +248,22 @@
         return NonMaxSuppressionAttrsT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == OperatorAttrs().LayerNormalizationAttrs:
         return LayerNormalizationAttrsT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == OperatorAttrs().RandomUniformAttrs:
         return RandomUniformAttrsT.InitFromBuf(table.Bytes, table.Pos)
     if unionType == OperatorAttrs().EluAttrs:
         return EluAttrsT.InitFromBuf(table.Bytes, table.Pos)
+    if unionType == OperatorAttrs().RandomUniformLikeAttrs:
+        return RandomUniformLikeAttrsT.InitFromBuf(table.Bytes, table.Pos)
+    if unionType == OperatorAttrs().RandomNormalAttrs:
+        return RandomNormalAttrsT.InitFromBuf(table.Bytes, table.Pos)
+    if unionType == OperatorAttrs().RandomNormalLikeAttrs:
+        return RandomNormalLikeAttrsT.InitFromBuf(table.Bytes, table.Pos)
+    if unionType == OperatorAttrs().GatherNDAttrs:
+        return GatherNDAttrsT.InitFromBuf(table.Bytes, table.Pos)
     return None
 
 
 class Scalar(object):
     NONE = 0
     IntScalar = 1
     FloatScalar = 2
@@ -1424,37 +1441,82 @@
         return 0
 
     # ConvTransposeAttrs
     def StridesIsNone(self):
         o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
         return o == 0
 
+    # ConvTransposeAttrs
+    def PadMode(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Uint8Flags, o + self._tab.Pos)
+        return 1
+
+    # ConvTransposeAttrs
+    def Pads(self, j):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        if o != 0:
+            a = self._tab.Vector(o)
+            return self._tab.Get(flatbuffers.number_types.Uint32Flags, a + flatbuffers.number_types.UOffsetTFlags.py_type(j * 4))
+        return 0
+
+    # ConvTransposeAttrs
+    def PadsAsNumpy(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        if o != 0:
+            return self._tab.GetVectorAsNumpy(flatbuffers.number_types.Uint32Flags, o)
+        return 0
+
+    # ConvTransposeAttrs
+    def PadsLength(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        if o != 0:
+            return self._tab.VectorLen(o)
+        return 0
+
+    # ConvTransposeAttrs
+    def PadsIsNone(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        return o == 0
+
 def ConvTransposeAttrsStart(builder):
-    builder.StartObject(1)
+    builder.StartObject(3)
 
 def ConvTransposeAttrsAddStrides(builder, strides):
     builder.PrependUOffsetTRelativeSlot(0, flatbuffers.number_types.UOffsetTFlags.py_type(strides), 0)
 
 def ConvTransposeAttrsStartStridesVector(builder, numElems):
     return builder.StartVector(4, numElems, 4)
 
+def ConvTransposeAttrsAddPadMode(builder, padMode):
+    builder.PrependUint8Slot(1, padMode, 1)
+
+def ConvTransposeAttrsAddPads(builder, pads):
+    builder.PrependUOffsetTRelativeSlot(2, flatbuffers.number_types.UOffsetTFlags.py_type(pads), 0)
+
+def ConvTransposeAttrsStartPadsVector(builder, numElems):
+    return builder.StartVector(4, numElems, 4)
+
 def ConvTransposeAttrsEnd(builder):
     return builder.EndObject()
 
 
 try:
     from typing import List
 except:
     pass
 
 class ConvTransposeAttrsT(object):
 
     # ConvTransposeAttrsT
     def __init__(self):
         self.strides = None  # type: List[int]
+        self.padMode = 1  # type: int
+        self.pads = None  # type: List[int]
 
     @classmethod
     def InitFromBuf(cls, buf, pos):
         convTransposeAttrs = ConvTransposeAttrs()
         convTransposeAttrs.Init(buf, pos)
         return cls.InitFromObj(convTransposeAttrs)
 
@@ -1476,28 +1538,47 @@
         if not convTransposeAttrs.StridesIsNone():
             if np is None:
                 self.strides = []
                 for i in range(convTransposeAttrs.StridesLength()):
                     self.strides.append(convTransposeAttrs.Strides(i))
             else:
                 self.strides = convTransposeAttrs.StridesAsNumpy()
+        self.padMode = convTransposeAttrs.PadMode()
+        if not convTransposeAttrs.PadsIsNone():
+            if np is None:
+                self.pads = []
+                for i in range(convTransposeAttrs.PadsLength()):
+                    self.pads.append(convTransposeAttrs.Pads(i))
+            else:
+                self.pads = convTransposeAttrs.PadsAsNumpy()
 
     # ConvTransposeAttrsT
     def Pack(self, builder):
         if self.strides is not None:
             if np is not None and type(self.strides) is np.ndarray:
                 strides = builder.CreateNumpyVector(self.strides)
             else:
                 ConvTransposeAttrsStartStridesVector(builder, len(self.strides))
                 for i in reversed(range(len(self.strides))):
                     builder.PrependUint32(self.strides[i])
                 strides = builder.EndVector()
+        if self.pads is not None:
+            if np is not None and type(self.pads) is np.ndarray:
+                pads = builder.CreateNumpyVector(self.pads)
+            else:
+                ConvTransposeAttrsStartPadsVector(builder, len(self.pads))
+                for i in reversed(range(len(self.pads))):
+                    builder.PrependUint32(self.pads[i])
+                pads = builder.EndVector()
         ConvTransposeAttrsStart(builder)
         if self.strides is not None:
             ConvTransposeAttrsAddStrides(builder, strides)
+        ConvTransposeAttrsAddPadMode(builder, self.padMode)
+        if self.pads is not None:
+            ConvTransposeAttrsAddPads(builder, pads)
         convTransposeAttrs = ConvTransposeAttrsEnd(builder)
         return convTransposeAttrs
 
 
 class EluAttrs(object):
     __slots__ = ['_tab']
 
@@ -1815,14 +1896,91 @@
     def Pack(self, builder):
         GatherAttrsStart(builder)
         GatherAttrsAddAxis(builder, self.axis)
         gatherAttrs = GatherAttrsEnd(builder)
         return gatherAttrs
 
 
+class GatherNDAttrs(object):
+    __slots__ = ['_tab']
+
+    @classmethod
+    def GetRootAs(cls, buf, offset=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
+        x = GatherNDAttrs()
+        x.Init(buf, n + offset)
+        return x
+
+    @classmethod
+    def GetRootAsGatherNDAttrs(cls, buf, offset=0):
+        """This method is deprecated. Please switch to GetRootAs."""
+        return cls.GetRootAs(buf, offset)
+    @classmethod
+    def GatherNDAttrsBufferHasIdentifier(cls, buf, offset, size_prefixed=False):
+        return flatbuffers.util.BufferHasIdentifier(buf, offset, b"\x52\x54\x45\x4E", size_prefixed=size_prefixed)
+
+    # GatherNDAttrs
+    def Init(self, buf, pos):
+        self._tab = flatbuffers.table.Table(buf, pos)
+
+    # GatherNDAttrs
+    def BatchDims(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Int32Flags, o + self._tab.Pos)
+        return 0
+
+def GatherNDAttrsStart(builder):
+    builder.StartObject(1)
+
+def GatherNDAttrsAddBatchDims(builder, batchDims):
+    builder.PrependInt32Slot(0, batchDims, 0)
+
+def GatherNDAttrsEnd(builder):
+    return builder.EndObject()
+
+
+
+class GatherNDAttrsT(object):
+
+    # GatherNDAttrsT
+    def __init__(self):
+        self.batchDims = 0  # type: int
+
+    @classmethod
+    def InitFromBuf(cls, buf, pos):
+        gatherNdattrs = GatherNDAttrs()
+        gatherNdattrs.Init(buf, pos)
+        return cls.InitFromObj(gatherNdattrs)
+
+    @classmethod
+    def InitFromPackedBuf(cls, buf, pos=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, pos)
+        return cls.InitFromBuf(buf, pos+n)
+
+    @classmethod
+    def InitFromObj(cls, gatherNdattrs):
+        x = GatherNDAttrsT()
+        x._UnPack(gatherNdattrs)
+        return x
+
+    # GatherNDAttrsT
+    def _UnPack(self, gatherNdattrs):
+        if gatherNdattrs is None:
+            return
+        self.batchDims = gatherNdattrs.BatchDims()
+
+    # GatherNDAttrsT
+    def Pack(self, builder):
+        GatherNDAttrsStart(builder)
+        GatherNDAttrsAddBatchDims(builder, self.batchDims)
+        gatherNdattrs = GatherNDAttrsEnd(builder)
+        return gatherNdattrs
+
+
 class GemmAttrs(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAs(cls, buf, offset=0):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = GemmAttrs()
@@ -2756,14 +2914,275 @@
     def Pack(self, builder):
         OneHotAttrsStart(builder)
         OneHotAttrsAddAxis(builder, self.axis)
         oneHotAttrs = OneHotAttrsEnd(builder)
         return oneHotAttrs
 
 
+class RandomNormalAttrs(object):
+    __slots__ = ['_tab']
+
+    @classmethod
+    def GetRootAs(cls, buf, offset=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
+        x = RandomNormalAttrs()
+        x.Init(buf, n + offset)
+        return x
+
+    @classmethod
+    def GetRootAsRandomNormalAttrs(cls, buf, offset=0):
+        """This method is deprecated. Please switch to GetRootAs."""
+        return cls.GetRootAs(buf, offset)
+    @classmethod
+    def RandomNormalAttrsBufferHasIdentifier(cls, buf, offset, size_prefixed=False):
+        return flatbuffers.util.BufferHasIdentifier(buf, offset, b"\x52\x54\x45\x4E", size_prefixed=size_prefixed)
+
+    # RandomNormalAttrs
+    def Init(self, buf, pos):
+        self._tab = flatbuffers.table.Table(buf, pos)
+
+    # RandomNormalAttrs
+    def Mean(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return 0.0
+
+    # RandomNormalAttrs
+    def Scale(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return 0.0
+
+    # RandomNormalAttrs
+    def Seed(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return None
+
+    # RandomNormalAttrs
+    def Shape(self, j):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
+        if o != 0:
+            a = self._tab.Vector(o)
+            return self._tab.Get(flatbuffers.number_types.Uint32Flags, a + flatbuffers.number_types.UOffsetTFlags.py_type(j * 4))
+        return 0
+
+    # RandomNormalAttrs
+    def ShapeAsNumpy(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
+        if o != 0:
+            return self._tab.GetVectorAsNumpy(flatbuffers.number_types.Uint32Flags, o)
+        return 0
+
+    # RandomNormalAttrs
+    def ShapeLength(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
+        if o != 0:
+            return self._tab.VectorLen(o)
+        return 0
+
+    # RandomNormalAttrs
+    def ShapeIsNone(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(10))
+        return o == 0
+
+def RandomNormalAttrsStart(builder):
+    builder.StartObject(4)
+
+def RandomNormalAttrsAddMean(builder, mean):
+    builder.PrependFloat32Slot(0, mean, 0.0)
+
+def RandomNormalAttrsAddScale(builder, scale):
+    builder.PrependFloat32Slot(1, scale, 0.0)
+
+def RandomNormalAttrsAddSeed(builder, seed):
+    builder.PrependFloat32Slot(2, seed, None)
+
+def RandomNormalAttrsAddShape(builder, shape):
+    builder.PrependUOffsetTRelativeSlot(3, flatbuffers.number_types.UOffsetTFlags.py_type(shape), 0)
+
+def RandomNormalAttrsStartShapeVector(builder, numElems):
+    return builder.StartVector(4, numElems, 4)
+
+def RandomNormalAttrsEnd(builder):
+    return builder.EndObject()
+
+
+try:
+    from typing import List
+except:
+    pass
+
+class RandomNormalAttrsT(object):
+
+    # RandomNormalAttrsT
+    def __init__(self):
+        self.mean = 0.0  # type: float
+        self.scale = 0.0  # type: float
+        self.seed = None  # type: Optional[float]
+        self.shape = None  # type: List[int]
+
+    @classmethod
+    def InitFromBuf(cls, buf, pos):
+        randomNormalAttrs = RandomNormalAttrs()
+        randomNormalAttrs.Init(buf, pos)
+        return cls.InitFromObj(randomNormalAttrs)
+
+    @classmethod
+    def InitFromPackedBuf(cls, buf, pos=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, pos)
+        return cls.InitFromBuf(buf, pos+n)
+
+    @classmethod
+    def InitFromObj(cls, randomNormalAttrs):
+        x = RandomNormalAttrsT()
+        x._UnPack(randomNormalAttrs)
+        return x
+
+    # RandomNormalAttrsT
+    def _UnPack(self, randomNormalAttrs):
+        if randomNormalAttrs is None:
+            return
+        self.mean = randomNormalAttrs.Mean()
+        self.scale = randomNormalAttrs.Scale()
+        self.seed = randomNormalAttrs.Seed()
+        if not randomNormalAttrs.ShapeIsNone():
+            if np is None:
+                self.shape = []
+                for i in range(randomNormalAttrs.ShapeLength()):
+                    self.shape.append(randomNormalAttrs.Shape(i))
+            else:
+                self.shape = randomNormalAttrs.ShapeAsNumpy()
+
+    # RandomNormalAttrsT
+    def Pack(self, builder):
+        if self.shape is not None:
+            if np is not None and type(self.shape) is np.ndarray:
+                shape = builder.CreateNumpyVector(self.shape)
+            else:
+                RandomNormalAttrsStartShapeVector(builder, len(self.shape))
+                for i in reversed(range(len(self.shape))):
+                    builder.PrependUint32(self.shape[i])
+                shape = builder.EndVector()
+        RandomNormalAttrsStart(builder)
+        RandomNormalAttrsAddMean(builder, self.mean)
+        RandomNormalAttrsAddScale(builder, self.scale)
+        RandomNormalAttrsAddSeed(builder, self.seed)
+        if self.shape is not None:
+            RandomNormalAttrsAddShape(builder, shape)
+        randomNormalAttrs = RandomNormalAttrsEnd(builder)
+        return randomNormalAttrs
+
+
+class RandomNormalLikeAttrs(object):
+    __slots__ = ['_tab']
+
+    @classmethod
+    def GetRootAs(cls, buf, offset=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
+        x = RandomNormalLikeAttrs()
+        x.Init(buf, n + offset)
+        return x
+
+    @classmethod
+    def GetRootAsRandomNormalLikeAttrs(cls, buf, offset=0):
+        """This method is deprecated. Please switch to GetRootAs."""
+        return cls.GetRootAs(buf, offset)
+    @classmethod
+    def RandomNormalLikeAttrsBufferHasIdentifier(cls, buf, offset, size_prefixed=False):
+        return flatbuffers.util.BufferHasIdentifier(buf, offset, b"\x52\x54\x45\x4E", size_prefixed=size_prefixed)
+
+    # RandomNormalLikeAttrs
+    def Init(self, buf, pos):
+        self._tab = flatbuffers.table.Table(buf, pos)
+
+    # RandomNormalLikeAttrs
+    def Mean(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return 0.0
+
+    # RandomNormalLikeAttrs
+    def Scale(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return 0.0
+
+    # RandomNormalLikeAttrs
+    def Seed(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return None
+
+def RandomNormalLikeAttrsStart(builder):
+    builder.StartObject(3)
+
+def RandomNormalLikeAttrsAddMean(builder, mean):
+    builder.PrependFloat32Slot(0, mean, 0.0)
+
+def RandomNormalLikeAttrsAddScale(builder, scale):
+    builder.PrependFloat32Slot(1, scale, 0.0)
+
+def RandomNormalLikeAttrsAddSeed(builder, seed):
+    builder.PrependFloat32Slot(2, seed, None)
+
+def RandomNormalLikeAttrsEnd(builder):
+    return builder.EndObject()
+
+
+
+class RandomNormalLikeAttrsT(object):
+
+    # RandomNormalLikeAttrsT
+    def __init__(self):
+        self.mean = 0.0  # type: float
+        self.scale = 0.0  # type: float
+        self.seed = None  # type: Optional[float]
+
+    @classmethod
+    def InitFromBuf(cls, buf, pos):
+        randomNormalLikeAttrs = RandomNormalLikeAttrs()
+        randomNormalLikeAttrs.Init(buf, pos)
+        return cls.InitFromObj(randomNormalLikeAttrs)
+
+    @classmethod
+    def InitFromPackedBuf(cls, buf, pos=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, pos)
+        return cls.InitFromBuf(buf, pos+n)
+
+    @classmethod
+    def InitFromObj(cls, randomNormalLikeAttrs):
+        x = RandomNormalLikeAttrsT()
+        x._UnPack(randomNormalLikeAttrs)
+        return x
+
+    # RandomNormalLikeAttrsT
+    def _UnPack(self, randomNormalLikeAttrs):
+        if randomNormalLikeAttrs is None:
+            return
+        self.mean = randomNormalLikeAttrs.Mean()
+        self.scale = randomNormalLikeAttrs.Scale()
+        self.seed = randomNormalLikeAttrs.Seed()
+
+    # RandomNormalLikeAttrsT
+    def Pack(self, builder):
+        RandomNormalLikeAttrsStart(builder)
+        RandomNormalLikeAttrsAddMean(builder, self.mean)
+        RandomNormalLikeAttrsAddScale(builder, self.scale)
+        RandomNormalLikeAttrsAddSeed(builder, self.seed)
+        randomNormalLikeAttrs = RandomNormalLikeAttrsEnd(builder)
+        return randomNormalLikeAttrs
+
+
 class RandomUniformAttrs(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAs(cls, buf, offset=0):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = RandomUniformAttrs()
@@ -2914,14 +3333,117 @@
         RandomUniformAttrsAddHigh(builder, self.high)
         RandomUniformAttrsAddLow(builder, self.low)
         RandomUniformAttrsAddSeed(builder, self.seed)
         randomUniformAttrs = RandomUniformAttrsEnd(builder)
         return randomUniformAttrs
 
 
+class RandomUniformLikeAttrs(object):
+    __slots__ = ['_tab']
+
+    @classmethod
+    def GetRootAs(cls, buf, offset=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
+        x = RandomUniformLikeAttrs()
+        x.Init(buf, n + offset)
+        return x
+
+    @classmethod
+    def GetRootAsRandomUniformLikeAttrs(cls, buf, offset=0):
+        """This method is deprecated. Please switch to GetRootAs."""
+        return cls.GetRootAs(buf, offset)
+    @classmethod
+    def RandomUniformLikeAttrsBufferHasIdentifier(cls, buf, offset, size_prefixed=False):
+        return flatbuffers.util.BufferHasIdentifier(buf, offset, b"\x52\x54\x45\x4E", size_prefixed=size_prefixed)
+
+    # RandomUniformLikeAttrs
+    def Init(self, buf, pos):
+        self._tab = flatbuffers.table.Table(buf, pos)
+
+    # RandomUniformLikeAttrs
+    def High(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(4))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return 0.0
+
+    # RandomUniformLikeAttrs
+    def Low(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(6))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return 0.0
+
+    # RandomUniformLikeAttrs
+    def Seed(self):
+        o = flatbuffers.number_types.UOffsetTFlags.py_type(self._tab.Offset(8))
+        if o != 0:
+            return self._tab.Get(flatbuffers.number_types.Float32Flags, o + self._tab.Pos)
+        return None
+
+def RandomUniformLikeAttrsStart(builder):
+    builder.StartObject(3)
+
+def RandomUniformLikeAttrsAddHigh(builder, high):
+    builder.PrependFloat32Slot(0, high, 0.0)
+
+def RandomUniformLikeAttrsAddLow(builder, low):
+    builder.PrependFloat32Slot(1, low, 0.0)
+
+def RandomUniformLikeAttrsAddSeed(builder, seed):
+    builder.PrependFloat32Slot(2, seed, None)
+
+def RandomUniformLikeAttrsEnd(builder):
+    return builder.EndObject()
+
+
+
+class RandomUniformLikeAttrsT(object):
+
+    # RandomUniformLikeAttrsT
+    def __init__(self):
+        self.high = 0.0  # type: float
+        self.low = 0.0  # type: float
+        self.seed = None  # type: Optional[float]
+
+    @classmethod
+    def InitFromBuf(cls, buf, pos):
+        randomUniformLikeAttrs = RandomUniformLikeAttrs()
+        randomUniformLikeAttrs.Init(buf, pos)
+        return cls.InitFromObj(randomUniformLikeAttrs)
+
+    @classmethod
+    def InitFromPackedBuf(cls, buf, pos=0):
+        n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, pos)
+        return cls.InitFromBuf(buf, pos+n)
+
+    @classmethod
+    def InitFromObj(cls, randomUniformLikeAttrs):
+        x = RandomUniformLikeAttrsT()
+        x._UnPack(randomUniformLikeAttrs)
+        return x
+
+    # RandomUniformLikeAttrsT
+    def _UnPack(self, randomUniformLikeAttrs):
+        if randomUniformLikeAttrs is None:
+            return
+        self.high = randomUniformLikeAttrs.High()
+        self.low = randomUniformLikeAttrs.Low()
+        self.seed = randomUniformLikeAttrs.Seed()
+
+    # RandomUniformLikeAttrsT
+    def Pack(self, builder):
+        RandomUniformLikeAttrsStart(builder)
+        RandomUniformLikeAttrsAddHigh(builder, self.high)
+        RandomUniformLikeAttrsAddLow(builder, self.low)
+        RandomUniformLikeAttrsAddSeed(builder, self.seed)
+        randomUniformLikeAttrs = RandomUniformLikeAttrsEnd(builder)
+        return randomUniformLikeAttrs
+
+
 class ReduceMeanAttrs(object):
     __slots__ = ['_tab']
 
     @classmethod
     def GetRootAs(cls, buf, offset=0):
         n = flatbuffers.encode.Get(flatbuffers.packer.uoffset, buf, offset)
         x = ReduceMeanAttrs()
@@ -3985,15 +4507,15 @@
 
 class OperatorNodeT(object):
 
     # OperatorNodeT
     def __init__(self):
         self.type = 0  # type: int
         self.attrsType = 0  # type: int
-        self.attrs = None  # type: Union[None, ArgMaxAttrsT, AveragePoolAttrsT, BatchNormalizationAttrsT, CastAttrsT, ConcatAttrsT, ConstantOfShapeAttrsT, ConvAttrsT, ConvTransposeAttrsT, FlattenAttrsT, GatherAttrsT, GemmAttrsT, GRUAttrsT, LeakyReluAttrsT, LSTMAttrsT, MaxPoolAttrsT, ReduceMeanAttrsT, ReshapeAttrsT, ResizeAttrsT, SplitAttrsT, SoftmaxAttrsT, TransposeAttrsT, ModAttrsT, ScatterElementsAttrsT, OneHotAttrsT, TopKAttrsT, HardSigmoidAttrsT, TriluAttrsT, ScatterNDAttrsT, NonMaxSuppressionAttrsT, LayerNormalizationAttrsT, RandomUniformAttrsT, EluAttrsT]
+        self.attrs = None  # type: Union[None, ArgMaxAttrsT, AveragePoolAttrsT, BatchNormalizationAttrsT, CastAttrsT, ConcatAttrsT, ConstantOfShapeAttrsT, ConvAttrsT, ConvTransposeAttrsT, FlattenAttrsT, GatherAttrsT, GemmAttrsT, GRUAttrsT, LeakyReluAttrsT, LSTMAttrsT, MaxPoolAttrsT, ReduceMeanAttrsT, ReshapeAttrsT, ResizeAttrsT, SplitAttrsT, SoftmaxAttrsT, TransposeAttrsT, ModAttrsT, ScatterElementsAttrsT, OneHotAttrsT, TopKAttrsT, HardSigmoidAttrsT, TriluAttrsT, ScatterNDAttrsT, NonMaxSuppressionAttrsT, LayerNormalizationAttrsT, RandomUniformAttrsT, EluAttrsT, RandomUniformLikeAttrsT, RandomNormalAttrsT, RandomNormalLikeAttrsT, GatherNDAttrsT]
         self.inputs = None  # type: List[int]
         self.outputs = None  # type: List[int]
 
     @classmethod
     def InitFromBuf(cls, buf, pos):
         operatorNode = OperatorNode()
         operatorNode.Init(buf, pos)
```

### Comparing `rten_convert-0.8.0/rten_convert.egg-info/PKG-INFO` & `rten_convert-0.9.0/rten_convert.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rten-convert
-Version: 0.8.0
+Version: 0.9.0
 Summary: Convert ONNX models to .rten format
 Project-URL: Homepage, https://github.com/robertknight/rten
 Project-URL: Issues, https://github.com/robertknight/rten/issues
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -43,7 +43,20 @@
 ## Development
 
 To install this tool from a checkout of the Git repository, run:
 
 ```sh
 pip install -e .
 ```
+
+After making changes, run the QA checks. First, install the development
+dependencies:
+
+```
+pip install -r requirements.dev.txt
+```
+
+Then run:
+
+```
+make check
+```
```

