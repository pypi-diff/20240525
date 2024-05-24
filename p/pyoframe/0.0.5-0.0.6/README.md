# Comparing `tmp/pyoframe-0.0.5.tar.gz` & `tmp/pyoframe-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoframe-0.0.5.tar", last modified: Fri May 17 09:07:05 2024, max compression
+gzip compressed data, was "pyoframe-0.0.6.tar", last modified: Fri May 24 22:50:53 2024, max compression
```

## Comparing `pyoframe-0.0.5.tar` & `pyoframe-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.481773 pyoframe-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 09:07:01.000000 pyoframe-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-17 09:07:05.481773 pyoframe-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-17 09:07:01.000000 pyoframe-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-17 09:07:01.000000 pyoframe-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:07:05.481773 pyoframe-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.473773 pyoframe-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.477773 pyoframe-0.0.5/src/pyoframe/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    50583 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/io_mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/model_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/user_defined.py
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-17 09:07:01.000000 pyoframe-0.0.5/src/pyoframe/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.477773 pyoframe-0.0.5/src/pyoframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 09:07:05.000000 pyoframe-0.0.5/src/pyoframe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:07:05.477773 pyoframe-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-17 09:07:01.000000 pyoframe-0.0.5/tests/test_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:50:53.820207 pyoframe-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-24 22:50:50.000000 pyoframe-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-24 22:50:53.820207 pyoframe-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-24 22:50:50.000000 pyoframe-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-24 22:50:50.000000 pyoframe-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:50:53.820207 pyoframe-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:50:53.812207 pyoframe-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:50:53.816207 pyoframe-0.0.6/src/pyoframe/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51139 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/io_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/model_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/user_defined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-24 22:50:50.000000 pyoframe-0.0.6/src/pyoframe/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:50:53.816207 pyoframe-0.0.6/src/pyoframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-24 22:50:53.000000 pyoframe-0.0.6/src/pyoframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-24 22:50:53.000000 pyoframe-0.0.6/src/pyoframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:50:53.000000 pyoframe-0.0.6/src/pyoframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-24 22:50:53.000000 pyoframe-0.0.6/src/pyoframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 22:50:53.000000 pyoframe-0.0.6/src/pyoframe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:50:53.816207 pyoframe-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-24 22:50:50.000000 pyoframe-0.0.6/tests/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-24 22:50:50.000000 pyoframe-0.0.6/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-24 22:50:50.000000 pyoframe-0.0.6/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-24 22:50:50.000000 pyoframe-0.0.6/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-24 22:50:50.000000 pyoframe-0.0.6/tests/test_solver.py
```

### Comparing `pyoframe-0.0.5/LICENSE` & `pyoframe-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/PKG-INFO` & `pyoframe-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoframe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Blazing fast linear program interface
 Author-email: Bravos Power <dev@bravospower.com>
 Project-URL: Homepage, https://bravos-power.github.io/pyoframe/
 Project-URL: documentation, https://bravos-power.github.io/pyoframe/
 Project-URL: repository, https://github.com/Bravos-Power/pyoframe/
 Project-URL: Issues, https://github.com/Bravos-Power/pyoframe/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyoframe-0.0.5/README.md` & `pyoframe-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/pyproject.toml` & `pyoframe-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyoframe"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name = "Bravos Power", email = "dev@bravospower.com" }]
 description = "Blazing fast linear program interface"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `pyoframe-0.0.5/src/pyoframe/_arithmetic.py` & `pyoframe-0.0.6/src/pyoframe/_arithmetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         def get_indices(expr):
             return expr.data.select(dims).unique(maintain_order=True)
 
         left_data, right_data = left.data, right.data
 
         strat = (left.unmatched_strategy, right.unmatched_strategy)
 
-        propogate_strat = propogatation_strategies[strat]
+        propogate_strat = propogatation_strategies[strat]  # type: ignore
 
         if strat == (UnmatchedStrategy.DROP, UnmatchedStrategy.DROP):
             left_data = left.data.join(get_indices(right), how="inner", on=dims)
             right_data = right.data.join(get_indices(left), how="inner", on=dims)
         elif strat == (UnmatchedStrategy.UNSET, UnmatchedStrategy.UNSET):
             assert (
                 not Config.disable_unmatched_checks
```

### Comparing `pyoframe-0.0.5/src/pyoframe/constants.py` & `pyoframe-0.0.6/src/pyoframe/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,19 @@
         except ValueError:
             return cls("unknown")
 
     @classmethod
     def from_termination_condition(
         cls, termination_condition: "TerminationCondition"
     ) -> "SolverStatus":
-        for status in STATUS_TO_TERMINATION_CONDITION_MAP:
-            if termination_condition in STATUS_TO_TERMINATION_CONDITION_MAP[status]:
+        for (
+            status,
+            termination_conditions,
+        ) in STATUS_TO_TERMINATION_CONDITION_MAP.items():
+            if termination_condition in termination_conditions:
                 return status
         return cls("unknown")
 
 
 class TerminationCondition(Enum):
     """
     Termination condition of the solver.
```

### Comparing `pyoframe-0.0.5/src/pyoframe/core.py` & `pyoframe-0.0.6/src/pyoframe/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -685,43 +685,51 @@
         """
         The value of the expression. Only available after the model has been solved.
 
         Examples:
             >>> import pyoframe as pf
             >>> m = pf.Model("max")
             >>> m.X = pf.Variable({"dim1": [1, 2, 3]}, ub=10)
-            >>> m.expr_1 = 2 * m.X
+            >>> m.expr_1 = 2 * m.X + 1
             >>> m.expr_2 = pf.sum(m.expr_1)
-            >>> m.objective = m.expr_2 + 3
+            >>> m.objective = m.expr_2 - 3
             >>> result = m.solve(log_to_console=False)
             >>> m.expr_1.value
             shape: (3, 2)
             ┌──────┬──────────┐
             │ dim1 ┆ solution │
             │ ---  ┆ ---      │
             │ i64  ┆ f64      │
             ╞══════╪══════════╡
-            │ 1    ┆ 20.0     │
-            │ 2    ┆ 20.0     │
-            │ 3    ┆ 20.0     │
+            │ 1    ┆ 21.0     │
+            │ 2    ┆ 21.0     │
+            │ 3    ┆ 21.0     │
             └──────┴──────────┘
             >>> m.expr_2.value
-            60.0
-            >>> m.objective.value
             63.0
         """
+        assert (
+            self._model is not None
+        ), "Expression must be added to the model to use .value"
         if self._model.result is None or self._model.result.solution is None:
             raise ValueError(
                 "Can't obtain value of expression since the model has not been solved."
             )
 
         df = (
             self.data.join(self._model.result.solution.primal, on=VAR_KEY, how="left")
+            .with_columns(
+                (
+                    pl.when(pl.col(VAR_KEY) == CONST_TERM)
+                    .then(1)
+                    .otherwise(pl.col(SOLUTION_KEY))
+                    * pl.col(COEF_KEY)
+                ).alias(SOLUTION_KEY)
+            )
             .drop(VAR_KEY)
-            .with_columns((pl.col(SOLUTION_KEY) * pl.col(COEF_KEY)))
             .drop(COEF_KEY)
         )
 
         dims = self.dimensions
         if dims is not None:
             df = df.group_by(dims, maintain_order=True)
         return df.sum()
@@ -920,14 +928,17 @@
     def slack(self):
         """
         The slack of the constraint.
         Will raise an error if the model has not already been solved.
         The first call to this property will load the slack values from the solver (lazy loading).
         """
         if SLACK_COL not in self.data.columns:
+            assert (
+                self._model is not None
+            ), "Constraint must be added to a model to get the slack."
             if self._model.solver is None:
                 raise ValueError("The model has not been solved yet.")
             self._model.solver.load_slack()
         return self.data.select(self.dimensions_unsafe + [SLACK_COL])
 
     @slack.setter
     def slack(self, value):
@@ -1156,15 +1167,15 @@
     # TODO: Breaking change, remove support for Iterable[AcceptableSets]
     def __init__(
         self,
         *indexing_sets: SetTypes | Iterable[SetTypes],
         lb: float | int | SupportsToExpr | None = None,
         ub: float | int | SupportsToExpr | None = None,
         vtype: VType | VTypeValue = VType.CONTINUOUS,
-        equals: SupportsToExpr = None,
+        equals: Optional[SupportsMath] = None,
     ):
         if lb is None:
             lb = float("-inf")
         if ub is None:
             ub = float("inf")
         if equals is not None:
             assert (
@@ -1218,14 +1229,17 @@
     def RC(self):
         """
         The reduced cost of the variable.
         Will raise an error if the model has not already been solved.
         The first call to this property will load the reduced costs from the solver (lazy loading).
         """
         if RC_COL not in self.data.columns:
+            assert (
+                self._model is not None
+            ), "Variable must be added to a model to get the reduced cost."
             if self._model.solver is None:
                 raise ValueError("The model has not been solved yet.")
             self._model.solver.load_rc()
         return self.data.select(self.dimensions_unsafe + [RC_COL])
 
     @RC.setter
     def RC(self, value):
```

### Comparing `pyoframe-0.0.5/src/pyoframe/io.py` & `pyoframe-0.0.6/src/pyoframe/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, Optional, TypeVar, Union
 from tqdm import tqdm
 
 from pyoframe.constants import CONST_TERM, VAR_KEY, ObjSense
 from pyoframe.core import Constraint, Variable
 from pyoframe.io_mappers import (
-    Base62ConstMapper,
-    Base62VarMapper,
+    Base36ConstMapper,
+    Base36VarMapper,
     IOMappers,
     Mapper,
     NamedMapper,
     NamedVariableMapper,
 )
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -127,41 +127,51 @@
 
 def get_var_map(m: "Model", use_var_names):
     if use_var_names:
         if m.var_map is not None:
             return m.var_map
         var_map = NamedVariableMapper(Variable)
     else:
-        var_map = Base62VarMapper(Variable)
+        var_map = Base36VarMapper(Variable)
 
     for v in m.variables:
         var_map.add(v)
     return var_map
 
 
 def to_file(
-    m: "Model", file_path: Optional[Union[str, Path]], use_var_names=False
+    m: "Model", file_path: Optional[Union[str, Path]] = None, use_var_names=False
 ) -> Path:
     """
     Write out a model to a lp file.
+
+    Args:
+        m: The model to write out.
+        file_path: The path to write the model to. If None, a temporary file is created. The caller is responsible for
+            deleting the file after use.
+        use_var_names: If True, variable names are used in the lp file. Otherwise, variable
+            indices are used.
+
+    Returns:
+        The path to the lp file.
     """
     if file_path is None:
         with NamedTemporaryFile(
             prefix="pyoframe-problem-", suffix=".lp", mode="w", delete=False
         ) as f:
             file_path = f.name
 
     file_path = Path(file_path)
     assert file_path.suffix == ".lp", f"File format `{file_path.suffix}` not supported."
 
     if file_path.exists():
         file_path.unlink()
 
     const_map = (
-        NamedMapper(Constraint) if use_var_names else Base62ConstMapper(Constraint)
+        NamedMapper(Constraint) if use_var_names else Base36ConstMapper(Constraint)
     )
     for c in m.constraints:
         const_map.add(c)
     var_map = get_var_map(m, use_var_names)
     m.io_mappers = IOMappers(var_map, const_map)
 
     with open(file_path, mode="w") as f:
```

### Comparing `pyoframe-0.0.5/src/pyoframe/io_mappers.py` & `pyoframe-0.0.6/src/pyoframe/io_mappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 from pyoframe.util import concat_dimensions
 from pyoframe.constants import CONST_TERM
 
 
 if TYPE_CHECKING:  # pragma: no cover
     from pyoframe.model import Variable
     from pyoframe.core import Constraint
-    from pyoframe.util import CountableModelElement
+    from pyoframe.model_element import ModelElementWithId
 
 
 @dataclass
 class IOMappers:
     var_map: "Mapper"
     const_map: "Mapper"
 
 
 class Mapper(ABC):
 
     NAME_COL = "__name"
 
-    def __init__(self, cls: Type["CountableModelElement"]) -> None:
+    def __init__(self, cls: Type["ModelElementWithId"]) -> None:
         self._ID_COL = cls.get_id_column_name()
         self.mapping_registry = pl.DataFrame(
             {self._ID_COL: [], Mapper.NAME_COL: []},
             schema={self._ID_COL: pl.UInt32, Mapper.NAME_COL: pl.String},
         )
 
     def add(self, element: Union["Variable", "Constraint"]) -> None:
         self._extend_registry(self._element_to_map(element))
 
     def _extend_registry(self, df: pl.DataFrame) -> None:
         self.mapping_registry = pl.concat([self.mapping_registry, df])
 
     @abstractmethod
-    def _element_to_map(self, element: "CountableModelElement") -> pl.DataFrame: ...
+    def _element_to_map(self, element: "ModelElementWithId") -> pl.DataFrame: ...
 
     def apply(
         self,
         df: pl.DataFrame,
         to_col: Optional[str] = None,
     ) -> pl.DataFrame:
         if df.height == 0:
@@ -103,21 +103,22 @@
             pl.DataFrame(
                 {self._ID_COL: [CONST_TERM], self.NAME_COL: [self.CONST_TERM_NAME]},
                 schema={self._ID_COL: pl.UInt32, self.NAME_COL: pl.String},
             )
         )
 
 
-class Base62Mapper(Mapper, ABC):
-    # Mapping between a base 62 character and its integer value
+class Base36Mapper(Mapper, ABC):
+    # Mapping between a base 36 character and its integer value
+    # Note: we must use only lowercase since Gurobi auto-converts variables that aren't in constraints to lowercase (kind of annoying)
     _CHAR_TABLE = pl.DataFrame(
-        {"char": list(string.digits + string.ascii_letters)},
+        {"char": list(string.digits + string.ascii_lowercase)},
     ).with_columns(pl.int_range(pl.len()).cast(pl.UInt32).alias("code"))
 
-    _BASE = _CHAR_TABLE.height  # _BASE = 62
+    _BASE = _CHAR_TABLE.height  # _BASE = 36
     _ZERO = _CHAR_TABLE.filter(pl.col("code") == 0).select("char").item()  # _ZERO = "0"
 
     @property
     @abstractmethod
     def _prefix(self) -> "str": ...
 
     def apply(
@@ -127,44 +128,44 @@
     ) -> pl.DataFrame:
         if df.height == 0:
             return df
 
         query = pl.concat_str(
             pl.lit(self._prefix),
             pl.col(self._ID_COL).map_batches(
-                Base62Mapper._to_base62,
+                Base36Mapper._to_base36,
                 return_dtype=pl.String,
                 is_elementwise=True,
             ),
         )
 
         if to_col is None:
             to_col = self._ID_COL
 
         return df.with_columns(query.alias(to_col))
 
     @classmethod
-    def _to_base62(cls, int_col: pl.Series) -> pl.Series:
-        """Returns a series of dtype str with a base 62 representation of the integers in int_col.
-        The letters 0-9a-zA-Z are used as symbols for the representation.
+    def _to_base36(cls, int_col: pl.Series) -> pl.Series:
+        """Returns a series of dtype str with a base 36 representation of the integers in int_col.
+        The letters 0-9A-Z are used as symbols for the representation.
 
         Examples:
 
             >>> import polars as pl
             >>> s = pl.Series([0,10,20,60,53,66], dtype=pl.UInt32)
-            >>> Base62Mapper._to_base62(s).to_list()
-            ['0', 'a', 'k', 'Y', 'R', '14']
+            >>> Base36Mapper._to_base36(s).to_list()
+            ['0', 'a', 'k', '1o', '1h', '1u']
 
             >>> s = pl.Series([0], dtype=pl.UInt32)
-            >>> Base62Mapper._to_base62(s).to_list()
+            >>> Base36Mapper._to_base36(s).to_list()
             ['0']
         """
         assert isinstance(
             int_col.dtype, pl.UInt32
-        ), "_to_base62() only works for UInt32 id columns"
+        ), "_to_base36() only works for UInt32 id columns"
 
         largest_id = int_col.max()
         if largest_id == 0:
             max_digits = 1
         else:
             max_digits = math.floor(math.log(largest_id, cls._BASE)) + 1  # type: ignore
 
@@ -189,28 +190,28 @@
             .replace("", cls._ZERO)
         )
 
     def _element_to_map(self, element) -> pl.DataFrame:
         return self.apply(element.ids.select(self._ID_COL), to_col=Mapper.NAME_COL)
 
 
-class Base62VarMapper(Base62Mapper):
+class Base36VarMapper(Base36Mapper):
     """
     Examples:
         >>> import polars as pl
         >>> from pyoframe import Model, Variable
         >>> from pyoframe.constants import VAR_KEY
         >>> m = Model("min")
         >>> m.x = Variable(pl.DataFrame({"t": range(1,63)}))
         >>> (m.x.filter(t=11)+1).to_str()
         '[11]: 1  + x[11]'
-        >>> (m.x.filter(t=11)+1).to_str(var_map=Base62VarMapper(Variable))
+        >>> (m.x.filter(t=11)+1).to_str(var_map=Base36VarMapper(Variable))
         '[11]: 1  + xb'
 
-        >>> Base62VarMapper(Variable).apply(pl.DataFrame({VAR_KEY: []}))
+        >>> Base36VarMapper(Variable).apply(pl.DataFrame({VAR_KEY: []}))
         shape: (0, 1)
         ┌───────────────┐
         │ __variable_id │
         │ ---           │
         │ null          │
         ╞═══════════════╡
         └───────────────┘
@@ -226,12 +227,12 @@
         self._extend_registry(df)
 
     @property
     def _prefix(self) -> "str":
         return "x"
 
 
-class Base62ConstMapper(Base62Mapper):
+class Base36ConstMapper(Base36Mapper):
 
     @property
     def _prefix(self) -> "str":
         return "c"
```

### Comparing `pyoframe-0.0.5/src/pyoframe/model.py` & `pyoframe-0.0.6/src/pyoframe/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         "name",
         "solver",
         "solver_model",
         "params",
         "result",
         "attr",
         "sense",
+        "objective",
     ]
 
     def __init__(self, min_or_max: Union[ObjSense, ObjSenseValue], name=None, **kwargs):
         super().__init__(**kwargs)
         self._variables: List[Variable] = []
         self._constraints: List[Constraint] = []
         self.sense = ObjSense(min_or_max)
@@ -71,45 +72,45 @@
     def constraints(self):
         return self._constraints
 
     @property
     def objective(self):
         return self._objective
 
+    @objective.setter
+    def objective(self, value):
+        value = Objective(value)
+        self._objective = value
+        value.on_add_to_model(self, "objective")
+
     def __setattr__(self, __name: str, __value: Any) -> None:
         if __name not in Model._reserved_attributes and not isinstance(
             __value, (ModelElement, pl.DataFrame, pd.DataFrame)
         ):
             raise PyoframeError(
                 f"Cannot set attribute '{__name}' on the model because it isn't of type ModelElement (e.g. Variable, Constraint, ...)"
             )
 
         if (
             isinstance(__value, ModelElement)
             and __name not in Model._reserved_attributes
         ):
-            if __name == "objective":
-                __value = Objective(__value)
-
             if isinstance(__value, ModelElementWithId):
                 assert not hasattr(
                     self, __name
                 ), f"Cannot create {__name} since it was already created."
 
             __value.on_add_to_model(self, __name)
 
             if isinstance(__value, Variable):
                 self._variables.append(__value)
                 if self.var_map is not None:
                     self.var_map.add(__value)
             elif isinstance(__value, Constraint):
                 self._constraints.append(__value)
-            elif isinstance(__value, Objective):
-                self._objective = __value
-                return
         return super().__setattr__(__name, __value)
 
     def __repr__(self) -> str:
         return f"""Model '{self.name}' ({len(self.variables)} vars, {len(self.constraints)} constrs, {1 if self.objective else "no"} obj)"""
 
     to_file = to_file
     solve = solve
```

### Comparing `pyoframe-0.0.5/src/pyoframe/model_element.py` & `pyoframe-0.0.6/src/pyoframe/model_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,36 +105,40 @@
 
 
 def _support_polars_method(method_name: str):
     """
     Wrapper to add a method to ModelElement that simply calls the underlying Polars method on the data attribute.
     """
 
-    def method(self: "SupportPolarsMethodMixin", *args, **kwargs):
+    def method(self: "SupportPolarsMethodMixin", *args, **kwargs) -> Any:
         result_from_polars = getattr(self.data, method_name)(*args, **kwargs)
         if isinstance(result_from_polars, pl.DataFrame):
             return self._new(result_from_polars)
         else:
             return result_from_polars
 
     return method
 
 
-class SupportPolarsMethodMixin:
+class SupportPolarsMethodMixin(ABC):
     rename = _support_polars_method("rename")
     with_columns = _support_polars_method("with_columns")
     filter = _support_polars_method("filter")
     estimated_size = _support_polars_method("estimated_size")
 
     @abstractmethod
     def _new(self, data: pl.DataFrame):
         """
         Used to create a new instance of the same class with the given data (for e.g. on .rename(), .with_columns(), etc.).
         """
 
+    @property
+    @abstractmethod
+    def data(self): ...
+
 
 class ModelElementWithId(ModelElement, AttrContainerMixin):
     """
     Provides a method that assigns a unique ID to each row in a DataFrame.
     IDs start at 1 and go up consecutively. No zero ID is assigned since it is reserved for the constant variable term.
     IDs are only unique for the subclass since different subclasses have different counters.
     """
```

### Comparing `pyoframe-0.0.5/src/pyoframe/monkey_patch.py` & `pyoframe-0.0.6/src/pyoframe/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/src/pyoframe/objective.py` & `pyoframe-0.0.6/src/pyoframe/objective.py`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/src/pyoframe/solvers.py` & `pyoframe-0.0.6/src/pyoframe/solvers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Code to interface with various solvers
 """
 
 from abc import abstractmethod, ABC
 from functools import lru_cache
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Type, Union, TYPE_CHECKING
+from typing import Any, Dict, Optional, Type, Union, TYPE_CHECKING
 
 import polars as pl
 
 from pyoframe.constants import (
     DUAL_KEY,
     SOLUTION_KEY,
     SLACK_COL,
@@ -46,15 +46,14 @@
 
 
 def solve(
     m: "Model",
     solver=None,
     directory: Optional[Union[Path, str]] = None,
     use_var_names=False,
-    env=None,
     log_fn=None,
     warmstart_fn=None,
     basis_fn=None,
     solution_file=None,
     log_to_console=True,
 ):
     if solver is None:
@@ -64,26 +63,28 @@
             )
         solver = available_solvers[0]
 
     if solver not in solver_registry:
         raise ValueError(f"Solver {solver} not recognized or supported.")
 
     solver_cls = solver_registry[solver]
-    m.solver = solver_cls(m, log_to_console)
-    m.solver_model = m.solver.create_solver_model(directory, use_var_names, env)
+    m.solver = solver_cls(
+        m,
+        log_to_console,
+        params={param: value for param, value in m.params},
+        directory=directory,
+    )
+    m.solver_model = m.solver.create_solver_model(use_var_names)
     m.solver.solver_model = m.solver_model
 
     for attr_container in [m.variables, m.constraints, [m]]:
         for container in attr_container:
             for param_name, param_value in container.attr:
                 m.solver.set_attr(container, param_name, param_value)
 
-    for param, value in m.params:
-        m.solver.set_param(param, value)
-
     result = m.solver.solve(log_fn, warmstart_fn, basis_fn, solution_file)
     result = m.solver.process_result(result)
     m.result = result
 
     if result.solution is not None:
         if m.objective is not None:
             m.objective.value = result.solution.objective
@@ -95,29 +96,28 @@
             for constraint in m.constraints:
                 constraint.dual = result.solution.dual
 
     return result
 
 
 class Solver(ABC):
-    def __init__(self, model, log_to_console):
+    def __init__(self, model: "Model", log_to_console, params, directory):
         self._model = model
         self.solver_model: Optional[Any] = None
-        self.log_to_console = log_to_console
+        self.log_to_console: bool = log_to_console
+        self.params = params
+        self.directory = directory
 
     @abstractmethod
-    def create_solver_model(self) -> Any: ...
+    def create_solver_model(self, use_var_names) -> Any: ...
 
     @abstractmethod
     def set_attr(self, element, param_name, param_value): ...
 
     @abstractmethod
-    def set_param(self, param_name, param_value): ...
-
-    @abstractmethod
     def solve(self, log_fn, warmstart_fn, basis_fn, solution_file) -> Result: ...
 
     @abstractmethod
     def process_result(self, results: Result) -> Result: ...
 
     def load_rc(self):
         rc = self._get_all_rc()
@@ -131,35 +131,50 @@
 
     @abstractmethod
     def _get_all_rc(self): ...
 
     @abstractmethod
     def _get_all_slack(self): ...
 
+    def dispose(self):
+        """
+        Clean up any resources that wouldn't be cleaned up by the garbage collector.
+
+        For now, this is only used by the Gurobi solver to call .dispose() on the solver model and Gurobi environment
+        which helps close a connection to the Gurobi Computer Server. Note that this effectively disables commands that
+        need access to the solver model (like .slack and .RC)
+        """
+
 
 class FileBasedSolver(Solver):
-    def create_solver_model(
-        self, directory: Optional[Union[Path, str]], use_var_names, env
-    ) -> Any:
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.problem_file: Optional[Path] = None
+        self.keep_files = self.directory is not None
+
+    def create_solver_model(self, use_var_names) -> Any:
         problem_file = None
+        directory = self.directory
         if directory is not None:
             if isinstance(directory, str):
                 directory = Path(directory)
             if not directory.exists():
                 directory.mkdir(parents=True)
             filename = (
                 self._model.name if self._model.name is not None else "pyoframe-problem"
             )
             problem_file = directory / f"{filename}.lp"
-        problem_file = self._model.to_file(problem_file, use_var_names=use_var_names)
+        self.problem_file = self._model.to_file(
+            problem_file, use_var_names=use_var_names
+        )
         assert self._model.io_mappers is not None
-        return self.create_solver_model_from_lp(problem_file, env)
+        return self.create_solver_model_from_lp()
 
     @abstractmethod
-    def create_solver_model_from_lp(self, problem_file: Path, env) -> Any: ...
+    def create_solver_model_from_lp(self) -> Any: ...
 
     def set_attr(self, element, param_name, param_value):
         if isinstance(param_value, pl.DataFrame):
             if isinstance(element, pf.Variable):
                 param_value = self._model.io_mappers.var_map.apply(param_value)
             elif isinstance(element, pf.Constraint):
                 param_value = self._model.io_mappers.const_map.apply(param_value)
@@ -212,51 +227,53 @@
         13: "suboptimal",
         14: "unknown",
         15: "terminated_by_limit",
         16: "internal_solver_error",
         17: "internal_solver_error",
     }
 
-    def create_solver_model_from_lp(self, problem_fn, env) -> Result:
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if not self.log_to_console:
+            self.params["LogToConsole"] = 0
+        self.env = None
+
+    def create_solver_model_from_lp(self) -> Any:
         """
         Solve a linear problem using the gurobi solver.
 
         This function communicates with gurobi using the gurubipy package.
         """
+        assert self.problem_file is not None
+        self.env = gurobipy.Env(params=self.params)
 
-        if env is None:
-            if self.log_to_console:
-                env = gurobipy.Env()
-            else:
-                # See https://support.gurobi.com/hc/en-us/articles/360044784552-How-do-I-suppress-all-console-output-from-Gurobi
-                env = gurobipy.Env(empty=True)
-                env.setParam("LogToConsole", 0)
-                env.start()
+        m = gurobipy.read(_path_to_str(self.problem_file), env=self.env)
+        if not self.keep_files:
+            self.problem_file.unlink()
 
-        m = gurobipy.read(_path_to_str(problem_fn), env=env)
         return m
 
-    def set_param(self, param_name, param_value):
-        self.solver_model.setParam(param_name, param_value)
-
     @lru_cache
     def _get_var_mapping(self):
+        assert self.solver_model is not None
         vars = self.solver_model.getVars()
         return vars, pl.DataFrame(
             {VAR_KEY: self.solver_model.getAttr("VarName", vars)}
         ).with_columns(i=pl.int_range(pl.len()))
 
     @lru_cache
     def _get_constraint_mapping(self):
+        assert self.solver_model is not None
         constraints = self.solver_model.getConstrs()
         return constraints, pl.DataFrame(
             {CONSTRAINT_KEY: self.solver_model.getAttr("ConstrName", constraints)}
         ).with_columns(i=pl.int_range(pl.len()))
 
     def set_attr_unmapped(self, element, param_name, param_value):
+        assert self.solver_model is not None
         if isinstance(element, pf.Model):
             self.solver_model.setAttr(param_name, param_value)
         elif isinstance(element, pf.Variable):
             v, v_map = self._get_var_mapping()
             param_value = param_value.join(v_map, on=VAR_KEY, how="left").drop(VAR_KEY)
             self.solver_model.setAttr(
                 param_name,
@@ -273,14 +290,15 @@
                 [c[i] for i in param_value["i"]],
                 param_value[param_name],
             )
         else:
             raise ValueError(f"Element type {type(element)} not recognized.")
 
     def solve(self, log_fn, warmstart_fn, basis_fn, solution_file) -> Result:
+        assert self.solver_model is not None
         m = self.solver_model
         if log_fn is not None:
             m.setParam("logfile", _path_to_str(log_fn))
         if warmstart_fn:
             m.read(_path_to_str(warmstart_fn))
 
         m.optimize()
@@ -341,13 +359,19 @@
         return pl.DataFrame(
             {
                 SLACK_COL: m.getAttr("Slack", constraints),
                 CONSTRAINT_KEY: m.getAttr("ConstrName", constraints),
             }
         )
 
+    def dispose(self):
+        if self.solver_model is not None:
+            self.solver_model.dispose()
+        if self.env is not None:
+            self.env.dispose()
+
 
 def _path_to_str(path: Union[Path, str]) -> str:
     """
     Convert a pathlib.Path to a string.
     """
     return str(path.resolve()) if isinstance(path, Path) else path
```

### Comparing `pyoframe-0.0.5/src/pyoframe/user_defined.py` & `pyoframe-0.0.6/src/pyoframe/user_defined.py`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/src/pyoframe/util.py` & `pyoframe-0.0.6/src/pyoframe/util.py`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/src/pyoframe.egg-info/PKG-INFO` & `pyoframe-0.0.6/src/pyoframe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoframe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Blazing fast linear program interface
 Author-email: Bravos Power <dev@bravospower.com>
 Project-URL: Homepage, https://bravos-power.github.io/pyoframe/
 Project-URL: documentation, https://bravos-power.github.io/pyoframe/
 Project-URL: repository, https://github.com/Bravos-Power/pyoframe/
 Project-URL: Issues, https://github.com/Bravos-Power/pyoframe/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyoframe-0.0.5/src/pyoframe.egg-info/SOURCES.txt` & `pyoframe-0.0.6/src/pyoframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/tests/test_arithmetic.py` & `pyoframe-0.0.6/tests/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/tests/test_examples.py` & `pyoframe-0.0.6/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/tests/test_io.py` & `pyoframe-0.0.6/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/tests/test_operations.py` & `pyoframe-0.0.6/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyoframe-0.0.5/tests/test_solver.py` & `pyoframe-0.0.6/tests/test_solver.py`

 * *Files identical despite different names*

