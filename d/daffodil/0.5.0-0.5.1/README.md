# Comparing `tmp/daffodil-0.5.0.tar.gz` & `tmp/daffodil-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daffodil-0.5.0.tar", last modified: Thu May 23 20:05:01 2024, max compression
+gzip compressed data, was "daffodil-0.5.1.tar", last modified: Sat May 25 15:36:10 2024, max compression
```

## Comparing `daffodil-0.5.0.tar` & `daffodil-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.763474 daffodil-0.5.0/
--rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.5.0/LICENSE
--rw-rw-rw-   0        0        0    54140 2024-05-23 20:05:01.759474 daffodil-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    53485 2024-05-23 19:59:10.000000 daffodil-0.5.0/README.md
--rw-rw-rw-   0        0        0      819 2024-05-23 19:55:35.000000 daffodil-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 20:05:01.763474 daffodil-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.709478 daffodil-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.724471 daffodil-0.5.0/src/daffodil/
--rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.0/src/daffodil/__init__.py
--rw-rw-rw-   0        0        0   221370 2024-05-23 19:58:46.000000 daffodil-0.5.0/src/daffodil/daf.py
--rw-rw-rw-   0        0        0    10430 2024-05-15 18:08:46.000000 daffodil-0.5.0/src/daffodil/keyedlist.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.750476 daffodil-0.5.0/src/daffodil/lib/
--rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.0/src/daffodil/lib/__init__.py
--rw-rw-rw-   0        0        0    43214 2024-05-15 19:07:31.000000 daffodil-0.5.0/src/daffodil/lib/daf_indexing.py
--rw-rw-rw-   0        0        0    31645 2024-05-02 16:49:22.000000 daffodil-0.5.0/src/daffodil/lib/daf_md.py
--rw-rw-rw-   0        0        0     7708 2024-05-02 16:49:22.000000 daffodil-0.5.0/src/daffodil/lib/daf_pandas.py
--rw-rw-rw-   0        0        0     5174 2024-05-02 03:32:58.000000 daffodil-0.5.0/src/daffodil/lib/daf_types.py
--rw-rw-rw-   0        0        0    51588 2024-05-20 23:41:53.000000 daffodil-0.5.0/src/daffodil/lib/daf_utils.py
--rw-rw-rw-   0        0        0     5796 2024-05-02 03:32:58.000000 daffodil-0.5.0/src/daffodil/lib/md_demo.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.757474 daffodil-0.5.0/src/daffodil.egg-info/
--rw-rw-rw-   0        0        0    54140 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.754505 daffodil-0.5.0/tests/
--rw-rw-rw-   0        0        0   164590 2024-05-15 19:07:31.000000 daffodil-0.5.0/tests/test_daf.py
--rw-rw-rw-   0        0        0     2202 2024-05-09 16:48:49.000000 daffodil-0.5.0/tests/test_keyedlist.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.988795 daffodil-0.5.1/
+-rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0    54140 2024-05-25 15:36:10.983788 daffodil-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    53485 2024-05-23 19:59:10.000000 daffodil-0.5.1/README.md
+-rw-rw-rw-   0        0        0      819 2024-05-25 15:04:51.000000 daffodil-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 15:36:10.988795 daffodil-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.860789 daffodil-0.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.886788 daffodil-0.5.1/src/daffodil/
+-rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.1/src/daffodil/__init__.py
+-rw-rw-rw-   0        0        0   221695 2024-05-25 15:29:13.000000 daffodil-0.5.1/src/daffodil/daf.py
+-rw-rw-rw-   0        0        0    10430 2024-05-15 18:08:46.000000 daffodil-0.5.1/src/daffodil/keyedlist.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.960787 daffodil-0.5.1/src/daffodil/lib/
+-rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.1/src/daffodil/lib/__init__.py
+-rw-rw-rw-   0        0        0    41798 2024-05-25 15:02:12.000000 daffodil-0.5.1/src/daffodil/lib/daf_indexing.py
+-rw-rw-rw-   0        0        0    31645 2024-05-02 16:49:22.000000 daffodil-0.5.1/src/daffodil/lib/daf_md.py
+-rw-rw-rw-   0        0        0     7708 2024-05-02 16:49:22.000000 daffodil-0.5.1/src/daffodil/lib/daf_pandas.py
+-rw-rw-rw-   0        0        0     5174 2024-05-02 03:32:58.000000 daffodil-0.5.1/src/daffodil/lib/daf_types.py
+-rw-rw-rw-   0        0        0    51588 2024-05-20 23:41:53.000000 daffodil-0.5.1/src/daffodil/lib/daf_utils.py
+-rw-rw-rw-   0        0        0     5796 2024-05-02 03:32:58.000000 daffodil-0.5.1/src/daffodil/lib/md_demo.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.980789 daffodil-0.5.1/src/daffodil.egg-info/
+-rw-rw-rw-   0        0        0    54140 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 15:36:10.000000 daffodil-0.5.1/src/daffodil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 15:36:10.971797 daffodil-0.5.1/tests/
+-rw-rw-rw-   0        0        0   164590 2024-05-15 19:07:31.000000 daffodil-0.5.1/tests/test_daf.py
+-rw-rw-rw-   0        0        0     2202 2024-05-09 16:48:49.000000 daffodil-0.5.1/tests/test_keyedlist.py
```

### Comparing `daffodil-0.5.0/LICENSE` & `daffodil-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/PKG-INFO` & `daffodil-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: daffodil
-Version: 0.5.0
+Version: 0.5.1
 Summary: Daffodil provides lightweight and fast 2-D dataframes
 Author-email: Ray Lutz <raylutz@cognisys.com>
 License: MIT
 Project-URL: Homepage, https://github.com/raylutz/daffodil
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: xlsx2csv==0.8.2
-Requires-Dist: Markdown==3.4.1
+Requires-Dist: xlsx2csv>=0.8.2
+Requires-Dist: Markdown>=3.4.1
 Provides-Extra: numpy
 Requires-Dist: numpy; extra == "numpy"
 
 ![daffodil_logo](https://github.com/raylutz/daffodil/assets/14955977/5e141583-0216-429d-9ba8-be938aa13017)
 
 # Python Daffodil
```

### Comparing `daffodil-0.5.0/README.md` & `daffodil-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/pyproject.toml` & `daffodil-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "daffodil"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
     {name = "Ray Lutz", email = "raylutz@cognisys.com"},
 ]
 description = "Daffodil provides lightweight and fast 2-D dataframes"
 readme = "README.md"
 requires-python = ">=3.6"
 
@@ -16,16 +16,16 @@
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "xlsx2csv==0.8.2",
-    "Markdown==3.4.1",
+    "xlsx2csv>=0.8.2",
+    "Markdown>=3.4.1",
 ]
 
 [project.optional-dependencies]
 numpy = ['numpy']
 
 [project.urls]
 Homepage = "https://github.com/raylutz/daffodil"
```

### Comparing `daffodil-0.5.0/src/daffodil/daf.py` & `daffodil-0.5.1/src/daffodil/daf.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,16 +223,22 @@
             Added .strip() method.
             correct icols when providing a single str column name, and when column names have more than one character each.
             Added 'flatten' in '.to_list' method which will combine lol to a single list.
             Added .num_rows() which will more robustly calculate the number of rows in edge cases.
             Fix unflattening issue discovered when running edge_test_utils.py.
             Updated documentation to reflect new approach to dtypes and flattening.
              
-    v0.5.1  (pending)
+    v0.5.1  (2024-05-25)
+            changed dependencies in pyproject.toml so they would allow newer versions.
+            Upgraded to Python 3.11 and upgraded all libraries to the latest.
+            Using venv311
     
+    v0.5.2  (pending)
+    
+            
             
     TODO
             add use of pickledjson to express contents of individual cells when not jsonable.
             tests: need to add
                 __str__ and __repr__
                 
                 apply_dtypes()
@@ -368,25 +374,28 @@
         1. run all tests and demos to verify validity of the version.
             in tests:
                 python test_daf.py
                 python test_keyedlist.py
                 python daf_demo.py
                 python daf_benchmarks.py
         2. Increment version number in pyproject.toml
+        3. Remove prior release
+                rm -r dist
         3. build the release
-                python -m build --sdist
+                python -m build
         4. Upload it
                 twine upload dist/*
                 
-        
+     
+    venv311\Scripts\activate     
 """       
     
     
-#VERSION  = 'v0.5.0'
-#VERSDATE = '2024-05-23'  
+#VERSION  = 'v0.5.1'
+#VERSDATE = '2024-05-25'  
 
 import os
 import sys
 import io
 import csv
 import copy
 import re
```

### Comparing `daffodil-0.5.0/src/daffodil/keyedlist.py` & `daffodil-0.5.1/src/daffodil/keyedlist.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/src/daffodil/lib/daf_indexing.py` & `daffodil-0.5.1/src/daffodil/lib/daf_indexing.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,42 +96,45 @@
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 """
 
-
 """
 See README file at this location: https://github.com/raylutz/Daf/blob/main/README.md
 """
 import sys
-import os
-sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.realpath(__file__)))))
+from pathlib import Path
+
+sys.path.append(str(Path(__file__).resolve().parents[2]))
+
 from daffodil.lib.daf_types import T_ls, T_li, T_doda, T_lb
-                            # T_lola, T_da, T_di, T_hllola, T_loda, T_dtype_dict, T_dola, T_dodi, T_la, T_lota, T_buff, T_df, T_ds, 
-                     
+# T_lola, T_da, T_di, T_hllola, T_loda, T_dtype_dict, T_dola, T_dodi, T_la, T_lota, T_buff, T_df, T_ds,
+
 import daffodil.lib.daf_utils as utils
-#import Daf.daf_md    as md
-import daffodil.lib.daf_indexing as indexing       # self import so internal references to indexing will work.
+# import Daf.daf_md    as md
+import daffodil.lib.daf_indexing as indexing  # self import so internal references to indexing will work.
 from daffodil.daf import Daf
 
+from typing import List, Dict, Any, Tuple, Optional, Union, cast, Type, Callable  #
+
+
+def fake_function(a: Optional[List[Dict[str, Tuple[int, Union[Any, str, Type, Callable]]]]] = None) -> Optional[int]:
+    return None or cast(int, 0)  # pragma: no cover
+
 
-from typing import List, Dict, Any, Tuple, Optional, Union, cast, Type, Callable #
-def fake_function(a: Optional[List[Dict[str, Tuple[int,Union[Any, str, Type, Callable ]]]]] = None) -> Optional[int]:
-    return None or cast(int, 0)   # pragma: no cover
-    
 indexing_version = 'version3'
 
 
 def _get_item(self,
-        slice_spec:   Union[slice, int, str, T_li, T_ls, T_lb, 
-                            Tuple[  Union[slice, int, str, T_li, T_ls, T_lb], 
-                                    Union[slice, int, str, T_li, T_ls, T_lb]]],
-        ) -> 'Daf':
+              slice_spec: Union[slice, int, str, T_li, T_ls, T_lb,
+              Tuple[Union[slice, int, str, T_li, T_ls, T_lb],
+              Union[slice, int, str, T_li, T_ls, T_lb]]],
+              ) -> 'Daf':
     """ allow selection and slicing using one or two specs:
         
             my_daf[2, 3]         -- select cell at row 2, col 3 and return value.
             my_daf[2]            -- select row 2, including all columns, return as a list.
             my_daf[2, :]         -- same as above
             my_daf[[2], :]       -- same as above
             my_daf[[2,5,8]]      -- select rows 2, 5, and 8, including all columns
@@ -162,42 +165,39 @@
             returns a consistent daf instance copied from the original, and with the data specified.
             always returns the simplest object possible.
             if multiple rows or columns are specified, they will be returned in the original orientation.
             if only one cell is selected, return a single value.
             If only one row is selected, return a list. If a dict is required, use select_irow()
             if only one col is selected, return a list.
         """
-    
-    
-    
+
     if indexing_version == 'version2':
         return indexing._get_item2(self, slice_spec)
-    elif indexing_version == 'version3':    
+    elif indexing_version == 'version3':
         return indexing._get_item3(self, slice_spec)
-        
-        
+
     return indexing._get_item1(self, slice_spec)
 
+
 def _set_item3(self, slice_spec):
     pass
 
 
 def _get_item3(self,
-        slice_spec:   Union[slice, int, str, T_li, T_ls, T_lb, 
-                            Tuple[  Union[slice, int, str, T_li, T_ls, T_lb], 
-                                    Union[slice, int, str, T_li, T_ls, T_lb]]],
-        ) -> 'Daf':
-
+               slice_spec: Union[slice, int, str, T_li, T_ls, T_lb,
+               Tuple[Union[slice, int, str, T_li, T_ls, T_lb],
+               Union[slice, int, str, T_li, T_ls, T_lb]]],
+               ) -> 'Daf':
     if isinstance(slice_spec, tuple) and len(slice_spec) == 2:
         # Handle parsing slices for  both rows and columns
         row_spec, col_spec = slice_spec
     else:
         row_spec = slice_spec
         col_spec = None
-        
+
     if isinstance(row_spec, (int, slice)) or utils.is_list_of_type(row_spec, int):
         sel_rows_daf = self.select_irows(irows=slice_spec)
     elif isinstance(row_spec, str) or utils.is_list_of_type(row_spec, str):
         sel_rows_daf = self.select_krows(krows=slice_spec)
     else:
         return self
 
@@ -206,59 +206,51 @@
 
     if isinstance(col_spec, (int, slice)) or utils.is_list_of_type(col_spec, int):
         return sel_rows_daf.select_icols(icols=slice_spec)
     elif isinstance(col_spec, str) or utils.is_list_of_type(col_spec, str):
         return sel_rows_daf.select_kcols(kcols=slice_spec)
     else:
         return sel_rows_daf
-        
-
-           
 
 
-
-    
-
 def _get_item1(self,
-        slice_spec:   Union[slice, int, str, T_li, T_ls, T_lb, 
-                            Tuple[  Union[slice, int, str, T_li, T_ls, T_lb], 
-                                    Union[slice, int, str, T_li, T_ls, T_lb]]],
-        ) -> 'Daf':
-
-
+               slice_spec: Union[slice, int, str, T_li, T_ls, T_lb,
+               Tuple[Union[slice, int, str, T_li, T_ls, T_lb],
+               Union[slice, int, str, T_li, T_ls, T_lb]]],
+               ) -> 'Daf':
     if isinstance(slice_spec, slice):
         # Handle slicing only rows
         return indexing._handle_slice(self, slice_spec, None)
-        
+
     elif isinstance(slice_spec, int):
         # Handle indexing a single row
         irow = slice_spec
         return indexing._handle_slice(self, slice(irow, irow + 1), None)
-        
+
     elif isinstance(slice_spec, str):
         # Handle indexing a single row using keyfield
         if not self.keyfield:
             raise RuntimeError("Use of string row spec requires keyfield defined.")
         irow = self.kd.get(slice_spec, -1)
         if irow < 0:
             raise RuntimeError("Row spec not a valid row key.")
-        
+
         return indexing._handle_slice(self, slice(irow, irow + 1), None)
-        
+
     elif isinstance(slice_spec, list):
         # single list of row indices
-        row_indices = indexing._row_indices_from_rowlist(self, slice_spec)            
+        row_indices = indexing._row_indices_from_rowlist(self, slice_spec)
         return indexing._handle_slice(self, row_indices, None)
-        
+
     elif isinstance(slice_spec, tuple) and len(slice_spec) == 2:
         # Handle slicing both rows and columns
         return indexing._handle_slice(self, slice_spec[0], slice_spec[1])
     else:
         raise TypeError("Unsupported indexing type. Use slices, integers, or tuples of slices and integers.")
-        
+
 
 def _handle_slice(self, row_slice: Union[slice, int, None], col_slice: Union[slice, int, str, None]) -> Any:
     """
     Handles the slicing operation for rows and columns in a Daf instance.
 
     Args:
     - row_slice (Union[slice, int, None]): The slice specification for rows.
@@ -268,206 +260,208 @@
     - Daf: A new Daf instance with sliced data based on the provided row and column specifications.
     or
     a single value if the resulting Daf is only one cell.
     or a list if a single row or col results
     """
     all_cols = self.columns()
     sliced_cols = all_cols
-    row_sliced_lol = self.lol   # default is no change
-    
+    row_sliced_lol = self.lol  # default is no change
+
     # handle simple cases first:
     # selecting a row spec is integer.
     if isinstance(row_slice, int):
         irow = row_slice
         # select one cell.
         if isinstance(col_slice, int):
             return self.lol[irow][col_slice]
         elif isinstance(col_slice, str):
             icol = self.hd[col_slice]
             return self.lol[irow][icol]
-            
+
         # full row    
         if col_slice is None:
             la = self.lol[irow]
-            
+
         # part of a row, according to a slice
         elif isinstance(col_slice, slice):
             start_col, stop_col, step_col = indexing._parse_slice(self, col_slice, row_or_col='col')
             la = self.lol[irow][start_col:stop_col:step_col]
-            
+
         # part of a row, according to a column list    
         elif isinstance(col_slice, list):
             # the following handles cases of integer list as well as str list of colnames.
             col_indices_li = indexing._col_indices_from_collist(self, col_slice)
             la = [self.lol[irow][icol] for icol in col_indices_li]
         return la
 
     # first handle the rows
     elif row_slice is None:
         # no specs, return the entire array.
         if col_slice is None:
-            return indexing._adjust_return_val(self)   # is this correct?
-        
+            return indexing._adjust_return_val(self)  # is this correct?
+
         # all rows, one column
         elif isinstance(col_slice, int) or isinstance(col_slice, str):
             if isinstance(col_slice, str):
                 icol = self.hd[col_slice]
             else:
                 icol = col_slice
             col_la = [row[icol] for row in self.lol]
             return col_la
 
         # part of all rows, according to a list    
-        elif isinstance(col_slice, list):    
+        elif isinstance(col_slice, list):
             col_indices_li = indexing._col_indices_from_collist(self, col_slice)
             row_col_sliced_lol = [[row[i] for i in col_indices_li] for row in self.lol]
             sliced_cols = [all_cols[i] for i in col_indices_li]
 
         elif isinstance(col_slice, slice):
             # use normal slice approach
             start_col, stop_col, step_col = indexing._parse_slice(self, col_slice, row_or_col='col')
             row_col_sliced_lol = [[row[icol] for icol in range(start_col, stop_col, step_col)] for row in self.lol]
             sliced_cols = [all_cols[icol] for icol in range(start_col, stop_col, step_col)]
             # also respect the column names
-            
+
         sliced_daf = Daf(lol=row_col_sliced_lol, cols=sliced_cols, dtypes=self.dtypes, keyfield=self.keyfield)
         return sliced_daf._adjust_return_val()
 
     # sliced or listed rows, first reduce the array by rows.
     elif isinstance(row_slice, list):
-        row_indices = indexing._row_indices_from_rowlist(self, row_slice)            
-            
+        row_indices = indexing._row_indices_from_rowlist(self, row_slice)
+
         if row_indices:
             row_sliced_lol = [self.lol[i] for i in row_indices]
         # else:
-            # row_sliced_lol = self.lol
-                
-    elif isinstance(row_slice, slice):    
+        # row_sliced_lol = self.lol
+
+    elif isinstance(row_slice, slice):
         start_row, stop_row, step_row = indexing._parse_slice(self, row_slice)
         row_sliced_lol = self.lol[start_row:stop_row:step_row]
     # else:
-        # row_sliced_lol = self.lol
+    # row_sliced_lol = self.lol
 
     # sliced rows, all columns
     if col_slice is None:
         row_col_sliced_lol = row_sliced_lol
-        
+
     #   one column    
     elif isinstance(col_slice, int) or isinstance(col_slice, str):
         if isinstance(col_slice, str):
             icol = self.hd[col_slice]
         else:
             icol = col_slice
-            
+
         col_la = [row[icol] for row in row_sliced_lol]
         return col_la
 
     # part of all sliced rows, according to a list    
-    elif isinstance(col_slice, list):    
+    elif isinstance(col_slice, list):
         col_indices_li = indexing._col_indices_from_collist(self, col_slice)
         row_col_sliced_lol = [[row[i] for i in col_indices_li] for row in row_sliced_lol]
         # also respect the column names, if they are defined.
         if self.hd:
             sliced_cols = [all_cols[i] for i in col_indices_li]
         else:
-            sliced_cols = None            
+            sliced_cols = None
 
     elif isinstance(col_slice, slice):
-                       
+
         # use normal slice approach
         start_col, stop_col, step_col = indexing._parse_slice(self, col_slice, row_or_col='col')
         row_col_sliced_lol = [[row[icol] for icol in range(start_col, stop_col, step_col)] for row in row_sliced_lol]
         # also respect the column names, if they are defined.
         if self.hd:
             sliced_cols = [self.columns()[icol] for icol in range(start_col, stop_col, step_col)]
         else:
-            sliced_cols = None            
+            sliced_cols = None
 
-    from daffodil.daf import Daf    
+    from daffodil.daf import Daf
     sliced_daf = Daf(lol=row_col_sliced_lol, cols=sliced_cols, dtypes=self.dtypes, keyfield=self.keyfield)
     return indexing._adjust_return_val(sliced_daf)
 
 
 def _adjust_return_val(self):
     # not sure if this is the correct way to go!
     # particularly with zero copy, this may not be correct.
     #
     # alternative is to use .tolist() and .todict()
     # if the method returns a daf.
     #
     # @@TODO: Must be fixed for zero_copy
-    
+
     num_cols = self.num_cols()
     num_rows = len(self.lol)
 
     if num_rows == 1 and num_cols == 1:
         # single value, just return it.
         return self.lol[0][0]
-        
+
     elif num_rows == 1 and num_cols > 1:
         # single row, return as list.
         return self.lol[0]
-            
+
     elif num_rows > 1 and num_cols == 1:
         # single column result as a list.
         return self.icol(0)
-        
+
     return self
-    
+
 
 def _col_indices_from_collist(self, collist) -> T_li:  # col_indices
 
     if not collist:
         return []
 
     first_item = collist[0]
-    if isinstance(first_item, str):             # probably list of column names (did not check them all)
+    if isinstance(first_item, str):  # probably list of column names (did not check them all)
         colnames = collist
         col_indices = [self.hd[col] for col in colnames]
-    elif isinstance(first_item, int):           # probably list of column indices (did not check them all)
+    elif isinstance(first_item, int):  # probably list of column indices (did not check them all)
         col_indices = collist
     else:
         raise ValueError("column slice, if a list, must be a list of strings or ints")
     return col_indices
-    
 
-def _row_indices_from_rowlist(self, rowlist) -> T_li: # row_indices
+
+def _row_indices_from_rowlist(self, rowlist) -> T_li:  # row_indices
     if not rowlist:
         return []
-        
+
     first_item = rowlist[0]
     if isinstance(first_item, str):
         if not self.keyfield:
             raise RuntimeError("keyfield must be defined to use str row keys")
         row_indices = [self.kd.get(rowkey, -1) for rowkey in rowlist]
     elif isinstance(first_item, int):
         row_indices = rowlist
     else:
         raise RuntimeError("list spec must use str or int values")
-        
+
     return row_indices
 
-def _parse_slice(self, s: Union[slice, int, None], row_or_col:str='row') -> Tuple[Optional[int], Optional[int], Optional[int]]:
+
+def _parse_slice(self, s: Union[slice, int, None], row_or_col: str = 'row') -> Tuple[
+    Optional[int], Optional[int], Optional[int]]:
     if isinstance(s, slice):
         start = s.start if s.start is not None else 0
-        
+
         stop = s.stop if s.stop is not None else (self.num_cols() if row_or_col == 'col' else len(self.lol))
-        
+
         step = s.step if s.step is not None else 1
         return start, stop, step
     elif isinstance(s, int):
         return s, s + 1, 1
     elif s is None:
         return None, None, None
-    
-            
-def _set_item(self, 
-        slice_spec: Union[int, Tuple[Union[slice, int, List[str], List[bool]], Union[slice, int, str, List[str], List[bool]]]], 
-        value: Any):
 
+
+def _set_item(self,
+              slice_spec: Union[
+                  int, Tuple[Union[slice, int, List[str], List[bool]], Union[slice, int, str, List[str], List[bool]]]],
+              value: Any):
     """
         Handles the assignment of values, lists or dicts to Daf elements.
         
         Can handle the following scenarios:
             my_daf[3] = list                   -- assign the entire row at index 3 to the list provided
             my_daf[[3]] = list                 -- same as above
             my_daf[3, :] = list                -- same as above.
@@ -509,202 +503,204 @@
 
     if indexing_version == 'version2':
         return _set_item2(self, slice_spec, value)
     if indexing_version == 'version3':
         return _set_item3(self, slice_spec, value)
     return _set_item1(self, slice_spec, value)
 
-def _set_item1(self, 
-        slice_spec: Union[int, Tuple[Union[slice, int, List[str], List[bool]], Union[slice, int, str, List[str], List[bool]]]], 
-        value: Any):
 
+def _set_item1(self,
+               slice_spec: Union[
+                   int, Tuple[Union[slice, int, List[str], List[bool]], Union[slice, int, str, List[str], List[bool]]]],
+               value: Any):
     if isinstance(slice_spec, int):
         irow = slice_spec
         # Assigning a row based on a single integer index and a value which is a list.
         # will trigger an error if the list is not the right length for the row.
         if isinstance(value, list):
             self.lol[irow] = value
-            
+
         # if value is a dict, use it and make sure the right columns are assigned per dict keys.    
         elif isinstance(value, dict):
             self.assign_record_irow(irow, record=value)
         else:
             # set the same value in the row for all columns.
             self.lol[irow] = [value] * len(self.lol[irow])
-        
+
     elif isinstance(slice_spec, list) and isinstance(value, self.__class__):
         # assign a number of rows to the data in daf provided.
         row_indices = self._row_indices_from_rowlist(slice_spec)
         for source_row, irow in enumerate(row_indices):
             self.lol[irow] = value.lol[source_row]
 
     elif isinstance(slice_spec, tuple):
         row_spec, col_spec = slice_spec
         if isinstance(row_spec, int) or isinstance(row_spec, str):
             if isinstance(row_spec, str) and self.keyfield:
                 irow = self.kd[row_spec]
             else:
                 irow = row_spec
-                
+
             if isinstance(col_spec, int):
                 # my_daf[irow, icol] = value       -- set cell irow, icol to value, where irow, icol are integers.
                 self.lol[irow][col_spec] = value
-                
+
             elif isinstance(col_spec, str):
                 # my_daf[irow, colname] = value    -- set a value in cell irow, col, where colname is a string.
                 icol = self.hd[col_spec]
                 self.lol[irow][icol] = value
-                
+
             elif isinstance(col_spec, list) and col_spec:
                 col_indices = indexing._col_indices_from_collist(self, col_spec)
-                    
+
                 # assign a number of columns specified in a list of colnames to a single row, from a list with only those columns.
                 for source_col, icol in enumerate(col_indices):
-                    self.lol[irow][icol] = value[source_col]                
-        
+                    self.lol[irow][icol] = value[source_col]
+
             elif isinstance(col_spec, slice):
                 # my_daf[irow, start:end] = value  -- set a value in cells in row irow, from columns start to end.
                 # my_daf[irow, start:end] = list   -- set values from a list in cells in row irow, from columns start to end.
                 col_start, col_stop, col_step = indexing._parse_slice(self, col_spec)
-                for idx, icol in enumerate(range(col_start, col_stop, col_step)):   # type: ignore
+                for idx, icol in enumerate(range(col_start, col_stop, col_step)):  # type: ignore
                     if isinstance(value, list):
                         self.lol[irow][icol] = value[idx]
                     else:
                         self.lol[irow][icol] = value
-                        
+
         elif isinstance(row_spec, slice):
             row_start, row_stop, row_step = indexing._parse_slice(self, row_spec)
-            
+
             if isinstance(col_spec, list) and col_spec:
                 col_indices = indexing._col_indices_from_collist(self, col_spec)
-                     
+
                 for source_row, irow in enumerate(range(row_start, row_stop, row_step)):
                     for source_col, icol in enumerate(col_indices):
                         self.lol[irow][icol] = value.lol[source_row][source_col]
-                    
-            
+
+
             elif isinstance(col_spec, int) or isinstance(col_spec, str):
                 if isinstance(col_spec, str):
                     icol = self.hd[col_spec]
                 else:
                     icol = col_spec
-            
-                for idx, irow in enumerate(range(row_start, row_stop, row_step)):       # type: ignore
+
+                for idx, irow in enumerate(range(row_start, row_stop, row_step)):  # type: ignore
                     if isinstance(value, list):
                         self.lol[irow][icol] = value[idx]
                     else:
                         self.lol[irow][icol] = value
-                        
+
         elif isinstance(row_spec, str) and self.keyfield:
             irow = self.kd[row_spec]
-            
+
             if isinstance(col_spec, list) and col_spec:
                 col_indices = indexing._col_indices_from_collist(self, col_spec)
 
                 for source_row, irow in enumerate(row_indices):
                     for source_col, icol in enumerate(col_indices):
                         self.lol[irow][icol] = value.lol[source_row][source_col]
-                        
+
             elif isinstance(col_spec, int) or isinstance(col_spec, str):
                 if isinstance(col_spec, str):
                     icol = self.hd[col_spec]
                 else:
                     icol = col_spec
-            
-                for idx, irow in enumerate(range(row_start, row_stop, row_step)):       # type: ignore
+
+                for idx, irow in enumerate(range(row_start, row_stop, row_step)):  # type: ignore
                     if isinstance(value, list):
                         self.lol[irow][icol] = value[idx]
                     else:
                         self.lol[irow][icol] = value
-                        
-            
+
+
         elif isinstance(row_spec, list):
             row_indices = indexing._row_indices_from_rowlist(self, row_spec)
-            
+
             if isinstance(col_spec, list) and col_spec:
                 col_indices = indexing._col_indices_from_collist(self, col_spec)
 
                 for source_row, irow in enumerate(row_indices):
                     for source_col, icol in enumerate(col_indices):
                         self.lol[irow][icol] = value.lol[source_row][source_col]
-                    
-            
+
+
             elif isinstance(col_spec, int) or isinstance(col_spec, str):
                 if isinstance(col_spec, str):
                     icol = self.hd[col_spec]
                 else:
                     icol = col_spec
-            
-                for idx, irow in enumerate(row_indices): 
+
+                for idx, irow in enumerate(row_indices):
                     if isinstance(value, list):
                         self.lol[irow][icol] = value[idx]
                     else:
                         self.lol[irow][icol] = value
         else:
             raise ValueError("Unsupported key type for assignment")
 
-        
+
     else:
         raise ValueError("Unsupported key type for assignment")
 
-    self._rebuild_kd()    
-    
-#===== VERSION 2 ======
+    self._rebuild_kd()
+
+
+# ===== VERSION 2 ======
+
+def _parse_itemidx(self, slice_spec: Union[slice, int, str, T_li, T_ls, T_lb], row_or_col: str = 'row',
+                   parse_doda: Optional[T_doda] = None) -> T_doda:  # parse_doda
 
-def _parse_itemidx(self, slice_spec: Union[slice, int, str, T_li, T_ls, T_lb], row_or_col:str='row', 
-                    parse_doda: Optional[T_doda]=None) -> T_doda: # parse_doda
-                    
     """ parse one index of the item specification using square brackets.
     
         if the return value is a boolean mask, then the rows or columns cannot be reordered.
         It is very costly to reorder columns. Rows can be reordered easily.
         Column order can be altered through a reordering table if desired. i.e. the kd could be
         used to reorder the columns. Therefore, the column calculations should go through 
         the kd to allow column order changes without changing the array.
         
         This function may be called twice in any parsing operation if the type is tuple.
         
     """
     if parse_doda is None:
-        parse_doda = {'row':{}, 'col':{}}
-    
+        parse_doda = {'row': {}, 'col': {}}
+
     if isinstance(slice_spec, slice):
         if slice_spec.start is None and slice_spec.stop is None:
             # no slicing.
             parse_doda[row_or_col] = {}
-            
+
         start_idx, stop_idx, step_idx = indexing._parse_slice(self, slice_spec, row_or_col=row_or_col)
-        
+
         if row_or_col == 'row':
             # save slice tuple directly and do not construct a list of indices
             parse_doda[row_or_col]['slice'] = (start_idx, stop_idx, step_idx)
-        else: 
+        else:
             # for col, always resolve to li
             parse_doda[row_or_col]['li'] = [idx for idx in range(start_idx, stop_idx, step_idx)]
-        
+
     elif isinstance(slice_spec, int):
         if row_or_col == 'row' or not self.kd:
             parse_doda[row_or_col]['li'] = [slice_spec]
         else:
             parse_doda[row_or_col]['li'] = [list(self.hd.values())[slice_spec]]
-            
+
     elif isinstance(slice_spec, str):
         if row_or_col == 'col':
             icol = self.hd[slice_spec]
             parse_doda[row_or_col]['li'] = [icol]
         else:
             irow = self.kd[slice_spec]
             parse_doda[row_or_col]['li'] = [irow]
-    
+
     elif isinstance(slice_spec, list) and slice_spec:
         first_item = slice_spec[0]
-        
+
         if isinstance(first_item, int):
             parse_doda[row_or_col]['li'] = slice_spec
-            
+
         elif isinstance(first_item, str):
             if row_or_col == 'col':
                 colnames_ls = slice_spec
                 icol_li = [self.hd.get(colname, -1) for colname in colnames_ls]
                 parse_doda[row_or_col]['li'] = icol_li
             else:
                 rowkeys_ls = slice_spec
@@ -713,225 +709,219 @@
 
         elif isinstance(first_item, bool):
             if row_or_col == 'row':
                 parse_doda[row_or_col]['lb'] = slice_spec
             else:
                 # for col, always resolve to li
                 parse_doda[row_or_col]['li'] = [idx for idx, istrue in enumerate(slice_spec) if istrue]
-            
+
     else:
         raise AttributeError("slice spec error")
-        
+
     return parse_doda
-        
 
-def _get_parse_doda(self, 
-        slice_spec:   Union[slice, int, str, T_li, T_ls, T_lb, 
-                            Tuple[  Union[slice, int, str, T_li, T_ls, T_lb], 
-                                    Union[slice, int, str, T_li, T_ls, T_lb]]],
-        ) -> T_doda: # parse_doda
+
+def _get_parse_doda(self,
+                    slice_spec: Union[slice, int, str, T_li, T_ls, T_lb,
+                    Tuple[Union[slice, int, str, T_li, T_ls, T_lb],
+                    Union[slice, int, str, T_li, T_ls, T_lb]]],
+                    ) -> T_doda:  # parse_doda
 
     if isinstance(slice_spec, tuple) and len(slice_spec) == 2:
         # Handle parsing slices for  both rows and columns
-        parse_doda = indexing._parse_itemidx(self, slice_spec[0], 
-                            row_or_col='row', 
-                            )
-        parse_doda = indexing._parse_itemidx(self, slice_spec[1], 
-                            row_or_col='col',
-                            parse_doda = parse_doda,
-                            )
-    else:
-        parse_doda = indexing._parse_itemidx(self, slice_spec, 
-                            row_or_col='row', 
-                            )
+        parse_doda = indexing._parse_itemidx(self, slice_spec[0],
+                                             row_or_col='row',
+                                             )
+        parse_doda = indexing._parse_itemidx(self, slice_spec[1],
+                                             row_or_col='col',
+                                             parse_doda=parse_doda,
+                                             )
+    else:
+        parse_doda = indexing._parse_itemidx(self, slice_spec,
+                                             row_or_col='row',
+                                             )
     return parse_doda
-    
-    
-def _get_item2(self,
-        slice_spec:   Union[slice, int, str, T_li, T_ls, T_lb, 
-                            Tuple[  Union[slice, int, str, T_li, T_ls, T_lb], 
-                                    Union[slice, int, str, T_li, T_ls, T_lb]]],
-        ) -> 'Daf':
 
+
+def _get_item2(self,
+               slice_spec: Union[slice, int, str, T_li, T_ls, T_lb,
+               Tuple[Union[slice, int, str, T_li, T_ls, T_lb],
+               Union[slice, int, str, T_li, T_ls, T_lb]]],
+               ) -> 'Daf':
     parse_doda = indexing._get_parse_doda(self, slice_spec)
-    
+
     return indexing._get_by_parse_doda(self, parse_doda)
-    
 
-def _set_item2(self,
-        slice_spec:   Union[slice, int, str, T_li, T_ls, T_lb, 
-                            Tuple[  Union[slice, int, str, T_li, T_ls, T_lb], 
-                                    Union[slice, int, str, T_li, T_ls, T_lb]]],
-        value: Any,              
-        ) -> 'Daf':
 
+def _set_item2(self,
+               slice_spec: Union[slice, int, str, T_li, T_ls, T_lb,
+               Tuple[Union[slice, int, str, T_li, T_ls, T_lb],
+               Union[slice, int, str, T_li, T_ls, T_lb]]],
+               value: Any,
+               ) -> 'Daf':
     parse_doda = indexing._get_parse_doda(self, slice_spec)
-    
+
     return indexing._set_by_parse_doda(self, parse_doda, value)
 
 
 def _get_by_parse_doda(self, parse_doda: T_doda) -> 'Daf':
-
     if not parse_doda['row'] and not parse_doda['col']:
         # return all rows and columns unchanged.
         return self
 
     if self.hd:
         all_cols = sliced_cols = list(self.hd.keys())
     else:
         all_cols = sliced_cols = None
-        
+
     if parse_doda['row']:
         if 'li' in parse_doda['row']:
             row_indices = parse_doda['row']['li']
             # list of indices specified
             row_sliced_lol = [self.lol[i] for i in row_indices if i >= 0]
-            
+
         elif 'slice' in parse_doda['row']:
             start, stop, step = parse_doda['row']['slice']
             # list of indices specified
             row_sliced_lol = [self.lol[i] for i in range(start, stop, step)]
-            
+
         elif 'lb' in parse_doda['row']:
             row_boolean_mask_lb = parse_doda['row']['lb']
             # list of indices specified
             row_sliced_lol = [self.lol[i] for i in range(len(self.lol)) if row_boolean_mask_lb[i]]
-            
+
     if parse_doda['col']:
         col_indices_li = parse_doda['col']['li']
         row_col_sliced_lol = [[row[i] for i in col_indices_li] for row in row_sliced_lol]
         # also respect the column names, if they are defined.
         if self.hd:
             sliced_cols = [all_cols[i] for i in col_indices_li]
 
     else:
         row_col_sliced_lol = row_sliced_lol
 
-    new_daf = self.clone_empty(lol=row_col_sliced_lol, cols=sliced_cols)        
+    new_daf = self.clone_empty(lol=row_col_sliced_lol, cols=sliced_cols)
 
     return new_daf._adjust_return_val()
-    
-        
-def _set_by_parse_doda(self, parse_doda: T_doda, value: Any) -> 'Daf':
 
+
+def _set_by_parse_doda(self, parse_doda: T_doda, value: Any) -> 'Daf':
     if not parse_doda['row'] and not parse_doda['col']:
         # return all rows and columns unchanged.
         return self
-        
+
     elif parse_doda['row'] and not parse_doda['col']:
         # no column spec, affect complete rows.
-        
+
         if 'li' in parse_doda['row'] and isinstance(value, self.__class__):
             row_indices = parse_doda['row']['li']
             # list of indices specified
             for source_row, irow in enumerate(row_indices):
                 self.lol[irow] = value.lol[source_row]
-            
+
         elif 'slice' in parse_doda['row']:
             start, stop, step = parse_doda['row']['slice']
             # slice specified
             for source_row, irow in enumerate(range(start, stop, step)):
                 self.lol[irow] = value.lol[source_row]
-            
+
         elif 'lb' in parse_doda['row']:
             row_boolean_mask_lb = parse_doda['row']['lb']
             # boolean mask specified
             source_row = 0
             for irow, istrue in enumerate(row_boolean_mask_lb):
                 if not istrue:
                     continue
                 self.lol[irow] = value.lol[source_row]
                 source_row += 1
         else:
             raise NotImplementedError
 
     elif parse_doda['col'] and not parse_doda['row']:
         # affecting only columns.
-        
+
         dest_col_li = parse_doda['col']['li']
         num_dest_cols = len(dest_col_li)
-        
+
         if num_dest_cols == 1 and isinstance(value, list):
             icol = dest_col_li[0]
             utils.assign_col_in_lol_at_icol(icol, col_la=value, lol=self.lol)
-          
+
         # scalar value: repeat in the entire column.  
         elif num_dest_cols == 1 and isinstance(value, (float, int, str)):
             icol = dest_col_li[0]
             utils.assign_col_in_lol_at_icol(icol, col_la=None, lol=self.lol, default=value)
-            
+
         elif num_dest_cols > 1 and isinstance(value, self.__class__):
             for irow in range(len(value.lol)):
                 for source_icol, dest_icol in enumerate(dest_col_li):
                     self.lol[irow][dest_icol] = value.lol[irow][source_icol]
         else:
             raise NotImplementedError
-                
+
     elif parse_doda['col'] and parse_doda['row']:
-                
+
         dest_col_li = parse_doda['col']['li']
         num_dest_cols = len(dest_col_li)
-        
+
         if 'li' in parse_doda['row'] or 'lb' in parse_doda['row']:
-        
+
             if 'lb' in parse_doda['row']:
                 dest_row_li = [idx for idx, istrue in enumerate(parse_doda['row']['lb']) if istrue]
             else:
                 dest_row_li = parse_doda['row']['li']
-                
+
             num_dest_rows = len(dest_row_li)
-            
+
             if num_dest_rows == 1:
                 irow = dest_row_li[0]
-            
+
                 if num_dest_cols == 1:
                     icol = dest_col_li[0]
                     self.lol[irow][icol] = value
-        
+
                 elif num_dest_cols > 1 and isinstance(value, list):
                     for source_icol, dest_icol in enumerate(dest_col_li):
                         self.lol[irow][dest_icol] = value[source_icol]
-                        
+
             elif num_dest_rows > 1 and isinstance(value, self.__class__):
                 for source_irow, dest_irow in enumerate(dest_row_li):
                     for source_icol, dest_icol in enumerate(dest_col_li):
-                        self.lol[dest_irow][dest_icol] = value.lol[source_irow][source_icol]            
+                        self.lol[dest_irow][dest_icol] = value.lol[source_irow][source_icol]
             else:
                 raise NotImplementedError
 
         elif 'slice' in parse_doda['row']:
             dest_row_start, dest_row_stop, dest_row_step = parse_doda['row']['slice']
             num_dest_rows = (dest_row_stop - dest_row_start) // dest_row_step
-            
+
             if num_dest_rows == 1:
                 irow = dest_row_start
-            
+
                 if num_dest_cols == 1:
                     icol = dest_col_li[0]
                     self.lol[irow][icol] = value
-        
+
                 elif num_dest_cols > 1 and isinstance(value, list):
                     for source_icol, dest_icol in enumerate(dest_col_li):
                         self.lol[irow][dest_icol] = value[source_icol]
-                        
+
             elif num_dest_rows > 1 and isinstance(value, list):
                 for source_irow, dest_irow in enumerate(range(dest_row_start, dest_row_stop, dest_row_step)):
                     for source_icol, dest_icol in enumerate(dest_col_li):
-                        self.lol[dest_irow][dest_icol] = value[source_irow]            
+                        self.lol[dest_irow][dest_icol] = value[source_irow]
 
             elif num_dest_rows > 1 and isinstance(value, self.__class__):
                 for source_irow, dest_irow in enumerate(range(dest_row_start, dest_row_stop, dest_row_step)):
                     for source_icol, dest_icol in enumerate(dest_col_li):
-                        self.lol[dest_irow][dest_icol] = value.lol[source_irow][source_icol]            
+                        self.lol[dest_irow][dest_icol] = value.lol[source_irow][source_icol]
             else:
-                import pdb; pdb.set_trace() #temp
+                import pdb;
+                pdb.set_trace()  # temp
                 pass
-                
+
                 raise NotImplementedError
-        
+
         else:
             raise NotImplementedError
 
-            
     return self
-            
-
```

### Comparing `daffodil-0.5.0/src/daffodil/lib/daf_md.py` & `daffodil-0.5.1/src/daffodil/lib/daf_md.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/src/daffodil/lib/daf_pandas.py` & `daffodil-0.5.1/src/daffodil/lib/daf_pandas.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/src/daffodil/lib/daf_types.py` & `daffodil-0.5.1/src/daffodil/lib/daf_types.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/src/daffodil/lib/daf_utils.py` & `daffodil-0.5.1/src/daffodil/lib/daf_utils.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/src/daffodil/lib/md_demo.py` & `daffodil-0.5.1/src/daffodil/lib/md_demo.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/src/daffodil.egg-info/PKG-INFO` & `daffodil-0.5.1/src/daffodil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: daffodil
-Version: 0.5.0
+Version: 0.5.1
 Summary: Daffodil provides lightweight and fast 2-D dataframes
 Author-email: Ray Lutz <raylutz@cognisys.com>
 License: MIT
 Project-URL: Homepage, https://github.com/raylutz/daffodil
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: xlsx2csv==0.8.2
-Requires-Dist: Markdown==3.4.1
+Requires-Dist: xlsx2csv>=0.8.2
+Requires-Dist: Markdown>=3.4.1
 Provides-Extra: numpy
 Requires-Dist: numpy; extra == "numpy"
 
 ![daffodil_logo](https://github.com/raylutz/daffodil/assets/14955977/5e141583-0216-429d-9ba8-be938aa13017)
 
 # Python Daffodil
```

### Comparing `daffodil-0.5.0/src/daffodil.egg-info/SOURCES.txt` & `daffodil-0.5.1/src/daffodil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/tests/test_daf.py` & `daffodil-0.5.1/tests/test_daf.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.5.0/tests/test_keyedlist.py` & `daffodil-0.5.1/tests/test_keyedlist.py`

 * *Files identical despite different names*

