# Comparing `tmp/dash_spread_grid-0.0.9.tar.gz` & `tmp/dash_spread_grid-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_spread_grid-0.0.9.tar", last modified: Tue Apr  9 17:54:55 2024, max compression
+gzip compressed data, was "dash_spread_grid-0.1.1.tar", last modified: Sat May 25 08:46:02 2024, max compression
```

## Comparing `dash_spread_grid-0.0.9.tar` & `dash_spread_grid-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.0.9/LICENSE
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.0.9/MANIFEST.in
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.0.9/README.md
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/dash_spread_grid/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3272 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid/DashSpreadGrid.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.0.9/dash_spread_grid/__init__.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid/_imports_.py
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    51727 2024-04-09 17:54:53.000000 dash_spread_grid-0.0.9/dash_spread_grid/dash_spread_grid.min.js
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   199999 2024-04-09 17:54:53.000000 dash_spread_grid-0.0.9/dash_spread_grid/dash_spread_grid.min.js.map
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6042 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid/metadata.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2332 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid/package-info.json
-drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/PKG-INFO
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-04-09 17:54:54.000000 dash_spread_grid-0.0.9/dash_spread_grid.egg-info/top_level.txt
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2332 2024-04-09 17:54:43.000000 dash_spread_grid-0.0.9/package.json
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-04-09 17:54:55.045855 dash_spread_grid-0.0.9/setup.cfg
--rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.0.9/setup.py
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-25 08:46:02.812154 dash_spread_grid-0.1.1/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.1/LICENSE
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      393 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.1/MANIFEST.in
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-25 08:46:02.812154 dash_spread_grid-0.1.1/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3703 2024-01-20 12:13:37.000000 dash_spread_grid-0.1.1/README.md
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-25 08:46:02.812154 dash_spread_grid-0.1.1/dash_spread_grid/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     3288 2024-05-25 08:46:02.000000 dash_spread_grid-0.1.1/dash_spread_grid/DashSpreadGrid.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2261 2024-01-18 13:13:06.000000 dash_spread_grid-0.1.1/dash_spread_grid/__init__.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       78 2024-05-25 08:46:02.000000 dash_spread_grid-0.1.1/dash_spread_grid/_imports_.py
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)    54181 2024-05-25 08:46:01.000000 dash_spread_grid-0.1.1/dash_spread_grid/dash_spread_grid.min.js
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)   210339 2024-05-25 08:46:01.000000 dash_spread_grid-0.1.1/dash_spread_grid/dash_spread_grid.min.js.map
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     6046 2024-05-25 08:46:02.000000 dash_spread_grid-0.1.1/dash_spread_grid/metadata.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-25 08:46:02.000000 dash_spread_grid-0.1.1/dash_spread_grid/package-info.json
+drwxr-xr-x   0 tomaszrewak  (1000) tomaszrewak  (1000)        0 2024-05-25 08:46:02.812154 dash_spread_grid-0.1.1/dash_spread_grid.egg-info/
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      259 2024-05-25 08:46:02.000000 dash_spread_grid-0.1.1/dash_spread_grid.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      457 2024-05-25 08:46:02.000000 dash_spread_grid-0.1.1/dash_spread_grid.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)        1 2024-05-25 08:46:02.000000 dash_spread_grid-0.1.1/dash_spread_grid.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       17 2024-05-25 08:46:02.000000 dash_spread_grid-0.1.1/dash_spread_grid.egg-info/top_level.txt
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)     2455 2024-05-25 08:45:51.000000 dash_spread_grid-0.1.1/package.json
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)       38 2024-05-25 08:46:02.812154 dash_spread_grid-0.1.1/setup.cfg
+-rw-r--r--   0 tomaszrewak  (1000) tomaszrewak  (1000)      510 2024-01-18 13:19:42.000000 dash_spread_grid-0.1.1/setup.py
```

### Comparing `dash_spread_grid-0.0.9/README.md` & `dash_spread_grid-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.0.9/dash_spread_grid/DashSpreadGrid.py` & `dash_spread_grid-0.1.1/dash_spread_grid/DashSpreadGrid.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 - columnWidths (list; optional)
 
 - columns (list; default [{ "type": "DATA-BLOCK" }])
 
 - data (boolean | number | string | dict | list; optional)
 
-- dataSelector (string; default "data[row.id][column.id]")
+- data_selector (string; default "data[row.id][column.id]")
 
-- editedCells (list; optional)
+- edited_cells (list; optional)
 
 - filtering (list; optional)
 
 - filters (list; optional)
 
 - focusedCell (dict; optional)
 
@@ -49,28 +49,28 @@
 
 - pinned_top (number; default 0)
 
 - rowHeights (list; optional)
 
 - rows (list; default [{ "type": "HEADER" }, { "type": "DATA-BLOCK" }])
 
-- selectedCells (list; optional)
+- selected_cells (list; optional)
 
-- sortBy (list; optional)
+- sort_by (list; optional)
 
 - sorting (list; optional)"""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_spread_grid'
     _type = 'DashSpreadGrid'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, data=Component.UNDEFINED, columns=Component.UNDEFINED, rows=Component.UNDEFINED, formatting=Component.UNDEFINED, filtering=Component.UNDEFINED, sorting=Component.UNDEFINED, dataSelector=Component.UNDEFINED, pinned_top=Component.UNDEFINED, pinned_bottom=Component.UNDEFINED, pinned_left=Component.UNDEFINED, pinned_right=Component.UNDEFINED, borderWidth=Component.UNDEFINED, focusedCell=Component.UNDEFINED, selectedCells=Component.UNDEFINED, highlightedCells=Component.UNDEFINED, editedCells=Component.UNDEFINED, filters=Component.UNDEFINED, sortBy=Component.UNDEFINED, columnWidths=Component.UNDEFINED, rowHeights=Component.UNDEFINED, clicked_cell=Component.UNDEFINED, clicked_custom_cell=Component.UNDEFINED, active_columns=Component.UNDEFINED, active_rows=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'active_columns', 'active_rows', 'borderWidth', 'clicked_cell', 'clicked_custom_cell', 'columnWidths', 'columns', 'data', 'dataSelector', 'editedCells', 'filtering', 'filters', 'focusedCell', 'formatting', 'highlightedCells', 'pinned_bottom', 'pinned_left', 'pinned_right', 'pinned_top', 'rowHeights', 'rows', 'selectedCells', 'sortBy', 'sorting']
+    def __init__(self, id=Component.UNDEFINED, data=Component.UNDEFINED, columns=Component.UNDEFINED, rows=Component.UNDEFINED, formatting=Component.UNDEFINED, filtering=Component.UNDEFINED, sorting=Component.UNDEFINED, data_selector=Component.UNDEFINED, pinned_top=Component.UNDEFINED, pinned_bottom=Component.UNDEFINED, pinned_left=Component.UNDEFINED, pinned_right=Component.UNDEFINED, borderWidth=Component.UNDEFINED, focusedCell=Component.UNDEFINED, selected_cells=Component.UNDEFINED, highlightedCells=Component.UNDEFINED, edited_cells=Component.UNDEFINED, filters=Component.UNDEFINED, sort_by=Component.UNDEFINED, columnWidths=Component.UNDEFINED, rowHeights=Component.UNDEFINED, clicked_cell=Component.UNDEFINED, clicked_custom_cell=Component.UNDEFINED, active_columns=Component.UNDEFINED, active_rows=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'active_columns', 'active_rows', 'borderWidth', 'clicked_cell', 'clicked_custom_cell', 'columnWidths', 'columns', 'data', 'data_selector', 'edited_cells', 'filtering', 'filters', 'focusedCell', 'formatting', 'highlightedCells', 'pinned_bottom', 'pinned_left', 'pinned_right', 'pinned_top', 'rowHeights', 'rows', 'selected_cells', 'sort_by', 'sorting']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'active_columns', 'active_rows', 'borderWidth', 'clicked_cell', 'clicked_custom_cell', 'columnWidths', 'columns', 'data', 'dataSelector', 'editedCells', 'filtering', 'filters', 'focusedCell', 'formatting', 'highlightedCells', 'pinned_bottom', 'pinned_left', 'pinned_right', 'pinned_top', 'rowHeights', 'rows', 'selectedCells', 'sortBy', 'sorting']
+        self.available_properties = ['id', 'active_columns', 'active_rows', 'borderWidth', 'clicked_cell', 'clicked_custom_cell', 'columnWidths', 'columns', 'data', 'data_selector', 'edited_cells', 'filtering', 'filters', 'focusedCell', 'formatting', 'highlightedCells', 'pinned_bottom', 'pinned_left', 'pinned_right', 'pinned_top', 'rowHeights', 'rows', 'selected_cells', 'sort_by', 'sorting']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         super(DashSpreadGrid, self).__init__(**args)
```

### Comparing `dash_spread_grid-0.0.9/dash_spread_grid/__init__.py` & `dash_spread_grid-0.1.1/dash_spread_grid/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_spread_grid-0.0.9/dash_spread_grid/dash_spread_grid.min.js` & `dash_spread_grid-0.1.1/dash_spread_grid/dash_spread_grid.min.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
                 __webpack_require__.d(__webpack_exports__, {
                     Z: () => __WEBPACK_DEFAULT_EXPORT__
                 });
                 var react__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(196),
                     react__WEBPACK_IMPORTED_MODULE_0___default = __webpack_require__.n(react__WEBPACK_IMPORTED_MODULE_0__),
                     prop_types__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(64),
                     prop_types__WEBPACK_IMPORTED_MODULE_1___default = __webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_1__),
-                    js_spread_grid__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(713);
+                    js_spread_grid__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(449);
 
                 function _typeof(e) {
                     return _typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     }, _typeof(e)
@@ -26,115 +26,115 @@
                 function _nonIterableRest() {
                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }
 
                 function _unsupportedIterableToArray(e, t) {
                     if (e) {
                         if ("string" == typeof e) return _arrayLikeToArray(e, t);
-                        var o = Object.prototype.toString.call(e).slice(8, -1);
-                        return "Object" === o && e.constructor && (o = e.constructor.name), "Map" === o || "Set" === o ? Array.from(e) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? _arrayLikeToArray(e, t) : void 0
+                        var n = Object.prototype.toString.call(e).slice(8, -1);
+                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? _arrayLikeToArray(e, t) : void 0
                     }
                 }
 
                 function _arrayLikeToArray(e, t) {
                     (null == t || t > e.length) && (t = e.length);
-                    for (var o = 0, n = new Array(t); o < t; o++) n[o] = e[o];
-                    return n
+                    for (var n = 0, o = new Array(t); n < t; n++) o[n] = e[n];
+                    return o
                 }
 
                 function _iterableToArrayLimit(e, t) {
-                    var o = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
-                    if (null != o) {
-                        var n, r, i, l, s = [],
+                    var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
+                    if (null != n) {
+                        var o, r, i, l, s = [],
                             a = !0,
                             c = !1;
                         try {
-                            if (i = (o = o.call(e)).next, 0 === t) {
-                                if (Object(o) !== o) return;
+                            if (i = (n = n.call(e)).next, 0 === t) {
+                                if (Object(n) !== n) return;
                                 a = !1
                             } else
-                                for (; !(a = (n = i.call(o)).done) && (s.push(n.value), s.length !== t); a = !0);
+                                for (; !(a = (o = i.call(n)).done) && (s.push(o.value), s.length !== t); a = !0);
                         } catch (e) {
                             c = !0, r = e
                         } finally {
                             try {
-                                if (!a && null != o.return && (l = o.return(), Object(l) !== l)) return
+                                if (!a && null != n.return && (l = n.return(), Object(l) !== l)) return
                             } finally {
                                 if (c) throw r
                             }
                         }
                         return s
                     }
                 }
 
                 function _arrayWithHoles(e) {
                     if (Array.isArray(e)) return e
                 }
 
                 function ownKeys(e, t) {
-                    var o = Object.keys(e);
+                    var n = Object.keys(e);
                     if (Object.getOwnPropertySymbols) {
-                        var n = Object.getOwnPropertySymbols(e);
-                        t && (n = n.filter((function(t) {
+                        var o = Object.getOwnPropertySymbols(e);
+                        t && (o = o.filter((function(t) {
                             return Object.getOwnPropertyDescriptor(e, t).enumerable
-                        }))), o.push.apply(o, n)
+                        }))), n.push.apply(n, o)
                     }
-                    return o
+                    return n
                 }
 
                 function _objectSpread(e) {
                     for (var t = 1; t < arguments.length; t++) {
-                        var o = null != arguments[t] ? arguments[t] : {};
-                        t % 2 ? ownKeys(Object(o), !0).forEach((function(t) {
-                            _defineProperty(e, t, o[t])
-                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(o)) : ownKeys(Object(o)).forEach((function(t) {
-                            Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(o, t))
+                        var n = null != arguments[t] ? arguments[t] : {};
+                        t % 2 ? ownKeys(Object(n), !0).forEach((function(t) {
+                            _defineProperty(e, t, n[t])
+                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ownKeys(Object(n)).forEach((function(t) {
+                            Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                         }))
                     }
                     return e
                 }
 
-                function _defineProperty(e, t, o) {
+                function _defineProperty(e, t, n) {
                     return (t = _toPropertyKey(t)) in e ? Object.defineProperty(e, t, {
-                        value: o,
+                        value: n,
                         enumerable: !0,
                         configurable: !0,
                         writable: !0
-                    }) : e[t] = o, e
+                    }) : e[t] = n, e
                 }
 
                 function _toPropertyKey(e) {
                     var t = _toPrimitive(e, "string");
                     return "symbol" == _typeof(t) ? t : String(t)
                 }
 
                 function _toPrimitive(e, t) {
                     if ("object" != _typeof(e) || !e) return e;
-                    var o = e[Symbol.toPrimitive];
-                    if (void 0 !== o) {
-                        var n = o.call(e, t || "default");
-                        if ("object" != _typeof(n)) return n;
+                    var n = e[Symbol.toPrimitive];
+                    if (void 0 !== n) {
+                        var o = n.call(e, t || "default");
+                        if ("object" != _typeof(o)) return o;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }
                     return ("string" === t ? String : Number)(e)
                 }
 
                 function isString(e) {
                     return "string" == typeof e || e instanceof String
                 }
 
                 function useResolvedFormatting(formatting) {
                     return (0, react__WEBPACK_IMPORTED_MODULE_0__.useMemo)((function() {
-                        var context = "{data, rows, columns, row, column, value, newValue, text, string}";
+                        var context = "{data, rows, columns, row, column, value, newValue, text, string, ctx}";
                         return formatting.map((function(rule) {
                             var mappedRule = {};
-                            if ("column" in rule && (mappedRule.column = rule.column), "row" in rule && (mappedRule.row = rule.row), "condition" in rule && (mappedRule.condition = eval("(".concat(context, ") => (").concat(rule.condition, ")"))), "value" in rule && (mappedRule.value = eval("(".concat(context, ")=> (").concat(rule.value, ")"))), "text" in rule && (mappedRule.text = eval("(".concat(context, ") => (").concat(rule.text, ")"))), "style" in rule && (mappedRule.style = isString(rule.style) ? eval("(".concat(context, ") => (").concat(rule.style, ")")) : rule.style), "padding" in rule && (mappedRule.padding = isString(rule.padding) ? eval("(".concat(context, ") => (").concat(rule.padding, ")")) : rule.padding), "edit" in rule)
+                            if ("column" in rule && (mappedRule.column = rule.column), "row" in rule && (mappedRule.row = rule.row), "condition" in rule && (mappedRule.condition = eval("(".concat(context, ") => (").concat(rule.condition, ")"))), "value" in rule && (mappedRule.value = eval("(".concat(context, ")=> (").concat(rule.value, ")"))), "text" in rule && (mappedRule.text = eval("(".concat(context, ") => (").concat(rule.text, ")"))), "style" in rule && (mappedRule.style = isString(rule.style) ? eval("(".concat(context, ") => (").concat(rule.style, ")")) : rule.style), "padding" in rule && (mappedRule.padding = isString(rule.padding) ? eval("(".concat(context, ") => (").concat(rule.padding, ")")) : rule.padding), "draw" in rule && (mappedRule.draw = eval("(".concat(context, ") => {").concat(rule.draw, "}"))), "edit" in rule)
                                 if (rule.edit) {
                                     var mappedEdit = {};
-                                    "validate" in rule.edit && (mappedEdit.validate = eval("({string}) => (".concat(rule.edit.validate, ")"))), "parse" in rule.edit && (mappedEdit.parse = eval("(".concat(context, ") => (").concat(rule.edit.parse, ")"))), "auto_commit" in rule.edit && (mappedEdit.autoCommit = rule.edit.auto_commit), mappedRule.edit = mappedEdit
+                                    "validate" in rule.edit && (mappedEdit.validate = eval("({string}) => (".concat(rule.edit.validate, ")"))), "parse" in rule.edit && (mappedEdit.parse = eval("(".concat(context, ") => (").concat(rule.edit.parse, ")"))), "auto_commit" in rule.edit && (mappedEdit.autoCommit = rule.edit.auto_commit), "toggle" in rule.edit && (mappedEdit.toggle = rule.edit.toggle), mappedRule.edit = mappedEdit
                                 } else mappedRule.edit = rule.edit;
                             return mappedRule
                         }))
                     }), [formatting])
                 }
 
                 function useResolvedFiltering(filtering) {
@@ -143,105 +143,129 @@
                         return filtering.map((function(rule) {
                             var mappedRule = {};
                             return "column" in rule && (mappedRule.column = rule.column), "row" in rule && (mappedRule.row = rule.row), "condition" in rule && (mappedRule.condition = eval("(".concat(context, ") => (").concat(rule.condition, ")"))), mappedRule
                         }))
                     }), [filtering])
                 }
 
+                function useResolvedDataSelector(dataSelector) {
+                    return (0, react__WEBPACK_IMPORTED_MODULE_0__.useMemo)((function() {
+                        return eval("({data, row, column}) => (".concat(dataSelector, ")"))
+                    }), [dataSelector])
+                }
+
                 function DashSpreadGrid(e) {
                     console.count("render DashSpreadGrid");
                     var t = e.setProps,
-                        o = (0, react__WEBPACK_IMPORTED_MODULE_0__.useRef)(0),
-                        n = e.data,
+                        n = (0, react__WEBPACK_IMPORTED_MODULE_0__.useRef)(0),
+                        o = e.data,
                         r = e.columns,
                         i = e.rows,
                         l = useResolvedFormatting(e.formatting),
                         s = useResolvedFiltering(e.filtering),
-                        a = e.pinned_top,
-                        c = e.pinned_bottom,
-                        u = e.pinned_left,
-                        d = e.pinned_right,
-                        p = e.filters,
-                        h = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        a = useResolvedDataSelector(e.data_selector),
+                        c = e.pinned_top,
+                        u = e.pinned_bottom,
+                        d = e.pinned_left,
+                        p = e.pinned_right,
+                        f = e.filters,
+                        h = e.edited_cells,
+                        _ = e.selected_cells,
+                        m = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                            t({
+                                selected_cells: e
+                            })
+                        }), [t]),
+                        g = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 filters: e
                             })
                         }), [t]),
-                        f = e.clicked_cell,
-                        m = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        y = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                            t({
+                                edited_cells: e
+                            })
+                        }), [t]),
+                        w = e.clicked_cell,
+                        E = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 clicked_cell: _objectSpread(_objectSpread({}, e), {}, {
-                                    n: o.current++
+                                    n: n.current++
                                 })
                             })
                         }), [t]),
-                        _ = e.clicked_custom_cell,
-                        g = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        b = e.clicked_custom_cell,
+                        v = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 clicked_custom_cell: _objectSpread(_objectSpread({}, e), {}, {
-                                    n: o.current++
+                                    n: n.current++
                                 })
                             })
                         }), [t]),
-                        y = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        x = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 active_columns: e
                             })
                         }), [t]),
-                        w = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
+                        R = (0, react__WEBPACK_IMPORTED_MODULE_0__.useCallback)((function(e) {
                             t({
                                 active_rows: e
                             })
                         }), [t]),
-                        b = _slicedToArray((0, react__WEBPACK_IMPORTED_MODULE_0__.useState)(null), 2),
-                        E = b[0],
-                        v = b[1];
-                    return E && (0, js_spread_grid__WEBPACK_IMPORTED_MODULE_2__.Z)(E, {
-                        data: n,
+                        A = _slicedToArray((0, react__WEBPACK_IMPORTED_MODULE_0__.useState)(null), 2),
+                        C = A[0],
+                        k = A[1];
+                    return C && (0, js_spread_grid__WEBPACK_IMPORTED_MODULE_2__.Z)(C, {
+                        data: o,
                         columns: r,
                         rows: i,
                         formatting: l,
                         filtering: s,
-                        pinnedTop: a,
-                        pinnedBottom: c,
-                        pinnedLeft: u,
-                        pinnedRight: d,
-                        filters: p,
-                        onFiltersChange: h,
-                        clickedCell: f,
-                        onCellClick: m,
-                        clickedCustomCell: _,
-                        onCustomCellClick: g,
-                        onActiveColumnsChange: y,
-                        onActiveRowsChange: w
+                        pinnedTop: c,
+                        pinnedBottom: u,
+                        pinnedLeft: d,
+                        pinnedRight: p,
+                        filters: f,
+                        dataSelector: a,
+                        editedCells: h,
+                        selectedCells: _,
+                        onSelectedCellsChange: m,
+                        onEditedCellsChange: y,
+                        onFiltersChange: g,
+                        clickedCell: w,
+                        onCellClick: E,
+                        clickedCustomCell: b,
+                        onCustomCellClick: v,
+                        onActiveColumnsChange: x,
+                        onActiveRowsChange: R
                     }), react__WEBPACK_IMPORTED_MODULE_0___default().createElement("div", {
-                        ref: v
+                        ref: k
                     })
                 }
                 DashSpreadGrid.propTypes = {
                     setProps: prop_types__WEBPACK_IMPORTED_MODULE_1___default().func,
                     id: prop_types__WEBPACK_IMPORTED_MODULE_1___default().string,
                     data: prop_types__WEBPACK_IMPORTED_MODULE_1___default().any,
                     columns: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     rows: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     formatting: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     filtering: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     sorting: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
-                    dataSelector: prop_types__WEBPACK_IMPORTED_MODULE_1___default().string,
+                    data_selector: prop_types__WEBPACK_IMPORTED_MODULE_1___default().string,
                     pinned_top: prop_types__WEBPACK_IMPORTED_MODULE_1___default().number,
                     pinned_bottom: prop_types__WEBPACK_IMPORTED_MODULE_1___default().number,
                     pinned_left: prop_types__WEBPACK_IMPORTED_MODULE_1___default().number,
                     pinned_right: prop_types__WEBPACK_IMPORTED_MODULE_1___default().number,
                     borderWidth: prop_types__WEBPACK_IMPORTED_MODULE_1___default().number,
                     focusedCell: prop_types__WEBPACK_IMPORTED_MODULE_1___default().object,
-                    selectedCells: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
+                    selected_cells: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     highlightedCells: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
-                    editedCells: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
+                    edited_cells: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     filters: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
-                    sortBy: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
+                    sort_by: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     columnWidths: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     rowHeights: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     clicked_cell: prop_types__WEBPACK_IMPORTED_MODULE_1___default().object,
                     clicked_custom_cell: prop_types__WEBPACK_IMPORTED_MODULE_1___default().object,
                     active_columns: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array,
                     active_rows: prop_types__WEBPACK_IMPORTED_MODULE_1___default().array
                 }, DashSpreadGrid.defaultProps = {
@@ -253,26 +277,26 @@
                         type: "HEADER"
                     }, {
                         type: "DATA-BLOCK"
                     }],
                     formatting: [],
                     filtering: [],
                     sorting: [],
-                    dataSelector: "data[row.id][column.id]",
+                    data_selector: "data[row.id][column.id]",
                     pinned_top: 0,
                     pinned_bottom: 0,
                     pinned_left: 0,
                     pinned_right: 0,
                     borderWidth: 1,
                     focusedCell: null,
-                    selectedCells: [],
+                    selected_cells: [],
                     highlightedCells: [],
-                    editedCells: [],
+                    edited_cells: [],
                     filters: [],
-                    sortBy: [],
+                    sort_by: [],
                     columnWidths: [],
                     rowHeights: [],
                     clicked_cell: null,
                     clicked_custom_cell: null,
                     active_columns: [],
                     active_rows: []
                 };
@@ -280,569 +304,627 @@
             },
             64: e => {
                 e.exports = window.PropTypes
             },
             196: e => {
                 e.exports = window.React
             },
-            713: (e, t, o) => {
-                function n(e) {
-                    return null === e ? "null" : Array.isArray(e) ? `[${e.map(n).join(",")}]` : "object" == typeof e ? (t = e, `{${Object.keys(t).sort().map((e=>`${e}:${n(t[e])}`)).join(",")}}`) : JSON.stringify(e);
+            449: (e, t, n) => {
+                function o(e) {
+                    return null === e ? "null" : Array.isArray(e) ? `[${e.map(o).join(",")}]` : "object" == typeof e ? (t = e, `{${Object.keys(t).sort().map((e=>`${e}:${o(t[e])}`)).join(",")}}`) : JSON.stringify(e);
                     var t
                 }
 
                 function r(e, t) {
-                    return "FILTER" === e.type ^ "FILTER" === t.type ? "FILTER" : "DATA" === e.type && "DATA" === t.type ? "DATA" : "OTHER"
+                    return "FILTER" === e.type ^ "FILTER" === t.type ? "FILTER" : "DATA"
                 }
 
-                function i(e, t, o, i) {
+                function i(e, t, n, i) {
                     return e.map((e => {
-                        const l = n(e.columnId),
-                            s = n(e.rowId);
-                        if (!o.has(l)) return null;
+                        const l = o(e.columnId),
+                            s = o(e.rowId);
+                        if (!n.has(l)) return null;
                         if (!i.has(s)) return null;
-                        const a = o.get(l),
+                        const a = n.get(l),
                             c = i.get(s);
                         return {
                             edit: t.resolve(c, a).edit,
                             cell: e,
                             type: r(a, c)
                         }
                     })).filter((e => e?.edit))
                 }
-                o.d(t, {
-                    Z: () => We
-                });
-                const l = "12px Calibri",
-                    s = {
-                        top: 2,
-                        right: 5,
-                        bottom: 2,
-                        left: 5
-                    };
 
-                function a(e, t) {
+                function l(e, t) {
                     return Math.round(e * t) / t
                 }
 
-                function c(e, t, o) {
-                    const n = e.state,
-                        r = e.canvases[`${t}-${o}`],
-                        i = n.sections[t],
-                        s = n.sections[o],
-                        c = s.columns,
-                        u = i.rows;
-                    if (0 === u.length || 0 === c.length) return void(r.parentElement && r.parentElement.removeChild(r));
+                function s(e, t, n) {
+                    const o = e.state,
+                        r = e.canvases[`${t}-${n}`],
+                        i = o.sections[t],
+                        s = o.sections[n],
+                        a = s.columns,
+                        c = i.rows;
+                    if (0 === c.length || 0 === a.length) return void(r.parentElement && r.parentElement.removeChild(r));
                     r.parentElement || e.element.appendChild(r), console.log("draw");
-                    const d = r.getContext("2d", {
+                    const u = r.getContext("2d", {
                             alpha: !1
                         }),
-                        p = n.scrollRect,
-                        h = n.textResolver,
-                        f = n.renderFormatResolver,
-                        m = n.borderWidth,
+                        d = o.scrollRect,
+                        p = o.textResolver,
+                        f = o.renderFormatResolver,
+                        h = o.borderWidth,
                         _ = i.showTopBorder,
-                        g = i.showBottomBorder,
-                        y = s.showLeftBorder,
-                        w = s.showRightBorder,
-                        b = m / 2,
-                        E = u.length - 1 + (_ ? 1 : 0) + (g ? 1 : 0),
-                        v = c.length - 1 + (y ? 1 : 0) + (w ? 1 : 0),
-                        x = u.map((e => e.height)),
-                        R = c.map((e => e.width)),
-                        C = R.reduce(((e, t) => e + t), 0) + v * m,
-                        A = x.reduce(((e, t) => e + t), 0) + E * m,
-                        k = "center" === o ? p.left : 0,
-                        I = "middle" === t ? p.top : 0,
-                        D = "center" === o ? p.width : s.width,
-                        M = "middle" === t ? p.height : i.height,
-                        T = R.reduce(((e, t, o) => {
-                            const n = e[o] + t + m;
-                            return e.push(n), e
-                        }), [y ? m : 0]),
-                        O = x.reduce(((e, t, o) => {
-                            const n = e[o] + t + m;
-                            return e.push(n), e
-                        }), [_ ? m : 0]),
-                        L = T.slice(0, -1),
-                        P = O.slice(0, -1),
-                        B = Math.max(L.findLastIndex((e => e <= k)), 0),
-                        S = L.findLastIndex((e => e <= k + D)),
-                        K = Math.max(P.findLastIndex((e => e <= I)), 0),
-                        W = P.findLastIndex((e => e <= I + M)),
-                        F = Math.max(B, y ? 0 : 1),
-                        N = S + (w ? 1 : 0),
-                        z = Math.max(K, _ ? 0 : 1),
-                        U = W + (g ? 1 : 0),
-                        j = Array.from({
-                            length: W - K + 1
+                        m = i.showBottomBorder,
+                        g = s.showLeftBorder,
+                        y = s.showRightBorder,
+                        w = h / 2,
+                        E = c.length - 1 + (_ ? 1 : 0) + (m ? 1 : 0),
+                        b = a.length - 1 + (g ? 1 : 0) + (y ? 1 : 0),
+                        v = c.map((e => e.height)),
+                        x = a.map((e => e.width)),
+                        R = x.reduce(((e, t) => e + t), 0) + b * h,
+                        A = v.reduce(((e, t) => e + t), 0) + E * h,
+                        C = "center" === n ? d.left : 0,
+                        k = "middle" === t ? d.top : 0,
+                        I = "center" === n ? d.width : s.width,
+                        D = "middle" === t ? d.height : i.height,
+                        T = x.reduce(((e, t, n) => {
+                            const o = e[n] + t + h;
+                            return e.push(o), e
+                        }), [g ? h : 0]),
+                        M = v.reduce(((e, t, n) => {
+                            const o = e[n] + t + h;
+                            return e.push(o), e
+                        }), [_ ? h : 0]),
+                        O = T.slice(0, -1),
+                        L = M.slice(0, -1),
+                        P = Math.max(O.findLastIndex((e => e <= C)), 0),
+                        B = O.findLastIndex((e => e <= C + I)),
+                        S = Math.max(L.findLastIndex((e => e <= k)), 0),
+                        K = L.findLastIndex((e => e <= k + D)),
+                        W = Math.max(P, g ? 0 : 1),
+                        F = B + (y ? 1 : 0),
+                        z = Math.max(S, _ ? 0 : 1),
+                        U = K + (m ? 1 : 0),
+                        N = Array.from({
+                            length: K - S + 1
                         }, ((e, t) => {
-                            const o = u[t + K];
+                            const n = c[t + S];
                             return Array.from({
-                                length: S - B + 1
+                                length: B - P + 1
                             }, ((e, t) => {
-                                const n = c[t + B];
-                                return f.resolve(o, n)
+                                const o = a[t + P];
+                                return f.resolve(n, o)
                             }))
                         })),
-                        H = (e, t) => j[e - K][t - B];
-                    r.width = Math.round(D * devicePixelRatio), r.height = Math.round(M * devicePixelRatio), r.style.width = `${D}px`, r.style.height = `${M}px`, r.style.marginLeft = `${k}px`, r.style.marginTop = `${I}px`, r.style.marginRight = C - D - k + "px", r.style.marginBottom = A - M - I + "px", d.fillStyle = "#E9E9E9", d.fillRect(0, 0, r.width, r.height);
-                    const q = (e, t) => {
-                            d.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (e - k) * devicePixelRatio, (t - I) * devicePixelRatio)
+                        j = (e, t) => N[e - S][t - P];
+                    r.width = Math.round(I * devicePixelRatio), r.height = Math.round(D * devicePixelRatio), r.style.width = `${I}px`, r.style.height = `${D}px`, r.style.marginLeft = `${C}px`, r.style.marginTop = `${k}px`, r.style.marginRight = R - I - C + "px", r.style.marginBottom = A - D - k + "px", u.fillStyle = "#E9E9E9", u.fillRect(0, 0, r.width, r.height);
+                    const H = (e, t) => {
+                            u.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (e - C) * devicePixelRatio, (t - k) * devicePixelRatio)
                         },
-                        $ = (e, t, o, n) => {
-                            d.beginPath(), d.rect(e, t, o, n), d.clip()
+                        q = (e, t, n, o) => {
+                            u.beginPath(), u.rect(e, t, n, o), u.clip()
                         };
-                    for (let e = B; e <= S; e++) {
-                        d.save(), q(T[e], 0), $(0, 0, R[e], A);
-                        for (let t = K; t <= W; t++) {
-                            const o = H(t, e),
-                                n = o.style,
-                                r = O[t],
+                    for (let e = P; e <= B; e++) {
+                        u.save(), H(T[e], 0), q(0, 0, x[e], A);
+                        for (let t = S; t <= K; t++) {
+                            const n = j(t, e),
+                                o = n.style,
+                                r = M[t],
                                 i = T[e],
-                                s = R[e],
-                                c = x[t],
-                                u = o.text,
-                                p = n.textAlign || "left",
-                                f = n.textBaseline || "middle",
-                                _ = o.padding;
-                            q(i, r), d.fillStyle = n.background || "white", d.fillRect(0, 0, s, c), "draw" in o && o.draw(d), n.highlight && (d.fillStyle = n.highlight, d.fillRect(0, 0, s, c)), n.corner && (d.fillStyle = n.corner, d.beginPath(), d.moveTo(s - 7, c), d.lineTo(s, c), d.lineTo(s, c - 7), d.fill()), d.fillStyle = n.foreground || "black", d.font = n.font || l, d.textAlign = p;
-                            const g = h.getFontMetrics(n.font),
-                                y = a("left" === p ? _.left : "center" === p ? s / 2 : "right" === p ? s - _.right : 0, devicePixelRatio),
-                                w = a("top" === f ? g.middle + g.topOffset + _.top : "middle" === f ? c / 2 + g.middle : "bottom" === f ? c + g.middle - g.bottomOffset - _.bottom : 0, devicePixelRatio);
-                            w - g.middle - g.topOffset >= 0 && w - g.middle + g.bottomOffset <= c ? d.fillText(u, y, w) : (d.strokeStyle = "#E9E9E9", d.lineWidth = m, d.beginPath(), d.moveTo(0, m + b), d.lineTo(s, m + b), d.moveTo(0, c - m - b), d.lineTo(s, c - m - b), d.stroke(), d.save(), $(0, 2 * m, s, c - 4 * m), d.fillText(u, y, w), d.restore())
+                                s = x[e],
+                                a = v[t],
+                                c = n.text,
+                                d = o.textBaseline || "middle",
+                                f = n.padding;
+                            if (H(i, r), u.fillStyle = o.background || "white", u.fillRect(0, 0, s, a), "draw" in n && n.draw(u), o.highlight && (u.fillStyle = o.highlight, u.fillRect(0, 0, s, a)), o.corner && (u.fillStyle = o.corner, u.beginPath(), u.moveTo(s - 7, a), u.lineTo(s, a), u.lineTo(s, a - 7), u.fill()), c) {
+                                u.fillStyle = o.foreground || "black", u.font = n.font;
+                                const e = p.getFontMetrics(n.font),
+                                    t = "center" == o.textAlign && p.measureWidth(c, n.font) > s - f.left - f.right ? "left" : o.textAlign || "left";
+                                u.textAlign = t;
+                                const r = l("left" === t ? f.left : "center" === t ? s / 2 : "right" === t ? s - f.right : 0, devicePixelRatio),
+                                    i = l("top" === d ? e.middle + e.topOffset + f.top : "middle" === d ? a / 2 + e.middle : "bottom" === d ? a + e.middle - e.bottomOffset - f.bottom : 0, devicePixelRatio);
+                                i - e.middle - e.topOffset >= 0 && i - e.middle + e.bottomOffset <= a ? u.fillText(c, r, i) : (u.strokeStyle = "#E9E9E9", u.lineWidth = h, u.beginPath(), u.moveTo(0, h + w), u.lineTo(s, h + w), u.moveTo(0, a - h - w), u.lineTo(s, a - h - w), u.stroke(), u.save(), q(0, 2 * h, s, a - 4 * h), u.fillText(c, r, i), u.restore())
+                            }
                         }
-                        d.restore()
+                        u.restore()
                     }
-                    q(0, 0);
-                    const V = (e, t, o, n, r) => {
+                    H(0, 0);
+                    const $ = (e, t, n, o, r) => {
                             if (!r) return;
-                            const i = r.width * m,
-                                l = t === n,
+                            if (0 === r.width) return;
+                            const i = r.width / devicePixelRatio,
+                                l = t === o,
                                 s = e - (l ? i / 2 : 0),
                                 a = t - (l ? 0 : i / 2),
-                                c = o + (l ? i / 2 : 0),
-                                u = n + (l ? 0 : i / 2);
-                            d.strokeStyle = r.color || "black", d.lineWidth = i, r.dash ? (d.setLineDash(r.dash.map((e => e / devicePixelRatio))), d.lineDashOffset = l ? s : a) : d.setLineDash([]), d.beginPath(), d.moveTo(s, a), d.lineTo(c, u), d.stroke()
+                                c = n + (l ? i / 2 : 0),
+                                d = o + (l ? 0 : i / 2);
+                            u.strokeStyle = r.color || "black", u.lineWidth = i, r.dash ? (u.setLineDash(r.dash.map((e => e / devicePixelRatio))), u.lineDashOffset = l ? s : a) : u.setLineDash([]), u.beginPath(), u.moveTo(s, a), u.lineTo(c, d), u.stroke()
                         },
-                        G = (e, t) => e ? t ? e.index > t.index ? e : t : e : t;
+                        V = (e, t) => e ? t ? e.index > t.index ? e : t : e : t;
                     for (let e = z; e <= U; e++) {
                         const t = e - 1,
-                            o = e;
-                        for (let e = B; e <= S; e++) {
-                            const n = G(t >= K ? H(t, e).style.borderBottom : null, o <= W ? H(o, e).style.borderTop : null);
-                            V(T[e] - b, O[o] - b, T[e + 1] - b, O[o] - b, n)
+                            n = e;
+                        for (let e = P; e <= B; e++) {
+                            const o = V(t >= S ? j(t, e).style.borderBottom : null, n <= K ? j(n, e).style.borderTop : null);
+                            $(T[e] - w, M[n] - w, T[e + 1] - w, M[n] - w, o)
                         }
                     }
-                    for (let e = F; e <= N; e++) {
+                    for (let e = W; e <= F; e++) {
                         const t = e - 1,
-                            o = e;
-                        for (let e = K; e <= W; e++) {
-                            const n = G(t >= B ? H(e, t).style.borderRight : null, o <= S ? H(e, o).style.borderLeft : null);
-                            V(T[o] - b, O[e] - b, T[o] - b, O[e + 1] - b, n)
+                            n = e;
+                        for (let e = S; e <= K; e++) {
+                            const o = V(t >= P ? j(e, t).style.borderRight : null, n <= B ? j(e, n).style.borderLeft : null);
+                            $(T[n] - w, M[e] - w, T[n] - w, M[e + 1] - w, o)
                         }
                     }
                 }
 
-                function u(e) {
+                function a(e) {
                     if (!e.error) try {
                         ! function(e) {
-                            c(e, "top", "left"), c(e, "top", "center"), c(e, "top", "right"), c(e, "middle", "left"), c(e, "middle", "center"), c(e, "middle", "right"), c(e, "bottom", "left"), c(e, "bottom", "center"), c(e, "bottom", "right"),
+                            s(e, "top", "left"), s(e, "top", "center"), s(e, "top", "right"), s(e, "middle", "left"), s(e, "middle", "center"), s(e, "middle", "right"), s(e, "bottom", "left"), s(e, "bottom", "center"), s(e, "bottom", "right"),
                                 function(e) {
                                     const t = e.element,
-                                        o = e.input,
-                                        n = e.state,
-                                        r = n.inputPlacement;
+                                        n = e.input,
+                                        o = e.state,
+                                        r = o.inputPlacement;
                                     if (!r) {
-                                        if (o.parentElement) {
-                                            const e = document.activeElement === o;
-                                            o.parentElement.removeChild(o), e && t.focus({
+                                        if (n.parentElement) {
+                                            const e = document.activeElement === n;
+                                            n.parentElement.removeChild(n), e && t.focus({
                                                 preventScroll: !0
                                             })
                                         }
                                         return
                                     }
                                     const i = e.canvases[r.section];
-                                    if (o.style.left = "left" in r ? `${r.left}px` : "0", o.style.top = "top" in r ? `${r.top}px` : "0", o.style.right = "right" in r ? `${r.right}px` : "0", o.style.bottom = "bottom" in r ? `${r.bottom}px` : "0", o.style.marginLeft = "marginLeft" in r ? `${r.marginLeft}px` : "0", o.style.marginTop = "marginTop" in r ? `${r.marginTop}px` : "0", o.style.width = `${r.width}px`, o.style.height = `${r.height}px`, o.style.gridArea = i.style.gridArea, o.style.zIndex = i.style.zIndex, o.style.backgroundColor = n.isTextValid ? "white" : "#eb3434", !o.parentElement) {
+                                    if (n.style.left = "left" in r ? `${r.left}px` : "0", n.style.top = "top" in r ? `${r.top}px` : "0", n.style.right = "right" in r ? `${r.right}px` : "0", n.style.bottom = "bottom" in r ? `${r.bottom}px` : "0", n.style.marginLeft = "marginLeft" in r ? `${r.marginLeft}px` : "0", n.style.marginTop = "marginTop" in r ? `${r.marginTop}px` : "0", n.style.width = `${r.width}px`, n.style.height = `${r.height}px`, n.style.gridArea = i.style.gridArea, n.style.zIndex = i.style.zIndex, n.style.backgroundColor = o.isTextValid ? "white" : "#eb3434", !n.parentElement) {
                                         const e = document.activeElement === t;
-                                        t.appendChild(o), e && o.focus({
+                                        t.appendChild(n), e && n.focus({
                                             preventScroll: !0
                                         })
                                     }
                                 }(e),
                                 function(e) {
                                     const t = e.element,
-                                        o = e.state;
-                                    o.resizableColumn && o.resizableRow ? t.style.cursor = "nwse-resize" : o.resizableColumn ? t.style.cursor = "col-resize" : o.resizableRow ? t.style.cursor = "row-resize" : t.style.cursor = "default"
+                                        n = e.state;
+                                    n.resizableColumn && n.resizableRow ? t.style.cursor = "nwse-resize" : n.resizableColumn ? t.style.cursor = "col-resize" : n.resizableRow ? t.style.cursor = "row-resize" : t.style.cursor = "default"
                                 }(e)
                         }(e)
                     } catch (t) {
                         e.error = t
                     }
                     e.error && function(e) {
+                        if (e.errorRendered) return;
+                        e.errorRendered = !0;
                         const t = e.element,
-                            o = e.error;
-                        t.style.backgroundColor = "#9f0000", t.style.color = "white", t.style.padding = "20px", t.style.display = "flex", t.style.flexDirection = "column", t.innerHTML = `\n        <div style="font-size: 16px;">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style="font-size: 20px; font-weight: bold; padding: 20px 0;">\n            ${o.message}\n        </div>\n        <div style="font-size: 16px; white-space: pre-wrap;">${o.stack}</div>\n    `
+                            n = e.error;
+                        t.style.backgroundColor = "#9f0000", t.style.color = "white", t.style.padding = "20px", t.style.display = "flex", t.style.flexDirection = "column", t.style.userSelect = "text", t.innerHTML = `\n        <div style="font-size: 16px;">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style="font-size: 20px; font-weight: bold; padding: 20px 0;">\n            ${n.message}\n        </div>\n        <div style="font-size: 16px; white-space: pre-wrap;">${n.stack}</div>\n    `
                     }(e)
                 }
+                n.d(t, {
+                    Z: () => qe
+                });
+                const c = {
+                    value: ({
+                        newValue: e
+                    }) => e || "",
+                    text: ({
+                        newValue: e
+                    }) => e || "Search...",
+                    edit: {
+                        validate: () => !0,
+                        parse: ({
+                            string: e
+                        }) => e,
+                        autoCommit: !0
+                    }
+                };
 
-                function d(e, t, o) {
+                function u(e, t, n) {
                     return [{
                         column: {
-                            match: "DATA"
+                            type: "DATA"
                         },
                         row: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         value: ({
                             column: e
                         }) => void 0 === e.header ? e.id : e.header
                     }, {
                         column: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         row: {
-                            match: "DATA"
+                            type: "DATA"
                         },
                         value: ({
                             row: e
                         }) => void 0 === e.header ? e.id : e.header
                     }, {
                         column: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         row: {
-                            match: "SPECIAL"
+                            type: "SPECIAL"
                         },
                         value: ""
                     }, {
                         column: {
-                            match: "SPECIAL"
+                            type: "SPECIAL"
                         },
                         row: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         value: ""
-                    }, ...o.map((({
-                        columnId: e,
-                        rowId: t,
-                        direction: n
-                    }, r) => ({
+                    }, {
                         column: {
-                            id: e
+                            type: "DATA"
                         },
                         row: {
-                            id: t
+                            type: "FILTER"
                         },
-                        text: ({
-                            column: e
-                        }) => `${o.length>1?r+1:""}${"ASC"===n?"⇣":"⇡"} ${e.header}`
-                    }))), {
+                        ...c
+                    }, {
                         column: {
-                            match: "ANY"
+                            type: "FILTER"
                         },
                         row: {
-                            match: "FILTER"
+                            type: "DATA"
                         },
-                        value: ({
-                            newValue: e
-                        }) => e || "",
-                        text: ({
-                            newValue: e
-                        }) => e || "Search...",
-                        edit: {
-                            validate: () => !0,
-                            parse: ({
-                                string: e
-                            }) => e,
-                            autoCommit: !0
-                        }
+                        ...c
                     }, {
                         column: {
-                            match: "DATA"
+                            type: "DATA"
                         },
                         row: {
-                            match: "DATA"
+                            type: "DATA"
                         },
                         value: t
-                    }, ...e]
+                    }, ...e, ...n.map((({
+                        columnId: e,
+                        rowId: t,
+                        direction: o
+                    }, r) => ({
+                        column: {
+                            id: e
+                        },
+                        row: {
+                            id: t
+                        },
+                        text: ({
+                            value: e,
+                            text: t
+                        }) => `${n.length>1?r+1:""}${"ASC"===o?"⇣":"⇡"} ${t||e}`
+                    })))]
                 }
+                const d = ["column", "row", "condition"];
 
                 function p(e) {
-                    return e
+                    return Object.keys(e).length > Object.keys(e).filter((e => d.includes(e))).length
                 }
 
-                function h(e, t) {
+                function f(e, t) {
+                    const n = [...d, ...t];
+                    return e.map((e => function(e, t) {
+                        const n = {};
+                        for (const o of t) o in e && (n[o] = e[o]);
+                        return n
+                    }(e, n))).filter(p)
+                }
+
+                function h(e) {
+                    return f(e, ["value", "text", "edit"])
+                }
+
+                function _(e, t) {
                     return t ? e + "99" : e + "33"
                 }
 
-                function f(e, t, o, r, i, l, s, a) {
-                    const c = o ? n(o.columnId) : null,
-                        u = o ? n(o.rowId) : null,
-                        d = null !== a,
-                        p = null !== s || d,
-                        f = (e, t, o, n) => {
-                            if (o < 0 || o >= e.length) return !1;
-                            if (n < 0 || n >= t.length) return !1;
-                            const i = e[o].key,
-                                l = t[n].key;
+                function m(e, t, n, r, i, l, s, a, c, u) {
+                    const d = n ? o(n.columnId) : null,
+                        p = n ? o(n.rowId) : null,
+                        f = null !== c,
+                        h = null !== a || f,
+                        m = u + 2,
+                        g = u + 4,
+                        y = (e, t, n, o) => {
+                            if (n < 0 || n >= e.length) return !1;
+                            if (o < 0 || o >= t.length) return !1;
+                            const i = e[n].key,
+                                l = t[o].key;
                             return r.isKeySelected(i, l)
                         },
-                        m = (e, t) => e ? [t] : [];
+                        w = (e, t) => e ? [t] : [];
                     return [{
                         column: {
-                            match: "ANY"
+                            type: "DATA"
+                        },
+                        row: {
+                            type: "FILTER"
+                        },
+                        style: ({
+                            newValue: e
+                        }) => ({
+                            background: "#FBFBFB",
+                            foreground: e ? "black" : "#cccccc",
+                            border: {
+                                width: 1,
+                                color: "gray"
+                            }
+                        })
+                    }, {
+                        column: {
+                            type: "FILTER"
                         },
                         row: {
-                            match: "FILTER"
+                            type: "DATA"
                         },
                         style: ({
                             newValue: e
                         }) => ({
                             background: "#FBFBFB",
                             foreground: e ? "black" : "#cccccc",
                             border: {
                                 width: 1,
                                 color: "gray"
                             }
                         })
                     }, {
                         column: {
-                            match: "ANY"
+                            type: "ANY"
                         },
                         row: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         style: {
                             background: "#F5F5F5",
                             border: {
-                                width: 1,
+                                width: u,
                                 color: "gray"
                             }
                         }
                     }, {
                         column: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         row: {
-                            match: "ANY"
+                            type: "ANY"
                         },
                         style: {
                             background: "#F5F5F5",
                             border: {
-                                width: 1,
+                                width: u,
                                 color: "gray"
                             }
                         }
                     }, {
                         column: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         row: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         style: {
                             background: "#E0E0E0"
                         }
-                    }, ...e, ...m(t && !d, {
+                    }, ...e, ...w(t && !f, {
                         column: {
-                            match: "ANY"
+                            type: "ANY"
                         },
                         row: {
                             id: t?.rowId
                         },
                         style: {
                             highlight: "#81948133"
                         }
-                    }), ...m(t && !p, {
+                    }), ...w(t && !h, {
                         column: {
                             id: t?.columnId
                         },
                         row: {
                             id: t?.rowId
                         },
                         style: {
                             highlight: "#81948188"
                         }
                     }), {
                         column: {
-                            match: "ANY"
+                            type: "ANY"
                         },
                         row: {
-                            match: "ANY"
+                            type: "ANY"
                         },
                         condition: ({
                             rows: e,
                             columns: t,
-                            row: o,
-                            column: n
-                        }) => f(e, t, o.index, n.index),
+                            row: n,
+                            column: o
+                        }) => y(e, t, n.index, o.index),
                         style: ({
                             rows: e,
                             columns: t,
-                            row: o,
-                            column: n,
+                            row: n,
+                            column: o,
                             edit: r
                         }) => ({
-                            ...f(e, t, o.index - 1, n.index) ? {} : {
+                            ...y(e, t, n.index - 1, o.index) ? {} : {
                                 borderTop: {
-                                    width: 3,
+                                    width: m,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            ...f(e, t, o.index + 1, n.index) ? {} : {
+                            ...y(e, t, n.index + 1, o.index) ? {} : {
                                 borderBottom: {
-                                    width: 3,
+                                    width: m,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            ...f(e, t, o.index, n.index - 1) ? {} : {
+                            ...y(e, t, n.index, o.index - 1) ? {} : {
                                 borderLeft: {
-                                    width: 3,
+                                    width: m,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            ...f(e, t, o.index, n.index + 1) ? {} : {
+                            ...y(e, t, n.index, o.index + 1) ? {} : {
                                 borderRight: {
-                                    width: 3,
+                                    width: m,
                                     color: "#596959",
                                     index: Number.MAX_SAFE_INTEGER
                                 }
                             },
-                            highlight: h(r ? "#798d9c" : "#819481", c !== n.key || u !== o.key)
+                            highlight: _(r ? "#798d9c" : "#819481", d !== o.key || p !== n.key)
                         })
                     }, {
                         column: {
-                            match: "ANY"
+                            type: "ANY"
                         },
                         row: {
-                            match: "ANY"
+                            type: "ANY"
                         },
                         condition: ({
                             row: e,
                             column: t
                         }) => i.isKeySelected(e.key, t.key),
                         style: ({
                             row: e,
                             column: t
                         }) => ({
-                            highlight: h("#93a8b8", c !== t.key || u !== e.key)
+                            highlight: _("#93a8b8", d !== t.key || p !== e.key)
                         })
-                    }, ...m(o, {
+                    }, ...w(n, {
                         column: {
-                            id: o?.columnId
+                            id: n?.columnId
                         },
                         row: {
-                            id: o?.rowId
+                            id: n?.rowId
                         },
                         style: {
                             highlight: "#ffffffaa"
                         }
-                    }), {
+                    }), ...s.map((({
+                        columnId: e,
+                        rowId: t,
+                        direction: n
+                    }, o) => ({
                         column: {
-                            match: "ANY"
+                            id: e
                         },
                         row: {
-                            match: "ANY"
+                            id: t
+                        },
+                        style: {
+                            highlight: "#0377fc44"
+                        }
+                    }))), {
+                        column: {
+                            type: "ANY"
+                        },
+                        row: {
+                            type: "ANY"
                         },
                         condition: ({
                             edit: e
                         }) => e,
                         style: {
                             corner: "#77777720"
                         }
                     }, {
                         column: {
-                            match: "ANY"
+                            type: "ANY"
                         },
                         row: {
-                            match: "ANY"
+                            type: "ANY"
                         },
                         condition: ({
                             row: e,
                             column: t
                         }) => l.hasValueByKey(e.key, t.key),
                         style: {
                             corner: "darkgreen"
                         }
-                    }, ...m(s, {
+                    }, ...w(a, {
                         column: {
-                            id: s
+                            id: a
                         },
                         row: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         style: {
                             borderRight: {
-                                width: 5,
+                                width: g,
                                 color: "cornflowerblue"
                             }
                         }
-                    }), ...m(a, {
+                    }), ...w(c, {
                         column: {
-                            match: "HEADER"
+                            type: "HEADER"
                         },
                         row: {
-                            id: a
+                            id: c
                         },
                         style: {
                             borderBottom: {
-                                width: 5,
+                                width: g,
                                 color: "cornflowerblue"
                             }
                         }
                     })]
                 }
 
-                function m(e, t) {
-                    const o = t.filter((e => "BEGIN" === e.pinned)).length,
-                        n = t.filter((e => "END" === e.pinned)).length,
-                        r = t.length - o - n,
+                function g(e, t) {
+                    const n = t.filter((e => "BEGIN" === e.pinned)).length,
+                        o = t.filter((e => "END" === e.pinned)).length,
+                        r = t.length - n - o,
                         i = e.filter((e => "BEGIN" === e.pinned)).length,
                         l = e.filter((e => "END" === e.pinned)).length,
                         s = e.length - i - l,
-                        a = t.slice(0, o),
-                        c = t.slice(t.length - n, t.length),
-                        u = t.slice(o, t.length - n),
+                        a = t.slice(0, n),
+                        c = t.slice(t.length - o, t.length),
+                        u = t.slice(n, t.length - o),
                         d = e.slice(0, i),
                         p = e.slice(e.length - l, e.length),
-                        h = e.slice(i, e.length - l),
-                        f = o > 0,
-                        m = i > 0,
-                        _ = r > 0 || !f,
-                        g = !f,
-                        y = !(n > 0),
-                        w = s > 0 || !m,
-                        b = !m,
-                        E = !(l > 0),
-                        v = (e, t, o) => {
+                        f = e.slice(i, e.length - l),
+                        h = n > 0,
+                        _ = i > 0,
+                        m = r > 0 || !h,
+                        g = !h,
+                        y = !(o > 0),
+                        w = s > 0 || !_,
+                        E = !_,
+                        b = !(l > 0),
+                        v = (e, t, n) => {
                             if (0 === e.length) return 0;
-                            const n = t ? e.at(0).topWithBorder : e.at(0).top;
-                            return (o ? e.at(-1).bottomWithBorder : e.at(-1).bottom) - n
+                            const o = t ? e.at(0).topWithBorder : e.at(0).top;
+                            return (n ? e.at(-1).bottomWithBorder : e.at(-1).bottom) - o
                         },
-                        x = (e, t, o) => {
+                        x = (e, t, n) => {
                             if (0 === e.length) return 0;
-                            const n = t ? e.at(0).leftWithBorder : e.at(0).left;
-                            return (o ? e.at(-1).rightWithBorder : e.at(-1).right) - n
+                            const o = t ? e.at(0).leftWithBorder : e.at(0).left;
+                            return (n ? e.at(-1).rightWithBorder : e.at(-1).right) - o
                         };
                     return {
                         top: {
                             rows: a,
                             showTopBorder: !0,
                             showBottomBorder: !0,
                             height: v(a, !0, !0)
                         },
                         bottom: {
                             rows: c,
-                            showTopBorder: _,
+                            showTopBorder: m,
                             showBottomBorder: !0,
-                            height: v(c, _, !0)
+                            height: v(c, m, !0)
                         },
                         middle: {
                             rows: u,
                             showTopBorder: g,
                             showBottomBorder: y,
                             height: v(u, g, y)
                         },
@@ -855,503 +937,532 @@
                         right: {
                             columns: p,
                             showLeftBorder: w,
                             showRightBorder: !0,
                             width: x(p, w, !0)
                         },
                         center: {
-                            columns: h,
-                            showLeftBorder: b,
-                            showRightBorder: E,
-                            width: x(h, b, E)
+                            columns: f,
+                            showLeftBorder: E,
+                            showRightBorder: b,
+                            width: x(f, E, b)
                         }
                     }
                 }
 
-                function _(e, t) {
+                function y(e, t) {
                     return [...e, ...t.map((e => ({
                         columnId: e.columnId,
                         rowId: e.rowId,
                         value: e.expression
                     })))]
                 }
-                class g {
+                class w {
                     constructor(e) {
                         this.lookup = new Map, e.forEach((e => {
-                            const t = n(e.rowId),
-                                o = n(e.columnId);
-                            this.lookup.has(t) || this.lookup.set(t, new Map), this.lookup.get(t).set(o, e.value)
+                            const t = o(e.rowId),
+                                n = o(e.columnId);
+                            this.lookup.has(t) || this.lookup.set(t, new Map), this.lookup.get(t).set(n, e.value)
                         }))
                     }
                     hasValueByKey(e, t) {
                         return this.lookup.has(e) && this.lookup.get(e).has(t)
                     }
                     getValueByKey(e, t) {
                         if (this.hasValueByKey(e, t)) return this.lookup.get(e).get(t)
                     }
                     hasValueById(e, t) {
-                        return this.hasValueByKey(n(e), n(t))
+                        return this.hasValueByKey(o(e), o(t))
                     }
                     getValueById(e, t) {
-                        return this.getValueByKey(n(e), n(t))
+                        return this.getValueByKey(o(e), o(t))
                     }
                 }
 
-                function y(e) {
-                    return new g(e)
+                function E(e) {
+                    return new w(e)
                 }
-                class w {
+                class b {
                     constructor(e) {
                         this.lookup = new Map, e.forEach((e => {
-                            const t = n(e.rowId),
-                                o = n(e.columnId);
-                            this.lookup.has(t) || this.lookup.set(t, new Set), this.lookup.get(t).add(o)
+                            const t = o(e.rowId),
+                                n = o(e.columnId);
+                            this.lookup.has(t) || this.lookup.set(t, new Set), this.lookup.get(t).add(n)
                         }))
                     }
                     isKeySelected(e, t) {
                         return this.lookup.has(e) && this.lookup.get(e).has(t)
                     }
                     isIdSelected(e, t) {
-                        return this.isKeySelected(n(e), n(t))
+                        return this.isKeySelected(o(e), o(t))
                     }
                 }
 
-                function b(e) {
-                    return new w(e)
+                function v(e) {
+                    return new b(e)
                 }
 
-                function E(e, t) {
+                function x(e, t) {
                     return "function" == typeof e ? e(t) : e
                 }
 
-                function v(e, t, o, n) {
-                    return e < o ? "BEGIN" : e >= t - n ? "END" : void 0
+                function R(e, t, n, o) {
+                    return e < n ? "BEGIN" : e >= t - o ? "END" : void 0
                 }
 
-                function x(e, t, o) {
+                function A(e, t, n) {
                     return e.map(((r, i) => {
                         const l = "id" in r ? r.id : r.type;
                         return {
                             ...r,
                             id: l,
                             type: r.type || "DATA",
                             index: i,
-                            key: n(l),
-                            pinned: v(i, e.length, t, o),
+                            key: o(l),
+                            pinned: R(i, e.length, t, n),
                             header: "header" in r ? r.header : l,
                             labels: r.labels || []
                         }
                     }))
                 }
 
-                function R(e, t, o, r) {
+                function C(e, t, n, r) {
                     const i = new Map(r.map((({
                         columnId: e,
                         width: t
-                    }) => [n(e), t])));
-                    return x(e, t, o).map((e => ({
+                    }) => [o(e), t])));
+                    return A(e, t, n).map((e => ({
                         ...e,
-                        width: i.has(e.key) ? i.get(e.key) : e.width
+                        width: i.has(e.key) ? i.get(e.key) : "width" in e ? e.width : "fit"
                     })))
                 }
 
-                function C(e, t, o, r) {
+                function k(e, t, n, r) {
                     const i = new Map(r.map((({
                         rowId: e,
                         height: t
-                    }) => [n(e), t])));
-                    return x(e, t, o).map((e => ({
+                    }) => [o(e), t])));
+                    return A(e, t, n).map((e => ({
                         ...e,
-                        height: i.has(e.key) ? i.get(e.key) : e.height
+                        height: i.has(e.key) ? i.get(e.key) : "height" in e ? e.height : "fit"
                     })))
                 }
 
-                function A(e, t, o) {
-                    let n = o;
+                function I(e, t, n) {
+                    let o = n;
                     return e.map(((e, r) => {
-                        const i = a("width" in e ? e.width : 100, t),
-                            l = {
+                        const i = l("width" in e ? e.width : 100, t),
+                            s = {
                                 ...e,
                                 index: r,
                                 width: i,
-                                leftWithBorder: n - o,
-                                left: n,
-                                right: n + i,
-                                rightWithBorder: n + i + o
+                                leftWithBorder: o - n,
+                                left: o,
+                                right: o + i,
+                                rightWithBorder: o + i + n
                             };
-                        return n += l.width + o, l
+                        return o += s.width + n, s
                     }))
                 }
 
-                function k(e, t, o) {
-                    let n = o;
+                function D(e, t, n) {
+                    let o = n;
                     return e.map(((e, r) => {
-                        const i = a("height" in e ? e.height : 20, t),
-                            l = {
+                        const i = l("height" in e ? e.height : 20, t),
+                            s = {
                                 ...e,
                                 index: r,
                                 height: i,
-                                topWithBorder: n - o,
-                                top: n,
-                                bottom: n + i,
-                                bottomWithBorder: n + i + o
+                                topWithBorder: o - n,
+                                top: o,
+                                bottom: o + i,
+                                bottomWithBorder: o + i + n
                             };
-                        return n += l.height + o, l
+                        return o += s.height + n, s
                     }))
                 }
-                const I = {
-                    HEADER: ["HEADER"],
-                    FILTER: ["FILTER"],
-                    DATA: ["DATA"],
-                    CUSTOM: ["CUSTOM"],
-                    ANY: ["HEADER", "DATA", "FILTER", "CUSTOM"],
-                    SPECIAL: ["HEADER", "FILTER", "CUSTOM"],
-                    undefined: []
-                };
-                class D {
+                const T = "12px Calibri",
+                    M = {
+                        top: 2,
+                        right: 5,
+                        bottom: 2,
+                        left: 5
+                    },
+                    O = {
+                        HEADER: ["HEADER"],
+                        FILTER: ["FILTER"],
+                        DATA: ["DATA"],
+                        CUSTOM: ["CUSTOM"],
+                        ANY: ["HEADER", "DATA", "FILTER", "CUSTOM"],
+                        SPECIAL: ["HEADER", "FILTER", "CUSTOM"],
+                        undefined: []
+                    };
+                class L {
                     byKey = new Map;
                     byIndex = new Map;
                     byLabel = new Map;
-                    byMatch = new Map
+                    byType = new Map
                 }
-                class M {
-                    lookup = new D;
+                class P {
+                    lookup = new L;
                     hasRules = !1;
-                    addRule(e, t, o) {
+                    addRule(e, t, n) {
                         if (this.hasRules = !0, Array.isArray(e))
-                            for (const n of e) this.addRule(n, t, o);
+                            for (const o of e) this.addRule(o, t, n);
                         else if (Array.isArray(t))
-                            for (const n of t) this.addRule(e, n, o);
+                            for (const o of t) this.addRule(e, o, n);
                         else {
                             e = e ? "id" in e ? {
-                                key: n(e.id)
+                                key: o(e.id)
                             } : e : {
-                                match: "DATA"
+                                type: "DATA"
                             }, t = t ? "id" in t ? {
-                                key: n(t.id)
+                                key: o(t.id)
                             } : t : {
-                                match: "DATA"
+                                type: "DATA"
                             }, "key" in e && i(this.lookup.byKey, e.key), "index" in e && i(this.lookup.byIndex, e.index), "label" in e && i(this.lookup.byLabel, e.label);
-                            for (const t of I[e.match]) i(this.lookup.byMatch, t)
+                            for (const t of O[e.type]) i(this.lookup.byType, t)
                         }
 
                         function r(e, t) {
-                            e.has(t) || e.set(t, []), e.get(t).push(o)
+                            e.has(t) || e.set(t, []), e.get(t).push(n)
                         }
 
-                        function i(e, o) {
-                            e.has(o) || e.set(o, new D), "key" in t && r(e.get(o).byKey, t.key), "index" in t && r(e.get(o).byIndex, t.index), "label" in t && r(e.get(o).byLabel, t.label);
-                            for (const n of I[t.match]) r(e.get(o).byMatch, n)
+                        function i(e, n) {
+                            e.has(n) || e.set(n, new L), "key" in t && r(e.get(n).byKey, t.key), "index" in t && r(e.get(n).byIndex, t.index), "label" in t && r(e.get(n).byLabel, t.label);
+                            for (const o of O[t.type]) r(e.get(n).byType, o)
                         }
                     }
                     getRules(e, t) {
-                        const o = [];
-                        if (!this.hasRules) return o;
+                        const n = [];
+                        if (!this.hasRules) return n;
 
-                        function n(e) {
-                            for (const t of e) o.push(t)
+                        function o(e) {
+                            for (const t of e) n.push(t)
                         }
 
                         function r(e) {
-                            e.byKey.has(t.key) && n(e.byKey.get(t.key)), e.byIndex.has(t.index) && n(e.byIndex.get(t.index)), e.byMatch.has(t.type) && n(e.byMatch.get(t.type));
-                            for (const o of t.labels) e.byLabel.has(o) && n(e.byLabel.get(o))
+                            e.byKey.has(t.key) && o(e.byKey.get(t.key)), e.byIndex.has(t.index) && o(e.byIndex.get(t.index)), e.byType.has(t.type) && o(e.byType.get(t.type));
+                            for (const n of t.labels) e.byLabel.has(n) && o(e.byLabel.get(n))
                         }
-                        this.lookup.byKey.has(e.key) && r(this.lookup.byKey.get(e.key)), this.lookup.byIndex.has(e.index) && r(this.lookup.byIndex.get(e.index)), this.lookup.byMatch.has(e.type) && r(this.lookup.byMatch.get(e.type));
+                        this.lookup.byKey.has(e.key) && r(this.lookup.byKey.get(e.key)), this.lookup.byIndex.has(e.index) && r(this.lookup.byIndex.get(e.index)), this.lookup.byType.has(e.type) && r(this.lookup.byType.get(e.type));
                         for (const t of e.labels) this.lookup.byLabel.has(t) && r(this.lookup.byLabel.get(t));
-                        return o
+                        return n
                     }
                 }
-                const T = ["borderTop", "borderRight", "borderBottom", "borderLeft"],
-                    O = {
+                const B = ["borderTop", "borderRight", "borderBottom", "borderLeft"],
+                    S = {
                         validate: () => !0,
-                        parse: e => e
+                        parse: ({
+                            string: e
+                        }) => e
                     };
 
-                function L(e, t) {
-                    const o = {
+                function K(e, t) {
+                    const n = {
                         ...e
                     };
-                    if ("border" in o) {
-                        for (const e of T) o[e] = o.border;
-                        delete o.border
+                    if ("border" in n) {
+                        for (const e of B) n[e] = n.border;
+                        delete n.border
                     }
-                    for (const e of T) e in o && (o[e] = {
-                        ...o[e],
+                    for (const e of B) e in n && (n[e] = {
+                        ...n[e],
                         index: t
                     });
-                    return o
+                    return n
                 }
-                class P {
+
+                function W(e, t) {
+                    if (!1 !== e.edit) return !0 === e.edit ? "edit" in t ? t.edit : S : "edit" in t ? {
+                        ...t.edit,
+                        ...e.edit
+                    } : {
+                        ...S,
+                        ...e.edit
+                    }
+                }
+                class F {
                     constructor(e) {
-                        this.rulesLookup = new M;
-                        for (const [t, o] of e.entries()) {
+                        this.rulesLookup = new P;
+                        for (const [t, n] of e.entries()) {
                             const e = {
                                 index: t
                             };
-                            "condition" in o && (e.condition = o.condition), "style" in o && (e.style = "function" == typeof o.style ? o.style : () => o.style), "value" in o && (e.value = "function" == typeof o.value ? o.value : () => o.value), "text" in o && (e.text = "function" == typeof o.text ? o.text : () => o.text), "padding" in o && (e.padding = "function" == typeof o.padding ? o.padding : () => o.padding), "edit" in o && (e.edit = o.edit), "draw" in o && (e.draw = o.draw), this.rulesLookup.addRule(o.column, o.row, e)
+                            "condition" in n && (e.condition = n.condition), "style" in n && (e.style = "function" == typeof n.style ? n.style : () => n.style), "value" in n && (e.value = "function" == typeof n.value ? n.value : () => n.value), "text" in n && (e.text = "function" == typeof n.text ? n.text : () => n.text), "font" in n && (e.font = "function" == typeof n.font ? n.font : () => n.font), "padding" in n && (e.padding = "function" == typeof n.padding ? n.padding : () => n.padding), "edit" in n && (e.edit = n.edit), "draw" in n && (e.draw = n.draw), this.rulesLookup.addRule(n.column, n.row, e)
                         }
                     }
-                    resolve(e, t, o, n, r, i) {
-                        const l = this.rulesLookup.getRules(r, n).sort(((e, t) => e.index - t.index)).filter(((e, t, o) => e.index !== o[t - 1]?.index));
-                        let a, c = {
+                    resolve(e, t, n, o, r, i) {
+                        const l = this.rulesLookup.getRules(r, o).sort(((e, t) => e.index - t.index)).filter(((e, t, n) => e.index !== n[t - 1]?.index));
+                        let s, a = {
                                 data: e,
                                 rows: t,
-                                columns: o,
-                                row: n,
+                                columns: n,
+                                row: o,
                                 column: r
                             },
-                            u = {},
-                            d = s;
-                        i.hasValueByKey(n.key, r.key) && (c = {
-                            ...c,
-                            newValue: i.getValueByKey(n.key, r.key)
+                            c = {},
+                            u = M,
+                            d = T;
+                        i.hasValueByKey(o.key, r.key) && (a = {
+                            ...a,
+                            newValue: i.getValueByKey(o.key, r.key)
                         });
                         for (const e of l)
-                            if ((!("condition" in e) || e.condition(c)) && ("value" in e && (c = {
+                            if ((!("condition" in e) || e.condition(a)) && ("value" in e && (a = {
+                                    ...a,
+                                    value: e.value(a)
+                                }), "style" in e && (c = {
                                     ...c,
-                                    value: e.value(c)
-                                }), "style" in e && (u = {
+                                    ...K(e.style(a), e.index)
+                                }), "text" in e && (a = {
+                                    ...a,
+                                    text: e.text(a)
+                                }), "font" in e && (d = e.font(a)), "padding" in e && (u = {
                                     ...u,
-                                    ...L(e.style(c), e.index)
-                                }), "text" in e && (c = {
-                                    ...c,
-                                    text: e.text(c)
-                                }), "padding" in e && (d = {
-                                    ...d,
-                                    ...e.padding(c)
-                                }), "edit" in e && (c = {
-                                    ...c,
-                                    edit: e.edit && "edit" in c ? {
-                                        ...c.edit,
-                                        ...e.edit
-                                    } : {
-                                        ...O,
-                                        ...e.edit
-                                    }
+                                    ...e.padding(a)
+                                }), "edit" in e && (a = {
+                                    ...a,
+                                    edit: W(e, a)
                                 }), "draw" in e)) {
-                                const t = c;
-                                a = o => e.draw({
+                                const t = a;
+                                s = n => e.draw({
                                     ...t,
-                                    ctx: o
+                                    ctx: n
                                 })
                             } const p = function(e) {
-                                return "text" in e ? e.text : void 0 !== e.value ? `${e.value}` : ""
-                            }(c),
-                            h = {
-                                style: u,
+                                return "text" in e ? `${e.text}` : "newValue" in e ? `${e.newValue}` : void 0 !== e.value ? `${e.value}` : ""
+                            }(a),
+                            f = {
+                                style: c,
                                 visible: !0,
                                 text: p,
-                                padding: d
+                                padding: u,
+                                font: d
                             };
-                        return "value" in c && (h.value = c.value), "edit" in c && (h.edit = c.edit), void 0 !== a && (h.draw = a), "text" in c && (h.text = c.text), h
+                        return "value" in a && (f.value = a.value), "edit" in a && void 0 !== a.edit && (f.edit = a.edit), void 0 !== s && (f.draw = s), f
                     }
                 }
 
-                function B(e) {
-                    return new P(e)
+                function z(e) {
+                    return new F(e)
                 }
-                class S {
-                    constructor(e, t, o, n, r) {
-                        this.formattingRules = e, this.data = t, this.rows = o, this.columns = n, this.edition = r
+                class U {
+                    constructor(e, t, n, o, r) {
+                        this.formattingRules = e, this.data = t, this.rows = n, this.columns = o, this.edition = r
                     }
                     resolve(e, t) {
                         return this.formattingRules.resolve(this.data, this.rows, this.columns, e, t, this.edition)
                     }
                 }
 
-                function K(e, t, o, n, r) {
-                    return new S(e, t, o, n, r)
+                function N(e, t, n, o, r) {
+                    return new U(e, t, n, o, r)
                 }
 
-                function W(e, t, o) {
+                function j(e, t, n) {
                     const r = new Map;
                     for (const i of e) {
-                        const e = n(i[t]),
-                            l = n(i[o]);
+                        const e = o(i[t]),
+                            l = o(i[n]);
                         r.has(e) || r.set(e, new Map), r.get(e).set(l, i.expression)
                     }
                     return r
                 }
 
-                function F(e, t, o, n, r, i, l) {
+                function H(e, t, n, o, r, i, l) {
                     if (0 === e.length) return r;
-                    const s = W(e, "columnId", "rowId"),
+                    const s = j(e, "columnId", "rowId"),
                         a = i.filter((e => "FILTER" !== e.type && s.has(e.key)));
                     return 0 === a.length ? r : r.filter((e => {
                         for (const c of a) {
-                            const a = o.resolve(n, r, i, e, c, l),
+                            const a = n.resolve(o, r, i, e, c, l),
                                 u = s.get(c.key);
-                            if (!t.resolve(n, r, i, e, c, a.value, a.text, u)) return !1
+                            if (!t.resolve(o, r, i, e, c, a.value, a.text, u)) return !1
                         }
                         return !0
                     }))
                 }
 
-                function N(e, t, o, n, r, i, l) {
+                function q(e, t, n, o, r, i, l) {
                     if (0 === e.length) return i;
-                    const s = W(e, "rowId", "columnId"),
+                    const s = j(e, "rowId", "columnId"),
                         a = r.filter((e => "FILTER" !== e.type && s.has(e.key)));
                     return 0 === a.length ? i : i.filter((e => {
                         for (const c of a) {
-                            const a = o.resolve(n, r, i, c, e, l),
+                            const a = n.resolve(o, r, i, c, e, l),
                                 u = s.get(c.key);
-                            if (!t.resolve(n, r, i, c, e, a.value, a.text, u)) return !1
+                            if (!t.resolve(o, r, i, c, e, a.value, a.text, u)) return !1
                         }
                         return !0
                     }))
                 }
 
-                function z(e, t, o, n) {
+                function $(e, t, n, o) {
                     return {
                         top: e,
                         bottom: t,
-                        left: o,
-                        right: n
+                        left: n,
+                        right: o
                     }
                 }
 
-                function U(e, t) {
+                function V(e, t) {
                     return {
                         width: e.length ? e.at(-1).rightWithBorder : 0,
                         height: t.length ? t.at(-1).bottomWithBorder : 0
                     }
                 }
-                class j {
+                class G {
                     constructor() {
                         this.canvas = document.createElement("canvas"), this.context = this.canvas.getContext("2d"), this.fontMetrics = new Map
                     }
                     measureWidth(e, t) {
-                        const o = this.context;
-                        return o.font = t || l, o.measureText(e).width
+                        if (!e) return 0;
+                        const n = this.context;
+                        return n.font = t || T, n.measureText(e).width
                     }
                     measureHeight(e, t) {
-                        let o = 1;
-                        for (const t of e) "\n" === t && o++;
-                        return o * this.getFontMetrics(t).height
+                        let n = 1;
+                        for (const t of e) "\n" === t && n++;
+                        return n * this.getFontMetrics(t).height
                     }
                     getFontMetrics(e) {
                         const t = e;
                         if (this.fontMetrics.has(t)) return this.fontMetrics.get(t);
-                        const o = this.context;
-                        o.font = e || l;
-                        const n = o.measureText("X"),
-                            r = (n.actualBoundingBoxDescent - n.actualBoundingBoxAscent) / 2,
+                        const n = this.context;
+                        n.font = e || T;
+                        const o = n.measureText("X"),
+                            r = (o.actualBoundingBoxDescent - o.actualBoundingBoxAscent) / 2,
                             i = {
-                                topOffset: r + n.fontBoundingBoxAscent,
+                                topOffset: r + o.fontBoundingBoxAscent,
                                 middle: -r,
-                                bottomOffset: n.fontBoundingBoxDescent - r,
-                                height: n.fontBoundingBoxAscent + n.fontBoundingBoxDescent
+                                bottomOffset: o.fontBoundingBoxDescent - r,
+                                height: o.fontBoundingBoxAscent + o.fontBoundingBoxDescent
                             };
                         return this.fontMetrics.set(t, i), i
                     }
                 }
 
-                function H() {
-                    return new j
+                function Y() {
+                    return new G
                 }
 
-                function q(e, t) {
+                function X(e, t) {
                     return t.top >= e.top && t.left >= e.left && t.top + t.height <= e.top + e.height && t.left + t.width <= e.left + e.width
                 }
 
-                function $(e, t) {
-                    const o = {
+                function Z(e, t) {
+                    const n = {
                         top: Math.max(e.top, t.top),
                         left: Math.max(e.left, t.left),
                         width: Math.min(e.left + e.width, t.left + t.width) - Math.max(e.left, t.left),
                         height: Math.min(e.top + e.height, t.top + t.height) - Math.max(e.top, t.top)
                     };
-                    return o.width >= 0 && o.height >= 0 ? o : {
+                    return n.width >= 0 && n.height >= 0 ? n : {
                         top: e.top,
                         left: e.left,
                         width: 0,
                         height: 0
                     }
                 }
 
-                function V(e, t) {
+                function J(e, t) {
                     return {
                         top: e.top - t,
                         left: e.left - t,
                         width: e.width + 2 * t,
                         height: e.height + 2 * t
                     }
                 }
 
-                function G(e) {
+                function Q(e) {
                     return e.width * e.height
                 }
 
-                function Y(e, t) {
+                function ee(e, t) {
                     return {
                         top: e.top,
                         left: e.left,
                         width: Math.max(0, e.width - t.left - t.right),
                         height: Math.max(0, e.height - t.top - t.bottom)
                     }
                 }
-                const X = 200,
-                    Z = 400,
-                    J = {
+                const te = 200,
+                    ne = 400,
+                    oe = {
                         left: 0,
                         top: 0,
                         width: 0,
                         height: 0
                     };
 
-                function Q(e) {
+                function re(e, t, n, o) {
+                    const r = t.x,
+                        i = t.y,
+                        l = e.scrollLeft,
+                        s = e.scrollTop,
+                        a = e.clientWidth,
+                        c = e.clientHeight;
+                    return {
+                        x: r <= n.left ? r : r >= a ? r + l : r >= a - n.right ? o.width - a + r : r + l,
+                        y: i <= n.top ? i : i >= c ? i + s : i >= c - n.bottom ? o.height - c + i : i + s
+                    }
+                }
+
+                function ie(e) {
                     return e.reduce(((e, t) => e.set(t.key, t)), new Map)
                 }
 
-                function ee(e, t, o, r, i, l, s, a) {
+                function le(e, t, n, r, i, l, s, a) {
                     if (!e) return [];
                     if (t) return [];
                     if (!r) return [];
-                    if (!o) return [];
-                    const c = n(o.columnId),
-                        u = n(o.rowId),
-                        d = n(r.columnId),
-                        p = n(r.rowId);
+                    if (!n) return [];
+                    const c = o(n.columnId),
+                        u = o(n.rowId),
+                        d = o(r.columnId),
+                        p = o(r.rowId);
                     if (!s.has(c)) return [];
                     if (!a.has(u)) return [];
                     if (!s.has(d)) return [];
                     if (!a.has(p)) return [];
-                    const h = Math.min(s.get(c).index, s.get(d).index),
-                        f = Math.max(s.get(c).index, s.get(d).index),
-                        m = Math.min(a.get(u).index, a.get(p).index),
-                        _ = Math.max(a.get(u).index, a.get(p).index);
-                    return i.slice(h, f + 1).flatMap((e => l.slice(m, _ + 1).map((t => ({
+                    const f = Math.min(s.get(c).index, s.get(d).index),
+                        h = Math.max(s.get(c).index, s.get(d).index),
+                        _ = Math.min(a.get(u).index, a.get(p).index),
+                        m = Math.max(a.get(u).index, a.get(p).index);
+                    return i.slice(f, h + 1).flatMap((e => l.slice(_, m + 1).map((t => ({
                         rowId: t.id,
                         columnId: e.id
                     })))))
                 }
 
-                function te(e, t) {
-                    const o = function(e) {
+                function se(e, t) {
+                    const n = function(e) {
                             return "BEGIN" === e.pinned ? "top" : "END" === e.pinned ? "bottom" : "middle"
                         }(t),
-                        n = function(e) {
+                        o = function(e) {
                             return "BEGIN" === e.pinned ? "left" : "END" === e.pinned ? "right" : "center"
                         }(e);
-                    return `${o}-${n}`
+                    return `${n}-${o}`
                 }
 
-                function oe(e, t, o, r, i) {
+                function ae(e, t, n, r, i) {
                     if (!t) return null;
-                    const l = n(t.columnId),
-                        s = n(t.rowId);
-                    if (!o.has(l)) return null;
+                    const l = o(t.columnId),
+                        s = o(t.rowId);
+                    if (!n.has(l)) return null;
                     if (!r.has(s)) return null;
-                    const a = o.get(l),
+                    const a = n.get(l),
                         c = r.get(s);
                     if (0 === e.length) return null;
                     const u = {
                         width: a.width,
                         height: c.height,
-                        section: te(a, c)
+                        section: se(a, c)
                     };
                     switch (c.pinned) {
                         case "BEGIN":
                             u.top = c.top;
                             break;
                         case "END":
                             u.bottom = i.top.height + i.middle.height + i.bottom.height - c.top - c.height;
@@ -1368,94 +1479,94 @@
                             break;
                         default:
                             u.marginLeft = a.left - i.left.width
                     }
                     return u
                 }
 
-                function ne(e, t) {
+                function ce(e, t) {
                     return t.every((t => t.edit.validate({
                         string: e
                     })))
                 }
 
-                function re(e) {
+                function ue(e) {
                     return Array.isArray(e) ? e.map(((e, t) => t)) : Object.keys(e)
                 }
 
-                function ie(e) {
-                    return re(e)
+                function de(e) {
+                    return ue(e)
                 }
 
-                function le(e) {
+                function pe(e) {
                     const t = new Set;
                     if (Array.isArray(e))
-                        for (const o of e)
-                            for (const e of re(o)) t.add(e);
+                        for (const n of e)
+                            for (const e of ue(n)) t.add(e);
                     else
-                        for (const o in e)
-                            for (const n of re(e[o])) t.add(n);
+                        for (const n in e)
+                            for (const o of ue(e[n])) t.add(o);
                     return [...t]
                 }
 
-                function se(e, t) {
+                function fe(e, t) {
                     if (!e.some((e => "DATA-BLOCK" === e.type))) return e;
-                    const o = [];
-                    for (const n of e)
-                        if ("DATA-BLOCK" === n.type) {
-                            const e = "selector" in n ? n.selector(t) : le(t);
-                            for (const t of e) o.push({
-                                ...n,
+                    const n = [];
+                    for (const o of e)
+                        if ("DATA-BLOCK" === o.type) {
+                            const e = "selector" in o ? o.selector(t) : pe(t);
+                            for (const t of e) n.push({
+                                ...o,
                                 id: t,
                                 type: "DATA"
                             })
-                        } else o.push(n);
-                    return o
+                        } else n.push(o);
+                    return n
                 }
 
-                function ae(e, t) {
+                function he(e, t) {
                     if (!e.some((e => "DATA-BLOCK" === e.type))) return e;
-                    const o = [];
-                    for (const n of e)
-                        if ("DATA-BLOCK" === n.type) {
-                            const e = "selector" in n ? n.selector(t) : ie(t);
-                            for (const t of e) o.push({
-                                ...n,
+                    const n = [];
+                    for (const o of e)
+                        if ("DATA-BLOCK" === o.type) {
+                            const e = "selector" in o ? o.selector(t) : de(t);
+                            for (const t of e) n.push({
+                                ...o,
                                 id: t,
                                 type: "DATA"
                             })
-                        } else o.push(n);
-                    return o
+                        } else n.push(o);
+                    return n
                 }
-                const ce = ({
+                const _e = ({
                     text: e,
                     expression: t
                 }) => e.includes(t);
-                class ue {
+                class me {
                     constructor(e) {
-                        this.rulesLookup = new M;
+                        this.rulesLookup = new P;
                         for (const t of e) {
                             const e = {
-                                by: n("by" in t ? t.by : "FILTER"),
-                                condition: t.condition || ce
+                                by: o("by" in t ? t.by : "FILTER"),
+                                condition: t.condition || _e
                             };
                             this.rulesLookup.addRule(t.column, t.row, e)
                         }
                     }
-                    resolve(e, t, o, n, r, i, l, s) {
-                        const a = this.rulesLookup.getRules(r, n);
-                        if (0 === a.length) return "DATA" !== n.type || "DATA" !== r.type || !s.has('"FILTER"') || ce({
+                    resolve(e, t, n, o, r, i, l, s) {
+                        const a = this.rulesLookup.getRules(r, o);
+                        if (0 === a.length) return "DATA" !== o.type || "DATA" !== r.type || !s.has('"FILTER"') || _e({
                             text: l,
                             expression: s.get('"FILTER"')
                         });
                         let c = {
                             data: e,
                             rows: t,
-                            columns: o,
-                            row: n,
+                            columns: n,
+                            row: o,
                             column: r,
                             value: i,
                             text: l
                         };
                         for (const e of a) {
                             if (!s.has(e.by)) continue;
                             const t = {
@@ -1464,484 +1575,496 @@
                             };
                             if (!e.condition(t)) return !1
                         }
                         return !0
                     }
                 }
 
-                function de(e) {
-                    return new ue(e)
+                function ge(e) {
+                    return new me(e)
                 }
 
-                function pe(e) {
-                    return e
+                function ye(e) {
+                    return f(e, ["value", "text"])
                 }
 
-                function he(e) {
-                    return e
+                function we(e) {
+                    return f(e, ["value", "text", "font", "padding"])
                 }
 
-                function fe(e, t, o, n, r, i) {
+                function Ee(e, t, n, o, r, i) {
                     if (e.every((e => "number" == typeof e.width))) return e;
                     const l = e => {
-                        const i = "width" in e ? e.width : "fit-once";
+                        const i = e.width;
                         if ("number" == typeof i) return i;
                         if (r.has(e.key)) {
                             const t = r.get(e.key);
                             if ("fit-once" === i && !t.dataOnly) return t.width;
                             if ("fit-data-once" === i && t.dataOnly) return t.width
                         }
                         let l = 0;
                         for (const r of t) {
                             if ("DATA" !== r.type && "fit-data-once" === i) continue;
                             if ("DATA" !== r.type && "fit-data" === i) continue;
-                            const t = n.resolve(r, e),
+                            const t = o.resolve(r, e),
                                 s = t.text,
                                 a = t.font,
                                 c = t.padding.left + t.padding.right,
-                                u = o.measureWidth(s, a) + c;
+                                u = n.measureWidth(s, a) + c;
                             l = Math.max(l, u)
                         }
                         return r.set(e.key, {
                             width: l,
                             dataOnly: "fit-data-once" === i
                         }), l
                     };
                     for (const e of r.keys()) i.has(e) || r.delete(e);
                     return e.map((e => ({
                         ...e,
                         width: l(e)
                     })))
                 }
 
-                function me(e, t, o, n, r, i) {
+                function be(e, t, n, o, r, i) {
                     if (t.every((e => "number" == typeof e.height))) return t;
                     const l = t => {
-                        const i = "height" in t ? t.height : "fit-once";
+                        const i = t.height;
                         if ("number" == typeof i) return i;
                         if (r.has(t.key)) {
                             const e = r.get(t.key);
                             if ("fit-once" === i && !e.dataOnly) return e.height;
                             if ("fit-data-once" === i && e.dataOnly) return e.height
                         }
                         let l = 0;
                         for (const r of e) {
                             if ("DATA" !== r.type && "fit-data-once" === i) continue;
                             if ("DATA" !== r.type && "fit-data" === i) continue;
-                            const e = n.resolve(t, r),
+                            const e = o.resolve(t, r),
                                 s = e.text,
                                 a = e.font,
                                 c = e.padding.top + e.padding.bottom,
-                                u = o.measureHeight(s, a) + c;
+                                u = n.measureHeight(s, a) + c;
                             l = Math.max(l, u)
                         }
                         return r.set(t.key, {
                             height: l,
                             dataOnly: "fit-data-once" === i
                         }), l
                     };
                     for (const e of r.keys()) i.has(e) || r.delete(e);
                     return t.map((e => ({
                         ...e,
                         height: l(e)
                     })))
                 }
 
-                function _e(e) {
+                function ve(e) {
                     return new Set(e.map((e => e.key)))
                 }
 
-                function ge(e) {
-                    return e
+                function xe(e) {
+                    return f(e, ["value", "text"])
                 }
 
-                function ye(e, t) {
+                function Re(e, t) {
                     return null != e.value && (null == t.value || e.value < t.value)
                 }
 
-                function we(e, t) {
+                function Ae(e, t) {
                     return null != e.value && (null == t.value || e.value > t.value)
                 }
-                class be {
+                class Ce {
                     constructor(e) {
-                        this.rulesLookup = new M;
+                        this.rulesLookup = new P;
                         for (const t of e) {
-                            const e = {
-                                by: stringifyId("by" in t ? t.by : "HEADER"),
-                                comparatorAsc: t.comparator || ye,
-                                comparatorDesc: (e, o) => -t.comparator(e, o) || we
-                            };
-                            this.rulesLookup.addRule(t.column, t.row, e)
+                            const e = t.comparator ? (e, n) => t.comparator(e, n) : (e, t) => Re(e, t),
+                                n = t.comparator ? (e, n) => !t.comparator(e, n) : (e, t) => Ae(e, t),
+                                r = {
+                                    by: o("by" in t ? t.by : "HEADER"),
+                                    comparatorAsc: e,
+                                    comparatorDesc: n
+                                };
+                            this.rulesLookup.addRule(t.column, t.row, r)
                         }
                     }
-                    resolve(e, t, o) {
-                        const n = this.rulesLookup.getRules(e, t);
-                        if (0 === n.length) return "DATA" !== t.type || "DATA" !== e.type ? null : o.has('"HEADER"') ? "ASC" === o.get('"HEADER"') ? ye : we : null;
-                        if (n.length > 1) throw new Error("Multiple sorting rules for the same cell");
-                        const r = n[0];
-                        return "ASC" === o.get(r.by) ? r.comparatorAsc : r.comparatorDesc
+                    resolve(e, t, n) {
+                        const o = this.rulesLookup.getRules(e, t);
+                        if (0 === o.length) return "DATA" !== t.type || "DATA" !== e.type ? null : n.has('"HEADER"') ? "ASC" === n.get('"HEADER"') ? Re : Ae : null;
+                        if (o.length > 1) throw new Error("Multiple sorting rules for the same cell");
+                        const r = o[0];
+                        return n.has(r.by) ? "ASC" === n.get(r.by) ? r.comparatorAsc : r.comparatorDesc : null
                     }
                 }
 
-                function Ee(e) {
-                    return new be(e)
+                function ke(e) {
+                    return new Ce(e)
                 }
 
-                function ve(e, t, o) {
+                function Ie(e, t, n) {
                     const r = new Map;
                     for (const i of e) {
-                        const e = n(i[t]),
-                            l = n(i[o]);
+                        const e = o(i[t]),
+                            l = o(i[n]);
                         r.has(e) || r.set(e, new Map), r.get(e).set(l, i.direction)
                     }
                     return r
                 }
 
-                function xe(e, t) {
+                function De(e, t) {
                     e.sort(((e, t) => {
-                        const o = e.comparator(e.cell, t.cell);
-                        return "number" == typeof o ? o : o ? -1 : 1
+                        const n = e.comparator(e.cell, t.cell);
+                        return "number" == typeof n ? n : n ? -1 : 1
                     })), t.push(...e.map((e => e.entity))), e.length = 0
                 }
 
-                function Re(e, t, o, r, i, l, s) {
+                function Te(e, t, n, r, i, l, s) {
                     if (0 === e.length) return i;
-                    const a = ve(e, "columnId", "rowId"),
+                    const a = Ie(e, "columnId", "rowId"),
                         c = new Map(l.map((e => [e.key, e]))),
-                        u = e.map((e => n(e.columnId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
+                        u = e.map((e => o(e.columnId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
                     if (0 === u.length) return i;
                     for (const e of u) {
-                        const n = [],
+                        const o = [],
                             c = [];
                         for (const u of i) {
                             const d = t.resolve(e, u, a.get(e.key));
                             if (!d) {
-                                xe(c, n), n.push(u);
+                                De(c, o), o.push(u);
                                 continue
                             }
                             const p = {
                                 entity: u,
                                 comparator: d,
-                                cell: o.resolve(r, i, l, u, e, s)
+                                cell: n.resolve(r, i, l, u, e, s)
                             };
-                            0 !== c.length && c[0].comparator !== d ? (xe(c, n), c.push(p)) : c.push(p)
+                            0 !== c.length && c[0].comparator !== d ? (De(c, o), c.push(p)) : c.push(p)
                         }
-                        xe(c, n), i = n
+                        De(c, o), i = o
                     }
                     return i
                 }
 
-                function Ce(e, t, o, r, i, l, s) {
+                function Me(e, t, n, r, i, l, s) {
                     if (0 === e.length) return l;
-                    const a = ve(e, "rowId", "columnId"),
+                    const a = Ie(e, "rowId", "columnId"),
                         c = new Map(i.map((e => [e.key, e]))),
-                        u = e.map((e => n(e.rowId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
+                        u = e.map((e => o(e.rowId))).filter((e => c.has(e))).map((e => c.get(e))).reverse();
                     if (0 === u.length) return l;
                     for (const e of u) {
-                        const n = [],
+                        const o = [],
                             c = [];
                         for (const u of l) {
                             const d = t.resolve(u, e, a.get(e.key));
                             if (!d) {
-                                xe(c, n), n.push(u);
+                                De(c, o), o.push(u);
                                 continue
                             }
                             const p = {
                                 entity: u,
                                 comparator: d,
-                                cell: o.resolve(r, i, l, e, u, s)
+                                cell: n.resolve(r, i, l, e, u, s)
                             };
-                            0 !== c.length && c[0].comparator !== d ? (xe(c, n), c.push(p)) : c.push(p)
+                            0 !== c.length && c[0].comparator !== d ? (De(c, o), c.push(p)) : c.push(p)
                         }
-                        xe(c, n), l = n
+                        De(c, o), l = o
                     }
                     return l
                 }
-                const Ae = 5;
+                const Oe = 5;
 
-                function ke(e, t, o, r, i) {
+                function Le(e, t, n, r, i, l, s, a) {
                     if (!r) return null;
-                    const l = t.get(n(r.columnId)),
-                        s = o.get(n(r.rowId)),
-                        a = i.x;
-                    return "HEADER" !== s.type ? null : a >= l.right - Ae && a <= l.right + Ae ? l.id : 0 === l.index || a < l.left - Ae || a > l.left + Ae ? null : e[l.index - 1].id
+                    const c = t.get(o(r.columnId));
+                    if ("HEADER" !== n.get(o(r.rowId)).type) return null;
+                    const u = re(i, l, s, a);
+                    if (!u) return null;
+                    const d = u.x;
+                    return d >= c.right - Oe && d <= c.right + Oe ? c.id : 0 === c.index || d < c.left - Oe || d > c.left + Oe ? null : e[c.index - 1].id
                 }
 
-                function Ie(e, t, o, r, i) {
+                function Pe(e, t, n, r, i, l, s, a) {
                     if (!r) return null;
-                    const l = t.get(n(r.columnId)),
-                        s = o.get(n(r.rowId)),
-                        a = i.y;
-                    return "HEADER" !== l.type ? null : a >= s.bottom - Ae && a <= s.bottom + Ae ? s.id : 0 === s.index || a < s.top - Ae || a > s.top + Ae ? null : e[s.index - 1].id
+                    const c = t.get(o(r.columnId)),
+                        u = n.get(o(r.rowId));
+                    if ("HEADER" !== c.type) return null;
+                    const d = re(i, l, s, a);
+                    if (!d) return null;
+                    const p = d.y;
+                    return p >= u.bottom - Oe && p <= u.bottom + Oe ? u.id : 0 === u.index || p < u.top - Oe || p > u.top + Oe ? null : e[u.index - 1].id
                 }
 
-                function De(e) {
+                function Be(e) {
                     return e.map((e => ({
                         columnId: "columnId" in e ? e.columnId : "HEADER",
                         rowId: "rowId" in e ? e.rowId : "HEADER",
                         direction: e.direction
                     })))
                 }
 
-                function Me(e) {
+                function Se(e) {
                     return e.map((e => ({
                         columnId: "columnId" in e ? e.columnId : "FILTER",
                         rowId: "rowId" in e ? e.rowId : "FILTER",
                         expression: e.expression
                     })))
                 }
 
-                function Te(e, t) {
+                function Ke(e, t) {
                     return function(e, t) {
-                        const o = e.filter((e => "DATA" === e.type)).map((e => e.id));
-                        return t(o), o
+                        const n = e.filter((e => "DATA" === e.type)).map((e => e.id));
+                        return t(n), n
                     }(e, t)
                 }
 
-                function Oe(e) {
+                function We(e) {
                     console.count("updateState");
                     const t = {
                             ...e.localOptions,
                             ...e.externalOptions
                         },
-                        o = e.memory,
-                        n = e.state;
-
-                    function r(e, t, n) {
-                        const r = o[e] && o[e].dependencies;
-                        return r && !n.some(((e, t) => e !== r[t])) || (o[e] = {
-                            value: t(...n),
-                            dependencies: n
-                        }), o[e].value
-                    }
-                    const l = window.devicePixelRatio,
-                        s = t.borderWidth / l,
-                        a = t.data,
-                        c = e.input.value,
-                        u = r("sortBy", De, [t.sortBy]),
-                        h = r("filters", Me, [t.filters]),
-                        g = r("textResolver", H, []),
-                        w = r("dataFormatting", d, [t.formatting, t.dataSelector, u]),
-                        v = r("editedCellsAndFilters", _, [t.editedCells, h]),
-                        x = r("edition", y, [v]),
-                        I = r("invokedColumns", E, [t.columns, a]),
-                        D = r("invokedRows", E, [t.rows, a]),
-                        M = r("unfoldedColumns", se, [I, a]),
-                        T = r("unfoldedRows", ae, [D, a]),
-                        O = r("unfilteredColumns", R, [M, t.pinnedLeft, t.pinnedRight, t.columnWidths]),
-                        L = r("unfilteredRows", C, [T, t.pinnedTop, t.pinnedBottom, t.rowHeights]),
-                        P = r("unfilteredColumnKeys", _e, [O]),
-                        S = r("unfilteredRowKeys", _e, [L]),
-                        W = r("filterFormatting", pe, [w]),
-                        j = r("filterFormattingRules", B, [W]),
-                        te = r("filteringRules", de, [t.filtering]),
-                        re = r("filteredColumns", N, [h, te, j, a, L, O, x]),
-                        ie = r("filteredRows", F, [h, te, j, a, L, O, x]),
-                        le = r("sortingFormatting", ge, [w]),
-                        ce = r("sortingFormattingRules", B, [le]),
-                        ue = r("sortingRules", Ee, [t.sorting]),
-                        ye = r("sortedColumns", Ce, [u, ue, ce, a, ie, re, x]),
-                        we = r("sortedRows", Re, [u, ue, ce, a, ie, re, x]),
-                        be = r("measureFormatting", he, [w]),
-                        ve = r("measureFormattingRules", B, [be]),
-                        xe = r("measureFormatResolver", K, [ve, a, we, ye, x]),
+                        n = e.memory,
+                        o = e.state,
+                        r = e.element;
+
+                    function l(e, t, o) {
+                        const r = n[e] && n[e].dependencies;
+                        return r && !o.some(((e, t) => e !== r[t])) || (n[e] = {
+                            value: t(...o),
+                            dependencies: o
+                        }), n[e].value
+                    }
+                    const s = window.devicePixelRatio,
+                        a = t.borderWidth / s,
+                        c = t.data,
+                        d = e.input.value,
+                        p = l("sortBy", Be, [t.sortBy]),
+                        f = l("filters", Se, [t.filters]),
+                        _ = l("textResolver", Y, []),
+                        w = l("dataFormatting", u, [t.formatting, t.dataSelector, p]),
+                        b = l("editedCellsAndFilters", y, [t.editedCells, f]),
+                        R = l("edition", E, [b]),
+                        A = l("invokedColumns", x, [t.columns, c]),
+                        T = l("invokedRows", x, [t.rows, c]),
+                        M = l("unfoldedColumns", fe, [A, c]),
+                        O = l("unfoldedRows", he, [T, c]),
+                        L = l("unfilteredColumns", C, [M, t.pinnedLeft, t.pinnedRight, t.columnWidths]),
+                        P = l("unfilteredRows", k, [O, t.pinnedTop, t.pinnedBottom, t.rowHeights]),
+                        B = l("unfilteredColumnKeys", ve, [L]),
+                        S = l("unfilteredRowKeys", ve, [P]),
+                        K = l("filterFormatting", ye, [w]),
+                        W = l("filterFormattingRules", z, [K]),
+                        F = l("filteringRules", ge, [t.filtering]),
+                        U = l("filteredColumns", q, [f, F, W, c, P, L, R]),
+                        j = l("filteredRows", H, [f, F, W, c, P, L, R]),
+                        G = l("sortingFormatting", xe, [w]),
+                        se = l("sortingFormattingRules", z, [G]),
+                        ue = l("sortingRules", ke, [t.sorting]),
+                        de = l("sortedColumns", Me, [p, ue, se, c, j, U, R]),
+                        pe = l("sortedRows", Te, [p, ue, se, c, j, U, R]),
+                        _e = l("measureFormatting", we, [w]),
+                        me = l("measureFormattingRules", z, [_e]),
+                        Re = l("measureFormatResolver", N, [me, c, pe, de, R]),
                         Ae = e.columnWidthCache,
-                        Oe = e.rowHeightCache,
-                        Le = r("measuredColumns", fe, [ye, we, g, xe, Ae, P]),
-                        Pe = r("measuredRows", me, [ye, we, g, xe, Oe, S]),
-                        Be = r("columns", A, [Le, l, s]),
-                        Se = r("rows", k, [Pe, l, s]),
-                        Ke = r("columnLookup", Q, [Be]),
-                        We = r("rowLookup", Q, [Se]),
-                        Fe = t.focusedCell,
-                        Ne = r("sections", m, [Be, Se]),
-                        ze = t.selectedCells,
-                        Ue = r("fixedSize", z, [Ne.top.height, Ne.bottom.height, Ne.left.width, Ne.right.width]),
-                        je = r("totalSize", U, [Be, Se]),
-                        He = function(e, t, o, n, r, i) {
+                        Ce = e.rowHeightCache,
+                        Ie = l("measuredColumns", Ee, [de, pe, _, Re, Ae, B]),
+                        De = l("measuredRows", be, [de, pe, _, Re, Ce, S]),
+                        Oe = l("columns", I, [Ie, s, a]),
+                        We = l("rows", D, [De, s, a]),
+                        Fe = l("columnLookup", ie, [Oe]),
+                        ze = l("rowLookup", ie, [We]),
+                        Ue = t.focusedCell,
+                        Ne = l("sections", g, [Oe, We]),
+                        je = t.selectedCells,
+                        He = l("fixedSize", $, [Ne.top.height, Ne.bottom.height, Ne.left.width, Ne.right.width]),
+                        qe = l("totalSize", V, [Oe, We]),
+                        $e = function(e, t, n, o, r, i) {
                             if (!t) return null;
                             if (t.x < 0 || t.y < 0 || t.x > i.width || t.y > i.height) return null;
-                            const l = e.scrollLeft,
-                                s = e.scrollTop,
-                                a = e.clientWidth,
-                                c = e.clientHeight,
-                                u = t.x <= r.left ? t.x : t.x >= a - r.right ? i.width - a + t.x : t.x + l,
-                                d = function(e, t) {
+                            const l = re(e, t, r, i),
+                                s = function(e, t) {
                                     if (0 === e.length) return -1;
                                     if (t < e[0].topWithBorder) return -1;
                                     if (t > e[e.length - 1].bottomWithBorder) return -1;
-                                    let o = 0,
-                                        n = e.length - 1;
-                                    for (; o <= n;) {
-                                        const r = Math.floor((o + n) / 2);
-                                        if (t < e[r].topWithBorder) n = r - 1;
+                                    let n = 0,
+                                        o = e.length - 1;
+                                    for (; n <= o;) {
+                                        const r = Math.floor((n + o) / 2);
+                                        if (t < e[r].topWithBorder) o = r - 1;
                                         else {
                                             if (!(t > e[r].bottomWithBorder)) return r;
-                                            o = r + 1
+                                            n = r + 1
                                         }
                                     }
                                     return -1
-                                }(o, t.y <= r.top ? t.y : t.y >= c - r.bottom ? i.height - c + t.y : t.y + s),
-                                p = function(e, t) {
+                                }(n, l.y),
+                                a = function(e, t) {
                                     if (0 === e.length) return -1;
                                     if (t < e[0].leftWithBorder) return -1;
                                     if (t > e[e.length - 1].rightWithBorder) return -1;
-                                    let o = 0,
-                                        n = e.length - 1;
-                                    for (; o <= n;) {
-                                        const r = Math.floor((o + n) / 2);
-                                        if (t < e[r].leftWithBorder) n = r - 1;
+                                    let n = 0,
+                                        o = e.length - 1;
+                                    for (; n <= o;) {
+                                        const r = Math.floor((n + o) / 2);
+                                        if (t < e[r].leftWithBorder) o = r - 1;
                                         else {
                                             if (!(t > e[r].rightWithBorder)) return r;
-                                            o = r + 1
+                                            n = r + 1
                                         }
                                     }
                                     return -1
-                                }(n, u);
-                            return -1 === d || -1 === p ? null : {
-                                rowId: o[d].id,
-                                columnId: n[p].id
+                                }(o, l.x);
+                            return -1 === s || -1 === a ? null : {
+                                rowId: n[s].id,
+                                columnId: o[a].id
                             }
-                        }(e.element, e.mousePosition, Se, Be, Ue, je),
-                        qe = e.resizingColumn || r("resizableColumn", ke, [Be, Ke, We, He, e.mousePosition]),
-                        $e = e.resizingRow || r("resizableRow", Ie, [Se, Ke, We, He, e.mousePosition]),
-                        Ve = r("highlightedCells", ee, [e.isMouseDown, !!qe || !!$e, Fe, He, Be, Se, Ke, We]),
-                        Ge = r("selection", b, [ze]),
-                        Ye = r("highlight", b, [Ve]),
-                        Xe = r("renderFormatting", f, [w, He, Fe, Ge, Ye, x, qe, $e]),
-                        Ze = r("renderFormattingRules", B, [Xe]),
-                        Je = r("renderFormatResolver", K, [Ze, a, Se, Be, x]),
-                        Qe = r("inputFormatting", p, [w]),
-                        et = r("inputFormattingRules", B, [Qe]),
-                        tt = r("inputFormatResolver", K, [et, a, Se, Be, x]),
-                        ot = r("editableCells", i, [ze, tt, Ke, We]),
-                        nt = r("inputPlacement", oe, [ot, Fe, Ke, We, Ne]),
-                        rt = r("isTextValid", ne, [c, ot]),
-                        it = function(e, t, o, n) {
+                        }(r, e.mousePosition, We, Oe, He, qe),
+                        Ve = e.resizingColumn || l("resizableColumn", Le, [Oe, Fe, ze, $e, r, e.mousePosition, He, qe]),
+                        Ge = e.resizingRow || l("resizableRow", Pe, [We, Fe, ze, $e, r, e.mousePosition, He, qe]),
+                        Ye = l("highlightedCells", le, [e.isMouseDown, !!Ve || !!Ge, Ue, $e, Oe, We, Fe, ze]),
+                        Xe = l("selection", v, [je]),
+                        Ze = l("highlight", v, [Ye]),
+                        Je = l("renderFormatting", m, [w, $e, Ue, Xe, Ze, R, p, Ve, Ge, t.borderWidth]),
+                        Qe = l("renderFormattingRules", z, [Je]),
+                        et = l("renderFormatResolver", N, [Qe, c, We, Oe, R]),
+                        tt = l("inputFormatting", h, [w]),
+                        nt = l("inputFormattingRules", z, [tt]),
+                        ot = l("inputFormatResolver", N, [nt, c, We, Oe, R]),
+                        rt = l("editableCells", i, [je, ot, Fe, ze]),
+                        it = l("inputPlacement", ae, [rt, Ue, Fe, ze, Ne]),
+                        lt = l("isTextValid", ce, [d, rt]),
+                        st = function(e, t, n, o) {
                             const r = {
-                                    width: n.getBoundingClientRect().width,
-                                    height: n.getBoundingClientRect().height
+                                    width: o.getBoundingClientRect().width,
+                                    height: o.getBoundingClientRect().height
                                 },
                                 i = {
-                                    left: n.scrollLeft,
-                                    top: n.scrollTop
+                                    left: o.scrollLeft,
+                                    top: o.scrollTop
                                 },
-                                l = e || J,
-                                s = Y({
+                                l = e || oe,
+                                s = ee({
                                     left: 0,
                                     top: 0,
                                     ...t
-                                }, o),
-                                a = Y({
+                                }, n),
+                                a = ee({
                                     ...i,
                                     ...r
-                                }, o),
-                                c = $(s, V(a, X)),
-                                u = $(s, V(a, Z));
-                            return q(s, l) && q(l, c) ? G(l) > 2 * G(u) ? u : l : u
-                        }(n?.scrollRect, je, Ue, e.element);
-                    r("activeColumns", Te, [Be, t.onActiveColumnsChange]), r("activeRows", Te, [Se, t.onActiveRowsChange]), e.state = {
+                                }, n),
+                                c = Z(s, J(a, te)),
+                                u = Z(s, J(a, ne));
+                            return X(s, l) && X(l, c) ? Q(l) > 2 * Q(u) ? u : l : u
+                        }(o?.scrollRect, qe, He, r);
+                    l("activeColumns", Ke, [Oe, t.onActiveColumnsChange]), l("activeRows", Ke, [We, t.onActiveRowsChange]), e.state = {
                         options: t,
-                        devicePixelRatio: l,
-                        borderWidth: s,
-                        data: a,
+                        devicePixelRatio: s,
+                        borderWidth: a,
+                        data: c,
                         dataFormatting: w,
-                        edition: x,
-                        filteredColumns: re,
-                        filteredRows: ie,
-                        columns: Be,
-                        rows: Se,
+                        edition: R,
+                        filteredColumns: U,
+                        filteredRows: j,
+                        columns: Oe,
+                        rows: We,
                         sections: Ne,
-                        selectedCells: ze,
-                        selection: Ge,
-                        highlight: Ye,
-                        hoveredCell: He,
-                        focusedCell: Fe,
-                        renderFormatting: Xe,
-                        renderFormatResolver: Je,
-                        inputFormatting: Qe,
-                        inputFormatResolver: tt,
-                        fixedSize: Ue,
-                        totalSize: je,
-                        textResolver: g,
-                        scrollRect: it,
-                        highlightedCells: Ve,
-                        inputPlacement: nt,
-                        columnLookup: Ke,
-                        rowLookup: We,
-                        text: c,
-                        isTextValid: rt,
-                        resizableColumn: qe,
-                        resizableRow: $e
+                        selectedCells: je,
+                        selection: Xe,
+                        highlight: Ze,
+                        hoveredCell: $e,
+                        focusedCell: Ue,
+                        renderFormatting: Je,
+                        renderFormatResolver: et,
+                        inputFormatting: tt,
+                        inputFormatResolver: ot,
+                        fixedSize: He,
+                        totalSize: qe,
+                        textResolver: _,
+                        scrollRect: st,
+                        highlightedCells: Ye,
+                        inputPlacement: it,
+                        columnLookup: Fe,
+                        rowLookup: ze,
+                        text: d,
+                        isTextValid: lt,
+                        resizableColumn: Ve,
+                        resizableRow: Ge
                     }
                 }
 
-                function Le(e) {
+                function Fe(e) {
                     if (!e.error) try {
-                        Oe(e)
+                        We(e)
                     } catch (t) {
                         e.error = t
                     }
                 }
 
-                function Pe(e, t) {
-                    const o = new w(t);
-                    return [...t, ...e.filter((e => !o.isIdSelected(e.rowId, e.columnId)))]
+                function ze(e, t) {
+                    const n = new b(t);
+                    return [...t, ...e.filter((e => !n.isIdSelected(e.rowId, e.columnId)))]
                 }
 
-                function Be(e, t) {
-                    const o = new w(t);
-                    return e.filter((e => !o.isIdSelected(e.rowId, e.columnId)))
+                function Ue(e, t) {
+                    const n = new b(t);
+                    return e.filter((e => !n.isIdSelected(e.rowId, e.columnId)))
                 }
 
-                function Se(e) {
+                function Ne(e) {
                     const t = e.currentTarget.getBoundingClientRect();
                     return {
                         x: e.clientX - t.left,
                         y: e.clientY - t.top
                     }
                 }
 
-                function Ke(e) {
+                function je(e, t) {
+                    return e.map((e => ({
+                        ...e,
+                        columnId: "id" in e ? e.id : t,
+                        rowId: "id" in e ? e.id : t
+                    })))
+                }
+
+                function He(e) {
                     if ("spread-grid-context" in e) return;
                     console.log("initialize");
                     const t = {
                             "top-left": document.createElement("canvas"),
                             "top-center": document.createElement("canvas"),
                             "top-right": document.createElement("canvas"),
                             "middle-left": document.createElement("canvas"),
                             "middle-center": document.createElement("canvas"),
                             "middle-right": document.createElement("canvas"),
                             "bottom-left": document.createElement("canvas"),
                             "bottom-center": document.createElement("canvas"),
                             "bottom-right": document.createElement("canvas")
                         },
-                        o = document.createElement("input");
-                    e.setAttribute("tabindex", "0"), e.setAttribute("style", "max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;"), e.classList.add("spread-grid"), t["top-left"].setAttribute("style", "position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;"), t["top-center"].setAttribute("style", "position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;"), t["top-right"].setAttribute("style", "position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;"), t["middle-left"].setAttribute("style", "position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;"), t["middle-center"].setAttribute("style", "grid-row: 2; grid-column: 2; z-index: 0;"), t["middle-right"].setAttribute("style", "position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;"), t["bottom-left"].setAttribute("style", "position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;"), t["bottom-center"].setAttribute("style", "position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;"), t["bottom-right"].setAttribute("style", "position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;"), o.setAttribute("style", "position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;");
+                        n = document.createElement("input");
+                    e.setAttribute("tabindex", "0"), e.setAttribute("style", "max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;"), e.classList.add("spread-grid"), t["top-left"].setAttribute("style", "position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;"), t["top-center"].setAttribute("style", "position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;"), t["top-right"].setAttribute("style", "position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;"), t["middle-left"].setAttribute("style", "position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;"), t["middle-center"].setAttribute("style", "grid-row: 2; grid-column: 2; z-index: 0;"), t["middle-right"].setAttribute("style", "position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;"), t["bottom-left"].setAttribute("style", "position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;"), t["bottom-center"].setAttribute("style", "position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;"), t["bottom-right"].setAttribute("style", "position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;"), n.setAttribute("style", "position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;");
                     const l = {
                         externalOptions: {},
                         state: null,
                         memory: {},
                         element: e,
                         canvases: t,
-                        input: o,
+                        input: n,
                         renderRequested: !1,
                         mousePosition: null,
                         isMouseDown: !1,
                         columnWidthCache: new Map,
                         rowHeightCache: new Map,
                         requestNewRender: () => {
                             l.renderRequested || (l.renderRequested = !0, requestAnimationFrame((() => {
-                                l.renderRequested = !1, Le(l), u(l)
+                                l.renderRequested = !1, Fe(l), a(l)
                             })))
                         },
-                        addEventListener: (e, t, o) => {
+                        addEventListener: (e, t, n) => {
                             e.addEventListener(t, (e => {
                                 try {
-                                    o(e)
+                                    n(e)
                                 } catch (e) {
                                     e.message = `[${t} event]: ${e.message}`, l.error = e, l.requestNewRender()
                                 }
                             }))
                         }
                     };
                     l.localOptions = {
@@ -1956,16 +2079,16 @@
                         }],
                         formatting: [],
                         filtering: [],
                         sorting: [],
                         dataSelector: ({
                             data: e,
                             row: t,
-                            column: o
-                        }) => e[t.id][o.id],
+                            column: n
+                        }) => e?.[t.id]?.[n.id],
                         pinnedTop: 0,
                         pinnedBottom: 0,
                         pinnedLeft: 0,
                         pinnedRight: 0,
                         borderWidth: 1,
                         focusedCell: null,
                         onFocusedCellChange: e => {
@@ -1998,356 +2121,362 @@
                         onRowHeightsChange: e => {
                             l.localOptions.rowHeights = e, l.requestNewRender()
                         },
                         onActiveColumnsChange: () => {},
                         onActiveRowsChange: () => {}
                     }, e["spread-grid-context"] = l;
                     const s = e => {
-                            o.value = e, o.dispatchEvent(new Event("input"))
+                            n.value = e, n.dispatchEvent(new Event("input"))
                         },
-                        a = e => {
+                        c = e => {
                             const t = l.state.options.selectedCells,
-                                o = l.state.inputFormatResolver,
-                                n = l.state.columnLookup,
+                                n = l.state.inputFormatResolver,
+                                o = l.state.columnLookup,
                                 r = l.state.rowLookup,
                                 a = l.state.text,
                                 c = l.state.isTextValid,
                                 u = l.state.options.onEditedCellsChange,
                                 d = l.state.options.onFiltersChange,
-                                p = i(t, o, n, r);
+                                p = i(t, n, o, r);
                             if ("" === a) return;
                             if (!c) return;
                             if (e && !p.every((e => e.edit.autoCommit))) return;
-                            const h = p.filter((e => "DATA" === e.type)),
-                                f = p.filter((e => "FILTER" === e.type));
-                            var m;
-                            m = h.map((e => ({
+                            const f = p.filter((e => "DATA" === e.type)),
+                                h = p.filter((e => "FILTER" === e.type));
+                            var _;
+                            _ = f.map((e => ({
                                 ...e.cell,
                                 value: e.edit.parse({
                                     string: a
                                 })
-                            }))), u(Pe(l.state.options.editedCells, m)), (e => {
-                                d(Pe(l.state.options.filters, e))
-                            })(f.map((e => ({
+                            }))), u(ze(l.state.options.editedCells, _)), (e => {
+                                d(ze(je(l.state.options.filters, "FILTER"), e))
+                            })(h.map((e => ({
                                 ...e.cell,
                                 expression: e.edit.parse({
                                     string: a
                                 })
                             })))), e || s("")
                         },
-                        c = e => {
+                        u = e => {
                             const t = l.state.options.selectedCells,
-                                o = l.state.options.onEditedCellsChange,
-                                n = l.state.options.onFiltersChange,
+                                n = l.state.options.onEditedCellsChange,
+                                o = l.state.options.onFiltersChange,
                                 r = i(t, l.state.inputFormatResolver, l.state.columnLookup, l.state.rowLookup);
                             var s;
-                            e && !r.every((e => e.edit.autoCommit)) || (s = t, o(Be(l.state.options.editedCells, s)), (e => {
-                                n(Be(l.state.options.filters, e))
+                            e && !r.every((e => e.edit.autoCommit)) || (s = t, n(Ue(l.state.options.editedCells, s)), (e => {
+                                o(Ue(je(l.state.options.filters, "FILTER"), e))
                             })(t))
                         };
                     l.addEventListener(e, "scroll", (e => {
                         l.requestNewRender()
                     })), l.addEventListener(e, "mouseenter", (e => {
-                        l.mousePosition = Se(e), l.requestNewRender()
-                    })), l.addEventListener(e, "mousemove", (e => {
-                        if (l.mousePosition = Se(e), l.resizingColumn) {
-                            const e = l.state.columnLookup.get(n(l.resizingColumn)),
-                                t = e.width,
-                                o = e.right,
-                                r = l.mousePosition.x,
-                                i = Math.max(10, r - o + t),
-                                s = l.state.options.columnWidths.filter((t => n(t.columnId) !== e.key)).concat([{
-                                    columnId: e.id,
-                                    width: i
+                        l.mousePosition = Ne(e), l.requestNewRender()
+                    })), l.addEventListener(e, "mousemove", (t => {
+                        if (l.mousePosition = Ne(t), l.resizingColumn) {
+                            const t = l.state.columnLookup.get(o(l.resizingColumn)),
+                                n = t.width,
+                                r = t.right,
+                                i = re(e, l.mousePosition, l.state.fixedSize, l.state.totalSize),
+                                s = Math.max(10, i.x - r + n),
+                                a = l.state.options.columnWidths.filter((e => o(e.columnId) !== t.key)).concat([{
+                                    columnId: t.id,
+                                    width: s
                                 }]);
-                            l.state.options.onColumnWidthsChange(s)
+                            l.state.options.onColumnWidthsChange(a)
                         }
                         if (l.resizingRow) {
-                            const e = l.state.rowLookup.get(n(l.resizingRow)),
-                                t = e.height,
-                                o = e.bottom,
-                                r = l.mousePosition.y,
-                                i = Math.max(10, r - o + t),
-                                s = l.state.options.rowHeights.filter((t => n(t.rowId) !== e.key)).concat([{
-                                    rowId: e.id,
-                                    height: i
+                            const t = l.state.rowLookup.get(o(l.resizingRow)),
+                                n = t.height,
+                                r = t.bottom,
+                                i = re(e, l.mousePosition, l.state.fixedSize, l.state.totalSize),
+                                s = Math.max(10, i.y - r + n),
+                                a = l.state.options.rowHeights.filter((e => o(e.rowId) !== t.key)).concat([{
+                                    rowId: t.id,
+                                    height: s
                                 }]);
-                            l.state.options.onRowHeightsChange(s)
+                            l.state.options.onRowHeightsChange(a)
                         }
                         l.requestNewRender()
                     })), l.addEventListener(e, "mouseleave", (() => {
                         l.mousePosition = null, l.requestNewRender()
                     })), l.addEventListener(e, "mousedown", (e => {
-                        Le(l), s(""), l.isMouseDown = !0, l.mouseDownPosition = l.mousePosition, l.mouseDownCell = l.state.hoveredCell, l.state.resizableColumn && (l.resizingColumn = l.state.resizableColumn), l.state.resizableRow && (l.resizingRow = l.state.resizableRow), l.state.resizableColumn || l.state.resizableRow || l.state.options.onFocusedCellChange(l.state.hoveredCell), e.ctrlKey || l.state.options.onSelectedCellsChange([]), l.requestNewRender()
+                        Fe(l), s(""), l.isMouseDown = !0, l.mouseDownPosition = l.mousePosition, l.mouseDownCell = l.state.hoveredCell, l.state.resizableColumn && (l.resizingColumn = l.state.resizableColumn), l.state.resizableRow && (l.resizingRow = l.state.resizableRow), l.state.resizableColumn || l.state.resizableRow || l.state.options.onFocusedCellChange(l.state.hoveredCell), e.ctrlKey || l.state.options.onSelectedCellsChange([]), l.requestNewRender()
                     })), l.addEventListener(e, "mouseup", (e => {
-                        Le(l), l.isMouseDown = !1, l.resizingColumn = null, l.resizingRow = null, l.state.options.onSelectedCellsChange(Pe(l.state.options.selectedCells, l.state.highlightedCells)), l.requestNewRender()
+                        Fe(l), l.isMouseDown = !1, l.resizingColumn = null, l.resizingRow = null, l.state.options.onSelectedCellsChange(ze(l.state.options.selectedCells, l.state.highlightedCells)), l.requestNewRender()
                     })), l.addEventListener(e, "pointerdown", (e => {
                         l.element.setPointerCapture(e.pointerId)
                     })), l.addEventListener(e, "pointerup", (e => {
                         l.element.releasePointerCapture(e.pointerId)
                     })), l.addEventListener(e, "click", (e => {
-                        Le(l);
+                        Fe(l);
                         const t = l.state.hoveredCell,
-                            o = l.mouseDownCell;
+                            n = l.mouseDownCell;
                         if (l.state.resizableColumn || l.state.resizableRow) return;
                         if (null === t) return;
-                        if (n(t.columnId) !== n(o.columnId)) return;
-                        if (n(t.rowId) !== n(o.rowId)) return;
-                        const i = l.state.columnLookup.get(n(t.columnId)),
-                            s = l.state.rowLookup.get(n(t.rowId)),
+                        if (o(t.columnId) !== o(n.columnId)) return;
+                        if (o(t.rowId) !== o(n.rowId)) return;
+                        const i = l.state.columnLookup.get(o(t.columnId)),
+                            s = l.state.rowLookup.get(o(t.rowId)),
                             a = l.state.options.sortBy,
                             c = l.state.inputFormatResolver.resolve(s, i);
                         if (c.edit?.toggle) {
-                            const e = function(e, t, o, n) {
-                                    const r = n.hasValueByKey(o.key, t.key) ? n.getValueByKey(o.key, t.key) : e.value,
+                            const e = function(e, t, n, o) {
+                                    const r = o.hasValueByKey(n.key, t.key) ? o.getValueByKey(n.key, t.key) : e.value,
                                         i = e.edit.toggle;
                                     return "function" == typeof i ? i({
                                         value: r
                                     }) : i[(i.indexOf(r) + 1) % i.length]
                                 }(c, i, s, l.state.edition),
-                                o = r(i, s);
-                            "DATA" === o && l.state.options.onEditedCellsChange(Pe(l.state.options.editedCells, [{
+                                n = r(i, s);
+                            "DATA" === n && l.state.options.onEditedCellsChange(ze(l.state.options.editedCells, [{
                                 ...t,
                                 value: e
-                            }])), "FILTER" === o && l.state.options.onFiltersChange(Pe(l.state.options.filters, [{
+                            }])), "FILTER" === n && l.state.options.onFiltersChange(ze(l.state.options.filters, [{
                                 ...t,
                                 expression: e
                             }]))
                         } else if ("DATA" === i.type && "DATA" === s.type) l.state.options.onCellClick(l.state.hoveredCell);
                         else if ("CUSTOM" === i.type || "CUSTOM" === s.type) l.state.options.onCustomCellClick(l.state.hoveredCell);
                         else if ("HEADER" === i.type || "HEADER" === s.type) {
-                            const t = function(e, t, o, r) {
+                            const t = function(e, t, n, r) {
                                 function i(e) {
-                                    return t.key === n(e.columnId || "HEADER") && o.key === n(e.rowId || "HEADER")
+                                    const r = "columnId" in e ? e.columnId : "HEADER",
+                                        i = "rowId" in e ? e.rowId : "HEADER";
+                                    return t.key === o(r) && n.key === o(i)
                                 }
                                 const l = ["ASC", "DESC", void 0],
                                     s = e.find(i),
                                     a = l.indexOf(s?.direction),
                                     c = l[(a + 1) % l.length],
                                     u = e.indexOf(s) === e.length - 1;
-                                return [...!r || !u && s ? [] : e.filter((e => !i(e))), ...c ? [{
+                                return [...!r || !u && s ? e.filter((e => ! function(e) {
+                                    const r = "columnId" in e ? e.columnId : "HEADER",
+                                        i = "rowId" in e ? e.rowId : "HEADER";
+                                    return "HEADER" === t.type && t.key === o(r) || "HEADER" === n.type && n.key === o(i)
+                                }(e))) : e.filter((e => !i(e))), ...c ? [{
                                     columnId: t.id,
-                                    rowId: o.id,
+                                    rowId: n.id,
                                     direction: c
                                 }] : []]
                             }(a, i, s, e.ctrlKey);
                             l.state.options.onSortByChange(t), l.state.options.onSelectedCellsChange([])
                         }
                     })), l.addEventListener(e, "dblclick", (e => {
-                        if (Le(l), l.state.resizableColumn) {
-                            const e = n(l.state.resizableColumn),
-                                t = l.state.options.columnWidths.filter((t => n(t.columnId) !== e));
+                        if (Fe(l), l.state.resizableColumn) {
+                            const e = o(l.state.resizableColumn),
+                                t = l.state.options.columnWidths.filter((t => o(t.columnId) !== e));
                             l.state.options.onColumnWidthsChange(t), l.columnWidthCache.delete(e)
                         }
                         if (l.state.resizableRow) {
-                            const e = n(l.state.resizableRow),
-                                t = l.state.options.rowHeights.filter((t => n(t.rowId) !== e));
+                            const e = o(l.state.resizableRow),
+                                t = l.state.options.rowHeights.filter((t => o(t.rowId) !== e));
                             l.state.options.onRowHeightsChange(t), l.rowHeightCache.delete(e)
                         }
                         const t = l.state.focusedCell;
                         if (null === t) return;
-                        const r = n(t.columnId),
-                            i = n(t.rowId),
+                        const r = o(t.columnId),
+                            i = o(t.rowId),
                             a = l.state.columnLookup,
                             c = l.state.rowLookup,
                             u = l.state.inputFormatResolver;
                         if (!a.has(r)) return;
                         if (!c.has(i)) return;
                         const d = a.get(r),
                             p = c.get(i),
-                            h = u.resolve(p, d),
-                            f = h.text;
-                        h.edit && (h.edit.toggle || (s(f), o?.select()))
+                            f = u.resolve(p, d),
+                            h = f.text;
+                        f.edit && (f.edit.toggle || (s(h), n?.select()))
                     })), l.addEventListener(e, "focus", (() => {
-                        o.parentElement && o.focus({
+                        n.parentElement && n.focus({
                             preventScroll: !0
                         })
                     })), l.addEventListener(e, "keydown", (e => {
-                        Le(l);
+                        Fe(l);
                         const t = l.state.focusedCell,
-                            o = l.state.columnLookup,
+                            n = l.state.columnLookup,
                             r = l.state.rowLookup,
                             i = l.state.options.selectedCells,
-                            u = l.state.options.onSelectedCellsChange,
+                            a = l.state.options.onSelectedCellsChange,
                             d = l.state.options.onFocusedCellChange,
                             p = l.state.options.editedCells,
-                            h = l.state.options.onEditedCellsChange,
-                            f = l.state.columns,
-                            m = l.state.rows,
-                            _ = l.state.text,
+                            f = l.state.options.onEditedCellsChange,
+                            h = l.state.columns,
+                            _ = l.state.rows,
+                            m = l.state.text,
                             g = l.state.inputFormatResolver,
                             y = (e, t) => {
-                                d(e), t.shiftKey ? u(Pe(i, [e])) : u([e])
+                                d(e), t.shiftKey ? a(ze(i, [e])) : a([e])
                             },
-                            b = (e, r) => {
+                            w = (e, r) => {
                                 if (!t) return;
-                                const i = n(t.columnId);
-                                if (!o.has(i)) return;
-                                const l = o.get(i).index,
-                                    s = Math.max(0, Math.min(f.length - 1, l + e));
+                                const i = o(t.columnId);
+                                if (!n.has(i)) return;
+                                const l = n.get(i).index,
+                                    s = Math.max(0, Math.min(h.length - 1, l + e));
                                 if (s === l) return;
                                 const a = {
                                     rowId: t.rowId,
-                                    columnId: f[s].id
+                                    columnId: h[s].id
                                 };
                                 y(a, r)
                             },
-                            E = (e, o) => {
+                            E = (e, n) => {
                                 if (!t) return;
-                                const i = n(t.rowId);
+                                const i = o(t.rowId);
                                 if (!r.has(i)) return;
                                 const l = r.get(i).index,
-                                    s = Math.max(0, Math.min(m.length - 1, l + e));
+                                    s = Math.max(0, Math.min(_.length - 1, l + e));
                                 if (s === l) return;
                                 const a = {
-                                    rowId: m[s].id,
+                                    rowId: _[s].id,
                                     columnId: t.columnId
                                 };
-                                y(a, o)
+                                y(a, n)
                             },
                             v = () => {
                                 e.preventDefault(), e.stopPropagation()
                             };
                         switch (e.key) {
                             case "Escape":
-                                "" !== _ ? s("") : i.length > 1 ? u([t]) : p.length > 0 ? h([]) : (d(null), u([]));
+                                "" !== m ? s("") : i.length > 1 ? a([t]) : p.length > 0 ? f([]) : (d(null), a([]));
                                 break;
                             case "Enter":
-                                a();
+                                c();
                                 break;
                             case "ArrowUp":
-                                v(), E(e.ctrlKey ? -m.length : -1, e);
+                                v(), E(e.ctrlKey ? -_.length : -1, e);
                                 break;
                             case "ArrowDown":
-                                v(), E(e.ctrlKey ? m.length : 1, e);
+                                v(), E(e.ctrlKey ? _.length : 1, e);
                                 break;
                             case "ArrowLeft":
-                                v(), b(e.ctrlKey ? -f.length : -1, e);
+                                v(), w(e.ctrlKey ? -h.length : -1, e);
                                 break;
                             case "ArrowRight":
-                                v(), b(e.ctrlKey ? f.length : 1, e);
+                                v(), w(e.ctrlKey ? h.length : 1, e);
                                 break;
                             case "Delete":
                             case "Backspace":
-                                c();
+                                u();
                                 break;
                             case "c":
                                 (e => {
                                     if (!e.ctrlKey) return;
-                                    const t = function(e, t, o, r) {
+                                    const t = function(e, t, n, r) {
                                         const i = new Map(t.map((e => [e.key, e]))),
-                                            l = new Map(o.map((e => [e.key, e]))),
+                                            l = new Map(n.map((e => [e.key, e]))),
                                             s = e.map((e => ({
-                                                columnKey: n(e.columnId),
-                                                rowKey: n(e.rowId)
+                                                columnKey: o(e.columnId),
+                                                rowKey: o(e.rowId)
                                             }))).filter((e => i.has(e.columnKey) && l.has(e.rowKey))),
                                             a = new Set(s.map((e => e.columnKey))),
                                             c = new Set(s.map((e => e.rowKey)));
                                         if (0 === s.length) return "";
-                                        const u = new w(e),
+                                        const u = new b(e),
                                             d = Math.min(...s.map((e => i.get(e.columnKey).index))),
                                             p = Math.max(...s.map((e => i.get(e.columnKey).index))),
-                                            h = Math.min(...s.map((e => l.get(e.rowKey).index))),
-                                            f = Math.max(...s.map((e => l.get(e.rowKey).index))),
-                                            m = [];
-                                        for (let e = h; e <= f; e++) {
-                                            const n = o[e],
-                                                i = n.key;
+                                            f = Math.min(...s.map((e => l.get(e.rowKey).index))),
+                                            h = Math.max(...s.map((e => l.get(e.rowKey).index))),
+                                            _ = [];
+                                        for (let e = f; e <= h; e++) {
+                                            const o = n[e],
+                                                i = o.key;
                                             if (c.has(i)) {
                                                 for (let e = d; e <= p; e++) {
-                                                    const o = t[e],
-                                                        l = o.key;
+                                                    const n = t[e],
+                                                        l = n.key;
                                                     if (a.has(l)) {
                                                         if (u.isKeySelected(i, l)) {
-                                                            const e = r.resolve(n, o).text;
-                                                            m.push(e)
+                                                            const e = r.resolve(o, n).text;
+                                                            _.push(e)
                                                         }
-                                                        e < p && m.push("\t")
+                                                        e < p && _.push("\t")
                                                     }
                                                 }
-                                                e < f && m.push("\n")
+                                                e < h && _.push("\n")
                                             }
                                         }
-                                        return m.join("")
-                                    }(i, f, m, g);
+                                        return _.join("")
+                                    }(i, h, _, g);
                                     if (navigator.clipboard) navigator.clipboard.writeText(t);
                                     else {
                                         const e = document.createElement("textarea");
                                         e.value = t, document.body.appendChild(e), e.select(), document.execCommand("copy"), document.body.removeChild(e)
                                     }
                                 })(e)
                         }
                     })), new ResizeObserver((() => {
                         l.requestNewRender()
-                    })).observe(e), l.addEventListener(o, "input", (e => {
-                        Le(l), e.target.value ? (a(!0), o.style.opacity = 1, o.style.pointerEvents = "auto") : (e.isTrusted && c(!0), o.style.opacity = 0, o.style.pointerEvents = "none")
-                    })), l.addEventListener(o, "click", (e => {
+                    })).observe(e), l.addEventListener(n, "input", (e => {
+                        Fe(l), e.target.value ? (c(!0), n.style.opacity = 1, n.style.pointerEvents = "auto") : (e.isTrusted && u(!0), n.style.opacity = 0, n.style.pointerEvents = "none")
+                    })), l.addEventListener(n, "click", (e => {
                         e.stopPropagation()
-                    })), l.addEventListener(o, "dblclick", (e => {
+                    })), l.addEventListener(n, "dblclick", (e => {
                         e.stopPropagation()
-                    })), l.addEventListener(o, "mousedown", (e => {
+                    })), l.addEventListener(n, "mousedown", (e => {
                         e.stopPropagation()
-                    })), l.addEventListener(o, "keydown", (e => {
+                    })), l.addEventListener(n, "keydown", (e => {
                         switch (e.key) {
                             case "Enter":
                             case "Escape":
                                 break;
                             case "Delete":
                             case "Backspace":
                             case "ArrowUp":
                             case "ArrowDown":
                             case "ArrowLeft":
                             case "ArrowRight":
-                                "" !== o.value && (e.stopPropagation(), l.requestNewRender());
+                                "" !== n.value && (e.stopPropagation(), l.requestNewRender());
                                 break;
                             default:
                                 e.stopPropagation(), l.requestNewRender()
                         }
                     }))
                 }
 
-                function We(e, t) {
-                    console.log("createGrid"), Ke(e);
-                    const o = e["spread-grid-context"];
-                    o.externalOptions = t, null === o.state ? (Le(o), u(o)) : o.requestNewRender()
+                function qe(e, t) {
+                    console.log("createGrid"), He(e);
+                    const n = e["spread-grid-context"];
+                    n.externalOptions = t, null === n.state ? (Fe(n), a(n)) : n.requestNewRender()
                 }
             }
         },
         __webpack_module_cache__ = {};
 
     function __webpack_require__(e) {
         var t = __webpack_module_cache__[e];
         if (void 0 !== t) return t.exports;
-        var o = __webpack_module_cache__[e] = {
+        var n = __webpack_module_cache__[e] = {
             exports: {}
         };
-        return __webpack_modules__[e](o, o.exports, __webpack_require__), o.exports
+        return __webpack_modules__[e](n, n.exports, __webpack_require__), n.exports
     }
     __webpack_require__.n = e => {
         var t = e && e.__esModule ? () => e.default : () => e;
         return __webpack_require__.d(t, {
             a: t
         }), t
     }, __webpack_require__.d = (e, t) => {
-        for (var o in t) __webpack_require__.o(t, o) && !__webpack_require__.o(e, o) && Object.defineProperty(e, o, {
+        for (var n in t) __webpack_require__.o(t, n) && !__webpack_require__.o(e, n) && Object.defineProperty(e, n, {
             enumerable: !0,
-            get: t[o]
+            get: t[n]
         })
     }, __webpack_require__.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), __webpack_require__.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     };
     var getCurrentScript = function() {
             var e = document.currentScript;
             if (!e) {
-                for (var t = document.getElementsByTagName("script"), o = [], n = 0; n < t.length; n++) o.push(t[n]);
-                e = (o = o.filter((function(e) {
+                for (var t = document.getElementsByTagName("script"), n = [], o = 0; o < t.length; o++) n.push(t[o]);
+                e = (n = n.filter((function(e) {
                     return !e.async && !e.text && !e.textContent
                 }))).slice(-1)[0]
             }
             return e
         },
         isLocalScript = function(e) {
             return /\/_dash-component-suites\//.test(e.src)
@@ -2357,20 +2486,20 @@
             get: (url = getCurrentScript().src.split("/").slice(0, -1).join("/") + "/", function() {
                 return url
             })
         }), "undefined" != typeof jsonpScriptSrc) {
         var __jsonpScriptSrc__ = jsonpScriptSrc;
         jsonpScriptSrc = function(e) {
             var t = getCurrentScript(),
-                o = isLocalScript(t),
-                n = __jsonpScriptSrc__(e);
-            if (!o) return n;
-            var r = n.split("/"),
+                n = isLocalScript(t),
+                o = __jsonpScriptSrc__(e);
+            if (!n) return o;
+            var r = o.split("/"),
                 i = r.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v0_0_9m1712685293"), r.splice(-1, 1, i.join(".")), r.join("/")
+            return i.splice(1, 0, "v0_1_1m1716626761"), r.splice(-1, 1, i.join(".")), r.join("/")
         }
     }
     var __webpack_exports__ = {};
     (() => {
         __webpack_require__.r(__webpack_exports__), __webpack_require__.d(__webpack_exports__, {
             DashSpreadGrid: () => e.Z
         });
```

### Comparing `dash_spread_grid-0.0.9/dash_spread_grid/dash_spread_grid.min.js.map` & `dash_spread_grid-0.1.1/dash_spread_grid/dash_spread_grid.min.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8776788015618993%*

 * *Differences: {"'mappings'": "'2rGAMA,SAASA,SAASC,GACd,MAAwB,iBAAVA,GAAsBA,aAAiBC,MACzD,CAEA,SAASC,sBAAsBC,YAC3B,OAAOC,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,yEAEhB,OAAOF,WAAWG,KAAI,SAAAC,MAClB,IAAMC,WAAa,CAAC,EAkBpB,GAhBI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAC9D,UAAWJ,OACXC,WAAWR,MAAQY,KAAK,IAADC,OAAKR,QAAO,SAAAQ,OAAQN,KAAKP,MAAK,OACrD,SAAUO,OACVC,WAAWM,KAAOF,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKO,KAAI,OACpD,UAAWP,OACXC […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "dash_spread_grid.min.js",
-    "mappings": "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",
+    "mappings": "2rGAMA,SAASA,SAASC,GACd,MAAwB,iBAAVA,GAAsBA,aAAiBC,MACzD,CAEA,SAASC,sBAAsBC,YAC3B,OAAOC,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,yEAEhB,OAAOF,WAAWG,KAAI,SAAAC,MAClB,IAAMC,WAAa,CAAC,EAkBpB,GAhBI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAC9D,UAAWJ,OACXC,WAAWR,MAAQY,KAAK,IAADC,OAAKR,QAAO,SAAAQ,OAAQN,KAAKP,MAAK,OACrD,SAAUO,OACVC,WAAWM,KAAOF,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKO,KAAI,OACpD,UAAWP,OACXC,WAAWO,MAAQhB,SAASQ,KAAKQ,OAASH,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKQ,MAAK,MAAOR,KAAKQ,OACzF,YAAaR,OACbC,WAAWQ,QAAUjB,SAASQ,KAAKS,SAAWJ,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKS,QAAO,MAAOT,KAAKS,SAC/F,SAAUT,OACVC,WAAWS,KAAOL,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKU,KAAI,OACpD,SAAUV,KACV,GAAIA,KAAKW,KAAM,CACX,IAAMC,WAAa,CAAC,EAChB,aAAcZ,KAAKW,OACnBC,WAAWC,SAAWR,KAAK,kBAADC,OAAmBN,KAAKW,KAAKE,SAAQ,OAC/D,UAAWb,KAAKW,OAChBC,WAAWE,MAAQT,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKW,KAAKG,MAAK,OAC3D,gBAAiBd,KAAKW,OACtBC,WAAWG,WAAaf,KAAKW,KAAKK,aAClC,WAAYhB,KAAKW,OACjBC,WAAWK,OAASjB,KAAKW,KAAKM,QAClChB,WAAWU,KAAOC,UACtB,MAEIX,WAAWU,KAAOX,KAAKW,KAG/B,OAAOV,UACX,GACJ,GAAG,CAACL,YACR,CAEA,SAASsB,qBAAqBC,WAC1B,OAAOtB,EAAAA,mCAAAA,UAAQ,WACX,IAAMC,QAAU,8DAEhB,OAAOqB,UAAUpB,KAAI,SAAAC,MACjB,IAAMC,WAAa,CAAC,EASpB,MAPI,WAAYD,OACZC,WAAWC,OAASF,KAAKE,QACzB,QAASF,OACTC,WAAWE,IAAMH,KAAKG,KACtB,cAAeH,OACfC,WAAWG,UAAYC,KAAK,IAADC,OAAKR,QAAO,UAAAQ,OAASN,KAAKI,UAAS,OAE3DH,UACX,GACJ,GAAG,CAACkB,WACR,CAEA,SAASC,wBAAwBC,cAC7B,OAAOxB,EAAAA,mCAAAA,UAAQ,WACX,OAAOQ,KAAK,6BAADC,OAA8Be,aAAY,KACzD,GAAG,CAACA,cACR,CAIA,SAASC,eAAeC,GACpBC,QAAQC,MAAM,yBAEd,IAAMC,EAAWH,EAAMG,SACjBC,GAAUC,EAAAA,mCAAAA,QAAO,GAEjBC,EAAON,EAAMM,KACbC,EAAUP,EAAMO,QAChBC,EAAOR,EAAMQ,KACbnC,EAAaD,sBAAsB4B,EAAM3B,YACzCuB,EAAYD,qBAAqBK,EAAMJ,WACvCE,EAAeD,wBAAwBG,EAAMS,eAC7CC,EAAYV,EAAMW,WAClBC,EAAeZ,EAAMa,cACrBC,EAAad,EAAMe,YACnBC,EAAchB,EAAMiB,aACpBC,EAAUlB,EAAMkB,QAChBC,EAAcnB,EAAMoB,aACpBC,EAAgBrB,EAAMsB,eACtBC,GAAwBC,EAAAA,mCAAAA,cAAY,SAACH,GACvClB,EAAS,CAAEmB,eAAgBD,GAC/B,GAAG,CAAClB,IACEsB,GAAkBD,EAAAA,mCAAAA,cAAY,SAACN,GACjCf,EAAS,CAAEe,QAAAA,GACf,GAAG,CAACf,IACEuB,GAAsBF,EAAAA,mCAAAA,cAAY,SAACL,GACrChB,EAAS,CAAEiB,aAAcD,GAC7B,GAAG,CAAChB,IACEwB,EAAc3B,EAAM4B,aACpBC,GAAcL,EAAAA,mCAAAA,cAAY,SAACM,GAC7B3B,EAAS,CAAEyB,aAAYG,cAAAA,cAAA,GAAOD,GAAI,IAAEE,EAAG5B,EAAQ6B,aACnD,GAAG,CAAC9B,IACE+B,EAAoBlC,EAAMmC,oBAC1BC,GAAoBZ,EAAAA,mCAAAA,cAAY,SAACM,GACnC3B,EAAS,CAAEgC,oBAAmBJ,cAAAA,cAAA,GAAOD,GAAI,IAAEE,EAAG5B,EAAQ6B,aAC1D,GAAG,CAAC9B,IACEkC,GAAwBb,EAAAA,mCAAAA,cAAY,SAACc,GACvCnC,EAAS,CAAEoC,eAAgBD,GAC/B,GAAG,CAACnC,IACEqC,GAAqBhB,EAAAA,mCAAAA,cAAY,SAACiB,GACpCtC,EAAS,CAAEuC,YAAaD,GAC5B,GAAG,CAACtC,IAEwCwC,EAAAC,gBAAdC,EAAAA,mCAAAA,UAAS,MAAK,GAArCC,EAAOH,EAAA,GAAEI,EAAUJ,EAAA,GA4B1B,OA1BIG,IACAE,EAAAA,4CAAAA,GAAWF,EAAS,CAChBxC,KAAAA,EACAC,QAAAA,EACAC,KAAAA,EACAnC,WAAAA,EACAuB,UAAAA,EACAc,UAAAA,EACAE,aAAAA,EACAE,WAAAA,EACAE,YAAAA,EACAE,QAAAA,EACApB,aAAAA,EACAqB,YAAAA,EACAE,cAAAA,EACAE,sBAAAA,EACAG,oBAAAA,EACAD,gBAAAA,EACAE,YAAAA,EACAE,YAAAA,EACAK,kBAAAA,EACAE,kBAAAA,EACAC,sBAAAA,EACAG,mBAAAA,IAGDS,6CAAAA,cAAoB,MAAO,CAAEC,IAAKH,GAC7C,CAIAhD,eAAeoD,UAAY,CAEvBhD,SAAUiD,kDAAAA,KAEVC,GAAID,kDAAAA,OAEJ9C,KAAM8C,kDAAAA,IAEN7C,QAAS6C,kDAAAA,MAET5C,KAAM4C,kDAAAA,MAEN/E,WAAY+E,kDAAAA,MAEZxD,UAAWwD,kDAAAA,MAEXE,QAASF,kDAAAA,MAET3C,cAAe2C,kDAAAA,OAEfzC,WAAYyC,kDAAAA,OAEZvC,cAAeuC,kDAAAA,OAEfrC,YAAaqC,kDAAAA,OAEbnC,aAAcmC,kDAAAA,OAEdG,YAAaH,kDAAAA,OAEbI,YAAaJ,kDAAAA,OAEb9B,eAAgB8B,kDAAAA,MAEhBK,iBAAkBL,kDAAAA,MAElBhC,aAAcgC,kDAAAA,MAEdlC,QAASkC,kDAAAA,MAETM,QAASN,kDAAAA,MAETO,aAAcP,kDAAAA,MAEdQ,WAAYR,kDAAAA,MAEZxB,aAAcwB,kDAAAA,OAEdjB,oBAAqBiB,kDAAAA,OAErBb,eAAgBa,kDAAAA,MAEhBV,YAAaU,kDAAAA,OAGjBrD,eAAe8D,aAAe,CAC1BvD,KAAM,GACNC,QAAS,CAAC,CAAE,KAAQ,eACpBC,KAAM,CAAC,CAAE,KAAQ,UAAY,CAAE,KAAQ,eACvCnC,WAAY,GACZuB,UAAW,GACX0D,QAAS,GACT7C,cAAe,0BACfE,WAAY,EACZE,cAAe,EACfE,YAAa,EACbE,aAAc,EACdsC,YAAa,EACbC,YAAa,KACblC,eAAgB,GAChBmC,iBAAkB,GAClBrC,aAAc,GACdF,QAAS,GACTwC,QAAS,GACTC,aAAc,GACdC,WAAY,GACZhC,aAAc,KACdO,oBAAqB,KACrBI,eAAgB,GAChBG,YAAa,IAGjB,+C,SChPAoB,EAAOC,QAAUC,OAAkB,S,UCAnCF,EAAOC,QAAUC,OAAc,K,gBCehB,SAASC,EAAYC,GAChC,OAAY,OAARA,EACO,OAEPC,MAAMC,QAAQF,GAPX,IAQmBA,EAVA1F,IAAIyF,GAEPI,KAAK,QAUT,iBAARH,GAtBUI,EAuBMJ,EAjBpB,IALMK,OAAOC,KAAKF,GAAQG,OACRjG,KAAI0F,GAClB,GAAGA,KAAOD,EAAYK,EAAOJ,QAGjBG,KAAK,SAmBrBK,KAAKC,UAAUT,GAhB1B,IATyBI,CA0BzB,CC1Be,SAASM,EAAgBjG,EAAQC,GAC5C,MAAoB,WAAhBD,EAAOkG,KAAiC,WAAbjG,EAAIiG,KACxB,SACJ,MACX,CCDe,SAASC,EAAiBzD,EAAe0D,EAAgBC,EAAcC,GAClF,OAAO5D,EAAc7C,KAAIsD,IACrB,MAAMoD,EAAYjB,EAAYnC,EAAKqD,UAC7BC,EAASnB,EAAYnC,EAAKuD,OAEhC,IAAKL,EAAaM,IAAIJ,GAClB,OAAO,KACX,IAAKD,EAAUK,IAAIF,GACf,OAAO,KAEX,MAAMzG,EAASqG,EAAaO,IAAIL,GAC1BtG,EAAMqG,EAAUM,IAAIH,GAE1B,MAAO,CACHhG,KAAM2F,EAAeS,QAAQ5G,EAAKD,GAAQS,KAC1C0C,KAAMA,EACN+C,KAAMD,EAAgBjG,EAAQC,GAClC,IACD6G,QAAO3D,GAAQA,GAAM1C,MAC5B,CCtBe,SAASsG,EAAcxH,EAAOyH,GACzC,OAAOC,KAAKC,MAAM3H,EAAQyH,GAAoBA,CAClD,CCAA,SAASG,EAAcvH,EAASwH,EAAUC,GACtC,MAAMC,EAAQ1H,EAAQ0H,MAChBC,EAAS3H,EAAQ4H,SAAS,GAAGJ,KAAYC,KACzCI,EAAkBH,EAAMI,SAASN,GACjCO,EAAoBL,EAAMI,SAASL,GACnCzF,EAAU+F,EAAkB/F,QAC5BC,EAAO4F,EAAgB5F,KAE7B,GAAoB,IAAhBA,EAAK+F,QAAmC,IAAnBhG,EAAQgG,OAG7B,YAFIL,EAAOM,eACPN,EAAOM,cAAcC,YAAYP,IAIpCA,EAAOM,eACRjI,EAAQuE,QAAQ4D,YAAYR,GAGhCjG,QAAQ0G,IAAI,QAIZ,MAAMC,EAAMV,EAAOW,WAAW,KAAM,CAAEC,OAAO,IAEvCC,EAAad,EAAMc,WACnBC,EAAef,EAAMe,aAErBjC,EAAiBkB,EAAMgB,qBACvB1D,EAAc0C,EAAM1C,YACpB2D,EACGd,EAAgBe,cADnBD,EAEMd,EAAgBgB,iBAFtBF,EAGIZ,EAAkBe,eAHtBH,EAIKZ,EAAkBgB,gBAEvBC,EAAehE,EAAc,EAG7BiE,EAFWhH,EAAK+F,OAEmB,GAAKW,EAAqB,EAAI,IAAMA,EAAwB,EAAI,GACnGO,EAFclH,EAAQgG,OAEc,GAAKW,EAAsB,EAAI,IAAMA,EAAuB,EAAI,GACpGtD,EAAapD,EAAKhC,KAAII,GAAOA,EAAI8I,SACjC/D,EAAepD,EAAQ/B,KAAIG,GAAUA,EAAOgJ,QAC5CC,EAAajE,EAAakE,QAAO,CAACC,EAAGC,IAAMD,EAAIC,GAAG,GAAKN,EAAsBlE,EAC7EyE,EAAcpE,EAAWiE,QAAO,CAACC,EAAGC,IAAMD,EAAIC,GAAG,GAAKP,EAAwBjE,EAE9E0E,EAAsB,WAAfjC,EACPe,EAAWkB,KACX,EACAC,EAAmB,WAAbnC,EACNgB,EAAWmB,IACX,EACAP,EAAuB,WAAf3B,EACRe,EAAWY,MACXrB,EAAkBqB,MAClBD,EAAsB,WAAb3B,EACTgB,EAAWW,OACXtB,EAAgBsB,OAGhBS,EAAoBxE,EAAakE,QAAO,CAACO,EAAKT,EAAOU,KACvD,MACMC,EADaF,EAAIC,GACKV,EAAQpE,EAEpC,OADA6E,EAAIG,KAAKD,GACFF,CAAG,GACX,CAAClB,EAAsB3D,EAAc,IAClCiF,EAAkB5E,EAAWiE,QAAO,CAACO,EAAKV,EAAQW,KACpD,MACMC,EADaF,EAAIC,GACKX,EAASnE,EAErC,OADA6E,EAAIG,KAAKD,GACFF,CAAG,GACX,CAAClB,EAAqB3D,EAAc,IAEjCkF,EAAgBN,EAAkBO,MAAM,GAAI,GAC5CC,EAAaH,EAAgBE,MAAM,GAAI,GAEvCE,EAAwBhD,KAAKiD,IAAIJ,EAAcK,eAAcR,GAAUA,GAAUL,IAAO,GACxFc,EAAwBN,EAAcK,eAAcR,GAAUA,GAAUL,EAAON,IAC/EqB,EAAqBpD,KAAKiD,IAAIF,EAAWG,eAAcR,GAAUA,GAAUJ,IAAM,GACjFe,EAAqBN,EAAWG,eAAcR,GAAUA,GAAUJ,EAAMR,IAExEwB,EAAgCtD,KAAKiD,IAAID,EAAuB1B,EAAsB,EAAI,GAC1FiC,EAAgCJ,GAAyB7B,EAAuB,EAAI,GACpFkC,EAAkCxD,KAAKiD,IAAIG,EAAoB9B,EAAqB,EAAI,GACxFmC,EAAkCJ,GAAsB/B,EAAwB,EAAI,GAEpFoC,EAAQnF,MAAMoF,KAAK,CAAEhD,OAAQ0C,EAAqBD,EAAqB,IAAK,CAACQ,EAAGC,KAClF,MAAM7K,EAAM4B,EAAKiJ,EAAWT,GAC5B,OAAO7E,MAAMoF,KAAK,CAAEhD,OAAQwC,EAAwBH,EAAwB,IAAK,CAACY,EAAGE,KACjF,MAAM/K,EAAS4B,EAAQmJ,EAAcd,GACrC,OAAO7D,EAAeS,QAAQ5G,EAAKD,EAAO,GAC5C,IAEAgL,EAAU,CAACF,EAAUC,IAAgBJ,EAAMG,EAAWT,GAAoBU,EAAcd,GAE9F1C,EAAOyB,MAAQ/B,KAAKC,MAAM8B,EAAQhC,kBAClCO,EAAOwB,OAAS9B,KAAKC,MAAM6B,EAAS/B,kBACpCO,EAAOjH,MAAM0I,MAAQ,GAAGA,MACxBzB,EAAOjH,MAAMyI,OAAS,GAAGA,MACzBxB,EAAOjH,MAAM2K,WAAa,GAAG3B,MAC7B/B,EAAOjH,MAAM4K,UAAY,GAAG3B,MAC5BhC,EAAOjH,MAAM6K,YAAiBlC,EAAaD,EAAQM,EAAxB,KAC3B/B,EAAOjH,MAAM8K,aAAkB/B,EAAcN,EAASQ,EAA1B,KAE5BtB,EAAIoD,UAAY,UAChBpD,EAAIqD,SAAS,EAAG,EAAG/D,EAAOyB,MAAOzB,EAAOwB,QAExC,MAAMwC,EAAe,CAACC,EAAGC,KACrBxD,EAAIsD,aAAavE,iBAAkB,EAAG,EAAGA,kBAAmBwE,EAAIlC,GAAQtC,kBAAmByE,EAAIlC,GAAOvC,iBAAiB,EAErH0E,EAAU,CAACF,EAAGC,EAAGzC,EAAOD,KAC1Bd,EAAI0D,YACJ1D,EAAI2D,KAAKJ,EAAGC,EAAGzC,EAAOD,GACtBd,EAAI4D,MAAM,EAId,IAAK,IAAId,EAAcd,EAAuBc,GAAeX,EAAuBW,IAAe,CAC/F9C,EAAI6D,OACJP,EAAa/B,EAAkBuB,GAAc,GAC7CW,EAAQ,EAAG,EAAG1G,EAAa+F,GAAc1B,GAEzC,IAAK,IAAIyB,EAAWT,EAAoBS,GAAYR,EAAoBQ,IAAY,CAChF,MAAM3H,EAAO6H,EAAQF,EAAUC,GACzBzK,EAAQ6C,EAAK7C,MACbyL,EAAUlC,EAAgBiB,GAC1BkB,EAAWxC,EAAkBuB,GAC7BkB,EAAYjH,EAAa+F,GACzBmB,EAAajH,EAAW6F,GACxBzK,EAAO8C,EAAK9C,KACZ8L,EAAe7L,EAAM6L,cAAgB,SACrC5L,EAAU4C,EAAK5C,QAwBrB,GAtBAgL,EAAaS,EAAUD,GAEvB9D,EAAIoD,UAAY/K,EAAM8L,YAAc,QACpCnE,EAAIqD,SAAS,EAAG,EAAGW,EAAWC,GAE1B,SAAU/I,GACVA,EAAK3C,KAAKyH,GAEV3H,EAAM+L,YACNpE,EAAIoD,UAAY/K,EAAM+L,UACtBpE,EAAIqD,SAAS,EAAG,EAAGW,EAAWC,IAG9B5L,EAAMgM,SACNrE,EAAIoD,UAAY/K,EAAMgM,OACtBrE,EAAI0D,YACJ1D,EAAIsE,OAAON,EAAY,EAAGC,GAC1BjE,EAAIuE,OAAOP,EAAWC,GACtBjE,EAAIuE,OAAOP,EAAWC,EAAa,GACnCjE,EAAIwE,QAGJpM,EAAM,CACN4H,EAAIoD,UAAY/K,EAAMoM,YAAc,QACpCzE,EAAI0E,KAAOxJ,EAAKwJ,KAEhB,MAAMC,EAAcvE,EAAawE,eAAe1J,EAAKwJ,MAE/CG,EAAgC,UAAnBxM,EAAMwM,WAAyBzE,EAAa0E,aAAa1M,EAAM8C,EAAKwJ,MAAQV,EAAY1L,EAAQ+I,KAAO/I,EAAQyM,MAC5H,OACA1M,EAAMwM,WAAa,OACzB7E,EAAI6E,UAAYA,EAGhB,MAAMG,EAAQlG,EACI,SAAd+F,EAAuBvM,EAAQ+I,KACb,WAAdwD,EAAyBb,EAAY,EACnB,UAAda,EAAwBb,EAAY1L,EAAQyM,MACxC,EACZhG,kBAGEkG,EAAQnG,EACO,QAAjBoF,EAAyBS,EAAYO,OAASP,EAAYQ,UAAY7M,EAAQgJ,IACzD,WAAjB4C,EAA4BD,EAAa,EAAIU,EAAYO,OACpC,WAAjBhB,EAA4BD,EAAaU,EAAYO,OAASP,EAAYS,aAAe9M,EAAQ+M,OAC7F,EACZtG,kBAGmBkG,EAAQN,EAAYO,OAASP,EAAYQ,WAAa,GAAKF,EAAQN,EAAYO,OAASP,EAAYS,cAAgBnB,EAGvIjE,EAAIsF,SAASlN,EAAM4M,EAAOC,IAI1BjF,EAAIuF,YAAc,UAClBvF,EAAIwF,UAAY7I,EAEhBqD,EAAI0D,YACJ1D,EAAIsE,OAAO,EAAG3H,EAAcgE,GAC5BX,EAAIuE,OAAOP,EAAWrH,EAAcgE,GACpCX,EAAIsE,OAAO,EAAGL,EAAatH,EAAcgE,GACzCX,EAAIuE,OAAOP,EAAWC,EAAatH,EAAcgE,GACjDX,EAAIyF,SAEJzF,EAAI6D,OACJJ,EAAQ,EAAG,EAAI9G,EAAaqH,EAAWC,EAAa,EAAItH,GAExDqD,EAAIsF,SAASlN,EAAM4M,EAAOC,GAE1BjF,EAAI0F,UAEZ,CACJ,CAEA1F,EAAI0F,SACR,CAEApC,EAAa,EAAG,GAMhB,MAAMqC,EAAa,CAACC,EAAIC,EAAIC,EAAIC,EAAI1N,KAChC,IAAKA,EACD,OACJ,GAAoB,IAAhBA,EAAM0I,MACN,OAEJ,MAAMA,EAAQ1I,EAAM0I,MAAQhC,iBAEtBiH,EAAeH,IAAOE,EAGtBE,EAAKL,GAAMI,EAAejF,EAAQ,EAAI,GACtCmF,EAAKL,GAAOG,EAA2B,EAAZjF,EAAQ,GACnCoF,EAAKL,GAAME,EAAejF,EAAQ,EAAI,GACtCqF,EAAKL,GAAOC,EAA2B,EAAZjF,EAAQ,GAEzCf,EAAIuF,YAAclN,EAAMgO,OAAS,QACjCrG,EAAIwF,UAAYzE,EAEZ1I,EAAMiO,MACNtG,EAAIuG,YAAYlO,EAAMiO,KAAK1O,KAAIN,GAASA,EAAQyH,oBAChDiB,EAAIwG,eAAkBR,EAAeC,EAAKC,GAG1ClG,EAAIuG,YAAY,IAGpBvG,EAAI0D,YACJ1D,EAAIsE,OAAO2B,EAAIC,GACflG,EAAIuE,OAAO4B,EAAIC,GACfpG,EAAIyF,QAAQ,EAGVgB,EAAe,CAACC,EAAcC,IAC3BD,EAGAC,EAGDD,EAAajF,MAAQkF,EAAalF,MAC3BiF,EAEJC,EALID,EAHAC,EAYf,IAAK,IAAIC,EAAwBpE,EAAiCoE,GAAyBnE,EAAiCmE,IAAyB,CACjJ,MAAMC,EAAcD,EAAwB,EACtCE,EAAiBF,EAEvB,IAAK,IAAI9D,EAAcd,EAAuBc,GAAeX,EAAuBW,IAAe,CAC/F,MAGMiE,EAAcN,EAHGI,GAAezE,EAAqBW,EAAQ8D,EAAa/D,GAAazK,MAAM2O,aAAe,KACxFF,GAAkBzE,EAAqBU,EAAQ+D,EAAgBhE,GAAazK,MAAM4O,UAAY,MAIxHtB,EACIpE,EAAkBuB,GAAenC,EACjCiB,EAAgBkF,GAAkBnG,EAClCY,EAAkBuB,EAAc,GAAKnC,EACrCiB,EAAgBkF,GAAkBnG,EAClCoG,EACR,CACJ,CAEA,IAAK,IAAIG,EAAsB5E,EAA+B4E,GAAuB3E,EAA+B2E,IAAuB,CACvI,MAAMC,EAAkBD,EAAsB,EACxCE,EAAmBF,EAEzB,IAAK,IAAIrE,EAAWT,EAAoBS,GAAYR,EAAoBQ,IAAY,CAChF,MAGMkE,EAAcN,EAHIU,GAAmBnF,EAAwBe,EAAQF,EAAUsE,GAAiB9O,MAAMgP,YAAc,KACjGD,GAAoBjF,EAAwBY,EAAQF,EAAUuE,GAAkB/O,MAAMiP,WAAa,MAI5H3B,EACIpE,EAAkB6F,GAAoBzG,EACtCiB,EAAgBiB,GAAYlC,EAC5BY,EAAkB6F,GAAoBzG,EACtCiB,EAAgBiB,EAAW,GAAKlC,EAChCoG,EACR,CACJ,CACJ,CA+Fe,SAASQ,EAAO5P,GAC3B,IAAKA,EAAQ6P,MACT,KA3CR,SAAwB7P,GACpBuH,EAAcvH,EAAS,MAAO,QAC9BuH,EAAcvH,EAAS,MAAO,UAC9BuH,EAAcvH,EAAS,MAAO,SAC9BuH,EAAcvH,EAAS,SAAU,QACjCuH,EAAcvH,EAAS,SAAU,UACjCuH,EAAcvH,EAAS,SAAU,SACjCuH,EAAcvH,EAAS,SAAU,QACjCuH,EAAcvH,EAAS,SAAU,UACjCuH,EAAcvH,EAAS,SAAU,SA7DrC,SAAqBA,GACjB,MAAMuE,EAAUvE,EAAQuE,QAClBuL,EAAQ9P,EAAQ8P,MAChBpI,EAAQ1H,EAAQ0H,MAChBqI,EAAiBrI,EAAMqI,eAE7B,IAAKA,EAAgB,CACjB,GAAID,EAAM7H,cAAe,CACrB,MAAM+H,EAAWC,SAASC,gBAAkBJ,EAC5CA,EAAM7H,cAAcC,YAAY4H,GAC5BE,GACAzL,EAAQ4L,MAAM,CAAEC,eAAe,GACvC,CACA,MACJ,CAEA,MAAMzI,EAAS3H,EAAQ4H,SAASmI,EAAeM,SAc/C,GAZAP,EAAMpP,MAAMgJ,KAAO,SAAUqG,EAAiB,GAAGA,EAAerG,SAAW,IAC3EoG,EAAMpP,MAAMiJ,IAAM,QAASoG,EAAiB,GAAGA,EAAepG,QAAU,IACxEmG,EAAMpP,MAAM0M,MAAQ,UAAW2C,EAAiB,GAAGA,EAAe3C,UAAY,IAC9E0C,EAAMpP,MAAMgN,OAAS,WAAYqC,EAAiB,GAAGA,EAAerC,WAAa,IACjFoC,EAAMpP,MAAM2K,WAAa,eAAgB0E,EAAiB,GAAGA,EAAe1E,eAAiB,IAC7FyE,EAAMpP,MAAM4K,UAAY,cAAeyE,EAAiB,GAAGA,EAAezE,cAAgB,IAC1FwE,EAAMpP,MAAM0I,MAAQ,GAAG2G,EAAe3G,UACtC0G,EAAMpP,MAAMyI,OAAS,GAAG4G,EAAe5G,WACvC2G,EAAMpP,MAAM4P,SAAW3I,EAAOjH,MAAM4P,SACpCR,EAAMpP,MAAM6P,OAAS5I,EAAOjH,MAAM6P,OAClCT,EAAMpP,MAAM8P,gBAAkB9I,EAAM+I,YAAc,QAAU,WAEvDX,EAAM7H,cAAe,CACtB,MAAM+H,EAAWC,SAASC,gBAAkB3L,EAC5CA,EAAQ4D,YAAY2H,GAChBE,GACAF,EAAMK,MAAM,CAAEC,eAAe,GACrC,CACJ,CA2BIM,CAAY1Q,GAzBhB,SAAsBA,GAClB,MAAMuE,EAAUvE,EAAQuE,QAClBmD,EAAQ1H,EAAQ0H,MAElBA,EAAMiJ,iBAAmBjJ,EAAMkJ,aAC/BrM,EAAQ7D,MAAMmQ,OAAS,cAClBnJ,EAAMiJ,gBACXpM,EAAQ7D,MAAMmQ,OAAS,aAClBnJ,EAAMkJ,aACXrM,EAAQ7D,MAAMmQ,OAAS,aAEvBtM,EAAQ7D,MAAMmQ,OAAS,SAC/B,CAcIC,CAAa9Q,EACjB,CA+BY+Q,CAAe/Q,EACnB,CACA,MAAO6P,GACH7P,EAAQ6P,MAAQA,CACpB,CAGA7P,EAAQ6P,OApChB,SAAqB7P,GACjB,GAAIA,EAAQgR,cACR,OAEJhR,EAAQgR,eAAgB,EAExB,MAAMzM,EAAUvE,EAAQuE,QAClBsL,EAAQ7P,EAAQ6P,MAEtBtL,EAAQ7D,MAAM8P,gBAAkB,UAChCjM,EAAQ7D,MAAMgO,MAAQ,QACtBnK,EAAQ7D,MAAMC,QAAU,OACxB4D,EAAQ7D,MAAMuQ,QAAU,OACxB1M,EAAQ7D,MAAMwQ,cAAgB,SAC9B3M,EAAQ7D,MAAMyQ,WAAa,OAC3B5M,EAAQ6M,UAAY,0OAKVvB,EAAMwB,yFAE2CxB,EAAMyB,mBAErE,CAaQC,CAAYvR,EACpB,C,kBC3ZA,MAAMwR,EAAa,CACf7R,MAAO,EAAG8R,cAAeA,GAAY,GACrChR,KAAM,EAAGgR,cAAeA,GAAY,YACpC5Q,KAAM,CACFE,SAAU,KAAM,EAChBC,MAAO,EAAG0Q,YAAaA,EACvBzQ,YAAY,IAIL,SAAS0Q,EAAkB7R,EAAYyB,EAAcqQ,GAChE,MAAO,CACH,CACIxR,OAAQ,CAAEkG,KAAM,QAChBjG,IAAK,CAAEiG,KAAM,UACb3G,MAAO,EAAGS,iBAA+ByR,IAAlBzR,EAAO0R,OAAuB1R,EAAO0E,GAAK1E,EAAO0R,QAE5E,CACI1R,OAAQ,CAAEkG,KAAM,UAChBjG,IAAK,CAAEiG,KAAM,QACb3G,MAAO,EAAGU,cAAyBwR,IAAfxR,EAAIyR,OAAuBzR,EAAIyE,GAAKzE,EAAIyR,QAEhE,CACI1R,OAAQ,CAAEkG,KAAM,UAChBjG,IAAK,CAAEiG,KAAM,WACb3G,MAAO,IAEX,CACIS,OAAQ,CAAEkG,KAAM,WAChBjG,IAAK,CAAEiG,KAAM,UACb3G,MAAO,IAEX,CACIS,OAAQ,CAAEkG,KAAM,QAChBjG,IAAK,CAAEiG,KAAM,aACVkL,GAEP,CACIpR,OAAQ,CAAEkG,KAAM,UAChBjG,IAAK,CAAEiG,KAAM,WACVkL,GAEP,CACIpR,OAAQ,CAAEkG,KAAM,QAChBjG,IAAK,CAAEiG,KAAM,QACb3G,MAAO4B,MAERzB,KAEA8R,EAAO3R,KAAI,EAAG2G,WAAUE,QAAOiL,aAAajI,KAAU,CACrD1J,OAAQ,CAAE0E,GAAI8B,GACdvG,IAAK,CAAEyE,GAAIgC,GACXrG,KAAM,EAAGd,QAAOc,UAAW,GAAGmR,EAAO5J,OAAS,EAAI8B,EAAQ,EAAI,KAAmB,QAAdiI,EAAsB,IAAM,OAAOtR,GAAQd,QAG1H,CCvDA,MAAMqS,EAAe,CAAC,SAAU,MAAO,aAWvC,SAASC,EAAU/R,GAIjB,OAHgB8F,OAAOC,KAAK/F,GAAM8H,OACfhC,OAAOC,KAAK/F,GAAMgH,QAAOvB,GAAOqM,EAAaE,SAASvM,KAAMqC,MAGjF,CAEe,SAASmK,EAAqBrS,EAAYsS,GACvD,MAAMC,EAAiB,IAAIL,KAAiBI,GAE5C,OAAOtS,EAAWG,KAAIC,GAnBxB,SAAgBA,EAAMkS,GACpB,MAAME,EAAc,CAAC,EACrB,IAAK,MAAMC,KAASH,EACdG,KAASrS,IACXoS,EAAYC,GAASrS,EAAKqS,IAE9B,OAAOD,CACT,CAYgChJ,CAAOpJ,EAAMmS,KAAiBnL,OAAO+K,EACrE,CCpBe,SAASO,EAAmB1S,GACvC,OAAOqS,EAAqBrS,EAAY,CAAC,QAAS,OAAQ,QAC9D,CCFA,SAAS2S,EAAkBC,EAAWC,GAClC,OAAIA,EACOD,EAAY,KAEZA,EAAY,IAC3B,CAEe,SAASE,EAAoB9S,EAAY+S,EAAa5N,EAAa6N,EAAWrG,EAAWsG,EAASnB,EAAQjB,EAAiBC,EAAc5L,GACpJ,MAAMgO,EAAmB/N,EAAcS,EAAYT,EAAY2B,UAAY,KACrEqM,EAAgBhO,EAAcS,EAAYT,EAAY6B,OAAS,KAE/DoM,EAAiC,OAAjBtC,EAChBuC,EAFuC,OAApBxC,GAEcuC,EACjCE,EAAuBpO,EAAc,EACrCqO,EAAuBrO,EAAc,EAErCsO,EAAa,CAACrR,EAAMD,EAASkJ,EAAUC,KACzC,GAAID,EAAW,GAAKA,GAAYjJ,EAAK+F,OACjC,OAAO,EACX,GAAImD,EAAc,GAAKA,GAAenJ,EAAQgG,OAC1C,OAAO,EAEX,MAAMnB,EAAS5E,EAAKiJ,GAAUvF,IACxBgB,EAAY3E,EAAQmJ,GAAaxF,IAEvC,OAAOmN,EAAUS,cAAc1M,EAAQF,EAAU,EAG/C6M,EAAW,CAAClT,EAAWI,IACrBJ,EACO,CAACI,GAED,GAGf,MAAO,CACH,CACIN,OAAQ,CAAEkG,KAAM,QAChBjG,IAAK,CAAEiG,KAAM,UACb5F,MAAO,EAAG+Q,eAAe,CAAGjF,WAAY,UAAWM,WAAY2E,EAAW,QAAU,UAAWgC,OAAQ,CAAErK,MAAO,EAAGsF,MAAO,WAE9H,CACItO,OAAQ,CAAEkG,KAAM,UAChBjG,IAAK,CAAEiG,KAAM,QACb5F,MAAO,EAAG+Q,eAAe,CAAGjF,WAAY,UAAWM,WAAY2E,EAAW,QAAU,UAAWgC,OAAQ,CAAErK,MAAO,EAAGsF,MAAO,WAE9H,CACItO,OAAQ,CAAEkG,KAAM,OAChBjG,IAAK,CAAEiG,KAAM,UACb5F,MAAO,CAAE8L,WAAY,UAAWiH,OAAQ,CAAErK,MAAOpE,EAAa0J,MAAO,UAEzE,CACItO,OAAQ,CAAEkG,KAAM,UAChBjG,IAAK,CAAEiG,KAAM,OACb5F,MAAO,CAAE8L,WAAY,UAAWiH,OAAQ,CAAErK,MAAOpE,EAAa0J,MAAO,UAEzE,CACItO,OAAQ,CAAEkG,KAAM,UAChBjG,IAAK,CAAEiG,KAAM,UACb5F,MAAO,CAAE8L,WAAY,eAEtB1M,KAOA0T,EAASX,IAAgBK,EAAe,CACvC9S,OAAQ,CAAEkG,KAAM,OAChBjG,IAAK,CAAEyE,GAAI+N,GAAa/L,OACxBpG,MAAO,CAAE+L,UAAW,kBAErB+G,EAASX,IAAgBM,EAAY,CACpC/S,OAAQ,CAAE0E,GAAI+N,GAAajM,UAC3BvG,IAAK,CAAEyE,GAAI+N,GAAa/L,OACxBpG,MAAO,CAAE+L,UAAW,eAExB,CACIrM,OAAQ,CAAEkG,KAAM,OAChBjG,IAAK,CAAEiG,KAAM,OACbhG,UAAW,EAAG2B,OAAMD,UAAS3B,MAAKD,YAAakT,EAAWrR,EAAMD,EAAS3B,EAAIyJ,MAAO1J,EAAO0J,OAC3FpJ,MAAO,EAAGuB,OAAMD,UAAS3B,MAAKD,SAAQS,WAAW,IACxCyS,EAAWrR,EAAMD,EAAS3B,EAAIyJ,MAAQ,EAAG1J,EAAO0J,OAA4G,CAAC,EAApG,CAAEwF,UAAW,CAAElG,MAAOgK,EAAsB1E,MAAO,UAAW5E,MAAO4J,OAAOC,sBACrIL,EAAWrR,EAAMD,EAAS3B,EAAIyJ,MAAQ,EAAG1J,EAAO0J,OAA+G,CAAC,EAAvG,CAAEuF,aAAc,CAAEjG,MAAOgK,EAAsB1E,MAAO,UAAW5E,MAAO4J,OAAOC,sBACxIL,EAAWrR,EAAMD,EAAS3B,EAAIyJ,MAAO1J,EAAO0J,MAAQ,GAAyG,CAAC,EAArG,CAAE6F,WAAY,CAAEvG,MAAOgK,EAAsB1E,MAAO,UAAW5E,MAAO4J,OAAOC,sBACtIL,EAAWrR,EAAMD,EAAS3B,EAAIyJ,MAAO1J,EAAO0J,MAAQ,GAA0G,CAAC,EAAtG,CAAE4F,YAAa,CAAEtG,MAAOgK,EAAsB1E,MAAO,UAAW5E,MAAO4J,OAAOC,mBAC5IlH,UAAWgG,EAAkB5R,EAAO,UAAY,UAAWmS,IAAqB5S,EAAOuF,KAAOsN,IAAkB5S,EAAIsF,QAG5H,CACIvF,OAAQ,CAAEkG,KAAM,OAChBjG,IAAK,CAAEiG,KAAM,OACbhG,UAAW,EAAGD,MAAKD,YAAaqM,EAAU8G,cAAclT,EAAIsF,IAAKvF,EAAOuF,KACxEjF,MAAO,EAAGL,MAAKD,aAAa,CACxBqM,UAAWgG,EAAkB,UAAWO,IAAqB5S,EAAOuF,KAAOsN,IAAkB5S,EAAIsF,WAGtG6N,EAASvO,EAAa,CACrB7E,OAAQ,CAAE0E,GAAIG,GAAa2B,UAC3BvG,IAAK,CAAEyE,GAAIG,GAAa6B,OACxBpG,MAAO,CAAE+L,UAAW,kBAErBmF,EAAO3R,KAAI,EAAG2G,WAAUE,QAAOiL,aAAajI,KAAU,CACrD1J,OAAQ,CAAE0E,GAAI8B,GACdvG,IAAK,CAAEyE,GAAIgC,GACXpG,MAAO,CAAE+L,UAAW,iBAExB,CACIrM,OAAQ,CAAEkG,KAAM,OAChBjG,IAAK,CAAEiG,KAAM,OACbhG,UAAW,EAAGO,UAAWA,EACzBH,MAAO,CAAEgM,OAAQ,cAErB,CACItM,OAAQ,CAAEkG,KAAM,OAChBjG,IAAK,CAAEiG,KAAM,OACbhG,UAAW,EAAGD,MAAKD,YAAa2S,EAAQa,cAAcvT,EAAIsF,IAAKvF,EAAOuF,KACtEjF,MAAO,CAAEgM,OAAQ,iBAElB8G,EAAS7C,EAAiB,CACzBvQ,OAAQ,CAAE0E,GAAI6L,GACdtQ,IAAK,CAAEiG,KAAM,UACb5F,MAAO,CAAEgP,YAAa,CAAEtG,MAAOiK,EAAsB3E,MAAO,wBAE7D8E,EAAS5C,EAAc,CACtBxQ,OAAQ,CAAEkG,KAAM,UAChBjG,IAAK,CAAEyE,GAAI8L,GACXlQ,MAAO,CAAE2O,aAAc,CAAEjG,MAAOiK,EAAsB3E,MAAO,qBAGzE,CCrIe,SAASmF,EAAY7R,EAASC,GACzC,MAAM6R,EAAY7R,EAAKiF,QAAO7G,GAAsB,UAAfA,EAAI0T,SAAoB/L,OACvDgM,EAAe/R,EAAKiF,QAAO7G,GAAsB,QAAfA,EAAI0T,SAAkB/L,OACxDiM,EAAehS,EAAK+F,OAAS8L,EAAYE,EACzCE,EAAalS,EAAQkF,QAAO9G,GAA4B,UAAlBA,EAAO2T,SAAoB/L,OACjEmM,EAAcnS,EAAQkF,QAAO9G,GAA4B,QAAlBA,EAAO2T,SAAkB/L,OAChEoM,EAAepS,EAAQgG,OAASkM,EAAaC,EAE7CE,EAAUpS,EAAKkI,MAAM,EAAG2J,GACxBQ,EAAarS,EAAKkI,MAAMlI,EAAK+F,OAASgM,EAAc/R,EAAK+F,QACzDuM,EAAatS,EAAKkI,MAAM2J,EAAW7R,EAAK+F,OAASgM,GACjDQ,EAAcxS,EAAQmI,MAAM,EAAG+J,GAC/BO,EAAezS,EAAQmI,MAAMnI,EAAQgG,OAASmM,EAAanS,EAAQgG,QACnE0M,EAAgB1S,EAAQmI,MAAM+J,EAAYlS,EAAQgG,OAASmM,GAE3DQ,EAAab,EAAY,EAGzBc,EAAiBV,EAAa,EAM9BW,EAPgBZ,EAAe,IAOSU,EAExCG,GAAuBH,EACvBI,IAXgBf,EAAe,GAc/BgB,EAVmBZ,EAAe,IAUSQ,EAE3CK,GAAwBL,EACxBM,IAdkBf,EAAc,GAgBhCgB,EAAY,CAAClT,EAAM2G,EAAeC,KACpC,GAAoB,IAAhB5G,EAAK+F,OACL,OAAO,EAEX,MAAM2B,EAAMf,EAAgB3G,EAAKmT,GAAG,GAAGC,cAAgBpT,EAAKmT,GAAG,GAAGzL,IAGlE,OAFed,EAAmB5G,EAAKmT,IAAI,GAAGE,iBAAmBrT,EAAKmT,IAAI,GAAG1H,QAE7D/D,CAAG,EAGjB4L,EAAW,CAACvT,EAAS8G,EAAgBC,KACvC,GAAuB,IAAnB/G,EAAQgG,OACR,OAAO,EAEX,MAAM0B,EAAOZ,EAAiB9G,EAAQoT,GAAG,GAAGI,eAAiBxT,EAAQoT,GAAG,GAAG1L,KAG3E,OAFcX,EAAkB/G,EAAQoT,IAAI,GAAGK,gBAAkBzT,EAAQoT,IAAI,GAAGhI,OAEjE1D,CAAI,EAUvB,MAAO,CACHC,IAAK,CACD1H,KAAMoS,EACNzL,eA3CiB,EA4CjBC,kBA3CoB,EA4CpBM,OAZUgM,EAAUd,GAjCH,GACG,IA8CxB3G,OAAQ,CACJzL,KAAMqS,EACN1L,cAAeiM,EACfhM,kBA/CuB,EAgDvBM,OAjBagM,EAAUb,EAAYO,GA/BZ,IAkD3BtH,OAAQ,CACJtL,KAAMsS,EACN3L,cAAekM,EACfjM,iBAAkBkM,EAClB5L,OAtBagM,EAAUZ,EAAYO,EAAqBC,IAwB5DrL,KAAM,CACF1H,QAASwS,EACT1L,gBAvDmB,EAwDnBC,iBAvDoB,EAwDpBK,MA3BUmM,EAASf,GA9BA,GACC,IA0DxBpH,MAAO,CACHpL,QAASyS,EACT3L,eAAgBkM,EAChBjM,iBA3DqB,EA4DrBK,MAhCWmM,EAASd,EAAcO,GA5Bb,IA8DzBU,OAAQ,CACJ1T,QAAS0S,EACT5L,eAAgBmM,EAChBlM,gBAAiBmM,EACjB9L,MArCYmM,EAASb,EAAeO,EAAsBC,IAwCtE,CCnGe,SAASS,EAAyB/S,EAAaD,GAC1D,MAAO,IAAIC,KAAgBD,EAAQ1C,KAAIiH,IAAU,CAAGN,SAAUM,EAAON,SAAUE,MAAOI,EAAOJ,MAAOnH,MAAOuH,EAAO0O,eACtH,CCAe,MAAMC,EACjB,WAAAC,CAAYlT,GACRmT,KAAKC,OAAS,IAAIC,IAElBrT,EAAYsT,SAAQ3S,IAChB,MAAMsD,EAASnB,EAAYnC,EAAKuD,OAC1BH,EAAYjB,EAAYnC,EAAKqD,UAE9BmP,KAAKC,OAAOjP,IAAIF,IACjBkP,KAAKC,OAAOG,IAAItP,EAAQ,IAAIoP,KAEhCF,KAAKC,OAAOhP,IAAIH,GAAQsP,IAAIxP,EAAWpD,EAAK5D,MAAM,GAE1D,CAEA,aAAAiU,CAAc/M,EAAQF,GAClB,OAAOoP,KAAKC,OAAOjP,IAAIF,IAAWkP,KAAKC,OAAOhP,IAAIH,GAAQE,IAAIJ,EAClE,CAEA,aAAAyP,CAAcvP,EAAQF,GAClB,GAAKoP,KAAKnC,cAAc/M,EAAQF,GAGhC,OAAOoP,KAAKC,OAAOhP,IAAIH,GAAQG,IAAIL,EACvC,CAEA,YAAA0P,CAAavP,EAAOF,GAChB,OAAOmP,KAAKnC,cAAclO,EAAYoB,GAAQpB,EAAYkB,GAC9D,CAEA,YAAA0P,CAAaxP,EAAOF,GAChB,OAAOmP,KAAKK,cAAc1Q,EAAYoB,GAAQpB,EAAYkB,GAC9D,EChCW,SAAS2P,EAAWC,GAC/B,OAAO,IAAIX,EAAQW,EACvB,CCHe,MAAMC,EACjB,WAAAX,CAAYhT,GACRiT,KAAKC,OAAS,IAAIC,IAElBnT,EAAcoT,SAAQ3S,IAClB,MAAMsD,EAASnB,EAAYnC,EAAKuD,OAC1BH,EAAYjB,EAAYnC,EAAKqD,UAE9BmP,KAAKC,OAAOjP,IAAIF,IACjBkP,KAAKC,OAAOG,IAAItP,EAAQ,IAAI6P,KAEhCX,KAAKC,OAAOhP,IAAIH,GAAQ8P,IAAIhQ,EAAU,GAE9C,CAEA,aAAA4M,CAAc1M,EAAQF,GAClB,OAAOoP,KAAKC,OAAOjP,IAAIF,IAAWkP,KAAKC,OAAOhP,IAAIH,GAAQE,IAAIJ,EAClE,CAEA,YAAAiQ,CAAa9P,EAAOF,GAChB,OAAOmP,KAAKxC,cAAc7N,EAAYoB,GAAQpB,EAAYkB,GAC9D,ECrBW,SAASiQ,EAAa/T,GACjC,OAAO,IAAI2T,EAAU3T,EACzB,CCJe,SAASgU,EAAWC,EAAehV,GAC9C,MAAgC,mBAAlBgV,EACRA,EAAchV,GACdgV,CACV,CCHe,SAASC,EAAUlN,EAAO9B,EAAQiP,EAAaC,GAC1D,OAAIpN,EAAQmN,EACD,QACPnN,GAAS9B,EAASkP,EACX,WADX,CAGJ,CCJA,SAASC,EAAYC,EAAUH,EAAaC,GACxC,OAAOE,EAASnX,KAAI,CAACsE,EAASuF,KAC1B,MAAMhF,EAAK,OAAQP,EAAUA,EAAQO,GAAKP,EAAQ+B,KAClD,MAAO,IACA/B,EACHO,GAAIA,EACJwB,KAAM/B,EAAQ+B,MAAQ,OACtBwD,MAAOA,EACPnE,IAAKD,EAAYZ,GACjBiP,OAAQiD,EAAUlN,EAAOsN,EAASpP,OAAQiP,EAAaC,GACvDpF,OAAQ,WAAYvN,EAAUA,EAAQuN,OAAShN,EAC/CuS,OAAQ9S,EAAQ8S,QAAU,GAC7B,GAET,CAEO,SAASC,EAAmBtV,EAASiV,EAAaC,EAAW9R,GAChE,MAAMmS,EAAe,IAAItB,IAAI7Q,EAAanF,KAAI,EAAG2G,WAAUwC,WAAY,CAAC1D,EAAYkB,GAAWwC,MAG/F,OAFwB+N,EAAYnV,EAASiV,EAAaC,GAEnCjX,KAAIG,IAAU,IAC9BA,EACHgJ,MAAOmO,EAAaxQ,IAAI3G,EAAOuF,KACzB4R,EAAavQ,IAAI5G,EAAOuF,KACxB,UAAWvF,EACPA,EAAOgJ,MACP,SAElB,CAEO,SAASoO,EAAgBvV,EAAMgV,EAAaC,EAAW7R,GAC1D,MAAMoS,EAAgB,IAAIxB,IAAI5Q,EAAWpF,KAAI,EAAG6G,QAAOqC,YAAa,CAACzD,EAAYoB,GAAQqC,MAGzF,OAFqBgO,EAAYlV,EAAMgV,EAAaC,GAEhCjX,KAAII,IAAO,IACxBA,EACH8I,OAAQsO,EAAc1Q,IAAI1G,EAAIsF,KACxB8R,EAAczQ,IAAI3G,EAAIsF,KACtB,WAAYtF,EACRA,EAAI8I,OACJ,SAElB,CC3CO,SAASuO,EAAiB1V,EAASoF,EAAkBpC,GACxD,IAAI0E,EAAO1E,EAEX,OAAOhD,EAAQ/B,KAAI,CAACG,EAAQ0J,KACxB,MACMV,EAAQjC,EADQ,UAAW/G,EAASA,EAAOgJ,MAAQ,IACdhC,GACrCuQ,EAAY,IACXvX,EACH0J,MAAOA,EACPV,MAAOA,EACPoM,eAAgB9L,EAAO1E,EACvB0E,KAAMA,EACN0D,MAAO1D,EAAON,EACdqM,gBAAiB/L,EAAON,EAAQpE,GAKpC,OAFA0E,GAAQiO,EAAUvO,MAAQpE,EAEnB2S,CAAS,GAExB,CAEO,SAASC,EAAc3V,EAAMmF,EAAkBpC,GAClD,IAAI2E,EAAM3E,EAEV,OAAO/C,EAAKhC,KAAI,CAACI,EAAKyJ,KAClB,MACMX,EAAShC,EADQ,WAAY9G,EAAMA,EAAI8I,OAAS,GACT/B,GACvCyQ,EAAS,IACRxX,EACHyJ,MAAOA,EACPX,OAAQA,EACRkM,cAAe1L,EAAM3E,EACrB2E,IAAKA,EACL+D,OAAQ/D,EAAMR,EACdmM,iBAAkB3L,EAAMR,EAASnE,GAKrC,OAFA2E,GAAOkO,EAAO1O,OAASnE,EAEhB6S,CAAM,GAErB,CC5CA,MAAMC,EAAc,eACdC,EAAiB,CAAEpO,IAAK,EAAGyD,MAAO,EAAGM,OAAQ,EAAGhE,KAAM,GCCtDsO,EAAc,CAChB,OAAU,CAAC,UACX,OAAU,CAAC,UACX,KAAQ,CAAC,QACT,OAAU,CAAC,UACX,IAAO,CAAC,SAAU,OAAQ,SAAU,UACpC,QAAW,CAAC,SAAU,SAAU,UAChCnG,UAAW,IAGf,MAAMoG,EACFC,MAAQ,IAAIjC,IACZkC,QAAU,IAAIlC,IACdmC,QAAU,IAAInC,IACdoC,OAAS,IAAIpC,IAGF,MAAMqC,EACjBtC,OAAS,IAAIiC,EACbM,UAAW,EAEX,OAAAC,CAAQpY,EAAQC,EAAKH,GAGjB,GAFA6V,KAAKwC,UAAW,EAEZ3S,MAAMC,QAAQzF,GACd,IAAK,MAAMqY,KAAKrY,EACZ2V,KAAKyC,QAAQC,EAAGpY,EAAKH,QAI7B,GAAI0F,MAAMC,QAAQxF,GACd,IAAK,MAAMqY,KAAKrY,EACZ0V,KAAKyC,QAAQpY,EAAQsY,EAAGxY,OAFhC,CAMAE,EAASA,EACH,OAAQA,EACJ,CAAEuF,IAAKD,EAAYtF,EAAO0E,KAC1B1E,EACJ,CAAEkG,KAAM,QACdjG,EAAMA,EACA,OAAQA,EACJ,CAAEsF,IAAKD,EAAYrF,EAAIyE,KACvBzE,EACJ,CAAEiG,KAAM,QAuBV,QAASlG,GACTuY,EAAc5C,KAAKC,OAAOkC,MAAO9X,EAAOuF,KACxC,UAAWvF,GACXuY,EAAc5C,KAAKC,OAAOmC,QAAS/X,EAAO0J,OAC1C,UAAW1J,GACXuY,EAAc5C,KAAKC,OAAOoC,QAAShY,EAAOwY,OAC9C,IAAK,MAAMtS,KAAQ0R,EAAY5X,EAAOkG,MAClCqS,EAAc5C,KAAKC,OAAOqC,OAAQ/R,EAzCtC,CAaA,SAASuS,EAAW7C,EAAQrQ,GACnBqQ,EAAOjP,IAAIpB,IACZqQ,EAAOG,IAAIxQ,EAAK,IAEpBqQ,EAAOhP,IAAIrB,GAAKqE,KAAK9J,EACzB,CAEA,SAASyY,EAAc3C,EAAQrQ,GACtBqQ,EAAOjP,IAAIpB,IACZqQ,EAAOG,IAAIxQ,EAAK,IAAIsS,GAEpB,QAAS5X,GACTwY,EAAW7C,EAAOhP,IAAIrB,GAAKuS,MAAO7X,EAAIsF,KACtC,UAAWtF,GACXwY,EAAW7C,EAAOhP,IAAIrB,GAAKwS,QAAS9X,EAAIyJ,OACxC,UAAWzJ,GACXwY,EAAW7C,EAAOhP,IAAIrB,GAAKyS,QAAS/X,EAAIuY,OAC5C,IAAK,MAAMtS,KAAQ0R,EAAY3X,EAAIiG,MAC/BuS,EAAW7C,EAAOhP,IAAIrB,GAAK0S,OAAQ/R,EAC3C,CAUJ,CAEA,QAAAwS,CAAS1Y,EAAQC,GACb,MAAM0Y,EAAQ,GAEd,IAAKhD,KAAKwC,SACN,OAAOQ,EAEX,SAASC,EAAYC,GACjB,IAAK,MAAM/Y,KAAQ+Y,EACfF,EAAM/O,KAAK9J,EACnB,CAEA,SAASgZ,EAAelD,GAChBA,EAAOkC,MAAMnR,IAAI1G,EAAIsF,MACrBqT,EAAYhD,EAAOkC,MAAMlR,IAAI3G,EAAIsF,MACjCqQ,EAAOmC,QAAQpR,IAAI1G,EAAIyJ,QACvBkP,EAAYhD,EAAOmC,QAAQnR,IAAI3G,EAAIyJ,QACnCkM,EAAOqC,OAAOtR,IAAI1G,EAAIiG,OACtB0S,EAAYhD,EAAOqC,OAAOrR,IAAI3G,EAAIiG,OACtC,IAAK,MAAMsS,KAASvY,EAAIgX,OAChBrB,EAAOoC,QAAQrR,IAAI6R,IACnBI,EAAYhD,EAAOoC,QAAQpR,IAAI4R,GAE3C,CAEI7C,KAAKC,OAAOkC,MAAMnR,IAAI3G,EAAOuF,MAC7BuT,EAAenD,KAAKC,OAAOkC,MAAMlR,IAAI5G,EAAOuF,MAC5CoQ,KAAKC,OAAOmC,QAAQpR,IAAI3G,EAAO0J,QAC/BoP,EAAenD,KAAKC,OAAOmC,QAAQnR,IAAI5G,EAAO0J,QAC9CiM,KAAKC,OAAOqC,OAAOtR,IAAI3G,EAAOkG,OAC9B4S,EAAenD,KAAKC,OAAOqC,OAAOrR,IAAI5G,EAAOkG,OACjD,IAAK,MAAMsS,KAASxY,EAAOiX,OACnBtB,KAAKC,OAAOoC,QAAQrR,IAAI6R,IACxBM,EAAenD,KAAKC,OAAOoC,QAAQpR,IAAI4R,IAG/C,OAAOG,CACX,ECjHJ,MAAMI,EAAc,CAAC,YAAa,cAAe,eAAgB,cAE3DC,EAAc,CAAErY,SAAU,KAAM,EAAMC,MAAO,EAAG0Q,YAAaA,GAGnE,SAAS2H,EAAa3Y,EAAOoJ,GACzB,MAAMwP,EAAW,IAAK5Y,GAEtB,GAAI,WAAY4Y,EAAU,CACtB,IAAK,MAAMC,KAAcJ,EACrBG,EAASC,GAAcD,EAAS7F,cAC7B6F,EAAS7F,MACpB,CAEA,IAAK,MAAM8F,KAAcJ,EACjBI,KAAcD,IACdA,EAASC,GAAc,IAAKD,EAASC,GAAazP,UAE1D,OAAOwP,CACX,CAYA,SAASE,EAAQtZ,EAAMF,GACnB,IAAkB,IAAdE,EAAKW,KAET,OAAkB,IAAdX,EAAKW,KACE,SAAUb,EAAUA,EAAQa,KAAOuY,EAC1C,SAAUpZ,EACH,IAAKA,EAAQa,QAASX,EAAKW,MAC/B,IAAKuY,KAAgBlZ,EAAKW,KACrC,CAMe,MAAM4Y,EACjB,WAAA3D,CAAYiD,GACRhD,KAAK2D,YAAc,IAAIpB,EAEvB,IAAK,MAAOxO,EAAO5J,KAAS6Y,EAAMY,UAAW,CACzC,MAAMC,EAAQ,CAAE9P,SAEZ,cAAe5J,IACf0Z,EAAMtZ,UAAYJ,EAAKI,WACvB,UAAWJ,IACX0Z,EAAMlZ,MAA8B,mBAAfR,EAAKQ,MAAuBR,EAAKQ,MAAQ,IAAMR,EAAKQ,OACzE,UAAWR,IACX0Z,EAAMja,MAA8B,mBAAfO,EAAKP,MAAuBO,EAAKP,MAAQ,IAAMO,EAAKP,OACzE,SAAUO,IACV0Z,EAAMnZ,KAA4B,mBAAdP,EAAKO,KAAsBP,EAAKO,KAAO,IAAMP,EAAKO,MACtE,SAAUP,IACV0Z,EAAM7M,KAA4B,mBAAd7M,EAAK6M,KAAsB7M,EAAK6M,KAAO,IAAM7M,EAAK6M,MACtE,YAAa7M,IACb0Z,EAAMjZ,QAAkC,mBAAjBT,EAAKS,QAAyBT,EAAKS,QAAU,IAAMT,EAAKS,SAC/E,SAAUT,IACV0Z,EAAM/Y,KAAOX,EAAKW,MAClB,SAAUX,IACV0Z,EAAMhZ,KAAOV,EAAKU,MAEtBmV,KAAK2D,YAAYlB,QAAQtY,EAAKE,OAAQF,EAAKG,IAAKuZ,EACpD,CACJ,CAEA,OAAA3S,CAAQlF,EAAME,EAAMD,EAAS3B,EAAKD,EAAQ2S,GACtC,MAAMgG,EAAQhD,KAAK2D,YACdZ,SAAS1Y,EAAQC,GACjB6F,MAAK,CAACqD,EAAGC,IAAMD,EAAEO,MAAQN,EAAEM,QAC3B5C,QAAO,CAACvH,EAAOmK,EAAO+P,IAAUla,EAAMmK,QAAU+P,EAAM/P,EAAQ,IAAIA,QAEvE,IAEIlJ,EAFAZ,EAAU,CAAE+B,OAAME,OAAMD,UAAS3B,MAAKD,UACtCM,EAAQ,CAAC,EAGTC,EAAUoX,EACVhL,EAAO+K,EAEP/E,EAAQa,cAAcvT,EAAIsF,IAAKvF,EAAOuF,OACtC3F,EAAU,IAAKA,EAASyR,SAAUsB,EAAQqD,cAAc/V,EAAIsF,IAAKvF,EAAOuF,OAE5E,IAAK,MAAMzF,KAAQ6Y,EACf,MAAI,cAAe7Y,IAASA,EAAKI,UAAUN,MAIvC,UAAWE,IACXF,EAAU,IAAKA,EAASL,MAAOO,EAAKP,MAAMK,KAC1C,UAAWE,IACXQ,EAAQ,IAAKA,KAAU2Y,EAAanZ,EAAKQ,MAAMV,GAAUE,EAAK4J,SAC9D,SAAU5J,IACVF,EAAU,IAAKA,EAASS,KAAMP,EAAKO,KAAKT,KACxC,SAAUE,IACV6M,EAAO7M,EAAK6M,KAAK/M,IACjB,YAAaE,IACbS,EAAU,IAAKA,KAAYT,EAAKS,QAAQX,KACxC,SAAUE,IACVF,EAAU,IAAKA,EAASa,KAAM2Y,EAAQtZ,EAAMF,KAC5C,SAAUE,GAAM,CAChB,MAAM4Z,EAAiB9Z,EACvBY,EAAQyH,GAAQnI,EAAKU,KAAK,IAAKkZ,EAAgBzR,OACnD,CAKJ,MAAM5H,EA7Fd,SAAiBT,GACb,MAAI,SAAUA,EACH,GAAGA,EAAQS,OAClB,aAAcT,EACP,GAAGA,EAAQyR,gBACAI,IAAlB7R,EAAQL,MACD,GAAGK,EAAQL,QACf,EACX,CAqFqBoa,CAAQ/Z,GACfga,EAAS,CACXtZ,QACAuZ,SAnCU,EAoCVxZ,OACAE,UACAoM,QAUJ,MAPI,UAAW/M,IACXga,EAAOra,MAAQK,EAAQL,OACvB,SAAUK,QAA4B6R,IAAjB7R,EAAQa,OAC7BmZ,EAAOnZ,KAAOb,EAAQa,WACbgR,IAATjR,IACAoZ,EAAOpZ,KAAOA,GAEXoZ,CACX,ECpIW,SAASE,EAAmBC,GACvC,OAAO,IAAIV,EAAgBU,EAC/B,CCJe,MAAMC,EACjB,WAAAtE,CAAYuE,EAAiBtY,EAAME,EAAMD,EAAS+Q,GAC9CgD,KAAKsE,gBAAkBA,EACvBtE,KAAKhU,KAAOA,EACZgU,KAAK9T,KAAOA,EACZ8T,KAAK/T,QAAUA,EACf+T,KAAKhD,QAAUA,CACnB,CAEA,OAAA9L,CAAQ5G,EAAKD,GACT,OAAO2V,KAAKsE,gBAAgBpT,QACxB8O,KAAKhU,KACLgU,KAAK9T,KACL8T,KAAK/T,QACL3B,EACAD,EACA2V,KAAKhD,QACb,ECfW,SAASuH,EAAkBD,EAAiBtY,EAAME,EAAMD,EAAS+Q,GAC5E,OAAO,IAAIqH,EAAeC,EAAiBtY,EAAME,EAAMD,EAAS+Q,EACpE,CCFA,SAASwH,EAAgB5X,EAAS6X,EAAYC,GAC1C,MAAMC,EAAe,IAAIzE,IACzB,IAAK,MAAM1S,KAAQZ,EAAS,CACxB,MAAMgY,EAAUjV,EAAYnC,EAAKiX,IAC3BI,EAAYlV,EAAYnC,EAAKkX,IAE9BC,EAAa3T,IAAI4T,IAClBD,EAAavE,IAAIwE,EAAS,IAAI1E,KAElCyE,EAAa1T,IAAI2T,GAASxE,IAAIyE,EAAWrX,EAAKqS,WAClD,CACA,OAAO8E,CACX,CAEO,SAASG,EAAgBlY,EAASmY,EAAgBT,EAAiBtY,EAAME,EAAMD,EAAS+Q,GAC3F,GAAuB,IAAnBpQ,EAAQqF,OACR,OAAO/F,EAEX,MAAMyY,EAAeH,EAAgB5X,EAAS,WAAY,SACpDoY,EAAkB/Y,EAAQkF,QAAO9G,GAA0B,WAAhBA,EAAOkG,MAAqBoU,EAAa3T,IAAI3G,EAAOuF,OAErG,OAA+B,IAA3BoV,EAAgB/S,OACT/F,EAEJA,EAAKiF,QAAO7G,IACf,IAAK,MAAMD,KAAU2a,EAAiB,CAClC,MAAMxX,EAAO8W,EAAgBpT,QAAQlF,EAAME,EAAMD,EAAS3B,EAAKD,EAAQ2S,GACjEiI,EAAgBN,EAAa1T,IAAI5G,EAAOuF,KAG9C,IAFgBmV,EAAe7T,QAAQlF,EAAME,EAAMD,EAAS3B,EAAKD,EAAQmD,EAAK5D,MAAO4D,EAAK9C,KAAMua,GAG5F,OAAO,CACf,CACA,OAAO,CAAI,GAEnB,CAEO,SAASC,EAAmBtY,EAASmY,EAAgBT,EAAiBtY,EAAME,EAAMD,EAAS+Q,GAC9F,GAAuB,IAAnBpQ,EAAQqF,OACR,OAAOhG,EAEX,MAAM0Y,EAAeH,EAAgB5X,EAAS,QAAS,YACjDuY,EAAejZ,EAAKiF,QAAO7G,GAAoB,WAAbA,EAAIiG,MAAqBoU,EAAa3T,IAAI1G,EAAIsF,OAEtF,OAA4B,IAAxBuV,EAAalT,OACNhG,EAEJA,EAAQkF,QAAO9G,IAClB,IAAK,MAAMC,KAAO6a,EAAc,CAC5B,MAAM3X,EAAO8W,EAAgBpT,QAAQlF,EAAME,EAAMD,EAAS3B,EAAKD,EAAQ2S,GACjEoI,EAAaT,EAAa1T,IAAI3G,EAAIsF,KAGxC,IAFgBmV,EAAe7T,QAAQlF,EAAME,EAAMD,EAAS3B,EAAKD,EAAQmD,EAAK5D,MAAO4D,EAAK9C,KAAM0a,GAG5F,OAAO,CACf,CACA,OAAO,CAAI,GAEnB,CC5De,SAASC,EAAazR,EAAK+D,EAAQhE,EAAM0D,GACpD,MAAO,CACHzD,IAAKA,EACL+D,OAAQA,EACRhE,KAAMA,EACN0D,MAAOA,EAEf,CCPe,SAASiO,EAAarZ,EAASC,GAC1C,MAAO,CACHmH,MAAOpH,EAAQgG,OAAShG,EAAQoT,IAAI,GAAGK,gBAAkB,EACzDtM,OAAQlH,EAAK+F,OAAS/F,EAAKmT,IAAI,GAAGE,iBAAmB,EAE7D,CCHe,MAAMgG,EACjB,WAAAxF,GACIC,KAAKpO,OAASsI,SAASsL,cAAc,UACrCxF,KAAK/V,QAAU+V,KAAKpO,OAAOW,WAAW,MACtCyN,KAAK/I,YAAc,IAAIiJ,GAC3B,CAEA,YAAA9I,CAAa1M,EAAMsM,GACf,IAAKtM,EACD,OAAO,EAEX,MAAM4H,EAAM0N,KAAK/V,QAIjB,OAHAqI,EAAI0E,KAAOA,GAAQ+K,EACCzP,EAAImT,YAAY/a,GAEjB2I,KACvB,CAEA,aAAAqS,CAAchb,EAAMsM,GAChB,IAAI2O,EAAQ,EACZ,IAAK,MAAMC,KAAQlb,EACF,OAATkb,GACAD,IAGR,OAAOA,EAAQ3F,KAAK9I,eAAeF,GAAM5D,MAC7C,CAEA,cAAA8D,CAAeF,GACX,MAAMpH,EAAMoH,EAEZ,GAAIgJ,KAAK/I,YAAYjG,IAAIpB,GACrB,OAAOoQ,KAAK/I,YAAYhG,IAAIrB,GAEhC,MAAM0C,EAAM0N,KAAK/V,QAGjBqI,EAAI0E,KAAOA,GAAQ+K,EAEnB,MAAM8D,EAAcvT,EAAImT,YAAY,KAE9BjO,GAAUqO,EAAYC,yBAA2BD,EAAYE,yBAA2B,EAKxF9O,EAAc,CAChBQ,UALcD,EAASqO,EAAYG,sBAMnCxO,QAASA,EACTE,aANiBmO,EAAYI,uBAAyBzO,EAOtDpE,OANWyS,EAAYG,sBAAwBH,EAAYI,wBAW/D,OAFAjG,KAAK/I,YAAYmJ,IAAIxQ,EAAKqH,GAEnBA,CACX,ECxDW,SAASiP,IACpB,OAAO,IAAIX,CACf,CCJO,SAASY,EAASC,EAAQnQ,GAC7B,OACIA,EAAKrC,KAAOwS,EAAOxS,KACnBqC,EAAKtC,MAAQyS,EAAOzS,MACpBsC,EAAKrC,IAAMqC,EAAK7C,QAAUgT,EAAOxS,IAAMwS,EAAOhT,QAC9C6C,EAAKtC,KAAOsC,EAAK5C,OAAS+S,EAAOzS,KAAOyS,EAAO/S,KAEvD,CAEO,SAAS6C,EAAKkQ,EAAQnQ,GACzB,MAAMoQ,EAAU,CACZzS,IAAKtC,KAAKiD,IAAI6R,EAAOxS,IAAKqC,EAAKrC,KAC/BD,KAAMrC,KAAKiD,IAAI6R,EAAOzS,KAAMsC,EAAKtC,MACjCN,MAAO/B,KAAKgV,IAAIF,EAAOzS,KAAOyS,EAAO/S,MAAO4C,EAAKtC,KAAOsC,EAAK5C,OAAS/B,KAAKiD,IAAI6R,EAAOzS,KAAMsC,EAAKtC,MACjGP,OAAQ9B,KAAKgV,IAAIF,EAAOxS,IAAMwS,EAAOhT,OAAQ6C,EAAKrC,IAAMqC,EAAK7C,QAAU9B,KAAKiD,IAAI6R,EAAOxS,IAAKqC,EAAKrC,MAGrG,OAAIyS,EAAQhT,OAAS,GAAKgT,EAAQjT,QAAU,EACjCiT,EAEJ,CACHzS,IAAKwS,EAAOxS,IACZD,KAAMyS,EAAOzS,KACbN,MAAO,EACPD,OAAQ,EAEhB,CAEO,SAASmT,EAAOtQ,EAAMuQ,GACzB,MAAO,CACH5S,IAAKqC,EAAKrC,IAAM4S,EAChB7S,KAAMsC,EAAKtC,KAAO6S,EAClBnT,MAAO4C,EAAK5C,MAAiB,EAATmT,EACpBpT,OAAQ6C,EAAK7C,OAAkB,EAAToT,EAE9B,CAEO,SAAS,EAAKvQ,GACjB,OAAOA,EAAK5C,MAAQ4C,EAAK7C,MAC7B,CAEO,SAASqT,GAASxQ,EAAMuQ,GAC3B,MAAO,CACH5S,IAAKqC,EAAKrC,IACVD,KAAMsC,EAAKtC,KACXN,MAAO/B,KAAKiD,IAAI,EAAG0B,EAAK5C,MAAQmT,EAAO7S,KAAO6S,EAAOnP,OACrDjE,OAAQ9B,KAAKiD,IAAI,EAAG0B,EAAK7C,OAASoT,EAAO5S,IAAM4S,EAAO7O,QAE9D,CC9CA,MAAM+O,GAAiB,IACjBC,GAAkB,IAClBC,GAAY,CACdjT,KAAM,EACNC,IAAK,EACLP,MAAO,EACPD,OAAQ,GCRG,SAASyT,GAAoBrY,EAASsY,EAAUC,EAAWC,GAExE,MAAMnR,EAAIiR,EAASjR,EACbC,EAAIgR,EAAShR,EAEbmR,EACEzY,EAAQ0Y,WADVD,EAECzY,EAAQ2Y,UAGTC,EACG5Y,EAAQ6Y,YADXD,EAEI5Y,EAAQ8Y,aAGlB,MAAO,CACLzR,EAAGA,GAAKkR,EAAUpT,KACdkC,EACAA,GAAKuR,EACHvR,EAAIoR,EACJpR,GAAKuR,EAAmBL,EAAU1P,MAChC2P,EAAU3T,MAAQ+T,EAAmBvR,EACrCA,EAAIoR,EACZnR,EAAGA,GAAKiR,EAAUnT,IACdkC,EACAA,GAAKsR,EACHtR,EAAImR,EACJnR,GAAKsR,EAAoBL,EAAUpP,OACjCqP,EAAU5T,OAASgU,EAAoBtR,EACvCA,EAAImR,EAEhB,CC/Be,SAASM,GAAUlG,GAC9B,OAAOA,EAAS9N,QAAO,CAAC0M,EAAQzR,IAAYyR,EAAOG,IAAI5R,EAAQoB,IAAKpB,IAAU,IAAI0R,IACtF,CCAe,SAASsH,GAAoBC,EAAarK,EAAYlO,EAAa4N,EAAa7Q,EAASC,EAAMwE,EAAcC,GACxH,IAAK8W,EACD,MAAO,GACX,GAAIrK,EACA,MAAO,GACX,IAAKN,EACD,MAAO,GACX,IAAK5N,EACD,MAAO,GAEX,MAAM+N,EAAmBtN,EAAYT,EAAY2B,UAC3CqM,EAAgBvN,EAAYT,EAAY6B,OACxC2W,EAAmB/X,EAAYmN,EAAYjM,UAC3C8W,EAAgBhY,EAAYmN,EAAY/L,OAE9C,IAAKL,EAAaM,IAAIiM,GAClB,MAAO,GACX,IAAKtM,EAAUK,IAAIkM,GACf,MAAO,GACX,IAAKxM,EAAaM,IAAI0W,GAClB,MAAO,GACX,IAAK/W,EAAUK,IAAI2W,GACf,MAAO,GAEX,MAAMC,EAAiBtW,KAAKgV,IAAI5V,EAAaO,IAAIgM,GAAkBlJ,MAAOrD,EAAaO,IAAIyW,GAAkB3T,OACvG8T,EAAiBvW,KAAKiD,IAAI7D,EAAaO,IAAIgM,GAAkBlJ,MAAOrD,EAAaO,IAAIyW,GAAkB3T,OACvG+T,EAAcxW,KAAKgV,IAAI3V,EAAUM,IAAIiM,GAAenJ,MAAOpD,EAAUM,IAAI0W,GAAe5T,OACxFgU,EAAczW,KAAKiD,IAAI5D,EAAUM,IAAIiM,GAAenJ,MAAOpD,EAAUM,IAAI0W,GAAe5T,OAE9F,OAAO9H,EAAQmI,MAAMwT,EAAgBC,EAAiB,GAAGG,SAAQ3d,GACtD6B,EAAKkI,MAAM0T,EAAaC,EAAc,GAAG7d,KAAII,IACzC,CACHyG,MAAOzG,EAAIyE,GACX8B,SAAUxG,EAAO0E,QAIjC,CCvBe,SAASkZ,GAAe5d,EAAQC,GAC3C,MAAMwH,EAjBV,SAA4BxH,GACxB,MAAmB,UAAfA,EAAI0T,OACG,MACQ,QAAf1T,EAAI0T,OACG,SACJ,QACX,CAW4BkK,CAAmB5d,GACrC0H,EAVV,SAA8B3H,GAC1B,MAAsB,UAAlBA,EAAO2T,OACA,OACW,QAAlB3T,EAAO2T,OACA,QACJ,QACX,CAI8BmK,CAAqB9d,GAE/C,MAAO,GAAGyH,KAAmBE,GACjC,CClBe,SAASoW,GAAkBC,EAAenZ,EAAawB,EAAcC,EAAWoB,GAC3F,IAAK7C,EACD,OAAO,KAEX,MAAM+N,EAAmBtN,EAAYT,EAAY2B,UAC3CqM,EAAgBvN,EAAYT,EAAY6B,OAE9C,IAAKL,EAAaM,IAAIiM,GAClB,OAAO,KACX,IAAKtM,EAAUK,IAAIkM,GACf,OAAO,KAEX,MAAM7S,EAASqG,EAAaO,IAAIgM,GAC1B3S,EAAMqG,EAAUM,IAAIiM,GAE1B,GAA6B,IAAzBmL,EAAcpW,OACd,OAAO,KAEX,MAAM6U,EAAW,CACbzT,MAAOhJ,EAAOgJ,MACdD,OAAQ9I,EAAI8I,OACZkH,QAAS2N,GAAe5d,EAAQC,IAGpC,OAAQA,EAAI0T,QACR,IAAK,QACD8I,EAASlT,IAAMtJ,EAAIsJ,IACnB,MACJ,IAAK,MACDkT,EAASnP,OAAS5F,EAAS6B,IAAIR,OAASrB,EAASyF,OAAOpE,OAASrB,EAAS4F,OAAOvE,OAAS9I,EAAIsJ,IAAMtJ,EAAI8I,OACxG,MACJ,QACI0T,EAASvR,UAAYjL,EAAIsJ,IAAM7B,EAAS6B,IAAIR,OAGpD,OAAQ/I,EAAO2T,QACX,IAAK,QACD8I,EAASnT,KAAOtJ,EAAOsJ,KACvB,MACJ,IAAK,MACDmT,EAASzP,MAAQtF,EAAS4B,KAAKN,MAAQtB,EAAS4N,OAAOtM,MAAQtB,EAASsF,MAAMhE,MAAQhJ,EAAOsJ,KAAOtJ,EAAOgJ,MAC3G,MACJ,QACIyT,EAASxR,WAAajL,EAAOsJ,KAAO5B,EAAS4B,KAAKN,MAG1D,OAAOyT,CACX,CClDe,SAASwB,GAAe5d,EAAM2d,GACzC,OAAOA,EAAcE,OAAM/a,GAAQA,EAAK1C,KAAKE,SAAS,CAAE2Q,OAAQjR,KACpE,CCFA,SAAS8d,GAAcnH,GACnB,OAAKxR,MAAMC,QAAQuR,GAGZA,EAASnX,KAAI,CAACgL,EAAGnB,IAAUA,IAFvB9D,OAAOC,KAAKmR,EAG3B,CAEA,SAASoH,GAAiBzc,GACtB,OAAOwc,GAAcxc,EACzB,CAEA,SAAS0c,GAAoB1c,GACzB,MAAMkE,EAAO,IAAIyQ,IAEjB,GAAI9Q,MAAMC,QAAQ9D,GACd,IAAK,MAAMwC,KAAWxC,EAClB,IAAK,MAAM+C,KAAMyZ,GAAcha,GAC3B0B,EAAK0Q,IAAI7R,QAGjB,IAAK,MAAMa,KAAO5D,EACd,IAAK,MAAM+C,KAAMyZ,GAAcxc,EAAK4D,IAChCM,EAAK0Q,IAAI7R,GAIrB,MAAO,IAAImB,EACf,CAEO,SAASyY,GAAmB1c,EAASD,GAGxC,IAFsBC,EAAQ2c,MAAKve,GAA0B,eAAhBA,EAAOkG,OAGhD,OAAOtE,EAEX,MAAM4c,EAAkB,GAExB,IAAK,MAAMxe,KAAU4B,EACjB,GAAoB,eAAhB5B,EAAOkG,KAAuB,CAC9B,MAAMuY,EAAM,aAAcze,EACpBA,EAAO0e,SAAS/c,GAChB0c,GAAoB1c,GAE1B,IAAK,MAAM+C,KAAM+Z,EACbD,EAAgB5U,KAAK,IACd5J,EACH0E,KACAwB,KAAM,QAGlB,MACIsY,EAAgB5U,KAAK5J,GAI7B,OAAOwe,CACX,CAEO,SAASG,GAAgB9c,EAAMF,GAGlC,IAFsBE,EAAK0c,MAAKte,GAAoB,eAAbA,EAAIiG,OAGvC,OAAOrE,EAEX,MAAM+c,EAAe,GAErB,IAAK,MAAM3e,KAAO4B,EACd,GAAiB,eAAb5B,EAAIiG,KAAuB,CAC3B,MAAMuY,EAAM,aAAcxe,EACpBA,EAAIye,SAAS/c,GACbyc,GAAiBzc,GAEvB,IAAK,MAAM+C,KAAM+Z,EACbG,EAAahV,KAAK,IACX3J,EACHyE,KACAwB,KAAM,QAGlB,MACI0Y,EAAahV,KAAK3J,GAI1B,OAAO2e,CACX,CClFA,MAAMC,GAAmB,EAAGxe,OAAMmV,gBAAiBnV,EAAKyR,SAAS0D,GAElD,MAAMsJ,GACjB,WAAApJ,CAAYiD,GACRhD,KAAK2D,YAAc,IAAIpB,EAEvB,IAAK,MAAMpY,KAAQ6Y,EAAO,CACtB,MAAMa,EAAQ,CACVuF,GAAIzZ,EAAY,OAAQxF,EAAOA,EAAKif,GAAK,UACzC7e,UAAWJ,EAAKI,WAAa2e,IAGjClJ,KAAK2D,YAAYlB,QAAQtY,EAAKE,OAAQF,EAAKG,IAAKuZ,EACpD,CACJ,CAEA,OAAA3S,CAAQlF,EAAME,EAAMD,EAAS3B,EAAKD,EAAQT,EAAOc,EAAMia,GACnD,MAAM3B,EAAQhD,KAAK2D,YAAYZ,SAAS1Y,EAAQC,GAEhD,GAAqB,IAAjB0Y,EAAM/Q,OACN,MAAiB,SAAb3H,EAAIiG,MAEY,SAAhBlG,EAAOkG,OAENoU,EAAa3T,IAAI,aAGfkY,GAAiB,CAAExe,OAAMmV,WAAY8E,EAAa1T,IAAI,cAGjE,IAAIhH,EAAU,CAAE+B,OAAME,OAAMD,UAAS3B,MAAKD,SAAQT,QAAOc,QAEzD,IAAK,MAAMP,KAAQ6Y,EAAO,CACtB,IAAK2B,EAAa3T,IAAI7G,EAAKif,IACvB,SAEJ,MAAMC,EAAgB,IAAKpf,EAAS4V,WAAY8E,EAAa1T,IAAI9G,EAAKif,KAEtE,IAAKjf,EAAKI,UAAU8e,GAChB,OAAO,CACf,CAEA,OAAO,CACX,EC5CW,SAASC,GAAkBhe,GACtC,OAAO,IAAI6d,GAAe7d,EAC9B,CCFe,SAASie,GAAoBxf,GACxC,OAAOqS,EAAqBrS,EAAY,CAAC,QAAS,QACtD,CCFe,SAASyf,GAAqBzf,GACzC,OAAOqS,EAAqBrS,EAAY,CAAC,QAAS,OAAQ,OAAQ,WACtE,CCAO,SAAS0f,GAAmBxd,EAASC,EAAMwG,EAAcjC,EAAgBiZ,EAAgBC,GAC5F,GAAI1d,EAAQsc,OAAMle,GAAkC,iBAAjBA,EAAOgJ,QACtC,OAAOpH,EAEX,MAAM2d,EAAgBvf,IAClB,MAAMwf,EAAiBxf,EAAOgJ,MAE9B,GAA8B,iBAAnBwW,EACP,OAAOA,EAEX,GAAIH,EAAe1Y,IAAI3G,EAAOuF,KAAM,CAChC,MAAMka,EAASJ,EAAezY,IAAI5G,EAAOuF,KAEzC,GAAuB,aAAnBia,IAAkCC,EAAOC,SACzC,OAAOD,EAAOzW,MAClB,GAAuB,kBAAnBwW,GAAsCC,EAAOC,SAC7C,OAAOD,EAAOzW,KACtB,CAEA,IAAIA,EAAQ,EACZ,IAAK,MAAM/I,KAAO4B,EAAM,CACpB,GAAiB,SAAb5B,EAAIiG,MAAsC,kBAAnBsZ,EACvB,SACJ,GAAiB,SAAbvf,EAAIiG,MAAsC,aAAnBsZ,EACvB,SAEJ,MAAMrc,EAAOiD,EAAeS,QAAQ5G,EAAKD,GACnCK,EAAO8C,EAAK9C,KACZsM,EAAOxJ,EAAKwJ,KACZpM,EAAU4C,EAAK5C,QAAQ+I,KAAOnG,EAAK5C,QAAQyM,MAE3Cf,EAAY5D,EAAa0E,aAAa1M,EAAMsM,GAAQpM,EAE1DyI,EAAQ/B,KAAKiD,IAAIlB,EAAOiD,EAC5B,CAOA,OALAoT,EAAetJ,IAAI/V,EAAOuF,IAAK,CAC3ByD,QACA0W,SAA6B,kBAAnBF,IAGPxW,CAAK,EAGhB,IAAK,MAAMzD,KAAO8Z,EAAexZ,OACxByZ,EAAY3Y,IAAIpB,IACjB8Z,EAAeM,OAAOpa,GAG9B,OAAO3D,EAAQ/B,KAAIG,IAAU,IACtBA,EACHgJ,MAAOuW,EAAcvf,MAE7B,CAEO,SAAS4f,GAAgBhe,EAASC,EAAMwG,EAAcjC,EAAgBiZ,EAAgBC,GACzF,GAAIzd,EAAKqc,OAAMje,GAA6B,iBAAfA,EAAI8I,SAC7B,OAAOlH,EAEX,MAAMge,EAAa5f,IACf,MAAM6f,EAAkB7f,EAAI8I,OAE5B,GAA+B,iBAApB+W,EACP,OAAOA,EAEX,GAAIT,EAAe1Y,IAAI1G,EAAIsF,KAAM,CAC7B,MAAMka,EAASJ,EAAezY,IAAI3G,EAAIsF,KAEtC,GAAwB,aAApBua,IAAmCL,EAAOC,SAC1C,OAAOD,EAAO1W,OAClB,GAAwB,kBAApB+W,GAAuCL,EAAOC,SAC9C,OAAOD,EAAO1W,MACtB,CAEA,IAAIA,EAAS,EACb,IAAK,MAAM/I,KAAU4B,EAAS,CAC1B,GAAoB,SAAhB5B,EAAOkG,MAAuC,kBAApB4Z,EAC1B,SACJ,GAAoB,SAAhB9f,EAAOkG,MAAuC,aAApB4Z,EAC1B,SAEJ,MAAM3c,EAAOiD,EAAeS,QAAQ5G,EAAKD,GACnCK,EAAO8C,EAAK9C,KACZsM,EAAOxJ,EAAKwJ,KACZpM,EAAU4C,EAAK5C,QAAQgJ,IAAMpG,EAAK5C,QAAQ+M,OAE1CpB,EAAa7D,EAAagT,cAAchb,EAAMsM,GAAQpM,EAE5DwI,EAAS9B,KAAKiD,IAAInB,EAAQmD,EAC9B,CAOA,OALAmT,EAAetJ,IAAI9V,EAAIsF,IAAK,CACxBwD,SACA2W,SAA8B,kBAApBI,IAGP/W,CAAM,EAGjB,IAAK,MAAMxD,KAAO8Z,EAAexZ,OACxByZ,EAAY3Y,IAAIpB,IACjB8Z,EAAeM,OAAOpa,GAG9B,OAAO1D,EAAKhC,KAAII,IAAO,IAChBA,EACH8I,OAAQ8W,EAAW5f,MAE3B,CChHe,SAAS8f,GAAQxG,GAC5B,OAAO,IAAIjD,IAAIiD,EAAQ1Z,KAAI2Z,GAASA,EAAMjU,MAC9C,CCAe,SAASya,GAAqBtgB,GACzC,OAAOqS,EAAqBrS,EAAY,CAAC,QAAS,QACtD,CCDA,SAASugB,GAAqBC,EAAKC,GAC/B,OAAiB1O,MAAbyO,EAAI3gB,QAESkS,MAAb0O,EAAI5gB,OAED2gB,EAAI3gB,MAAQ4gB,EAAI5gB,MAC3B,CAEA,SAAS6gB,GAAsBF,EAAKC,GAChC,OAAiB1O,MAAbyO,EAAI3gB,QAESkS,MAAb0O,EAAI5gB,OAED2gB,EAAI3gB,MAAQ4gB,EAAI5gB,MAC3B,CAEe,MAAM8gB,GACjB,WAAA3K,CAAYiD,GACRhD,KAAK2D,YAAc,IAAIpB,EAEvB,IAAK,MAAMpY,KAAQ6Y,EAAO,CACtB,MAAM2H,EAAgBxgB,EAAKygB,WACrB,CAACL,EAAKC,IAAQrgB,EAAKygB,WAAWL,EAAKC,GACnC,CAACD,EAAKC,IAAQF,GAAqBC,EAAKC,GACxCK,EAAiB1gB,EAAKygB,WACtB,CAACL,EAAKC,KAASrgB,EAAKygB,WAAWL,EAAKC,GACpC,CAACD,EAAKC,IAAQC,GAAsBF,EAAKC,GAEzC3G,EAAQ,CACVuF,GAAIzZ,EAAY,OAAQxF,EAAOA,EAAKif,GAAK,UACzCuB,cAAeA,EACfE,eAAgBA,GAGpB7K,KAAK2D,YAAYlB,QAAQtY,EAAKE,OAAQF,EAAKG,IAAKuZ,EACpD,CACJ,CAEA,OAAA3S,CAAQ7G,EAAQC,EAAKwgB,GACjB,MAAM9H,EAAQhD,KAAK2D,YAAYZ,SAAS1Y,EAAQC,GAEhD,GAAqB,IAAjB0Y,EAAM/Q,OACN,MAAiB,SAAb3H,EAAIiG,MAEY,SAAhBlG,EAAOkG,KADA,KAGNua,EAAa9Z,IAAI,YAGkB,QAAjC8Z,EAAa7Z,IAAI,YAClBqZ,GACAG,GAJK,KAOf,GAAIzH,EAAM/Q,OAAS,EACf,MAAM,IAAI8Y,MAAM,4CAEpB,MAAM5gB,EAAO6Y,EAAM,GAEnB,OAAK8H,EAAa9Z,IAAI7G,EAAKif,IAGU,QAA9B0B,EAAa7Z,IAAI9G,EAAKif,IACvBjf,EAAKwgB,cACLxgB,EAAK0gB,eAJA,IAKf,EClEW,SAASG,GAAgBhc,GACpC,OAAO,IAAI0b,GAAa1b,EAC5B,CCFA,SAASic,GAAgBpP,EAAQ4I,EAAYC,GACzC,MAAMoG,EAAe,IAAI5K,IACzB,IAAK,MAAM1S,KAAQqO,EAAQ,CACvB,MAAM+I,EAAUjV,EAAYnC,EAAKiX,IAC3BI,EAAYlV,EAAYnC,EAAKkX,IAE9BoG,EAAa9Z,IAAI4T,IAClBkG,EAAa1K,IAAIwE,EAAS,IAAI1E,KAElC4K,EAAa7Z,IAAI2T,GAASxE,IAAIyE,EAAWrX,EAAKwO,UAClD,CACA,OAAO8O,CACX,CAEA,SAASI,GAAMC,EAAMlH,GACjBkH,EAAKhb,MAAK,CAACoa,EAAKC,KACZ,MAAMvG,EAASsG,EAAIK,WAAWL,EAAI/c,KAAMgd,EAAIhd,MAC5C,MAAsB,iBAAXyW,EACAA,EACJA,GAAU,EAAI,CAAC,IAE1BA,EAAOhQ,QAAQkX,EAAKjhB,KAAI2Z,GAASA,EAAMuH,UACvCD,EAAKlZ,OAAS,CAClB,CAEO,SAASoZ,GAAcxP,EAAQyP,EAAchH,EAAiBtY,EAAME,EAAMD,EAAS+Q,GACtF,GAAsB,IAAlBnB,EAAO5J,OACP,OAAO/F,EAEX,MAAM4e,EAAeG,GAAgBpP,EAAQ,WAAY,SACnDnL,EAAe,IAAIwP,IAAIjU,EAAQ/B,KAAIG,GAAU,CAACA,EAAOuF,IAAKvF,MAC1DkhB,EAAgB1P,EACjB3R,KAAIsD,GAAQmC,EAAYnC,EAAKqD,YAC7BM,QAAOvB,GAAOc,EAAaM,IAAIpB,KAC/B1F,KAAI0F,GAAOc,EAAaO,IAAIrB,KAC5B4b,UAEL,GAA6B,IAAzBD,EAActZ,OACd,OAAO/F,EAEX,IAAK,MAAM7B,KAAUkhB,EAAe,CAChC,MAAMtH,EAAS,GACTkH,EAAO,GAEb,IAAK,MAAM7gB,KAAO4B,EAAM,CACpB,MAAM0e,EAAaU,EAAapa,QAAQ7G,EAAQC,EAAKwgB,EAAa7Z,IAAI5G,EAAOuF,MAE7E,IAAKgb,EAAY,CACbM,GAAMC,EAAMlH,GACZA,EAAOhQ,KAAK3J,GACZ,QACJ,CAEA,MACMuZ,EAAQ,CAAEuH,OAAQ9gB,EAAKsgB,aAAYpd,KAD5B8W,EAAgBpT,QAAQlF,EAAME,EAAMD,EAAS3B,EAAKD,EAAQ2S,IAGnD,IAAhBmO,EAAKlZ,QAKLkZ,EAAK,GAAGP,aAAeA,GAK3BM,GAAMC,EAAMlH,GACZkH,EAAKlX,KAAK4P,IAVNsH,EAAKlX,KAAK4P,EAWlB,CAEAqH,GAAMC,EAAMlH,GACZ/X,EAAO+X,CACX,CAEA,OAAO/X,CACX,CAEO,SAASuf,GAAiB5P,EAAQyP,EAAchH,EAAiBtY,EAAME,EAAMD,EAAS+Q,GACzF,GAAsB,IAAlBnB,EAAO5J,OACP,OAAOhG,EAEX,MAAM6e,EAAeG,GAAgBpP,EAAQ,QAAS,YAChDlL,EAAY,IAAIuP,IAAIhU,EAAKhC,KAAII,GAAO,CAACA,EAAIsF,IAAKtF,MAC9CohB,EAAa7P,EACd3R,KAAIsD,GAAQmC,EAAYnC,EAAKuD,SAC7BI,QAAOvB,GAAOe,EAAUK,IAAIpB,KAC5B1F,KAAI0F,GAAOe,EAAUM,IAAIrB,KACzB4b,UAEL,GAA0B,IAAtBE,EAAWzZ,OACX,OAAOhG,EAEX,IAAK,MAAM3B,KAAOohB,EAAY,CAC1B,MAAMzH,EAAS,GACTkH,EAAO,GAEb,IAAK,MAAM9gB,KAAU4B,EAAS,CAC1B,MAAM2e,EAAaU,EAAapa,QAAQ7G,EAAQC,EAAKwgB,EAAa7Z,IAAI3G,EAAIsF,MAE1E,IAAKgb,EAAY,CACbM,GAAMC,EAAMlH,GACZA,EAAOhQ,KAAK5J,GACZ,QACJ,CAEA,MACMwZ,EAAQ,CAAEuH,OAAQ/gB,EAAQugB,aAAYpd,KAD/B8W,EAAgBpT,QAAQlF,EAAME,EAAMD,EAAS3B,EAAKD,EAAQ2S,IAGnD,IAAhBmO,EAAKlZ,QAKLkZ,EAAK,GAAGP,aAAeA,GAK3BM,GAAMC,EAAMlH,GACZkH,EAAKlX,KAAK4P,IAVNsH,EAAKlX,KAAK4P,EAWlB,CAEAqH,GAAMC,EAAMlH,GACZhY,EAAUgY,CACd,CAEA,OAAOhY,CACX,CC9HA,MAAM0f,GAAa,EAIZ,SAASC,GAAmB3f,EAASyE,EAAcC,EAAWmM,EAAatO,EAASqd,EAAe9E,EAAWC,GACjH,IAAKlK,EACD,OAAO,KAEX,MAAMzS,EAASqG,EAAaO,IAAItB,EAAYmN,EAAYjM,WAGxD,GAAiB,WAFLF,EAAUM,IAAItB,EAAYmN,EAAY/L,QAE1CR,KACJ,OAAO,KAEX,MAAMub,EAAmBjF,GAAoBrY,EAASqd,EAAe9E,EAAWC,GAChF,IAAK8E,EACD,OAAO,KACX,MAAMjW,EAAIiW,EAAiBjW,EAE3B,OAAIA,GAAKxL,EAAOgN,MAAQsU,IAAc9V,GAAKxL,EAAOgN,MAAQsU,GAC/CthB,EAAO0E,GAEG,IAAjB1E,EAAO0J,OAEP8B,EAAIxL,EAAOsJ,KAAOgY,IAAc9V,EAAIxL,EAAOsJ,KAAOgY,GAD3C,KAIJ1f,EAAQ5B,EAAO0J,MAAQ,GAAGhF,EACrC,CAEO,SAASgd,GAAgB7f,EAAMwE,EAAcC,EAAWmM,EAAatO,EAASqd,EAAe9E,EAAWC,GAC3G,IAAKlK,EACD,OAAO,KAEX,MAAMzS,EAASqG,EAAaO,IAAItB,EAAYmN,EAAYjM,WAClDvG,EAAMqG,EAAUM,IAAItB,EAAYmN,EAAY/L,QAElD,GAAoB,WAAhB1G,EAAOkG,KACP,OAAO,KAEX,MAAMub,EAAmBjF,GAAoBrY,EAASqd,EAAe9E,EAAWC,GAChF,IAAK8E,EACD,OAAO,KACX,MAAMhW,EAAIgW,EAAiBhW,EAE3B,OAAIA,GAAKxL,EAAIqN,OAASgU,IAAc7V,GAAKxL,EAAIqN,OAASgU,GAC3CrhB,EAAIyE,GAEG,IAAdzE,EAAIyJ,OAEJ+B,EAAIxL,EAAIsJ,IAAM+X,IAAc7V,EAAIxL,EAAIsJ,IAAM+X,GADnC,KAIJzf,EAAK5B,EAAIyJ,MAAQ,GAAGhF,EAC/B,CCzDe,SAASid,GAAkBnQ,GACtC,OAAOA,EAAO3R,KAAIiG,IAAQ,CACtBU,SAAU,aAAcV,EAAOA,EAAKU,SAAW,SAC/CE,MAAO,UAAWZ,EAAOA,EAAKY,MAAQ,SACtCiL,UAAW7L,EAAK6L,aAExB,CCNe,SAASiQ,GAAmBrf,GACvC,OAAOA,EAAQ1C,KAAIiH,IAAU,CACzBN,SAAU,aAAcM,EAASA,EAAON,SAAW,SACnDE,MAAO,UAAWI,EAASA,EAAOJ,MAAQ,SAC1C8O,WAAY1O,EAAO0O,cAE3B,CCIO,SAASqM,GAAiBjgB,EAASkgB,GACtC,OAXJ,SAAmBvI,EAASuI,GACxB,MAAMrD,EAAMlF,EACPzS,QAAO0S,GAAwB,SAAfA,EAAMtT,OACtBrG,KAAI2Z,GAASA,EAAM9U,KAIxB,OAFAod,EAASrD,GAEFA,CACX,CAGWsD,CAAUngB,EAASkgB,EAC9B,CC0BA,SAASE,GAAoBpiB,GACzB0B,QAAQC,MAAM,eAEd,MAAM0gB,EAAU,IAAKriB,EAAQsiB,gBAAiBtiB,EAAQuiB,iBAChDC,EAASxiB,EAAQwiB,OACjBC,EAAgBziB,EAAQ0H,MACxBnD,EAAUvE,EAAQuE,QAGxB,SAASme,EAAM/c,EAAKgd,EAAMC,GACtB,MAAMC,EAAuBL,EAAO7c,IAAQ6c,EAAO7c,GAAKid,aAGxD,OAFKC,IAAwBD,EAAajE,MAAK,CAACmE,EAAYhZ,IAAUgZ,IAAeD,EAAqB/Y,OACtG0Y,EAAO7c,GAAO,CAAEhG,MAAOgjB,KAAQC,GAAeA,iBAC3CJ,EAAO7c,GAAKhG,KACvB,CAEA,MAAMyH,EAAmB3B,OAAO2B,iBAC1BpC,EAAcqd,EAAQrd,YAAcoC,EACpCrF,EAAOsgB,EAAQtgB,KACftB,EAAOT,EAAQ8P,MAAMnQ,MACrBiS,EAAS8Q,EAAM,SAAUX,GAAmB,CAACM,EAAQzQ,SACrDjP,EAAU+f,EAAM,UAAWV,GAAoB,CAACK,EAAQ1f,UACxD8F,EAAeia,EAAM,eAAgBzG,EAAiB,IACtD9B,EAAiBuI,EAAM,iBAAkB/Q,EAAmB,CAAC0Q,EAAQviB,WAAYuiB,EAAQ9gB,aAAcqQ,IACvG4E,EAAwBkM,EAAM,wBAAyB/M,EAA0B,CAAC0M,EAAQzf,YAAaD,IACvGoQ,EAAU2P,EAAM,UAAWnM,EAAY,CAACC,IACxCuM,EAAiBL,EAAM,iBAAkB5L,EAAY,CAACuL,EAAQrgB,QAASD,IACvEihB,EAAcN,EAAM,cAAe5L,EAAY,CAACuL,EAAQpgB,KAAMF,IAG9D6c,EAAkB8D,EAAM,kBAAmBhE,GAAoB,CAACqE,EAAgBhhB,IAChFid,EAAe0D,EAAM,eAAgB3D,GAAiB,CAACiE,EAAajhB,IACpEkhB,EAAoBP,EAAM,oBAAqBpL,EAAoB,CAACsH,EAAiByD,EAAQ9f,WAAY8f,EAAQ5f,YAAa4f,EAAQjd,eACtI8d,EAAiBR,EAAM,iBAAkBlL,EAAiB,CAACwH,EAAcqD,EAAQlgB,UAAWkgB,EAAQhgB,aAAcggB,EAAQhd,aAC1H8d,EAAuBT,EAAM,uBAAwBvC,GAAS,CAAC8C,IAC/DG,EAAoBV,EAAM,oBAAqBvC,GAAS,CAAC+C,IAGzDG,EAAmBX,EAAM,mBAAoBpD,GAAqB,CAACnF,IACnEmJ,EAAwBZ,EAAM,wBAAyBxI,EAAoB,CAACmJ,IAC5EvI,EAAiB4H,EAAM,iBAAkBrD,GAAmB,CAACgD,EAAQhhB,YACrE0Z,EAAkB2H,EAAM,kBAAmBzH,EAAoB,CAACtY,EAASmY,EAAgBwI,EAAuBvhB,EAAMmhB,EAAgBD,EAAmBlQ,IACzJmI,EAAewH,EAAM,eAAgB7H,EAAiB,CAAClY,EAASmY,EAAgBwI,EAAuBvhB,EAAMmhB,EAAgBD,EAAmBlQ,IAGhJwQ,EAAoBb,EAAM,oBAAqBtC,GAAsB,CAACjG,IACtEqJ,GAAyBd,EAAM,yBAA0BxI,EAAoB,CAACqJ,IAC9ElC,GAAeqB,EAAM,eAAgB3B,GAAiB,CAACsB,EAAQtd,UAK/D0e,GAJgBf,EAAM,gBAAiBlB,GAAkB,CAAC5P,EAAQyP,GAAcmC,GAAwBzhB,EAAMmZ,EAAcH,EAAiBhI,IAK7I2Q,GAJahB,EAAM,aAActB,GAAe,CAACxP,EAAQyP,GAAcmC,GAAwBzhB,EAAMmZ,EAAcH,EAAiBhI,IAOpI4Q,GAAoBjB,EAAM,oBAAqBnD,GAAsB,CAACpF,IACtEyJ,GAAyBlB,EAAM,yBAA0BxI,EAAoB,CAACyJ,KAC9EE,GAAwBnB,EAAM,wBAAyBpI,EAAmB,CAACsJ,GAAwB7hB,EAAM2hB,GAAYD,GAAe1Q,IACpI+Q,GAAmB9jB,EAAQ8jB,iBAC3BC,GAAiB/jB,EAAQ+jB,eACzBC,GAAkBtB,EAAM,kBAAmBlD,GAAoB,CAACiE,GAAeC,GAAYjb,EAAcob,GAAuBC,GAAkBX,IAClJc,GAAevB,EAAM,eAAgB1C,GAAiB,CAACyD,GAAeC,GAAYjb,EAAcob,GAAuBE,GAAgBX,IAGvIphB,GAAU0gB,EAAM,UAAWhL,EAAkB,CAACsM,GAAiB5c,EAAkBpC,IACjF/C,GAAOygB,EAAM,OAAQ9K,EAAe,CAACqM,GAAc7c,EAAkBpC,IACrEyB,GAAeic,EAAM,eAAgBpF,GAAW,CAACtb,KACjD0E,GAAYgc,EAAM,YAAapF,GAAW,CAACrb,KAC3CgD,GAAcod,EAAQpd,YACtB6C,GAAW4a,EAAM,WAAY7O,EAAa,CAAC7R,GAASC,KACpDa,GAAgBuf,EAAQvf,cACxBga,GAAY4F,EAAM,YAAatH,EAAc,CAACtT,GAAS6B,IAAIR,OAAQrB,GAAS4F,OAAOvE,OAAQrB,GAAS4B,KAAKN,MAAOtB,GAASsF,MAAMhE,QAC/H2T,GAAY2F,EAAM,YAAarH,EAAc,CAACrZ,GAASC,KAEvD4Q,GC7GK,SAAwBtO,EAASqd,EAAe3f,EAAMD,EAAS8a,EAAWC,GACrF,IAAK6E,EACD,OAAO,KACX,GAAIA,EAAchW,EAAI,GAAKgW,EAAc/V,EAAI,GAAK+V,EAAchW,EAAImR,EAAU3T,OAASwY,EAAc/V,EAAIkR,EAAU5T,OAC/G,OAAO,KAEX,MAAM0Y,EAAmBjF,GAAoBrY,EAASqd,EAAe9E,EAAWC,GAC1EmH,ECXK,SAAqBjiB,EAAM4J,GACtC,GAAoB,IAAhB5J,EAAK+F,OACL,OAAQ,EACZ,GAAI6D,EAAI5J,EAAK,GAAGoT,cACZ,OAAQ,EACZ,GAAIxJ,EAAI5J,EAAKA,EAAK+F,OAAS,GAAGsN,iBAC1B,OAAQ,EAEZ,IAAI6O,EAAQ,EACRC,EAAQniB,EAAK+F,OAAS,EAE1B,KAAOmc,GAASC,GAAO,CACnB,MAAMC,EAAQhd,KAAKid,OAAOH,EAAQC,GAAS,GAE3C,GAAIvY,EAAI5J,EAAKoiB,GAAOhP,cAChB+O,EAAQC,EAAQ,MACf,MAAIxY,EAAI5J,EAAKoiB,GAAO/O,kBAIrB,OAAO+O,EAHPF,EAAQE,EAAQ,CAGJ,CACpB,CAEA,OAAQ,CACZ,CDb0BE,CAAYtiB,EAAM4f,EAAiBhW,GACnD2Y,EEZK,SAAwBxiB,EAAS4J,GAC5C,GAAuB,IAAnB5J,EAAQgG,OACR,OAAQ,EACZ,GAAI4D,EAAI5J,EAAQ,GAAGwT,eACf,OAAQ,EACZ,GAAI5J,EAAI5J,EAAQA,EAAQgG,OAAS,GAAGyN,gBAChC,OAAQ,EAEZ,IAAI0O,EAAQ,EACRC,EAAQpiB,EAAQgG,OAAS,EAE7B,KAAOmc,GAASC,GAAO,CACnB,MAAMC,EAAQhd,KAAKid,OAAOH,EAAQC,GAAS,GAE3C,GAAIxY,EAAI5J,EAAQqiB,GAAO7O,eACnB4O,EAAQC,EAAQ,MACf,MAAIzY,EAAI5J,EAAQqiB,GAAO5O,iBAIxB,OAAO4O,EAHPF,EAAQE,EAAQ,CAGJ,CACpB,CAEA,OAAQ,CACZ,CFZ6BI,CAAeziB,EAAS6f,EAAiBjW,GAElE,OAAuB,IAAnBsY,IAA8C,IAAtBM,EACjB,KAEJ,CACH1d,MAAO7E,EAAKiiB,GAAepf,GAC3B8B,SAAU5E,EAAQwiB,GAAkB1f,GAE5C,CD4FwB4f,CAAengB,EAASvE,EAAQ4hB,cAAe3f,GAAMD,GAAS8a,GAAWC,IACvFpM,GAAkB3Q,EAAQ2kB,gBAAkBjC,EAAM,kBAAmBf,GAAoB,CAAC3f,GAASyE,GAAcC,GAAWmM,GAAatO,EAASvE,EAAQ4hB,cAAe9E,GAAWC,KACpLnM,GAAe5Q,EAAQ4kB,aAAelC,EAAM,eAAgBZ,GAAiB,CAAC7f,GAAMwE,GAAcC,GAAWmM,GAAatO,EAASvE,EAAQ4hB,cAAe9E,GAAWC,KAGrK7X,GAAmBwd,EAAM,mBAAoBnF,GAAqB,CAFpDvd,EAAQwd,cACP7M,MAAqBC,GACwD3L,GAAa4N,GAAa7Q,GAASC,GAAMwE,GAAcC,KACnJoM,GAAY4P,EAAM,YAAa7L,EAAc,CAAC/T,KAC9C2J,GAAYiW,EAAM,YAAa7L,EAAc,CAAC3R,KAE9C2f,GAAmBnC,EAAM,mBAAoB9P,EAAqB,CAACuH,EAAgBtH,GAAa5N,GAAa6N,GAAWrG,GAAWsG,EAASnB,EAAQjB,GAAiBC,GAAcyR,EAAQrd,cAC3L8f,GAAwBpC,EAAM,wBAAyBxI,EAAoB,CAAC2K,KAC5Enc,GAAuBga,EAAM,uBAAwBpI,EAAmB,CAACwK,GAAuB/iB,EAAME,GAAMD,GAAS+Q,IACrHgS,GAAkBrC,EAAM,kBAAmBlQ,EAAoB,CAAC2H,IAChE6K,GAAuBtC,EAAM,uBAAwBxI,EAAoB,CAAC6K,KAC1EE,GAAsBvC,EAAM,sBAAuBpI,EAAmB,CAAC0K,GAAsBjjB,EAAME,GAAMD,GAAS+Q,IAClHqL,GAAgBsE,EAAM,gBAAiBnc,EAAkB,CAACzD,GAAemiB,GAAqBxe,GAAcC,KAC5GqJ,GAAiB2S,EAAM,iBAAkBvE,GAAmB,CAACC,GAAenZ,GAAawB,GAAcC,GAAWoB,KAClH2I,GAAciS,EAAM,cAAerE,GAAgB,CAAC5d,EAAM2d,KAG1D5V,GtB1HK,SAAuB0c,EAAUnI,EAAWD,EAAWvY,GAElE,MAAM4gB,EAAO,CACT/b,MAAO7E,EAAQ6gB,wBAAwBhc,MACvCD,OAAQ5E,EAAQ6gB,wBAAwBjc,QAEtC6T,EAAe,CACjBtT,KAAMnF,EAAQ0Y,WACdtT,IAAKpF,EAAQ2Y,WAGXmI,EAAiBH,GAAYvI,GAG7BR,EAASK,GADG,CAAE9S,KAAM,EAAGC,IAAK,KAAMoT,GACLD,GAC7BtU,EAAagU,GAAS,IAAKQ,KAAiBmI,GAAQrI,GACpDwI,EAAqBrZ,EAAKkQ,EAAQG,EAAO9T,EAAYiU,KACrD8I,EAAsBtZ,EAAKkQ,EAAQG,EAAO9T,EAAYkU,KAE5D,OAAKR,EAASC,EAAQkJ,IAGjBnJ,EAASmJ,EAAgBC,GAG1B,EAAKD,GAAkB,EAAI,EAAKE,GACzBA,EAEJF,EARIE,CASf,CsB6FuBC,CAAc/C,GAAeja,WAAYuU,GAAWD,GAAWvY,GAGlFme,EAAM,gBAAiBT,GAAkB,CAACjgB,GAASqgB,EAAQve,wBAC3D4e,EAAM,aAAcT,GAAkB,CAAChgB,GAAMogB,EAAQpe,qBAErDjE,EAAQ0H,MAAQ,CACZ2a,UACAjb,mBACApC,cACAjD,OACAoY,iBACApH,UACAgI,kBACAG,eACAlZ,WACAC,QACA6F,YACAhF,iBACAgQ,aACArG,aACAoG,eACA5N,eACA4f,oBACAnc,wBACAqc,mBACAE,uBACAnI,aACAC,aACAtU,eACAD,cACAtD,oBACA6K,kBACAtJ,gBACAC,aACAjG,OACAgQ,eACAE,mBACAC,gBAER,CAEe,SAAS6U,GAAYzlB,GAChC,IAAKA,EAAQ6P,MACT,IACIuS,GAAoBpiB,EACxB,CAAE,MAAO6P,GACL7P,EAAQ6P,MAAQA,CACpB,CAER,CIrLe,SAAS6V,GAAiBC,EAAeC,GACpD,MAAM9S,EAAY,IAAI2D,EAAUmP,GAChC,MAAO,IAAIA,KAAaD,EAAcze,QAAO3D,IAASuP,EAAU8D,aAAarT,EAAKuD,MAAOvD,EAAKqD,YAClG,CCHe,SAASif,GAAgBF,EAAeG,GACnD,MAAMhT,EAAY,IAAI2D,EAAUqP,GAChC,OAAOH,EAAcze,QAAO3D,IAASuP,EAAU8D,aAAarT,EAAKuD,MAAOvD,EAAKqD,WACjF,CCLe,SAASmf,GAAiBC,GACrC,MACMha,EADUga,EAAMC,cACDb,wBACrB,MAAO,CACHxZ,EAAGoa,EAAME,QAAUla,EAAKtC,KACxBmC,EAAGma,EAAMG,QAAUna,EAAKrC,IAEhC,CCPO,SAASyc,GAAiBrb,EAAOsb,GACpC,OAAOtb,EAAM9K,KAAIsD,IAAQ,IAClBA,EACHqD,SAAU,OAAQrD,EAAOA,EAAKuB,GAAKuhB,EACnCvf,MAAO,OAAQvD,EAAOA,EAAKuB,GAAKuhB,KAExC,CCQA,SAASC,GAAW/hB,GAChB,GAAI,wBAAyBA,EAAS,OAEtC7C,QAAQ0G,IAAI,cAEZ,MAAMR,EAAW,CACb,WAAYqI,SAASsL,cAAc,UACnC,aAActL,SAASsL,cAAc,UACrC,YAAatL,SAASsL,cAAc,UACpC,cAAetL,SAASsL,cAAc,UACtC,gBAAiBtL,SAASsL,cAAc,UACxC,eAAgBtL,SAASsL,cAAc,UACvC,cAAetL,SAASsL,cAAc,UACtC,gBAAiBtL,SAASsL,cAAc,UACxC,eAAgBtL,SAASsL,cAAc,WAErCzL,EAAQG,SAASsL,cAAc,SAErChX,EAAQgiB,aAAa,WAAY,KACjChiB,EAAQgiB,aAAa,QAAS,oQAC9BhiB,EAAQiiB,UAAU7P,IAAI,eACtB/O,EAAS,YAAY2e,aAAa,QAAS,+EAC3C3e,EAAS,cAAc2e,aAAa,QAAS,sEAC7C3e,EAAS,aAAa2e,aAAa,QAAS,gFAC5C3e,EAAS,eAAe2e,aAAa,QAAS,uEAC9C3e,EAAS,iBAAiB2e,aAAa,QAAS,4CAChD3e,EAAS,gBAAgB2e,aAAa,QAAS,wEAC/C3e,EAAS,eAAe2e,aAAa,QAAS,kFAC9C3e,EAAS,iBAAiB2e,aAAa,QAAS,yEAChD3e,EAAS,gBAAgB2e,aAAa,QAAS,mFAC/CzW,EAAMyW,aAAa,QAAS,0NAE5B,MAAMvmB,EAAU,CACZuiB,gBAAiB,CAAC,EAClB7a,MAAO,KACP8a,OAAQ,CAAC,EACTje,QAASA,EACTqD,SAAUA,EACVkI,MAAOA,EACP2W,iBAAiB,EACjB7E,cAAe,KACfpE,aAAa,EACbsG,iBAAkB,IAAI7N,IACtB8N,eAAgB,IAAI9N,IAGxBjW,iBAA2B,KACnBA,EAAQymB,kBACZzmB,EAAQymB,iBAAkB,EAC1BC,uBAAsB,KAClB1mB,EAAQymB,iBAAkB,EAC1BhB,GAAYzlB,GACZ4P,EAAO5P,EAAQ,IACjB,EAGNA,iBAA2B,CAACuE,EAAS+B,EAAMqgB,KACvCpiB,EAAQqiB,iBAAiBtgB,GAAO0f,IAC5B,IACIW,EAASX,EACb,CACA,MAAOnW,GACHA,EAAMwB,QAAU,IAAI/K,aAAgBuJ,EAAMwB,UAC1CrR,EAAQ6P,MAAQA,EAChB7P,EAAQ6mB,kBACZ,IACF,GAGN7mB,EAAQsiB,aAAe,CACnBvgB,KAAM,GACNC,QAAS,CAAC,CAAEsE,KAAM,eAClBrE,KAAM,CAAC,CAAEqE,KAAM,UAAY,CAAEA,KAAM,eACnCxG,WAAY,GACZuB,UAAW,GACX0D,QAAS,GACTxD,aAAc,EAAGQ,OAAM1B,MAAKD,YAAa2B,IAAO1B,EAAIyE,MAAM1E,EAAO0E,IACjE3C,UAAW,EACXE,aAAc,EACdE,WAAY,EACZE,YAAa,EACbuC,YAAa,EACbC,YAAa,KACb6hB,oBAAsB7hB,IAClBjF,EAAQsiB,aAAard,YAAcA,EACnCjF,EAAQ6mB,kBAAkB,EAE9B/jB,cAAe,GACfE,sBAAwBF,IACpB9C,EAAQsiB,aAAaxf,cAAgBA,EACrC9C,EAAQ6mB,kBAAkB,EAE9B3hB,iBAAkB,GAClBtC,YAAa,GACbO,oBAAsBP,IAElB5C,EAAQsiB,aAAa1f,YAAcA,EACnC5C,EAAQ6mB,kBAAkB,EAE9BlkB,QAAS,GACTO,gBAAkBP,IACd3C,EAAQsiB,aAAa3f,QAAUA,EAC/B3C,EAAQ6mB,kBAAkB,EAE9BjV,OAAQ,GACRmV,eAAiBnV,IACb5R,EAAQsiB,aAAa1Q,OAASA,EAC9B5R,EAAQ6mB,kBAAkB,EAE9BvjB,YAAa,OACbO,kBAAmB,OACnBuB,aAAc,GACd4hB,qBAAuB5hB,IACnBpF,EAAQsiB,aAAald,aAAeA,EACpCpF,EAAQ6mB,kBAAkB,EAE9BxhB,WAAY,GACZ4hB,mBAAqB5hB,IACjBrF,EAAQsiB,aAAajd,WAAaA,EAClCrF,EAAQ6mB,kBAAkB,EAE9B/iB,sBAAuB,OACvBG,mBAAoB,QAGxBM,EAAQ,uBAAyBvE,EAEjC,MAAMknB,EAAWzmB,IACbqP,EAAMnQ,MAAQc,EACdqP,EAAMqX,cAAc,IAAIC,MAAM,SAAS,EAGrCC,EAAUpmB,IACZ,MAAM6B,EAAgB9C,EAAQ0H,MAAM2a,QAAQvf,cACtC0D,EAAiBxG,EAAQ0H,MAAMud,oBAC/Bxe,EAAezG,EAAQ0H,MAAMjB,aAC7BC,EAAY1G,EAAQ0H,MAAMhB,UAC1BjG,EAAOT,EAAQ0H,MAAMjH,KACrBgQ,EAAczQ,EAAQ0H,MAAM+I,YAC5B6W,EAAiBtnB,EAAQ0H,MAAM2a,QAAQlf,oBACvCokB,EAAavnB,EAAQ0H,MAAM2a,QAAQnf,gBAGnCkb,EAAgB7X,EAAiBzD,EAAe0D,EAAgBC,EAAcC,GAEpF,GAAa,KAATjG,EACA,OACJ,IAAKgQ,EACD,OACJ,GAAIxP,IAAemd,EAAcE,OAAM/a,GAAQA,EAAK1C,KAAKI,aACrD,OAEJ,MAAMumB,EAAYpJ,EAAclX,QAAO3D,GAAsB,SAAdA,EAAK+C,OAC9CmhB,EAAcrJ,EAAclX,QAAO3D,GAAsB,WAAdA,EAAK+C,OAZ/B,IAACyE,IAcTyc,EAAUvnB,KAAIsD,IAAQ,IAAMA,EAAKA,KAAM5D,MAAO4D,EAAK1C,KAAKG,MAAM,CAAE0Q,OAAQjR,QAdrD6mB,EAAe5B,GAAiB1lB,EAAQ0H,MAAM2a,QAAQzf,YAAamI,IAClF,CAACA,IAAUwc,EAAW7B,GAAiBU,GAAiBpmB,EAAQ0H,MAAM2a,QAAQ1f,QAAS,UAAWoI,GAAO,EAc5H2c,CAAWD,EAAYxnB,KAAIsD,IAAQ,IAAMA,EAAKA,KAAMqS,WAAYrS,EAAK1C,KAAKG,MAAM,CAAE0Q,OAAQjR,SAErFQ,GACDimB,EAAQ,GAAG,EAGbS,EAAS1mB,IACX,MAAM6B,EAAgB9C,EAAQ0H,MAAM2a,QAAQvf,cACtCwkB,EAAiBtnB,EAAQ0H,MAAM2a,QAAQlf,oBACvCokB,EAAavnB,EAAQ0H,MAAM2a,QAAQnf,gBAMnCkb,EAAgB7X,EAAiBzD,EAHhB9C,EAAQ0H,MAAMud,oBAChBjlB,EAAQ0H,MAAMjB,aACjBzG,EAAQ0H,MAAMhB,WAJN,IAACqE,EAOvB9J,IAAemd,EAAcE,OAAM/a,GAAQA,EAAK1C,KAAKI,eAP9B8J,EAUTjI,EAVmBwkB,EAAezB,GAAgB7lB,EAAQ0H,MAAM2a,QAAQzf,YAAamI,IACjF,CAACA,IAAUwc,EAAW1B,GAAgBO,GAAiBpmB,EAAQ0H,MAAM2a,QAAQ1f,QAAS,UAAWoI,GAAO,EAU9H6c,CAAc9kB,GAAc,EAKhC9C,EAAQ4mB,iBAAiBriB,EAAS,UAAWyhB,IAKzChmB,EAAQ6mB,kBAAkB,IAG9B7mB,EAAQ4mB,iBAAiBriB,EAAS,cAAeyhB,IAC7ChmB,EAAQ4hB,cAAgBmE,GAAiBC,GACzChmB,EAAQ6mB,kBAAkB,IAG9B7mB,EAAQ4mB,iBAAiBriB,EAAS,aAAcyhB,IAG5C,GAFAhmB,EAAQ4hB,cAAgBmE,GAAiBC,GAErChmB,EAAQ2kB,eAAgB,CACxB,MAAMvkB,EAASJ,EAAQ0H,MAAMjB,aAAaO,IAAItB,EAAY1F,EAAQ2kB,iBAC5DkD,EAAcznB,EAAOgJ,MACrB0e,EAAc1nB,EAAOgN,MACrByU,EAAmBjF,GAAoBrY,EAASvE,EAAQ4hB,cAAe5hB,EAAQ0H,MAAMoV,UAAW9c,EAAQ0H,MAAMqV,WAC9GgL,EAAiB1gB,KAAKiD,IAAI,GAAIuX,EAAiBjW,EAAIkc,EAAcD,GAEjEG,EADuBhoB,EAAQ0H,MAAM2a,QAAQjd,aAE9C8B,QAAO2gB,GAAeniB,EAAYmiB,EAAYjhB,YAAcxG,EAAOuF,MACnEnF,OAAO,CAAC,CAAEoG,SAAUxG,EAAO0E,GAAIsE,MAAO2e,KAC3C/nB,EAAQ0H,MAAM2a,QAAQ2E,qBAAqBgB,EAC/C,CACA,GAAIhoB,EAAQ4kB,YAAa,CACrB,MAAMvkB,EAAML,EAAQ0H,MAAMhB,UAAUM,IAAItB,EAAY1F,EAAQ4kB,cACtDqD,EAAY5nB,EAAI8I,OAChB+e,EAAY7nB,EAAIqN,OAChBmU,EAAmBjF,GAAoBrY,EAASvE,EAAQ4hB,cAAe5hB,EAAQ0H,MAAMoV,UAAW9c,EAAQ0H,MAAMqV,WAC9GoL,EAAe9gB,KAAKiD,IAAI,GAAIuX,EAAiBhW,EAAIqc,EAAYD,GAE7DG,EADqBpoB,EAAQ0H,MAAM2a,QAAQhd,WAE5C6B,QAAO+gB,GAAaviB,EAAYuiB,EAAUnhB,SAAWzG,EAAIsF,MACzDnF,OAAO,CAAC,CAAEsG,MAAOzG,EAAIyE,GAAIqE,OAAQgf,KACtCnoB,EAAQ0H,MAAM2a,QAAQ4E,mBAAmBmB,EAC7C,CAGApoB,EAAQ6mB,kBAAkB,IAG9B7mB,EAAQ4mB,iBAAiBriB,EAAS,cAAc,KAC5CvE,EAAQ4hB,cAAgB,KACxB5hB,EAAQ6mB,kBAAkB,IAK9B7mB,EAAQ4mB,iBAAiBriB,EAAS,aAAcyhB,IAC5CP,GAAYzlB,GACZknB,EAAQ,IAERlnB,EAAQwd,aAAc,EACtBxd,EAAQqoB,kBAAoBroB,EAAQ4hB,cACpC5hB,EAAQsoB,cAAgBtoB,EAAQ0H,MAAMmL,YAElC7S,EAAQ0H,MAAMiJ,kBACd3Q,EAAQ2kB,eAAiB3kB,EAAQ0H,MAAMiJ,iBAEvC3Q,EAAQ0H,MAAMkJ,eACd5Q,EAAQ4kB,YAAc5kB,EAAQ0H,MAAMkJ,cAEnC5Q,EAAQ0H,MAAMiJ,iBAAoB3Q,EAAQ0H,MAAMkJ,cACjD5Q,EAAQ0H,MAAM2a,QAAQyE,oBAAoB9mB,EAAQ0H,MAAMmL,aAGvDmT,EAAMuC,SACPvoB,EAAQ0H,MAAM2a,QAAQrf,sBAAsB,IAEhDhD,EAAQ6mB,kBAAkB,IAG9B7mB,EAAQ4mB,iBAAiBriB,EAAS,WAAYyhB,IAC1CP,GAAYzlB,GAEZA,EAAQwd,aAAc,EACtBxd,EAAQ2kB,eAAiB,KACzB3kB,EAAQ4kB,YAAc,KAEtB5kB,EAAQ0H,MAAM2a,QAAQrf,sBAAsB0iB,GAAiB1lB,EAAQ0H,MAAM2a,QAAQvf,cAAe9C,EAAQ0H,MAAMxC,mBAChHlF,EAAQ6mB,kBAAkB,IAG9B7mB,EAAQ4mB,iBAAiBriB,EAAS,eAAgByhB,IAC9ChmB,EAAQuE,QAAQikB,kBAAkBxC,EAAMyC,UAAU,IAGtDzoB,EAAQ4mB,iBAAiBriB,EAAS,aAAcyhB,IAC5ChmB,EAAQuE,QAAQmkB,sBAAsB1C,EAAMyC,UAAU,IAG1DzoB,EAAQ4mB,iBAAiBriB,EAAS,SAAUyhB,IACxCP,GAAYzlB,GAEZ,MAAMuD,EAAOvD,EAAQ0H,MAAMmL,YACrByV,EAAgBtoB,EAAQsoB,cAE9B,GAAItoB,EAAQ0H,MAAMiJ,iBAAmB3Q,EAAQ0H,MAAMkJ,aAC/C,OACJ,GAAa,OAATrN,EACA,OACJ,GAAImC,EAAYnC,EAAKqD,YAAclB,EAAY4iB,EAAc1hB,UACzD,OACJ,GAAIlB,EAAYnC,EAAKuD,SAAWpB,EAAY4iB,EAAcxhB,OACtD,OAEJ,MAAM1G,EAASJ,EAAQ0H,MAAMjB,aAAaO,IAAItB,EAAYnC,EAAKqD,WACzDvG,EAAML,EAAQ0H,MAAMhB,UAAUM,IAAItB,EAAYnC,EAAKuD,QACnD8K,EAAS5R,EAAQ0H,MAAM2a,QAAQzQ,OAE/B+W,EADiB3oB,EAAQ0H,MAAMud,oBACLhe,QAAQ5G,EAAKD,GAE7C,GAAIuoB,EAAS9nB,MAAMM,OAAQ,CACvB,MACMsQ,EC1TH,SAAyBlO,EAAMnD,EAAQC,EAAK0S,GACvD,MAAMpT,EAAQoT,EAAQa,cAAcvT,EAAIsF,IAAKvF,EAAOuF,KAC9CoN,EAAQqD,cAAc/V,EAAIsF,IAAKvF,EAAOuF,KACtCpC,EAAK5D,MACLwB,EAASoC,EAAK1C,KAAKM,OAEzB,MAAsB,mBAAXA,EACAA,EAAO,CAACxB,UAEZwB,GAAQA,EAAOynB,QAAQjpB,GAAS,GAAKwB,EAAO6G,OACvD,CDgT6B6gB,CAAgBF,EAAUvoB,EAAQC,EADnCL,EAAQ0H,MAAMqL,SAExB+V,EAAWziB,EAAgBjG,EAAQC,GACxB,SAAbyoB,GACA9oB,EAAQ0H,MAAM2a,QAAQlf,oBAAoBuiB,GAAiB1lB,EAAQ0H,MAAM2a,QAAQzf,YAAa,CAAC,IAAKW,EAAM5D,MAAO8R,MACpG,WAAbqX,GACA9oB,EAAQ0H,MAAM2a,QAAQnf,gBAAgBwiB,GAAiB1lB,EAAQ0H,MAAM2a,QAAQ1f,QAAS,CAAC,IAAKY,EAAMqS,WAAYnE,KACtH,MAAO,GAAoB,SAAhBrR,EAAOkG,MAAgC,SAAbjG,EAAIiG,KACrCtG,EAAQ0H,MAAM2a,QAAQ/e,YAAYtD,EAAQ0H,MAAMmL,kBAC7C,GAAoB,WAAhBzS,EAAOkG,MAAkC,WAAbjG,EAAIiG,KACvCtG,EAAQ0H,MAAM2a,QAAQxe,kBAAkB7D,EAAQ0H,MAAMmL,kBACnD,GAAoB,WAAhBzS,EAAOkG,MAAkC,WAAbjG,EAAIiG,KAAmB,CAC1D,MAAMyiB,EEnUH,SAAsBnX,EAAQxR,EAAQC,EAAKkoB,GAGtD,SAASS,EAAc9oB,GACnB,MAAM0G,EAAW,aAAc1G,EAAOA,EAAK0G,SAAW,SAChDE,EAAQ,UAAW5G,EAAOA,EAAK4G,MAAQ,SAE7C,OAAO1G,EAAOuF,MAAQD,EAAYkB,IAAavG,EAAIsF,MAAQD,EAAYoB,EAC3E,CAUA,MAAMmiB,EAAgB,CAAC,MAAO,YAAQpX,GAChCqX,EAActX,EAAOuX,KAAKH,GAC1BI,EAAiBH,EAAcL,QAAQM,GAAanX,WACpDsX,EAAeJ,GAAeG,EAAiB,GAAKH,EAAcjhB,QAClEshB,EAAa1X,EAAOgX,QAAQM,KAAiBtX,EAAO5J,OAAS,EAOnE,MAAO,KANeugB,IAAYe,GAAeJ,EAG3CtX,EAAO1K,QAAOhH,IAhBpB,SAAsCA,GAClC,MAAM0G,EAAW,aAAc1G,EAAOA,EAAK0G,SAAW,SAChDE,EAAQ,UAAW5G,EAAOA,EAAK4G,MAAQ,SAE7C,MAAuB,WAAhB1G,EAAOkG,MAAqBlG,EAAOuF,MAAQD,EAAYkB,IAC1C,WAAbvG,EAAIiG,MAAqBjG,EAAIsF,MAAQD,EAAYoB,EAC5D,CAU6ByiB,CAA6BrpB,KADpD0R,EAAO1K,QAAOhH,IAAS8oB,EAAc9oB,QAE1BmpB,EAAe,CAAC,CAAEziB,SAAUxG,EAAO0E,GAAIgC,MAAOzG,EAAIyE,GAAIiN,UAAWsX,IAAkB,GAGxG,CFqS8BG,CAAa5X,EAAQxR,EAAQC,EAAK2lB,EAAMuC,SAC1DvoB,EAAQ0H,MAAM2a,QAAQ0E,eAAegC,GACrC/oB,EAAQ0H,MAAM2a,QAAQrf,sBAAsB,GAChD,KAGJhD,EAAQ4mB,iBAAiBriB,EAAS,YAAayhB,IAG3C,GAFAP,GAAYzlB,GAERA,EAAQ0H,MAAMiJ,gBAAiB,CAC/B,MAAM8Y,EAAqB/jB,EAAY1F,EAAQ0H,MAAMiJ,iBAC/CqX,EAAkBhoB,EAAQ0H,MAAM2a,QAAQjd,aAAa8B,QAAO2gB,GAAeniB,EAAYmiB,EAAYjhB,YAAc6iB,IACvHzpB,EAAQ0H,MAAM2a,QAAQ2E,qBAAqBgB,GAC3ChoB,EAAQ8jB,iBAAiB/D,OAAO0J,EACpC,CACA,GAAIzpB,EAAQ0H,MAAMkJ,aAAc,CAC5B,MAAM8Y,EAAkBhkB,EAAY1F,EAAQ0H,MAAMkJ,cAC5CwX,EAAgBpoB,EAAQ0H,MAAM2a,QAAQhd,WAAW6B,QAAO+gB,GAAaviB,EAAYuiB,EAAUnhB,SAAW4iB,IAC5G1pB,EAAQ0H,MAAM2a,QAAQ4E,mBAAmBmB,GACzCpoB,EAAQ+jB,eAAehE,OAAO2J,EAClC,CAEA,MAAMzkB,EAAcjF,EAAQ0H,MAAMzC,YAClC,GAAoB,OAAhBA,EACA,OAEJ,MAAM+N,EAAmBtN,EAAYT,EAAY2B,UAC3CqM,EAAgBvN,EAAYT,EAAY6B,OACxCL,EAAezG,EAAQ0H,MAAMjB,aAC7BC,EAAY1G,EAAQ0H,MAAMhB,UAC1BF,EAAiBxG,EAAQ0H,MAAMud,oBAErC,IAAKxe,EAAaM,IAAIiM,GAClB,OACJ,IAAKtM,EAAUK,IAAIkM,GACf,OAEJ,MAAM7S,EAASqG,EAAaO,IAAIgM,GAC1B3S,EAAMqG,EAAUM,IAAIiM,GACpB1P,EAAOiD,EAAeS,QAAQ5G,EAAKD,GACnCK,EAAO8C,EAAK9C,KAEb8C,EAAK1C,OAEN0C,EAAK1C,KAAKM,SAGd+lB,EAAQzmB,GACRqP,GAAO6Z,UAAQ,IAGnB3pB,EAAQ4mB,iBAAiBriB,EAAS,SAAS,KACnCuL,EAAM7H,eACN6H,EAAMK,MAAM,CAAEC,eAAe,GAAO,IAG5CpQ,EAAQ4mB,iBAAiBriB,EAAS,WAAYyhB,IAE1CP,GAAYzlB,GAEZ,MAAMiF,EAAcjF,EAAQ0H,MAAMzC,YAC5BwB,EAAezG,EAAQ0H,MAAMjB,aAC7BC,EAAY1G,EAAQ0H,MAAMhB,UAC1B5D,EAAgB9C,EAAQ0H,MAAM2a,QAAQvf,cACtC8mB,EAAmB5pB,EAAQ0H,MAAM2a,QAAQrf,sBAEzC6mB,EAAiB7pB,EAAQ0H,MAAM2a,QAAQyE,oBACvClkB,EAAc5C,EAAQ0H,MAAM2a,QAAQzf,YACpC0kB,EAAiBtnB,EAAQ0H,MAAM2a,QAAQlf,oBACvCnB,EAAUhC,EAAQ0H,MAAM1F,QACxBC,EAAOjC,EAAQ0H,MAAMzF,KACrBxB,EAAOT,EAAQ0H,MAAMjH,KACrBwkB,EAAsBjlB,EAAQ0H,MAAMud,oBAEpC6E,EAAU,CAACvmB,EAAMyiB,KACnB6D,EAAetmB,GAEXyiB,EAAM+D,SAZsBH,EAAiBlE,GAAiB5iB,EAa7C,CAACS,KAElBqmB,EAAiB,CAACrmB,GAAM,EAG1BymB,EAAoB,CAACjgB,EAAQic,KAC/B,IAAK/gB,EACD,OAEJ,MAAM+N,EAAmBtN,EAAYT,EAAY2B,UACjD,IAAKH,EAAaM,IAAIiM,GAClB,OAEJ,MAAMiX,EAAqBxjB,EAAaO,IAAIgM,GAAkBlJ,MACxDogB,EAAiB7iB,KAAKiD,IAAI,EAAGjD,KAAKgV,IAAIra,EAAQgG,OAAS,EAAGiiB,EAAqBlgB,IACrF,GAAImgB,IAAmBD,EACnB,OAEJ,MAAME,EAAiB,CAAErjB,MAAO7B,EAAY6B,MAAOF,SAAU5E,EAAQkoB,GAAgBplB,IAErFglB,EAAQK,EAAgBnE,EAAM,EAG5BoE,EAAkB,CAACrgB,EAAQic,KAC7B,IAAK/gB,EACD,OAEJ,MAAMgO,EAAgBvN,EAAYT,EAAY6B,OAC9C,IAAKJ,EAAUK,IAAIkM,GACf,OAEJ,MAAMoX,EAAkB3jB,EAAUM,IAAIiM,GAAenJ,MAC/CwgB,EAAcjjB,KAAKiD,IAAI,EAAGjD,KAAKgV,IAAIpa,EAAK+F,OAAS,EAAGqiB,EAAkBtgB,IAC5E,GAAIugB,IAAgBD,EAChB,OAEJ,MAAMF,EAAiB,CAAErjB,MAAO7E,EAAKqoB,GAAaxlB,GAAI8B,SAAU3B,EAAY2B,UAE5EkjB,EAAQK,EAAgBnE,EAAM,EAG5BuE,EAAiB,KACnBvE,EAAMuE,iBACNvE,EAAMwE,iBAAiB,EAqC3B,OAAQxE,EAAMrgB,KACV,IAAK,SAlCQ,KAATlF,EACAymB,EAAQ,IAEHpkB,EAAckF,OAAS,EAC5B4hB,EAAiB,CAAC3kB,IAEbrC,EAAYoF,OAAS,EAC1Bsf,EAAe,KAGfuC,EAAe,MACfD,EAAiB,KAyBjB,MACJ,IAAK,QACDvC,IACA,MACJ,IAAK,UAGDkD,IACAH,EAAgBpE,EAAMuC,SAAWtmB,EAAK+F,QAAU,EAAGge,GACnD,MACJ,IAAK,YACDuE,IACAH,EAAgBpE,EAAMuC,QAAUtmB,EAAK+F,OAAS,EAAGge,GACjD,MACJ,IAAK,YACDuE,IACAP,EAAkBhE,EAAMuC,SAAWvmB,EAAQgG,QAAU,EAAGge,GACxD,MACJ,IAAK,aACDuE,IACAP,EAAkBhE,EAAMuC,QAAUvmB,EAAQgG,OAAS,EAAGge,GACtD,MACJ,IAAK,SACL,IAAK,YACD2B,IACA,MACJ,IAAK,IA/Ce,CAAC3B,IACrB,IAAKA,EAAMuC,QACP,OAEJ,MAAMkC,EGldH,SAA0B3nB,EAAed,EAASC,EAAMuE,GACnE,MAAMC,EAAe,IAAIwP,IAAIjU,EAAQ/B,KAAIG,GAAU,CAACA,EAAOuF,IAAKvF,MAC1DsG,EAAY,IAAIuP,IAAIhU,EAAKhC,KAAII,GAAO,CAACA,EAAIsF,IAAKtF,MAC9CqqB,EAAmB5nB,EAAc7C,KAAIsD,IAAQ,CAC/CoD,UAAWjB,EAAYnC,EAAKqD,UAC5BC,OAAQnB,EAAYnC,EAAKuD,WACzBI,QAAO3D,GAAQkD,EAAaM,IAAIxD,EAAKoD,YAAcD,EAAUK,IAAIxD,EAAKsD,UACpE8jB,EAAkB,IAAIjU,IAAIgU,EAAiBzqB,KAAIsD,GAAQA,EAAKoD,aAC5DikB,EAAe,IAAIlU,IAAIgU,EAAiBzqB,KAAIsD,GAAQA,EAAKsD,UAE/D,GAAgC,IAA5B6jB,EAAiB1iB,OACjB,MAAO,GAEX,MAAM8K,EAAY,IAAI2D,EAAU3T,GAC1B6a,EAAiBtW,KAAKgV,OAAOqO,EAAiBzqB,KAAIsD,GAAQkD,EAAaO,IAAIzD,EAAKoD,WAAWmD,SAC3F8T,EAAiBvW,KAAKiD,OAAOogB,EAAiBzqB,KAAIsD,GAAQkD,EAAaO,IAAIzD,EAAKoD,WAAWmD,SAC3F+T,EAAcxW,KAAKgV,OAAOqO,EAAiBzqB,KAAIsD,GAAQmD,EAAUM,IAAIzD,EAAKsD,QAAQiD,SAClFgU,EAAczW,KAAKiD,OAAOogB,EAAiBzqB,KAAIsD,GAAQmD,EAAUM,IAAIzD,EAAKsD,QAAQiD,SAElF+gB,EAAgB,GAEtB,IAAK,IAAI3f,EAAW2S,EAAa3S,GAAY4S,EAAa5S,IAAY,CAClE,MAAM7K,EAAM4B,EAAKiJ,GACXrE,EAASxG,EAAIsF,IAEnB,GAAKilB,EAAa7jB,IAAIF,GAAtB,CAGA,IAAK,IAAIsE,EAAcwS,EAAgBxS,GAAeyS,EAAgBzS,IAAe,CACjF,MAAM/K,EAAS4B,EAAQmJ,GACjBxE,EAAYvG,EAAOuF,IAEzB,GAAKglB,EAAgB5jB,IAAIJ,GAAzB,CAGA,GAAImM,EAAUS,cAAc1M,EAAQF,GAAY,CAC5C,MAAMgiB,EAAWniB,EAAeS,QAAQ5G,EAAKD,GAAQK,KACrDoqB,EAAc7gB,KAAK2e,EACvB,CAEIxd,EAAcyS,GACdiN,EAAc7gB,KAAK,KARX,CAShB,CAEIkB,EAAW4S,GACX+M,EAAc7gB,KAAK,KAnBX,CAoBhB,CAEA,OAAO6gB,EAAc/kB,KAAK,GAC9B,CHiakCglB,CAAiBhoB,EAAed,EAASC,EAAMgjB,GAErE,GAAI8F,UAAUC,UACVD,UAAUC,UAAUC,UAAUR,OAC3B,CACH,MAAMS,EAAWjb,SAASsL,cAAc,YACxC2P,EAASvrB,MAAQ8qB,EACjBxa,SAASkb,KAAKhjB,YAAY+iB,GAC1BA,EAASvB,SACT1Z,SAASmb,YAAY,QACrBnb,SAASkb,KAAKjjB,YAAYgjB,EAC9B,GAiCIG,CAAgBrF,GAIxB,IAGJ,IAAIsF,gBAAe,KACftrB,EAAQ6mB,kBAAkB,IAC3B0E,QAAQhnB,GAEXvE,EAAQ4mB,iBAAiB9W,EAAO,SAAUkW,IAEtCP,GAAYzlB,GAERgmB,EAAMwF,OAAO7rB,OACb0nB,GAAO,GAEPvX,EAAMpP,MAAM+qB,QAAU,EACtB3b,EAAMpP,MAAMgrB,cAAgB,SAGxB1F,EAAM2F,WACNhE,GAAM,GAEV7X,EAAMpP,MAAM+qB,QAAU,EACtB3b,EAAMpP,MAAMgrB,cAAgB,OAChC,IAGJ1rB,EAAQ4mB,iBAAiB9W,EAAO,SAAUkW,IACtCA,EAAMwE,iBAAiB,IAG3BxqB,EAAQ4mB,iBAAiB9W,EAAO,YAAakW,IACzCA,EAAMwE,iBAAiB,IAG3BxqB,EAAQ4mB,iBAAiB9W,EAAO,aAAckW,IAC1CA,EAAMwE,iBAAiB,IAG3BxqB,EAAQ4mB,iBAAiB9W,EAAO,WAAYkW,IACxC,OAAQA,EAAMrgB,KACV,IAAK,QACL,IAAK,SACD,MACJ,IAAK,SACL,IAAK,YACL,IAAK,UACL,IAAK,YACL,IAAK,YACL,IAAK,aACmB,KAAhBmK,EAAMnQ,QACNqmB,EAAMwE,kBACNxqB,EAAQ6mB,oBAEZ,MACJ,QACIb,EAAMwE,kBAENxqB,EAAQ6mB,mBAEhB,GAER,CAEe,SAASpiB,GAAWF,EAAS8d,GACxC3gB,QAAQ0G,IAAI,cAEZke,GAAW/hB,GAEX,MAAMvE,EAAUuE,EAAQ,uBACxBvE,EAAQuiB,gBAAkBF,EAEJ,OAAlBriB,EAAQ0H,OACR+d,GAAYzlB,GAEZ4P,EAAO5P,IAGPA,EAAQ6mB,kBAEhB,C,GInlBI+E,yBAA2B,CAAC,EAGhC,SAASC,oBAAoBC,GAE5B,IAAIC,EAAeH,yBAAyBE,GAC5C,QAAqBja,IAAjBka,EACH,OAAOA,EAAavmB,QAGrB,IAAID,EAASqmB,yBAAyBE,GAAY,CAGjDtmB,QAAS,CAAC,GAOX,OAHAwmB,oBAAoBF,GAAUvmB,EAAQA,EAAOC,QAASqmB,qBAG/CtmB,EAAOC,OACf,CCrBAqmB,oBAAoBpoB,EAAK8B,IACxB,IAAI0mB,EAAS1mB,GAAUA,EAAO2mB,WAC7B,IAAO3mB,EAAiB,QACxB,IAAM,EAEP,OADAsmB,oBAAoBM,EAAEF,EAAQ,CAAE1iB,EAAG0iB,IAC5BA,CAAM,ECLdJ,oBAAoBM,EAAI,CAAC3mB,EAAS4mB,KACjC,IAAI,IAAIzmB,KAAOymB,EACXP,oBAAoBQ,EAAED,EAAYzmB,KAASkmB,oBAAoBQ,EAAE7mB,EAASG,IAC5EK,OAAOsmB,eAAe9mB,EAASG,EAAK,CAAE4mB,YAAY,EAAMvlB,IAAKolB,EAAWzmB,IAE1E,ECNDkmB,oBAAoBQ,EAAI,CAACG,EAAKC,IAAUzmB,OAAO0mB,UAAUC,eAAeC,KAAKJ,EAAKC,GCClFZ,oBAAoBnT,EAAKlT,IACH,oBAAXqnB,QAA0BA,OAAOC,aAC1C9mB,OAAOsmB,eAAe9mB,EAASqnB,OAAOC,YAAa,CAAEntB,MAAO,WAE7DqG,OAAOsmB,eAAe9mB,EAAS,aAAc,CAAE7F,OAAO,GAAO,ECL9D,IAAIotB,iBAAmB,WACnB,IAAIC,EAAS/c,SAASgd,cACtB,IAAKD,EAAQ,CAOT,IAHA,IAAIE,EAAcjd,SAASkd,qBAAqB,UAC5CC,EAAU,GAELC,EAAI,EAAGA,EAAIH,EAAYllB,OAAQqlB,IACpCD,EAAQpjB,KAAKkjB,EAAYG,IAI7BL,GADAI,EAAUA,EAAQlmB,QAAO,SAASomB,GAAK,OAAQA,EAAEC,QAAUD,EAAE7sB,OAAS6sB,EAAEE,WAAa,KACpErjB,OAAO,GAAG,EAC/B,CAEA,OAAO6iB,CACX,EAEIS,cAAgB,SAAST,GACzB,MAAO,6BAA6BU,KAAKV,EAAOW,IACpD,EAMYC,IAQZ,GAZA5nB,OAAOsmB,eAAeT,oBAAqB,IAAK,CAC5C7kB,KAGQ4mB,IAFSb,mBAEIY,IAAIE,MAAM,KAAK1jB,MAAM,GAAI,GAAGrE,KAAK,KAAO,IAElD,WACH,OAAO8nB,GACX,KAIsB,oBAAnBE,eAAgC,CACvC,IAAIC,mBAAqBD,eACzBA,eAAiB,SAASE,GACtB,IAAIhB,EAASD,mBACTkB,EAAUR,cAAcT,GAExBW,EAAMI,mBAAmBC,GAE7B,IAAIC,EACA,OAAON,EAGX,IAAIO,EAAeP,EAAIE,MAAM,KACzBM,EAAgBD,EAAa/jB,OAAO,GAAG,GAAG0jB,MAAM,KAKpD,OAHAM,EAAcC,OAAO,EAAG,EAAG,qBAC3BF,EAAaE,QAAQ,EAAG,EAAGD,EAAcroB,KAAK,MAEvCooB,EAAapoB,KAAK,IAC7B,CACJ,C",
     "names": [
         "isString",
         "value",
         "String",
         "useResolvedFormatting",
         "formatting",
         "useMemo",
@@ -16,43 +16,54 @@
         "row",
         "condition",
         "eval",
         "concat",
         "text",
         "style",
         "padding",
+        "draw",
         "edit",
         "mappedEdit",
         "validate",
         "parse",
         "autoCommit",
         "auto_commit",
+        "toggle",
         "useResolvedFiltering",
         "filtering",
+        "useResolvedDataSelector",
+        "dataSelector",
         "DashSpreadGrid",
         "props",
         "console",
         "count",
         "setProps",
         "counter",
         "useRef",
         "data",
         "columns",
         "rows",
+        "data_selector",
         "pinnedTop",
         "pinned_top",
         "pinnedBottom",
         "pinned_bottom",
         "pinnedLeft",
         "pinned_left",
         "pinnedRight",
         "pinned_right",
         "filters",
-        "onFiltersChange",
+        "editedCells",
+        "edited_cells",
+        "selectedCells",
+        "selected_cells",
+        "onSelectedCellsChange",
         "useCallback",
+        "onFiltersChange",
+        "onEditedCellsChange",
         "clickedCell",
         "clicked_cell",
         "onCellClick",
         "cell",
         "_objectSpread",
         "n",
         "current",
@@ -73,57 +84,49 @@
         "createGrid",
         "React",
         "ref",
         "propTypes",
         "PropTypes",
         "id",
         "sorting",
-        "dataSelector",
         "borderWidth",
         "focusedCell",
-        "selectedCells",
         "highlightedCells",
-        "editedCells",
-        "sortBy",
+        "sort_by",
         "columnWidths",
         "rowHeights",
         "defaultProps",
         "module",
         "exports",
         "window",
+        "stringifyId",
         "key",
         "Array",
         "isArray",
         "join",
         "object",
         "Object",
         "keys",
         "sort",
         "JSON",
         "stringify",
-        "getCellType",
+        "getCellEditType",
         "type",
         "getEditableCells",
         "formatResolver",
         "columnLookup",
         "rowLookup",
         "columnKey",
         "columnId",
         "rowKey",
         "rowId",
         "has",
         "get",
         "resolve",
         "filter",
-        "defaultFont",
-        "defaultPadding",
-        "top",
-        "right",
-        "bottom",
-        "left",
         "roundToPixels",
         "devicePixelRatio",
         "Math",
         "round",
         "renderSection",
         "vertical",
         "horizontal",
@@ -155,14 +158,16 @@
         "height",
         "width",
         "totalWidth",
         "reduce",
         "a",
         "b",
         "totalHeight",
+        "left",
+        "top",
         "horizontalOffsets",
         "acc",
         "index",
         "offset",
         "push",
         "verticalOffsets",
         "columnOffsets",
@@ -198,32 +203,34 @@
         "rect",
         "clip",
         "save",
         "cellTop",
         "cellLeft",
         "cellWidth",
         "cellHeight",
-        "textAlign",
         "textBaseline",
         "background",
-        "draw",
         "highlight",
         "corner",
         "moveTo",
         "lineTo",
         "fill",
         "foreground",
         "font",
         "fontMetrics",
         "getFontMetrics",
+        "textAlign",
+        "measureWidth",
+        "right",
         "textX",
         "textY",
         "middle",
         "topOffset",
         "bottomOffset",
+        "bottom",
         "fillText",
         "strokeStyle",
         "lineWidth",
         "stroke",
         "restore",
         "drawBorder",
         "x1",
@@ -269,39 +276,52 @@
         "isTextValid",
         "renderInput",
         "resizableColumn",
         "resizableRow",
         "cursor",
         "renderCursor",
         "renderInternal",
+        "errorRendered",
         "display",
         "flexDirection",
+        "userSelect",
         "innerHTML",
         "message",
         "stack",
         "renderError",
+        "filterRule",
+        "newValue",
+        "string",
         "getDataFormatting",
-        "match",
+        "sortBy",
         "undefined",
         "header",
         "direction",
-        "newValue",
-        "string",
+        "commonFields",
+        "hasImpact",
+        "includes",
+        "getReducedFormatting",
+        "fields",
+        "acceptedFields",
+        "reducedRule",
+        "field",
         "getInputFormatting",
         "getHighlightColor",
         "baseColor",
         "isStrong",
         "getRenderFormatting",
         "hoveredCell",
         "selection",
         "edition",
         "focusedColumnKey",
         "focusedRowKey",
         "isResizingRow",
         "isResizing",
+        "selectionBorderWidth",
+        "resizableBorderWidth",
         "isSelected",
         "isKeySelected",
         "optional",
         "border",
         "Number",
         "MAX_SAFE_INTEGER",
         "hasValueByKey",
@@ -366,20 +386,22 @@
         "widthsLookup",
         "getResolvedRows",
         "heightsLookup",
         "getPlacedColumns",
         "newColumn",
         "getPlacedRows",
         "newRow",
-        "matchMapping",
+        "defaultFont",
+        "defaultPadding",
+        "typeMapping",
         "Lookup",
         "byKey",
         "byIndex",
         "byLabel",
-        "byMatch",
+        "byType",
         "RulesLookup",
         "hasRules",
         "addRule",
         "c",
         "r",
         "addColumnRule",
         "label",
@@ -390,14 +412,15 @@
         "newRules",
         "gatherRowRules",
         "borderTypes",
         "defaultEdit",
         "indexBorders",
         "newStyle",
         "borderType",
+        "getEdit",
         "FormattingRules",
         "rulesLookup",
         "entries",
         "entry",
         "array",
         "currentContext",
         "getText",
@@ -421,15 +444,14 @@
         "getFilteredColumns",
         "filteredRows",
         "rowFilters",
         "getFixedSize",
         "getTotalSize",
         "TextResolver",
         "createElement",
-        "measureWidth",
         "measureText",
         "measureHeight",
         "lines",
         "char",
         "textMetrics",
         "actualBoundingBoxDescent",
         "actualBoundingBoxAscent",
@@ -442,14 +464,24 @@
         "min",
         "expand",
         "margin",
         "subtract",
         "requiredMargin",
         "preloadedMargin",
         "emptyRect",
+        "getInternalPosition",
+        "position",
+        "fixedSize",
+        "totalSize",
+        "scrollOffset",
+        "scrollLeft",
+        "scrollTop",
+        "clientSize",
+        "clientWidth",
+        "clientHeight",
         "getLookup",
         "getHighlightedCells",
         "isMouseDown",
         "hoveredColumnKey",
         "hoveredRowKey",
         "minColumnIndex",
         "maxColumnIndex",
@@ -457,29 +489,27 @@
         "maxRowIndex",
         "flatMap",
         "getCellSection",
         "getVerticalSection",
         "getHorizontalSection",
         "getInputPlacement",
         "editableCells",
-        "position",
         "getIsTextValid",
         "every",
         "getDefaultIds",
         "getDefaultRowIds",
         "getDefaultColumnIds",
         "getUnfoldedColumns",
         "some",
         "unfoldedColumns",
         "ids",
         "selector",
         "getUnfoldedRows",
         "unfoldedRows",
         "defaultCondition",
-        "includes",
         "FilteringRules",
         "by",
         "filterContext",
         "getFilteringRules",
         "getFilterFormatting",
         "getMeasureFormatting",
         "getMeasuredColumns",
@@ -496,15 +526,14 @@
         "getKeys",
         "getSortingFormatting",
         "defaultComparatorAsc",
         "lhs",
         "rhs",
         "defaultComparatorDesc",
         "SortingRules",
-        "stringifyId",
         "comparatorAsc",
         "comparator",
         "comparatorDesc",
         "sortByLookup",
         "Error",
         "getSortingRules",
         "getSortByLookup",
@@ -516,14 +545,15 @@
         "sortedColumns",
         "reverse",
         "getSortedColumns",
         "sortedRows",
         "grabOffset",
         "getResizableColumn",
         "mousePosition",
+        "internalPosition",
         "getResizableRow",
         "getResolvedSortBy",
         "getResolvedFilters",
         "getActiveColumns",
         "callback",
         "getActive",
         "updateStateInternal",
@@ -552,22 +582,14 @@
         "measureFormatting",
         "measureFormattingRules",
         "measureFormatResolver",
         "columnWidthCache",
         "rowHeightCache",
         "measuredColumns",
         "measuredRows",
-        "fixedSize",
-        "totalSize",
-        "scrollOffset",
-        "scrollLeft",
-        "scrollTop",
-        "clientSize",
-        "clientWidth",
-        "clientHeight",
         "hoverRowIndex",
         "iterA",
         "iterC",
         "iterB",
         "floor",
         "getRowIndex",
         "hoverColumnIndex",
@@ -594,25 +616,25 @@
         "getReducedCells",
         "cellsToRemove",
         "getMousePosition",
         "event",
         "currentTarget",
         "clientX",
         "clientY",
+        "getWithAssumedId",
+        "defaultId",
         "initialize",
         "setAttribute",
         "classList",
         "renderRequested",
         "requestAnimationFrame",
         "listener",
         "addEventListener",
         "requestNewRender",
         "onFocusedCellChange",
-        "onSelectedCellsChange",
-        "onEditedCellsChange",
         "onSortByChange",
         "onColumnWidthsChange",
         "onRowHeightsChange",
         "setText",
         "dispatchEvent",
         "Event",
         "accept",
@@ -634,26 +656,26 @@
         "mouseDownPosition",
         "mouseDownCell",
         "ctrlKey",
         "setPointerCapture",
         "pointerId",
         "releasePointerCapture",
         "cellData",
-        "toggle",
         "indexOf",
         "getToggledValue",
         "cellType",
         "newSortBy",
         "isCurrentRule",
         "directionLoop",
         "currentRule",
         "find",
         "directionIndex",
         "newDirection",
         "isLastRule",
+        "isConflictingWithCurrentRule",
         "getNewSortBy",
         "resizableColumnKey",
         "resizableRowKey",
         "select",
         "setSelectedCells",
         "setFocusedCell",
         "arrowTo",
@@ -730,44 +752,46 @@
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///./src/lib/components/DashSpreadGrid.jsx",
         "webpack:///external window \"PropTypes\"",
         "webpack:///external window \"React\"",
         "webpack:///../lib/src/core-utils/stringifyId.js",
-        "webpack:///../lib/src/state-utils/getCellType.js",
+        "webpack:///../lib/src/state-utils/getCellEditType.js",
         "webpack:///../lib/src/state-utils/getEditableCells.js",
-        "webpack:///../lib/src/core-utils/defaults.js",
         "webpack:///../lib/src/core-utils/roundToPixels.js",
         "webpack:///../lib/src/core/render.js",
         "webpack:///../lib/src/state-utils/getDataFormatting.js",
+        "webpack:///../lib/src/state-utils/getReducedFormatting.js",
         "webpack:///../lib/src/state-utils/getInputFormatting.js",
         "webpack:///../lib/src/state-utils/getRenderFormatting.js",
         "webpack:///../lib/src/state-utils/getSections.js",
         "webpack:///../lib/src/state-utils/getEditedCellsAndFilters.js",
         "webpack:///../lib/src/types/Edition.js",
         "webpack:///../lib/src/state-utils/getEdition.js",
         "webpack:///../lib/src/types/Selection.js",
         "webpack:///../lib/src/state-utils/getSelection.js",
         "webpack:///../lib/src/state-utils/getInvoked.js",
         "webpack:///../lib/src/state-utils/getPinned.js",
         "webpack:///../lib/src/state-utils/getResolved.js",
         "webpack:///../lib/src/state-utils/getPlaced.js",
+        "webpack:///../lib/src/core-utils/defaults.js",
         "webpack:///../lib/src/types/RulesLookup.js",
         "webpack:///../lib/src/types/FormattingRules.js",
         "webpack:///../lib/src/state-utils/getFormattingRules.js",
         "webpack:///../lib/src/types/FormatResolver.js",
         "webpack:///../lib/src/state-utils/getFormatResolver.js",
         "webpack:///../lib/src/state-utils/getFiltered.js",
         "webpack:///../lib/src/state-utils/getFixedSize.js",
         "webpack:///../lib/src/state-utils/getTotalSize.js",
         "webpack:///../lib/src/types/TextResolver.js",
         "webpack:///../lib/src/state-utils/getTextResolver.js",
         "webpack:///../lib/src/core-utils/rect.js",
         "webpack:///../lib/src/state-utils/getScrollRect.js",
+        "webpack:///../lib/src/state-utils/getInternalPosition.js",
         "webpack:///../lib/src/state-utils/getLookup.js",
         "webpack:///../lib/src/state-utils/getHighlightedCells.js",
         "webpack:///../lib/src/state-utils/getCellSection.js",
         "webpack:///../lib/src/state-utils/getInputPlacement.js",
         "webpack:///../lib/src/state-utils/getIsTextValid.js",
         "webpack:///../lib/src/state-utils/getUnfolded.js",
         "webpack:///../lib/src/types/FilteringRules.js",
@@ -787,93 +811,97 @@
         "webpack:///../lib/src/core/state.js",
         "webpack:///../lib/src/state-utils/getHoveredCell.js",
         "webpack:///../lib/src/state-utils/getRowIndex.js",
         "webpack:///../lib/src/state-utils/getColumnIndex.js",
         "webpack:///../lib/src/state-utils/getCombinedCells.js",
         "webpack:///../lib/src/state-utils/getReducedCells.js",
         "webpack:///../lib/src/state-utils/getMousePosition.js",
+        "webpack:///../lib/src/state-utils/getWithAssumedId.js",
         "webpack:///../lib/src/index.js",
         "webpack:///../lib/src/state-utils/getToggledValue.js",
         "webpack:///../lib/src/state-utils/getNewSortBy.js",
         "webpack:///../lib/src/state-utils/getClipboardData.js",
         "webpack:///webpack/bootstrap",
         "webpack:///webpack/runtime/compat get default export",
         "webpack:///webpack/runtime/define property getters",
         "webpack:///webpack/runtime/hasOwnProperty shorthand",
         "webpack:///webpack/runtime/make namespace object",
         "webpack:///webpack/runtime/compat"
     ],
     "sourcesContent": [
-        "/* eslint-disable import/prefer-default-export */\n\nimport React, { useCallback, useMemo, useRef, useState } from 'react';\nimport PropTypes from 'prop-types';\nimport createGrid from 'js-spread-grid';\n\nfunction isString(value) {\n    return typeof value === 'string' || value instanceof String;\n}\n\nfunction useResolvedFormatting(formatting) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, newValue, text, string}';\n\n        return formatting.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n            if ('value' in rule)\n                mappedRule.value = eval(`(${context})=> (${rule.value})`);\n            if ('text' in rule)\n                mappedRule.text = eval(`(${context}) => (${rule.text})`);\n            if ('style' in rule)\n                mappedRule.style = isString(rule.style) ? eval(`(${context}) => (${rule.style})`) : rule.style;\n            if ('padding' in rule)\n                mappedRule.padding = isString(rule.padding) ? eval(`(${context}) => (${rule.padding})`) : rule.padding;\n            if ('edit' in rule)\n                if (rule.edit) {\n                    const mappedEdit = {};\n                    if ('validate' in rule.edit)\n                        mappedEdit.validate = eval(`({string}) => (${rule.edit.validate})`);\n                    if ('parse' in rule.edit)\n                        mappedEdit.parse = eval(`(${context}) => (${rule.edit.parse})`);\n                    if ('auto_commit' in rule.edit)\n                        mappedEdit.autoCommit = rule.edit.auto_commit;\n                    mappedRule.edit = mappedEdit;\n                }\n                else {\n                    mappedRule.edit = rule.edit;\n                }\n\n            return mappedRule;\n        });\n    }, [formatting]);\n}\n\nfunction useResolvedFiltering(filtering) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, text, expression}';\n\n        return filtering.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n\n            return mappedRule;\n        });\n    }, [filtering]);\n}\n\n// TODO: Write description\n// TODO: Rename to DashSpreadGrid\nfunction DashSpreadGrid(props) {\n    console.count('render DashSpreadGrid');\n\n    const setProps = props.setProps;\n    const counter = useRef(0);\n\n    const data = props.data;\n    const columns = props.columns;\n    const rows = props.rows;\n    const formatting = useResolvedFormatting(props.formatting);\n    const filtering = useResolvedFiltering(props.filtering);\n    const pinnedTop = props.pinned_top;\n    const pinnedBottom = props.pinned_bottom;\n    const pinnedLeft = props.pinned_left;\n    const pinnedRight = props.pinned_right;\n    const filters = props.filters;\n    const onFiltersChange = useCallback((filters) => {\n        setProps({ filters });\n    }, [setProps]);\n    const clickedCell = props.clicked_cell;\n    const onCellClick = useCallback((cell) => {\n        setProps({ clicked_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const clickedCustomCell = props.clicked_custom_cell;\n    const onCustomCellClick = useCallback((cell) => {\n        setProps({ clicked_custom_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const onActiveColumnsChange = useCallback((activeColumns) => {\n        setProps({ active_columns: activeColumns });\n    }, [setProps]);\n    const onActiveRowsChange = useCallback((activeRows) => {\n        setProps({ active_rows: activeRows });\n    }, [setProps]);\n\n    const [element, setElement] = useState(null);\n\n    if (element)\n        createGrid(element, {\n            data,\n            columns,\n            rows,\n            formatting,\n            filtering,\n            pinnedTop,\n            pinnedBottom,\n            pinnedLeft,\n            pinnedRight,\n            filters,\n            onFiltersChange,\n            clickedCell,\n            onCellClick,\n            clickedCustomCell,\n            onCustomCellClick,\n            onActiveColumnsChange,\n            onActiveRowsChange\n        });\n\n    return React.createElement(\"div\", { ref: setElement });\n};\n\n// TODO: add descriptions\n// TODO: Fix types\nDashSpreadGrid.propTypes = {\n    // _\n    setProps: PropTypes.func,\n    // _\n    id: PropTypes.string,\n    // _\n    data: PropTypes.any,\n    // _\n    columns: PropTypes.array,\n    // _\n    rows: PropTypes.array,\n    // _\n    formatting: PropTypes.array,\n    // _\n    filtering: PropTypes.array,\n    // _\n    sorting: PropTypes.array,\n    // _\n    dataSelector: PropTypes.string,\n    // _\n    pinned_top: PropTypes.number,\n    // _\n    pinned_bottom: PropTypes.number,\n    // _\n    pinned_left: PropTypes.number,\n    // _\n    pinned_right: PropTypes.number,\n    // _\n    borderWidth: PropTypes.number,\n    // _\n    focusedCell: PropTypes.object,\n    // _\n    selectedCells: PropTypes.array,\n    // _\n    highlightedCells: PropTypes.array,\n    // _\n    editedCells: PropTypes.array,\n    // _\n    filters: PropTypes.array,\n    // _\n    sortBy: PropTypes.array,\n    // _\n    columnWidths: PropTypes.array,\n    // _\n    rowHeights: PropTypes.array,\n    // _\n    clicked_cell: PropTypes.object,\n    // _\n    clicked_custom_cell: PropTypes.object,\n    // _\n    active_columns: PropTypes.array,\n    // _\n    active_rows: PropTypes.array\n};\n\nDashSpreadGrid.defaultProps = {\n    data: [],\n    columns: [{ \"type\": \"DATA-BLOCK\" }],\n    rows: [{ \"type\": \"HEADER\" }, { \"type\": \"DATA-BLOCK\" }],\n    formatting: [],\n    filtering: [],\n    sorting: [],\n    dataSelector: \"data[row.id][column.id]\",\n    pinned_top: 0,\n    pinned_bottom: 0,\n    pinned_left: 0,\n    pinned_right: 0,\n    borderWidth: 1,\n    focusedCell: null,\n    selectedCells: [],\n    highlightedCells: [],\n    editedCells: [],\n    filters: [],\n    sortBy: [],\n    columnWidths: [],\n    rowHeights: [],\n    clicked_cell: null,\n    clicked_custom_cell: null,\n    active_columns: [],\n    active_rows: []\n};\n\nexport default DashSpreadGrid;\n",
+        "/* eslint-disable import/prefer-default-export */\n\nimport React, { useCallback, useMemo, useRef, useState } from 'react';\nimport PropTypes from 'prop-types';\nimport createGrid from 'js-spread-grid';\n\nfunction isString(value) {\n    return typeof value === 'string' || value instanceof String;\n}\n\nfunction useResolvedFormatting(formatting) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, newValue, text, string, ctx}';\n\n        return formatting.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n            if ('value' in rule)\n                mappedRule.value = eval(`(${context})=> (${rule.value})`);\n            if ('text' in rule)\n                mappedRule.text = eval(`(${context}) => (${rule.text})`);\n            if ('style' in rule)\n                mappedRule.style = isString(rule.style) ? eval(`(${context}) => (${rule.style})`) : rule.style;\n            if ('padding' in rule)\n                mappedRule.padding = isString(rule.padding) ? eval(`(${context}) => (${rule.padding})`) : rule.padding;\n            if ('draw' in rule)\n                mappedRule.draw = eval(`(${context}) => {${rule.draw}}`);\n            if ('edit' in rule)\n                if (rule.edit) {\n                    const mappedEdit = {};\n                    if ('validate' in rule.edit)\n                        mappedEdit.validate = eval(`({string}) => (${rule.edit.validate})`);\n                    if ('parse' in rule.edit)\n                        mappedEdit.parse = eval(`(${context}) => (${rule.edit.parse})`);\n                    if ('auto_commit' in rule.edit)\n                        mappedEdit.autoCommit = rule.edit.auto_commit;\n                    if ('toggle' in rule.edit)\n                        mappedEdit.toggle = rule.edit.toggle;\n                    mappedRule.edit = mappedEdit;\n                }\n                else {\n                    mappedRule.edit = rule.edit;\n                }\n\n            return mappedRule;\n        });\n    }, [formatting]);\n}\n\nfunction useResolvedFiltering(filtering) {\n    return useMemo(() => {\n        const context = '{data, rows, columns, row, column, value, text, expression}';\n\n        return filtering.map(rule => {\n            const mappedRule = {};\n\n            if ('column' in rule)\n                mappedRule.column = rule.column;\n            if ('row' in rule)\n                mappedRule.row = rule.row;\n            if ('condition' in rule)\n                mappedRule.condition = eval(`(${context}) => (${rule.condition})`);\n\n            return mappedRule;\n        });\n    }, [filtering]);\n}\n\nfunction useResolvedDataSelector(dataSelector) {\n    return useMemo(() => {\n        return eval(`({data, row, column}) => (${dataSelector})`);\n    }, [dataSelector]);\n}\n\n// TODO: Write description\n// TODO: Rename to DashSpreadGrid\nfunction DashSpreadGrid(props) {\n    console.count('render DashSpreadGrid');\n\n    const setProps = props.setProps;\n    const counter = useRef(0);\n\n    const data = props.data;\n    const columns = props.columns;\n    const rows = props.rows;\n    const formatting = useResolvedFormatting(props.formatting);\n    const filtering = useResolvedFiltering(props.filtering);\n    const dataSelector = useResolvedDataSelector(props.data_selector);\n    const pinnedTop = props.pinned_top;\n    const pinnedBottom = props.pinned_bottom;\n    const pinnedLeft = props.pinned_left;\n    const pinnedRight = props.pinned_right;\n    const filters = props.filters;\n    const editedCells = props.edited_cells;\n    const selectedCells = props.selected_cells;\n    const onSelectedCellsChange = useCallback((selectedCells) => {\n        setProps({ selected_cells: selectedCells });\n    }, [setProps]);\n    const onFiltersChange = useCallback((filters) => {\n        setProps({ filters });\n    }, [setProps]);\n    const onEditedCellsChange = useCallback((editedCells) => {\n        setProps({ edited_cells: editedCells });\n    }, [setProps]);\n    const clickedCell = props.clicked_cell;\n    const onCellClick = useCallback((cell) => {\n        setProps({ clicked_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const clickedCustomCell = props.clicked_custom_cell;\n    const onCustomCellClick = useCallback((cell) => {\n        setProps({ clicked_custom_cell: { ...cell, n: counter.current++ } });\n    }, [setProps]);\n    const onActiveColumnsChange = useCallback((activeColumns) => {\n        setProps({ active_columns: activeColumns });\n    }, [setProps]);\n    const onActiveRowsChange = useCallback((activeRows) => {\n        setProps({ active_rows: activeRows });\n    }, [setProps]);\n\n    const [element, setElement] = useState(null);\n\n    if (element)\n        createGrid(element, {\n            data,\n            columns,\n            rows,\n            formatting,\n            filtering,\n            pinnedTop,\n            pinnedBottom,\n            pinnedLeft,\n            pinnedRight,\n            filters,\n            dataSelector,\n            editedCells,\n            selectedCells,\n            onSelectedCellsChange,\n            onEditedCellsChange,\n            onFiltersChange,\n            clickedCell,\n            onCellClick,\n            clickedCustomCell,\n            onCustomCellClick,\n            onActiveColumnsChange,\n            onActiveRowsChange\n        });\n\n    return React.createElement(\"div\", { ref: setElement });\n};\n\n// TODO: add descriptions\n// TODO: Fix types\nDashSpreadGrid.propTypes = {\n    // _\n    setProps: PropTypes.func,\n    // _\n    id: PropTypes.string,\n    // _\n    data: PropTypes.any,\n    // _\n    columns: PropTypes.array,\n    // _\n    rows: PropTypes.array,\n    // _\n    formatting: PropTypes.array,\n    // _\n    filtering: PropTypes.array,\n    // _\n    sorting: PropTypes.array,\n    // _\n    data_selector: PropTypes.string,\n    // _\n    pinned_top: PropTypes.number,\n    // _\n    pinned_bottom: PropTypes.number,\n    // _\n    pinned_left: PropTypes.number,\n    // _\n    pinned_right: PropTypes.number,\n    // _\n    borderWidth: PropTypes.number,\n    // _\n    focusedCell: PropTypes.object,\n    // _\n    selected_cells: PropTypes.array,\n    // _\n    highlightedCells: PropTypes.array,\n    // _\n    edited_cells: PropTypes.array,\n    // _\n    filters: PropTypes.array,\n    // _\n    sort_by: PropTypes.array,\n    // _\n    columnWidths: PropTypes.array,\n    // _\n    rowHeights: PropTypes.array,\n    // _\n    clicked_cell: PropTypes.object,\n    // _\n    clicked_custom_cell: PropTypes.object,\n    // _\n    active_columns: PropTypes.array,\n    // _\n    active_rows: PropTypes.array\n};\n\nDashSpreadGrid.defaultProps = {\n    data: [],\n    columns: [{ \"type\": \"DATA-BLOCK\" }],\n    rows: [{ \"type\": \"HEADER\" }, { \"type\": \"DATA-BLOCK\" }],\n    formatting: [],\n    filtering: [],\n    sorting: [],\n    data_selector: \"data[row.id][column.id]\",\n    pinned_top: 0,\n    pinned_bottom: 0,\n    pinned_left: 0,\n    pinned_right: 0,\n    borderWidth: 1,\n    focusedCell: null,\n    selected_cells: [],\n    highlightedCells: [],\n    edited_cells: [],\n    filters: [],\n    sort_by: [],\n    columnWidths: [],\n    rowHeights: [],\n    clicked_cell: null,\n    clicked_custom_cell: null,\n    active_columns: [],\n    active_rows: []\n};\n\nexport default DashSpreadGrid;\n",
         "module.exports = window[\"PropTypes\"];",
         "module.exports = window[\"React\"];",
         "function stringifyObject(object) {\n    const keys = Object.keys(object).sort();\n    const stringified = keys.map(key => {\n        return `${key}:${stringifyId(object[key])}`\n    });\n\n    return `{${stringified.join(',')}}`;\n}\n\nfunction stringifyArray(array) {\n    const stringified = array.map(stringifyId);\n\n    return `[${stringified.join(',')}]`;\n}\n\nexport default function stringifyId(key) {\n    if (key === null)\n        return 'null'\n\n    if (Array.isArray(key))\n        return stringifyArray(key)\n\n    if (typeof key === 'object')\n        return stringifyObject(key)\n\n    return JSON.stringify(key)\n}",
-        "export default function getCellType(column, row) {\n    if (column.type === 'FILTER' ^ row.type === 'FILTER')\n        return 'FILTER';\n    if (column.type === 'DATA' && row.type === 'DATA')\n        return 'DATA';\n    return 'OTHER';\n}",
-        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getCellType from \"./getCellType.js\";\n\nexport default function getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup) {\n    return selectedCells.map(cell => {\n        const columnKey = stringifyId(cell.columnId);\n        const rowKey = stringifyId(cell.rowId);\n\n        if (!columnLookup.has(columnKey))\n            return null;\n        if (!rowLookup.has(rowKey))\n            return null;\n\n        const column = columnLookup.get(columnKey);\n        const row = rowLookup.get(rowKey);\n\n        return {\n            edit: formatResolver.resolve(row, column).edit,\n            cell: cell,\n            type: getCellType(column, row)\n        }\n    }).filter(cell => cell?.edit);\n}",
-        "const defaultFont = '12px Calibri';\nconst defaultPadding = { top: 2, right: 5, bottom: 2, left: 5 };\n\nexport { defaultFont, defaultPadding };",
+        "export default function getCellEditType(column, row) {\n    if (column.type === 'FILTER' ^ row.type === 'FILTER')\n        return 'FILTER';\n    return 'DATA';\n}",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getCellEditType from \"./getCellEditType.js\";\n\nexport default function getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup) {\n    return selectedCells.map(cell => {\n        const columnKey = stringifyId(cell.columnId);\n        const rowKey = stringifyId(cell.rowId);\n\n        if (!columnLookup.has(columnKey))\n            return null;\n        if (!rowLookup.has(rowKey))\n            return null;\n\n        const column = columnLookup.get(columnKey);\n        const row = rowLookup.get(rowKey);\n\n        return {\n            edit: formatResolver.resolve(row, column).edit,\n            cell: cell,\n            type: getCellEditType(column, row)\n        }\n    }).filter(cell => cell?.edit);\n}",
         "export default function roundToPixels(value, devicePixelRatio) {\n    return Math.round(value * devicePixelRatio) / devicePixelRatio;\n}",
-        "import { defaultFont } from \"../core-utils/defaults.js\";\nimport roundToPixels from \"../core-utils/roundToPixels.js\";\n\nfunction renderSection(context, vertical, horizontal) {\n    const state = context.state;\n    const canvas = context.canvases[`${vertical}-${horizontal}`];\n    const verticalSection = state.sections[vertical];\n    const horizontalSection = state.sections[horizontal];\n    const columns = horizontalSection.columns;\n    const rows = verticalSection.rows;\n\n    if (rows.length === 0 || columns.length === 0) {\n        if (canvas.parentElement)\n            canvas.parentElement.removeChild(canvas);\n        return;\n    }\n\n    if (!canvas.parentElement)\n        context.element.appendChild(canvas);\n\n    // Checking how often this is called\n    console.log('draw');\n\n    // TODO: Borders are still blurry after scrolling at high zoom-out levels\n\n    const ctx = canvas.getContext(\"2d\", { alpha: false });\n    // TODO: Make that \"1\" configurable as cell spacing\n    const scrollRect = state.scrollRect;\n    const textResolver = state.textResolver;\n    // TODO: Make sure those formatters are split based on the rule areas\n    const formatResolver = state.renderFormatResolver;\n    const borderWidth = state.borderWidth;\n    const sectionBorders = {\n        top: verticalSection.showTopBorder,\n        bottom: verticalSection.showBottomBorder,\n        left: horizontalSection.showLeftBorder,\n        right: horizontalSection.showRightBorder\n    };\n    const borderOffset = borderWidth / 2;\n    const rowCount = rows.length;\n    const columnCount = columns.length;\n    const horizontalBorderCount = rowCount - 1 + (sectionBorders.top ? 1 : 0) + (sectionBorders.bottom ? 1 : 0);\n    const verticalBorderCount = columnCount - 1 + (sectionBorders.left ? 1 : 0) + (sectionBorders.right ? 1 : 0);\n    const rowHeights = rows.map(row => row.height);\n    const columnWidths = columns.map(column => column.width);\n    const totalWidth = columnWidths.reduce((a, b) => a + b, 0) + verticalBorderCount * borderWidth;\n    const totalHeight = rowHeights.reduce((a, b) => a + b, 0) + horizontalBorderCount * borderWidth;\n\n    const left = horizontal === 'center'\n        ? scrollRect.left\n        : 0;\n    const top = vertical === 'middle'\n        ? scrollRect.top\n        : 0;\n    const width = horizontal === 'center'\n        ? scrollRect.width\n        : horizontalSection.width;\n    const height = vertical === 'middle'\n        ? scrollRect.height\n        : verticalSection.height;\n\n    // TODO: Move somewhere else\n    const horizontalOffsets = columnWidths.reduce((acc, width, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + width + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.left ? borderWidth : 0]);\n    const verticalOffsets = rowHeights.reduce((acc, height, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + height + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.top ? borderWidth : 0]);\n\n    const columnOffsets = horizontalOffsets.slice(0, -1);\n    const rowOffsets = verticalOffsets.slice(0, -1);\n\n    const minVisibleColumnIndex = Math.max(columnOffsets.findLastIndex(offset => offset <= left), 0);\n    const maxVisibleColumnIndex = columnOffsets.findLastIndex(offset => offset <= left + width);\n    const minVisibleRowIndex = Math.max(rowOffsets.findLastIndex(offset => offset <= top), 0);\n    const maxVisibleRowIndex = rowOffsets.findLastIndex(offset => offset <= top + height);\n\n    const minVisibleVerticalBorderIndex = Math.max(minVisibleColumnIndex, sectionBorders.left ? 0 : 1);\n    const maxVisibleVerticalBorderIndex = maxVisibleColumnIndex + (sectionBorders.right ? 1 : 0);\n    const minVisibleHorizontalBorderIndex = Math.max(minVisibleRowIndex, sectionBorders.top ? 0 : 1);\n    const maxVisibleHorizontalBorderIndex = maxVisibleRowIndex + (sectionBorders.bottom ? 1 : 0);\n\n    const cells = Array.from({ length: maxVisibleRowIndex - minVisibleRowIndex + 1 }, (_, rowIndex) => {\n        const row = rows[rowIndex + minVisibleRowIndex];\n        return Array.from({ length: maxVisibleColumnIndex - minVisibleColumnIndex + 1 }, (_, columnIndex) => {\n            const column = columns[columnIndex + minVisibleColumnIndex];\n            return formatResolver.resolve(row, column);\n        });\n    });\n    const getCell = (rowIndex, columnIndex) => cells[rowIndex - minVisibleRowIndex][columnIndex - minVisibleColumnIndex];\n\n    canvas.width = Math.round(width * devicePixelRatio);\n    canvas.height = Math.round(height * devicePixelRatio);\n    canvas.style.width = `${width}px`;\n    canvas.style.height = `${height}px`;\n    canvas.style.marginLeft = `${left}px`;\n    canvas.style.marginTop = `${top}px`;\n    canvas.style.marginRight = `${totalWidth - width - left}px`;\n    canvas.style.marginBottom = `${totalHeight - height - top}px`;;\n\n    ctx.fillStyle = \"#E9E9E9\";\n    ctx.fillRect(0, 0, canvas.width, canvas.height);\n\n    const setTransform = (x, y) => {\n        ctx.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (x - left) * devicePixelRatio, (y - top) * devicePixelRatio);\n    };\n    const setClip = (x, y, width, height) => {\n        ctx.beginPath();\n        ctx.rect(x, y, width, height);\n        ctx.clip();\n    };\n\n    // Draw cells\n    for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n        ctx.save();\n        setTransform(horizontalOffsets[columnIndex], 0);\n        setClip(0, 0, columnWidths[columnIndex], totalHeight);\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const cell = getCell(rowIndex, columnIndex);\n            const style = cell.style;\n            const cellTop = verticalOffsets[rowIndex];\n            const cellLeft = horizontalOffsets[columnIndex];\n            const cellWidth = columnWidths[columnIndex];\n            const cellHeight = rowHeights[rowIndex];\n            const text = cell.text;\n            const textAlign = style.textAlign || 'left';\n            const textBaseline = style.textBaseline || 'middle';\n            const padding = cell.padding;\n\n            setTransform(cellLeft, cellTop);\n\n            ctx.fillStyle = style.background || 'white';\n            ctx.fillRect(0, 0, cellWidth, cellHeight);\n\n            if ('draw' in cell)\n                cell.draw(ctx);\n\n            if (style.highlight) {\n                ctx.fillStyle = style.highlight;\n                ctx.fillRect(0, 0, cellWidth, cellHeight);\n            }\n\n            if (style.corner) {\n                ctx.fillStyle = style.corner;\n                ctx.beginPath();\n                ctx.moveTo(cellWidth - 7, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight - 7);\n                ctx.fill();\n            }\n\n            ctx.fillStyle = style.foreground || 'black';\n            ctx.font = style.font || defaultFont;\n            ctx.textAlign = textAlign;\n\n            const fontMetrics = textResolver.getFontMetrics(style.font);\n\n            // TODO: Make sure that values are rounded using devicePixelRatio\n            const textX = roundToPixels(\n                textAlign === 'left' ? padding.left :\n                    textAlign === 'center' ? cellWidth / 2 :\n                        textAlign === 'right' ? cellWidth - padding.right :\n                            0,\n                devicePixelRatio\n            );\n\n            const textY = roundToPixels(\n                textBaseline === 'top' ? fontMetrics.middle + fontMetrics.topOffset + padding.top :\n                    textBaseline === 'middle' ? cellHeight / 2 + fontMetrics.middle :\n                        textBaseline === 'bottom' ? cellHeight + fontMetrics.middle - fontMetrics.bottomOffset - padding.bottom :\n                            0,\n                devicePixelRatio\n            );\n\n            const fitsVertically = textY - fontMetrics.middle - fontMetrics.topOffset >= 0 && textY - fontMetrics.middle + fontMetrics.bottomOffset <= cellHeight;\n\n            if (fitsVertically) {\n                ctx.fillText(text, textX, textY);\n            }\n            else {\n                // TODO: Clip if the text is too high (and draw some indicator if you do)\n                ctx.strokeStyle = '#E9E9E9';\n                ctx.lineWidth = borderWidth;\n\n                ctx.beginPath();\n                ctx.moveTo(0, borderWidth + borderOffset);\n                ctx.lineTo(cellWidth, borderWidth + borderOffset);\n                ctx.moveTo(0, cellHeight - borderWidth - borderOffset);\n                ctx.lineTo(cellWidth, cellHeight - borderWidth - borderOffset);\n                ctx.stroke();\n\n                ctx.save();\n                setClip(0, 2 * borderWidth, cellWidth, cellHeight - 4 * borderWidth);\n\n                ctx.fillText(text, textX, textY);\n\n                ctx.restore();\n            }\n        }\n\n        ctx.restore();\n    }\n\n    setTransform(0, 0);\n\n    // Draw borders\n\n    // TODO: clip drawing area to the middle of neighboring columns/rows (might be useful for redrawing only the changed cells)\n    // TODO: move somewhere (?)\n    const drawBorder = (x1, y1, x2, y2, style) => {\n        if (!style)\n            return;\n\n        const width = style.width * borderWidth;\n\n        const isHorizontal = y1 === y2;\n\n        // TODO: Don't add offset if the border is not continued\n        const xa = x1 - (isHorizontal ? width / 2 : 0);\n        const ya = y1 - (!isHorizontal ? width / 2 : 0);\n        const xb = x2 + (isHorizontal ? width / 2 : 0);\n        const yb = y2 + (!isHorizontal ? width / 2 : 0);\n\n        ctx.strokeStyle = style.color || 'black'; // TODO: resolve this color earlier\n        ctx.lineWidth = width;\n\n        if (style.dash) {\n            ctx.setLineDash(style.dash.map(value => value / devicePixelRatio));\n            ctx.lineDashOffset = (isHorizontal ? xa : ya);\n        }\n        else {\n            ctx.setLineDash([]);\n        }\n\n        ctx.beginPath();\n        ctx.moveTo(xa, ya);\n        ctx.lineTo(xb, yb);\n        ctx.stroke();\n    }\n\n    const selectBorder = (borderStyleA, borderStyleB) => {\n        if (!borderStyleA)\n            return borderStyleB;\n\n        if (!borderStyleB)\n            return borderStyleA;\n\n        if (borderStyleA.index > borderStyleB.index)\n            return borderStyleA;\n\n        return borderStyleB;\n    }\n\n    // TODO: Move somewhere else (?)\n    for (let horizontalBorderIndex = minVisibleHorizontalBorderIndex; horizontalBorderIndex <= maxVisibleHorizontalBorderIndex; horizontalBorderIndex++) {\n        const topRowIndex = horizontalBorderIndex - 1;\n        const bottomRowIndex = horizontalBorderIndex;\n\n        for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n            const topBorderStyle = topRowIndex >= minVisibleRowIndex ? getCell(topRowIndex, columnIndex).style.borderBottom : null;\n            const bottomBorderStyle = bottomRowIndex <= maxVisibleRowIndex ? getCell(bottomRowIndex, columnIndex).style.borderTop : null;\n\n            const borderStyle = selectBorder(topBorderStyle, bottomBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[columnIndex] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                horizontalOffsets[columnIndex + 1] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                borderStyle);\n        }\n    }\n\n    for (let verticalBorderIndex = minVisibleVerticalBorderIndex; verticalBorderIndex <= maxVisibleVerticalBorderIndex; verticalBorderIndex++) {\n        const leftColumnIndex = verticalBorderIndex - 1;\n        const rightColumnIndex = verticalBorderIndex;\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const leftBorderStyle = leftColumnIndex >= minVisibleColumnIndex ? getCell(rowIndex, leftColumnIndex).style.borderRight : null;\n            const rightBorderStyle = rightColumnIndex <= maxVisibleColumnIndex ? getCell(rowIndex, rightColumnIndex).style.borderLeft : null;\n\n            const borderStyle = selectBorder(leftBorderStyle, rightBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex] - borderOffset,\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex + 1] - borderOffset,\n                borderStyle);\n        }\n    }\n}\n\nfunction renderInput(context) {\n    const element = context.element;\n    const input = context.input;\n    const state = context.state;\n    const inputPlacement = state.inputPlacement;\n\n    if (!inputPlacement) {\n        if (input.parentElement) {\n            const hasFocus = document.activeElement === input;\n            input.parentElement.removeChild(input);\n            if (hasFocus)\n                element.focus({ preventScroll: true });\n        }\n        return;\n    }\n\n    const canvas = context.canvases[inputPlacement.section];\n\n    input.style.left = 'left' in inputPlacement ? `${inputPlacement.left}px` : '0';\n    input.style.top = 'top' in inputPlacement ? `${inputPlacement.top}px` : '0';\n    input.style.right = 'right' in inputPlacement ? `${inputPlacement.right}px` : '0';\n    input.style.bottom = 'bottom' in inputPlacement ? `${inputPlacement.bottom}px` : '0';\n    input.style.marginLeft = 'marginLeft' in inputPlacement ? `${inputPlacement.marginLeft}px` : '0';\n    input.style.marginTop = 'marginTop' in inputPlacement ? `${inputPlacement.marginTop}px` : '0';\n    input.style.width = `${inputPlacement.width}px`;\n    input.style.height = `${inputPlacement.height}px`;\n    input.style.gridArea = canvas.style.gridArea;\n    input.style.zIndex = canvas.style.zIndex;\n    input.style.backgroundColor = state.isTextValid ? 'white' : '#eb3434';\n\n    if (!input.parentElement) {\n        const hasFocus = document.activeElement === element;\n        element.appendChild(input);\n        if (hasFocus)\n            input.focus({ preventScroll: true });\n    }\n}\n\nfunction renderCursor(context) {\n    const element = context.element;\n    const state = context.state;\n\n    if (state.resizableColumn && state.resizableRow)\n        element.style.cursor = 'nwse-resize';\n    else if (state.resizableColumn)\n        element.style.cursor = 'col-resize';\n    else if (state.resizableRow)\n        element.style.cursor = 'row-resize';\n    else\n        element.style.cursor = 'default';\n}\n\nfunction renderInternal(context) {\n    renderSection(context, 'top', 'left');\n    renderSection(context, 'top', 'center');\n    renderSection(context, 'top', 'right');\n    renderSection(context, 'middle', 'left');\n    renderSection(context, 'middle', 'center');\n    renderSection(context, 'middle', 'right');\n    renderSection(context, 'bottom', 'left');\n    renderSection(context, 'bottom', 'center');\n    renderSection(context, 'bottom', 'right');\n\n    renderInput(context);\n    renderCursor(context);\n}\n\nfunction renderError(context) {\n    const element = context.element;\n    const error = context.error;\n\n    element.style.backgroundColor = '#9f0000';\n    element.style.color = 'white';\n    element.style.padding = '20px';\n    element.style.display = 'flex';\n    element.style.flexDirection = 'column';\n    element.innerHTML = `\n        <div style=\"font-size: 16px;\">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style=\"font-size: 20px; font-weight: bold; padding: 20px 0;\">\n            ${error.message}\n        </div>\n        <div style=\"font-size: 16px; white-space: pre-wrap;\">${error.stack}</div>\n    `;\n}\n\nexport default function render(context) {\n    if (!context.error) {\n        try {\n            renderInternal(context);\n        }\n        catch (error) {\n            context.error = error;\n        }\n    }\n\n    if (context.error)\n        renderError(context);\n}",
-        "export default function getDataFormatting(formatting, dataSelector, sortBy) {\n    return [\n        {\n            column: { match: 'DATA' },\n            row: { match: 'HEADER' },\n            value: ({ column }) => column.header === undefined ? column.id : column.header\n        },\n        {\n            column: { match: 'HEADER' },\n            row: { match: 'DATA' },\n            value: ({ row }) => row.header === undefined ? row.id : row.header\n        },\n        {\n            column: { match: 'HEADER' },\n            row: { match: 'SPECIAL' },\n            value: ''\n        },\n        {\n            column: { match: 'SPECIAL' },\n            row: { match: 'HEADER' },\n            value: ''\n        },\n        ...sortBy.map(({ columnId, rowId, direction }, index) => ({\n            column: { id: columnId },\n            row: { id: rowId },\n            text: ({ column }) => `${sortBy.length > 1 ? index + 1 : ''}${direction === 'ASC' ? '\u21e3' : '\u21e1'} ${column.header}`\n        })),\n        {\n            column: { match: 'ANY' },\n            row: { match: 'FILTER' },\n            value: ({ newValue }) => newValue || '',\n            text: ({ newValue }) => newValue || 'Search...', // TODO: Move to render formatting?\n            edit: {\n                validate: () => true,\n                parse: ({ string }) => string,\n                autoCommit: true\n            },\n        },\n        {\n            column: { match: 'DATA' },\n            row: { match: 'DATA' },\n            value: dataSelector\n        },\n        ...formatting\n    ];\n}",
-        "export default function getInputFormatting(formatting) {\n    return formatting;\n}",
-        "import stringifyId from '../core-utils/stringifyId.js';\n\nfunction getHighlightColor(baseColor, isStrong) {\n    if (isStrong)\n        return baseColor + '99';\n    else\n        return baseColor + '33';\n}\n\nexport default function getRenderFormatting(formatting, hoveredCell, focusedCell, selection, highlight, edition, resizableColumn, resizableRow) {\n    const focusedColumnKey = focusedCell ? stringifyId(focusedCell.columnId) : null;\n    const focusedRowKey = focusedCell ? stringifyId(focusedCell.rowId) : null;\n    const isResizingColumn = resizableColumn !== null;\n    const isResizingRow = resizableRow !== null;\n    const isResizing = isResizingColumn || isResizingRow;\n\n    const isSelected = (rows, columns, rowIndex, columnIndex) => {\n        if (rowIndex < 0 || rowIndex >= rows.length)\n            return false;\n        if (columnIndex < 0 || columnIndex >= columns.length)\n            return false;\n\n        const rowKey = rows[rowIndex].key;\n        const columnKey = columns[columnIndex].key;\n\n        return selection.isKeySelected(rowKey, columnKey);\n    };\n\n    const optional = (condition, style) => {\n        if (condition)\n            return [style];\n        else\n            return [];\n    }\n\n    return [\n        {\n            column: { match: 'ANY' },\n            row: { match: 'FILTER' },\n            style: ({ newValue }) => ({ background: '#FBFBFB', foreground: newValue ? 'black' : '#cccccc', border: { width: 1, color: 'gray' } })\n        },\n        {\n            column: { match: 'ANY' },\n            row: { match: 'HEADER' },\n            style: { background: '#F5F5F5', border: { width: 1, color: 'gray' } }\n        },\n        {\n            column: { match: 'HEADER' },\n            row: { match: 'ANY' },\n            style: { background: '#F5F5F5', border: { width: 1, color: 'gray' } }\n        },\n        {\n            column: { match: 'HEADER' },\n            row: { match: 'HEADER' },\n            style: { background: '#E0E0E0' }\n        },\n        ...formatting,\n        // TODO: optionally re-enable\n        // ...optional(hoveredCell && !isResizingColumn, {\n        //     column: { id: hoveredCell?.columnId },\n        //     row: { match: 'ANY' },\n        //     style: { highlight: '#81948133' },\n        // }),\n        ...optional(hoveredCell && !isResizingRow, {\n            column: { match: 'ANY' },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948133' },\n        }),\n        ...optional(hoveredCell && !isResizing, {\n            column: { id: hoveredCell?.columnId },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948188' },\n        }),\n        {\n            column: { match: 'ANY' },\n            row: { match: 'ANY' },\n            condition: ({ rows, columns, row, column }) => isSelected(rows, columns, row.index, column.index),\n            style: ({ rows, columns, row, column, edit }) => ({\n                ...(!isSelected(rows, columns, row.index - 1, column.index) ? { borderTop: { width: 3, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index + 1, column.index) ? { borderBottom: { width: 3, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index - 1) ? { borderLeft: { width: 3, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index + 1) ? { borderRight: { width: 3, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                highlight: getHighlightColor(edit ? '#798d9c' : '#819481', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            }),\n        },\n        {\n            column: { match: 'ANY' },\n            row: { match: 'ANY' },\n            condition: ({ row, column }) => highlight.isKeySelected(row.key, column.key),\n            style: ({ row, column }) => ({\n                highlight: getHighlightColor('#93a8b8', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            })\n        },\n        ...optional(focusedCell, {\n            column: { id: focusedCell?.columnId },\n            row: { id: focusedCell?.rowId },\n            style: { highlight: '#ffffffaa' }\n        }),\n        {\n            column: { match: 'ANY' },\n            row: { match: 'ANY' },\n            condition: ({ edit }) => edit,\n            style: { corner: '#77777720' },\n        },\n        {\n            column: { match: 'ANY' },\n            row: { match: 'ANY' },\n            condition: ({ row, column }) => edition.hasValueByKey(row.key, column.key),\n            style: { corner: 'darkgreen' },\n        },\n        ...optional(resizableColumn, {\n            column: { id: resizableColumn },\n            row: { match: 'HEADER' },\n            style: { borderRight: { width: 5, color: 'cornflowerblue' } }\n        }),\n        ...optional(resizableRow, {\n            column: { match: 'HEADER' },\n            row: { id: resizableRow },\n            style: { borderBottom: { width: 5, color: 'cornflowerblue' } }\n        }),\n    ];\n}",
+        "import roundToPixels from \"../core-utils/roundToPixels.js\";\n\nfunction renderSection(context, vertical, horizontal) {\n    const state = context.state;\n    const canvas = context.canvases[`${vertical}-${horizontal}`];\n    const verticalSection = state.sections[vertical];\n    const horizontalSection = state.sections[horizontal];\n    const columns = horizontalSection.columns;\n    const rows = verticalSection.rows;\n\n    if (rows.length === 0 || columns.length === 0) {\n        if (canvas.parentElement)\n            canvas.parentElement.removeChild(canvas);\n        return;\n    }\n\n    if (!canvas.parentElement)\n        context.element.appendChild(canvas);\n\n    // Checking how often this is called\n    console.log('draw');\n\n    // TODO: Borders are still blurry after scrolling at high zoom-out levels\n\n    const ctx = canvas.getContext(\"2d\", { alpha: false });\n    // TODO: Make that \"1\" configurable as cell spacing\n    const scrollRect = state.scrollRect;\n    const textResolver = state.textResolver;\n    // TODO: Make sure those formatters are split based on the rule areas\n    const formatResolver = state.renderFormatResolver;\n    const borderWidth = state.borderWidth;\n    const sectionBorders = {\n        top: verticalSection.showTopBorder,\n        bottom: verticalSection.showBottomBorder,\n        left: horizontalSection.showLeftBorder,\n        right: horizontalSection.showRightBorder\n    };\n    const borderOffset = borderWidth / 2;\n    const rowCount = rows.length;\n    const columnCount = columns.length;\n    const horizontalBorderCount = rowCount - 1 + (sectionBorders.top ? 1 : 0) + (sectionBorders.bottom ? 1 : 0);\n    const verticalBorderCount = columnCount - 1 + (sectionBorders.left ? 1 : 0) + (sectionBorders.right ? 1 : 0);\n    const rowHeights = rows.map(row => row.height);\n    const columnWidths = columns.map(column => column.width);\n    const totalWidth = columnWidths.reduce((a, b) => a + b, 0) + verticalBorderCount * borderWidth;\n    const totalHeight = rowHeights.reduce((a, b) => a + b, 0) + horizontalBorderCount * borderWidth;\n\n    const left = horizontal === 'center'\n        ? scrollRect.left\n        : 0;\n    const top = vertical === 'middle'\n        ? scrollRect.top\n        : 0;\n    const width = horizontal === 'center'\n        ? scrollRect.width\n        : horizontalSection.width;\n    const height = vertical === 'middle'\n        ? scrollRect.height\n        : verticalSection.height;\n\n    // TODO: Move somewhere else\n    const horizontalOffsets = columnWidths.reduce((acc, width, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + width + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.left ? borderWidth : 0]);\n    const verticalOffsets = rowHeights.reduce((acc, height, index) => {\n        const prevOffset = acc[index];\n        const offset = prevOffset + height + borderWidth;\n        acc.push(offset);\n        return acc;\n    }, [sectionBorders.top ? borderWidth : 0]);\n\n    const columnOffsets = horizontalOffsets.slice(0, -1);\n    const rowOffsets = verticalOffsets.slice(0, -1);\n\n    const minVisibleColumnIndex = Math.max(columnOffsets.findLastIndex(offset => offset <= left), 0);\n    const maxVisibleColumnIndex = columnOffsets.findLastIndex(offset => offset <= left + width);\n    const minVisibleRowIndex = Math.max(rowOffsets.findLastIndex(offset => offset <= top), 0);\n    const maxVisibleRowIndex = rowOffsets.findLastIndex(offset => offset <= top + height);\n\n    const minVisibleVerticalBorderIndex = Math.max(minVisibleColumnIndex, sectionBorders.left ? 0 : 1);\n    const maxVisibleVerticalBorderIndex = maxVisibleColumnIndex + (sectionBorders.right ? 1 : 0);\n    const minVisibleHorizontalBorderIndex = Math.max(minVisibleRowIndex, sectionBorders.top ? 0 : 1);\n    const maxVisibleHorizontalBorderIndex = maxVisibleRowIndex + (sectionBorders.bottom ? 1 : 0);\n\n    const cells = Array.from({ length: maxVisibleRowIndex - minVisibleRowIndex + 1 }, (_, rowIndex) => {\n        const row = rows[rowIndex + minVisibleRowIndex];\n        return Array.from({ length: maxVisibleColumnIndex - minVisibleColumnIndex + 1 }, (_, columnIndex) => {\n            const column = columns[columnIndex + minVisibleColumnIndex];\n            return formatResolver.resolve(row, column);\n        });\n    });\n    const getCell = (rowIndex, columnIndex) => cells[rowIndex - minVisibleRowIndex][columnIndex - minVisibleColumnIndex];\n\n    canvas.width = Math.round(width * devicePixelRatio);\n    canvas.height = Math.round(height * devicePixelRatio);\n    canvas.style.width = `${width}px`;\n    canvas.style.height = `${height}px`;\n    canvas.style.marginLeft = `${left}px`;\n    canvas.style.marginTop = `${top}px`;\n    canvas.style.marginRight = `${totalWidth - width - left}px`;\n    canvas.style.marginBottom = `${totalHeight - height - top}px`;;\n\n    ctx.fillStyle = \"#E9E9E9\";\n    ctx.fillRect(0, 0, canvas.width, canvas.height);\n\n    const setTransform = (x, y) => {\n        ctx.setTransform(devicePixelRatio, 0, 0, devicePixelRatio, (x - left) * devicePixelRatio, (y - top) * devicePixelRatio);\n    };\n    const setClip = (x, y, width, height) => {\n        ctx.beginPath();\n        ctx.rect(x, y, width, height);\n        ctx.clip();\n    };\n\n    // Draw cells\n    for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n        ctx.save();\n        setTransform(horizontalOffsets[columnIndex], 0);\n        setClip(0, 0, columnWidths[columnIndex], totalHeight);\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const cell = getCell(rowIndex, columnIndex);\n            const style = cell.style;\n            const cellTop = verticalOffsets[rowIndex];\n            const cellLeft = horizontalOffsets[columnIndex];\n            const cellWidth = columnWidths[columnIndex];\n            const cellHeight = rowHeights[rowIndex];\n            const text = cell.text;\n            const textBaseline = style.textBaseline || 'middle';\n            const padding = cell.padding;\n\n            setTransform(cellLeft, cellTop);\n\n            ctx.fillStyle = style.background || 'white';\n            ctx.fillRect(0, 0, cellWidth, cellHeight);\n\n            if ('draw' in cell)\n                cell.draw(ctx);\n\n            if (style.highlight) {\n                ctx.fillStyle = style.highlight;\n                ctx.fillRect(0, 0, cellWidth, cellHeight);\n            }\n\n            if (style.corner) {\n                ctx.fillStyle = style.corner;\n                ctx.beginPath();\n                ctx.moveTo(cellWidth - 7, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight);\n                ctx.lineTo(cellWidth, cellHeight - 7);\n                ctx.fill();\n            }\n\n            if (text) {\n                ctx.fillStyle = style.foreground || 'black';\n                ctx.font = cell.font;\n\n                const fontMetrics = textResolver.getFontMetrics(cell.font);\n\n                const textAlign = (style.textAlign == 'center' && textResolver.measureWidth(text, cell.font) > cellWidth - padding.left - padding.right)\n                    ? 'left'\n                    : style.textAlign || 'left';\n                ctx.textAlign = textAlign;\n\n                // TODO: Make sure that values are rounded using devicePixelRatio\n                const textX = roundToPixels(\n                    textAlign === 'left' ? padding.left :\n                        textAlign === 'center' ? cellWidth / 2 :\n                            textAlign === 'right' ? cellWidth - padding.right :\n                                0,\n                    devicePixelRatio\n                );\n\n                const textY = roundToPixels(\n                    textBaseline === 'top' ? fontMetrics.middle + fontMetrics.topOffset + padding.top :\n                        textBaseline === 'middle' ? cellHeight / 2 + fontMetrics.middle :\n                            textBaseline === 'bottom' ? cellHeight + fontMetrics.middle - fontMetrics.bottomOffset - padding.bottom :\n                                0,\n                    devicePixelRatio\n                );\n\n                const fitsVertically = textY - fontMetrics.middle - fontMetrics.topOffset >= 0 && textY - fontMetrics.middle + fontMetrics.bottomOffset <= cellHeight;\n\n                if (fitsVertically) {\n                    ctx.fillText(text, textX, textY);\n                }\n                else {\n                    // TODO: Clip if the text is too high (and draw some indicator if you do)\n                    ctx.strokeStyle = '#E9E9E9';\n                    ctx.lineWidth = borderWidth;\n\n                    ctx.beginPath();\n                    ctx.moveTo(0, borderWidth + borderOffset);\n                    ctx.lineTo(cellWidth, borderWidth + borderOffset);\n                    ctx.moveTo(0, cellHeight - borderWidth - borderOffset);\n                    ctx.lineTo(cellWidth, cellHeight - borderWidth - borderOffset);\n                    ctx.stroke();\n\n                    ctx.save();\n                    setClip(0, 2 * borderWidth, cellWidth, cellHeight - 4 * borderWidth);\n\n                    ctx.fillText(text, textX, textY);\n\n                    ctx.restore();\n                }\n            }\n        }\n\n        ctx.restore();\n    }\n\n    setTransform(0, 0);\n\n    // Draw borders\n\n    // TODO: clip drawing area to the middle of neighboring columns/rows (might be useful for redrawing only the changed cells)\n    // TODO: move somewhere (?)\n    const drawBorder = (x1, y1, x2, y2, style) => {\n        if (!style)\n            return;\n        if (style.width === 0)\n            return;\n\n        const width = style.width / devicePixelRatio\n\n        const isHorizontal = y1 === y2;\n\n        // TODO: Don't add offset if the border is not continued\n        const xa = x1 - (isHorizontal ? width / 2 : 0);\n        const ya = y1 - (!isHorizontal ? width / 2 : 0);\n        const xb = x2 + (isHorizontal ? width / 2 : 0);\n        const yb = y2 + (!isHorizontal ? width / 2 : 0);\n\n        ctx.strokeStyle = style.color || 'black'; // TODO: resolve this color earlier\n        ctx.lineWidth = width;\n\n        if (style.dash) {\n            ctx.setLineDash(style.dash.map(value => value / devicePixelRatio));\n            ctx.lineDashOffset = (isHorizontal ? xa : ya);\n        }\n        else {\n            ctx.setLineDash([]);\n        }\n\n        ctx.beginPath();\n        ctx.moveTo(xa, ya);\n        ctx.lineTo(xb, yb);\n        ctx.stroke();\n    }\n\n    const selectBorder = (borderStyleA, borderStyleB) => {\n        if (!borderStyleA)\n            return borderStyleB;\n\n        if (!borderStyleB)\n            return borderStyleA;\n\n        if (borderStyleA.index > borderStyleB.index)\n            return borderStyleA;\n\n        return borderStyleB;\n    }\n\n    // TODO: Move somewhere else (?)\n    for (let horizontalBorderIndex = minVisibleHorizontalBorderIndex; horizontalBorderIndex <= maxVisibleHorizontalBorderIndex; horizontalBorderIndex++) {\n        const topRowIndex = horizontalBorderIndex - 1;\n        const bottomRowIndex = horizontalBorderIndex;\n\n        for (let columnIndex = minVisibleColumnIndex; columnIndex <= maxVisibleColumnIndex; columnIndex++) {\n            const topBorderStyle = topRowIndex >= minVisibleRowIndex ? getCell(topRowIndex, columnIndex).style.borderBottom : null;\n            const bottomBorderStyle = bottomRowIndex <= maxVisibleRowIndex ? getCell(bottomRowIndex, columnIndex).style.borderTop : null;\n\n            const borderStyle = selectBorder(topBorderStyle, bottomBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[columnIndex] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                horizontalOffsets[columnIndex + 1] - borderOffset,\n                verticalOffsets[bottomRowIndex] - borderOffset,\n                borderStyle);\n        }\n    }\n\n    for (let verticalBorderIndex = minVisibleVerticalBorderIndex; verticalBorderIndex <= maxVisibleVerticalBorderIndex; verticalBorderIndex++) {\n        const leftColumnIndex = verticalBorderIndex - 1;\n        const rightColumnIndex = verticalBorderIndex;\n\n        for (let rowIndex = minVisibleRowIndex; rowIndex <= maxVisibleRowIndex; rowIndex++) {\n            const leftBorderStyle = leftColumnIndex >= minVisibleColumnIndex ? getCell(rowIndex, leftColumnIndex).style.borderRight : null;\n            const rightBorderStyle = rightColumnIndex <= maxVisibleColumnIndex ? getCell(rowIndex, rightColumnIndex).style.borderLeft : null;\n\n            const borderStyle = selectBorder(leftBorderStyle, rightBorderStyle);\n\n            drawBorder(\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex] - borderOffset,\n                horizontalOffsets[rightColumnIndex] - borderOffset,\n                verticalOffsets[rowIndex + 1] - borderOffset,\n                borderStyle);\n        }\n    }\n}\n\nfunction renderInput(context) {\n    const element = context.element;\n    const input = context.input;\n    const state = context.state;\n    const inputPlacement = state.inputPlacement;\n\n    if (!inputPlacement) {\n        if (input.parentElement) {\n            const hasFocus = document.activeElement === input;\n            input.parentElement.removeChild(input);\n            if (hasFocus)\n                element.focus({ preventScroll: true });\n        }\n        return;\n    }\n\n    const canvas = context.canvases[inputPlacement.section];\n\n    input.style.left = 'left' in inputPlacement ? `${inputPlacement.left}px` : '0';\n    input.style.top = 'top' in inputPlacement ? `${inputPlacement.top}px` : '0';\n    input.style.right = 'right' in inputPlacement ? `${inputPlacement.right}px` : '0';\n    input.style.bottom = 'bottom' in inputPlacement ? `${inputPlacement.bottom}px` : '0';\n    input.style.marginLeft = 'marginLeft' in inputPlacement ? `${inputPlacement.marginLeft}px` : '0';\n    input.style.marginTop = 'marginTop' in inputPlacement ? `${inputPlacement.marginTop}px` : '0';\n    input.style.width = `${inputPlacement.width}px`;\n    input.style.height = `${inputPlacement.height}px`;\n    input.style.gridArea = canvas.style.gridArea;\n    input.style.zIndex = canvas.style.zIndex;\n    input.style.backgroundColor = state.isTextValid ? 'white' : '#eb3434';\n\n    if (!input.parentElement) {\n        const hasFocus = document.activeElement === element;\n        element.appendChild(input);\n        if (hasFocus)\n            input.focus({ preventScroll: true });\n    }\n}\n\nfunction renderCursor(context) {\n    const element = context.element;\n    const state = context.state;\n\n    if (state.resizableColumn && state.resizableRow)\n        element.style.cursor = 'nwse-resize';\n    else if (state.resizableColumn)\n        element.style.cursor = 'col-resize';\n    else if (state.resizableRow)\n        element.style.cursor = 'row-resize';\n    else\n        element.style.cursor = 'default';\n}\n\nfunction renderInternal(context) {\n    renderSection(context, 'top', 'left');\n    renderSection(context, 'top', 'center');\n    renderSection(context, 'top', 'right');\n    renderSection(context, 'middle', 'left');\n    renderSection(context, 'middle', 'center');\n    renderSection(context, 'middle', 'right');\n    renderSection(context, 'bottom', 'left');\n    renderSection(context, 'bottom', 'center');\n    renderSection(context, 'bottom', 'right');\n\n    renderInput(context);\n    renderCursor(context);\n}\n\nfunction renderError(context) {\n    if (context.errorRendered)\n        return;\n\n    context.errorRendered = true;\n\n    const element = context.element;\n    const error = context.error;\n\n    element.style.backgroundColor = '#9f0000';\n    element.style.color = 'white';\n    element.style.padding = '20px';\n    element.style.display = 'flex';\n    element.style.flexDirection = 'column';\n    element.style.userSelect = 'text';\n    element.innerHTML = `\n        <div style=\"font-size: 16px;\">\n            An error occurred while rendering the grid, please contact the support.\n        </div>\n        <div style=\"font-size: 20px; font-weight: bold; padding: 20px 0;\">\n            ${error.message}\n        </div>\n        <div style=\"font-size: 16px; white-space: pre-wrap;\">${error.stack}</div>\n    `;\n}\n\nexport default function render(context) {\n    if (!context.error) {\n        try {\n            renderInternal(context);\n        }\n        catch (error) {\n            context.error = error;\n        }\n    }\n\n    if (context.error)\n        renderError(context);\n}",
+        "const filterRule = {\n    value: ({ newValue }) => newValue || '',\n    text: ({ newValue }) => newValue || 'Search...', // TODO: Move to render formatting?\n    edit: {\n        validate: () => true,\n        parse: ({ string }) => string,\n        autoCommit: true\n    }\n};\n\nexport default function getDataFormatting(formatting, dataSelector, sortBy) {\n    return [\n        {\n            column: { type: 'DATA' },\n            row: { type: 'HEADER' },\n            value: ({ column }) => column.header === undefined ? column.id : column.header\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'DATA' },\n            value: ({ row }) => row.header === undefined ? row.id : row.header\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'SPECIAL' },\n            value: ''\n        },\n        {\n            column: { type: 'SPECIAL' },\n            row: { type: 'HEADER' },\n            value: ''\n        },\n        {\n            column: { type: 'DATA' },\n            row: { type: 'FILTER' },\n            ...filterRule\n        },\n        {\n            column: { type: 'FILTER' },\n            row: { type: 'DATA' },\n            ...filterRule\n        },\n        {\n            column: { type: 'DATA' },\n            row: { type: 'DATA' },\n            value: dataSelector\n        },\n        ...formatting,\n        // TODO: Fix headers of sorted rows\n        ...sortBy.map(({ columnId, rowId, direction }, index) => ({\n            column: { id: columnId },\n            row: { id: rowId },\n            text: ({ value, text }) => `${sortBy.length > 1 ? index + 1 : ''}${direction === 'ASC' ? '\u21e3' : '\u21e1'} ${text || value}`\n        })),\n    ];\n}",
+        "const commonFields = ['column', 'row', 'condition'];\n\nfunction reduce(rule, fields) {\n  const reducedRule = {};\n  for (const field of fields) {\n    if (field in rule)\n      reducedRule[field] = rule[field];\n  }\n  return reducedRule;\n}\n\nfunction hasImpact(rule) {\n  const allKeys = Object.keys(rule).length;\n  const commonKeys = Object.keys(rule).filter(key => commonFields.includes(key)).length;\n\n  return allKeys > commonKeys;\n}\n\nexport default function getReducedFormatting(formatting, fields) {\n  const acceptedFields = [...commonFields, ...fields];\n\n  return formatting.map(rule => reduce(rule, acceptedFields)).filter(hasImpact);\n}",
+        "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getInputFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text', 'edit']);\n}",
+        "import stringifyId from '../core-utils/stringifyId.js';\n\nfunction getHighlightColor(baseColor, isStrong) {\n    if (isStrong)\n        return baseColor + '99';\n    else\n        return baseColor + '33';\n}\n\nexport default function getRenderFormatting(formatting, hoveredCell, focusedCell, selection, highlight, edition, sortBy, resizableColumn, resizableRow, borderWidth) {\n    const focusedColumnKey = focusedCell ? stringifyId(focusedCell.columnId) : null;\n    const focusedRowKey = focusedCell ? stringifyId(focusedCell.rowId) : null;\n    const isResizingColumn = resizableColumn !== null;\n    const isResizingRow = resizableRow !== null;\n    const isResizing = isResizingColumn || isResizingRow;\n    const selectionBorderWidth = borderWidth + 2;\n    const resizableBorderWidth = borderWidth + 4;\n\n    const isSelected = (rows, columns, rowIndex, columnIndex) => {\n        if (rowIndex < 0 || rowIndex >= rows.length)\n            return false;\n        if (columnIndex < 0 || columnIndex >= columns.length)\n            return false;\n\n        const rowKey = rows[rowIndex].key;\n        const columnKey = columns[columnIndex].key;\n\n        return selection.isKeySelected(rowKey, columnKey);\n    };\n\n    const optional = (condition, style) => {\n        if (condition)\n            return [style];\n        else\n            return [];\n    }\n\n    return [\n        {\n            column: { type: 'DATA' },\n            row: { type: 'FILTER' },\n            style: ({ newValue }) => ({ background: '#FBFBFB', foreground: newValue ? 'black' : '#cccccc', border: { width: 1, color: 'gray' } })\n        },\n        {\n            column: { type: 'FILTER' },\n            row: { type: 'DATA' },\n            style: ({ newValue }) => ({ background: '#FBFBFB', foreground: newValue ? 'black' : '#cccccc', border: { width: 1, color: 'gray' } })\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'HEADER' },\n            style: { background: '#F5F5F5', border: { width: borderWidth, color: 'gray' } }\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'ANY' },\n            style: { background: '#F5F5F5', border: { width: borderWidth, color: 'gray' } }\n        },\n        {\n            column: { type: 'HEADER' },\n            row: { type: 'HEADER' },\n            style: { background: '#E0E0E0' }\n        },\n        ...formatting,\n        // TODO: optionally re-enable\n        // ...optional(hoveredCell && !isResizingColumn, {\n        //     column: { id: hoveredCell?.columnId },\n        //     row: { type: 'ANY' },\n        //     style: { highlight: '#81948133' },\n        // }),\n        ...optional(hoveredCell && !isResizingRow, {\n            column: { type: 'ANY' },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948133' },\n        }),\n        ...optional(hoveredCell && !isResizing, {\n            column: { id: hoveredCell?.columnId },\n            row: { id: hoveredCell?.rowId },\n            style: { highlight: '#81948188' },\n        }),\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ rows, columns, row, column }) => isSelected(rows, columns, row.index, column.index),\n            style: ({ rows, columns, row, column, edit }) => ({\n                ...(!isSelected(rows, columns, row.index - 1, column.index) ? { borderTop: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index + 1, column.index) ? { borderBottom: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index - 1) ? { borderLeft: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                ...(!isSelected(rows, columns, row.index, column.index + 1) ? { borderRight: { width: selectionBorderWidth, color: '#596959', index: Number.MAX_SAFE_INTEGER } } : {}),\n                highlight: getHighlightColor(edit ? '#798d9c' : '#819481', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            }),\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ row, column }) => highlight.isKeySelected(row.key, column.key),\n            style: ({ row, column }) => ({\n                highlight: getHighlightColor('#93a8b8', focusedColumnKey !== column.key || focusedRowKey !== row.key)\n            })\n        },\n        ...optional(focusedCell, {\n            column: { id: focusedCell?.columnId },\n            row: { id: focusedCell?.rowId },\n            style: { highlight: '#ffffffaa' }\n        }),\n        ...sortBy.map(({ columnId, rowId, direction }, index) => ({\n            column: { id: columnId },\n            row: { id: rowId },\n            style: { highlight: '#0377fc44' }\n        })),\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ edit }) => edit,\n            style: { corner: '#77777720' },\n        },\n        {\n            column: { type: 'ANY' },\n            row: { type: 'ANY' },\n            condition: ({ row, column }) => edition.hasValueByKey(row.key, column.key),\n            style: { corner: 'darkgreen' },\n        },\n        ...optional(resizableColumn, {\n            column: { id: resizableColumn },\n            row: { type: 'HEADER' },\n            style: { borderRight: { width: resizableBorderWidth, color: 'cornflowerblue' } }\n        }),\n        ...optional(resizableRow, {\n            column: { type: 'HEADER' },\n            row: { id: resizableRow },\n            style: { borderBottom: { width: resizableBorderWidth, color: 'cornflowerblue' } }\n        }),\n    ];\n}",
         "export default function getSections(columns, rows) {\n    const topLength = rows.filter(row => row.pinned === 'BEGIN').length; // TODO: optimize\n    const bottomLength = rows.filter(row => row.pinned === 'END').length;\n    const middleLength = rows.length - topLength - bottomLength;\n    const leftLength = columns.filter(column => column.pinned === 'BEGIN').length;\n    const rightLength = columns.filter(column => column.pinned === 'END').length;\n    const centerLength = columns.length - leftLength - rightLength;\n\n    const topRows = rows.slice(0, topLength);\n    const bottomRows = rows.slice(rows.length - bottomLength, rows.length);\n    const middleRows = rows.slice(topLength, rows.length - bottomLength);\n    const leftColumns = columns.slice(0, leftLength);\n    const rightColumns = columns.slice(columns.length - rightLength, columns.length);\n    const centerColumns = columns.slice(leftLength, columns.length - rightLength);\n\n    const hasTopRows = topLength > 0;\n    const hasBottomRows = bottomLength > 0;\n    const hasMiddleRows = middleLength > 0;\n    const hasLeftColumns = leftLength > 0;\n    const hasRightColumns = rightLength > 0;\n    const hasCenterColumns = centerLength > 0;\n\n    const topShowTopBorder = true;\n    const topShowBottomBorder = true;\n    const bottomShowTopBorder = hasMiddleRows || !hasTopRows;\n    const bottomShowBottomBorder = true;\n    const middleShowTopBorder = !hasTopRows;\n    const middleShowBottomBorder = !hasBottomRows;\n    const leftShowLeftBorder = true;\n    const leftShowRightBorder = true;\n    const rightShowLeftBorder = hasCenterColumns || !hasLeftColumns;\n    const rightShowRightBorder = true;\n    const centerShowLeftBorder = !hasLeftColumns;\n    const centerShowRightBorder = !hasRightColumns;\n\n    const getHeight = (rows, showTopBorder, showBottomBorder) => {\n        if (rows.length === 0)\n            return 0;\n\n        const top = showTopBorder ? rows.at(0).topWithBorder : rows.at(0).top;\n        const bottom = showBottomBorder ? rows.at(-1).bottomWithBorder : rows.at(-1).bottom;\n\n        return bottom - top;\n    }\n\n    const getWidth = (columns, showLeftBorder, showRightBorder) => {\n        if (columns.length === 0)\n            return 0;\n\n        const left = showLeftBorder ? columns.at(0).leftWithBorder : columns.at(0).left;\n        const right = showRightBorder ? columns.at(-1).rightWithBorder : columns.at(-1).right;\n\n        return right - left;\n    }\n\n    const topHeight = getHeight(topRows, topShowTopBorder, topShowBottomBorder);\n    const bottomHeight = getHeight(bottomRows, bottomShowTopBorder, bottomShowBottomBorder);\n    const middleHeight = getHeight(middleRows, middleShowTopBorder, middleShowBottomBorder);\n    const leftWidth = getWidth(leftColumns, leftShowLeftBorder, leftShowRightBorder);\n    const rightWidth = getWidth(rightColumns, rightShowLeftBorder, rightShowRightBorder);\n    const centerWidth = getWidth(centerColumns, centerShowLeftBorder, centerShowRightBorder);\n\n    return {\n        top: {\n            rows: topRows,\n            showTopBorder: topShowTopBorder,\n            showBottomBorder: topShowBottomBorder,\n            height: topHeight\n        },\n        bottom: {\n            rows: bottomRows,\n            showTopBorder: bottomShowTopBorder,\n            showBottomBorder: bottomShowBottomBorder,\n            height: bottomHeight\n        },\n        middle: {\n            rows: middleRows,\n            showTopBorder: middleShowTopBorder,\n            showBottomBorder: middleShowBottomBorder,\n            height: middleHeight\n        },\n        left: {\n            columns: leftColumns,\n            showLeftBorder: leftShowLeftBorder,\n            showRightBorder: leftShowRightBorder,\n            width: leftWidth\n        },\n        right: {\n            columns: rightColumns,\n            showLeftBorder: rightShowLeftBorder,\n            showRightBorder: rightShowRightBorder,\n            width: rightWidth\n        },\n        center: {\n            columns: centerColumns,\n            showLeftBorder: centerShowLeftBorder,\n            showRightBorder: centerShowRightBorder,\n            width: centerWidth\n        }\n    };\n}",
         "// TODO: Move\nexport default function getEditedCellsAndFilters(editedCells, filters) {\n    return [...editedCells, ...filters.map(filter => ({ columnId: filter.columnId, rowId: filter.rowId, value: filter.expression }))];\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\n// TODO: write unit tests\nexport default class Edition {\n    constructor(editedCells) {\n        this.lookup = new Map();\n\n        editedCells.forEach(cell => {\n            const rowKey = stringifyId(cell.rowId);\n            const columnKey = stringifyId(cell.columnId);\n\n            if (!this.lookup.has(rowKey))\n                this.lookup.set(rowKey, new Map());\n\n            this.lookup.get(rowKey).set(columnKey, cell.value);\n        });\n    }\n\n    hasValueByKey(rowKey, columnKey) {\n        return this.lookup.has(rowKey) && this.lookup.get(rowKey).has(columnKey);\n    }\n\n    getValueByKey(rowKey, columnKey) {\n        if (!this.hasValueByKey(rowKey, columnKey))\n            return undefined;\n\n        return this.lookup.get(rowKey).get(columnKey);\n    }\n\n    hasValueById(rowId, columnId) {\n        return this.hasValueByKey(stringifyId(rowId), stringifyId(columnId));\n    }\n\n    getValueById(rowId, columnId) {\n        return this.getValueByKey(stringifyId(rowId), stringifyId(columnId));\n    }\n}",
         "import Edition from \"../types/Edition.js\";\n\n// TODO: Move\nexport default function getEdition(editedCellsAndFilters) {\n    return new Edition(editedCellsAndFilters);\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default class Selection {\n    constructor(selectedCells) {\n        this.lookup = new Map();\n\n        selectedCells.forEach(cell => {\n            const rowKey = stringifyId(cell.rowId);\n            const columnKey = stringifyId(cell.columnId);\n\n            if (!this.lookup.has(rowKey))\n                this.lookup.set(rowKey, new Set());\n\n            this.lookup.get(rowKey).add(columnKey);\n        });\n    }\n\n    isKeySelected(rowKey, columnKey) {\n        return this.lookup.has(rowKey) && this.lookup.get(rowKey).has(columnKey);\n    }\n\n    isIdSelected(rowId, columnId) {\n        return this.isKeySelected(stringifyId(rowId), stringifyId(columnId));\n    }\n}",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getSelection(selectedCells) {\n    return new Selection(selectedCells);\n}\n",
         "export default function getInvoked(columnsOrRows, data) {\n    return typeof columnsOrRows === 'function'\n        ? columnsOrRows(data)\n        : columnsOrRows;\n}\n",
         "// TODO: Move\nexport default function getPinned(index, length, pinnedBegin, pinnedEnd) {\n    if (index < pinnedBegin)\n        return \"BEGIN\";\n    if (index >= length - pinnedEnd)\n        return \"END\";\n    return undefined;\n}\n",
-        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getPinned from \"./getPinned.js\";\n\nfunction getResolved(elements, pinnedBegin, pinnedEnd) {\n    return elements.map((element, index) => {\n        const id = 'id' in element ? element.id : element.type;\n        return {\n            ...element,\n            id: id,\n            type: element.type || \"DATA\",\n            index: index,\n            key: stringifyId(id),\n            pinned: getPinned(index, elements.length, pinnedBegin, pinnedEnd),\n            header: 'header' in element ? element.header : id,\n            labels: element.labels || []\n        };\n    });\n}\n\nexport function getResolvedColumns(columns, pinnedBegin, pinnedEnd, columnWidths) {\n    const widthsLookup = new Map(columnWidths.map(({ columnId, width }) => [stringifyId(columnId), width]));\n    const resolvedColumns = getResolved(columns, pinnedBegin, pinnedEnd);\n\n    return resolvedColumns.map(column => ({\n        ...column,\n        width: widthsLookup.has(column.key)\n            ? widthsLookup.get(column.key)\n            : column.width\n    }));\n}\n\nexport function getResolvedRows(rows, pinnedBegin, pinnedEnd, rowHeights) {\n    const heightsLookup = new Map(rowHeights.map(({ rowId, height }) => [stringifyId(rowId), height]));\n    const resolvedRows = getResolved(rows, pinnedBegin, pinnedEnd);\n\n    return resolvedRows.map(row => ({\n        ...row,\n        height: heightsLookup.has(row.key)\n            ? heightsLookup.get(row.key)\n            : row.height\n    }));\n}\n",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getPinned from \"./getPinned.js\";\n\nfunction getResolved(elements, pinnedBegin, pinnedEnd) {\n    return elements.map((element, index) => {\n        const id = 'id' in element ? element.id : element.type;\n        return {\n            ...element,\n            id: id,\n            type: element.type || \"DATA\",\n            index: index,\n            key: stringifyId(id),\n            pinned: getPinned(index, elements.length, pinnedBegin, pinnedEnd),\n            header: 'header' in element ? element.header : id,\n            labels: element.labels || []\n        };\n    });\n}\n\nexport function getResolvedColumns(columns, pinnedBegin, pinnedEnd, columnWidths) {\n    const widthsLookup = new Map(columnWidths.map(({ columnId, width }) => [stringifyId(columnId), width]));\n    const resolvedColumns = getResolved(columns, pinnedBegin, pinnedEnd);\n\n    return resolvedColumns.map(column => ({\n        ...column,\n        width: widthsLookup.has(column.key)\n            ? widthsLookup.get(column.key)\n            : 'width' in column\n                ? column.width\n                : 'fit'\n    }));\n}\n\nexport function getResolvedRows(rows, pinnedBegin, pinnedEnd, rowHeights) {\n    const heightsLookup = new Map(rowHeights.map(({ rowId, height }) => [stringifyId(rowId), height]));\n    const resolvedRows = getResolved(rows, pinnedBegin, pinnedEnd);\n\n    return resolvedRows.map(row => ({\n        ...row,\n        height: heightsLookup.has(row.key)\n            ? heightsLookup.get(row.key)\n            : 'height' in row\n                ? row.height\n                : 'fit'\n    }));\n}\n",
         "import roundToPixels from \"../core-utils/roundToPixels.js\";\n\nexport function getPlacedColumns(columns, devicePixelRatio, borderWidth) {\n    let left = borderWidth;\n\n    return columns.map((column, index) => {\n        const assignedWidth = 'width' in column ? column.width : 100;\n        const width = roundToPixels(assignedWidth, devicePixelRatio);\n        const newColumn = {\n            ...column,\n            index: index,\n            width: width,\n            leftWithBorder: left - borderWidth,\n            left: left,\n            right: left + width,\n            rightWithBorder: left + width + borderWidth\n        };\n\n        left += newColumn.width + borderWidth;\n\n        return newColumn;\n    });\n}\n\nexport function getPlacedRows(rows, devicePixelRatio, borderWidth) {\n    let top = borderWidth;\n\n    return rows.map((row, index) => {\n        const assignedHeight = 'height' in row ? row.height : 20;\n        const height = roundToPixels(assignedHeight, devicePixelRatio);\n        const newRow = {\n            ...row,\n            index: index,\n            height: height,\n            topWithBorder: top - borderWidth,\n            top: top,\n            bottom: top + height,\n            bottomWithBorder: top + height + borderWidth\n        };\n\n        top += newRow.height + borderWidth;\n\n        return newRow;\n    });\n}\n",
-        "import stringifyId from \"../core-utils/stringifyId.js\";\n\nconst matchMapping = {\n    'HEADER': ['HEADER'],\n    'FILTER': ['FILTER'],\n    'DATA': ['DATA'],\n    'CUSTOM': ['CUSTOM'],\n    'ANY': ['HEADER', 'DATA', 'FILTER', 'CUSTOM'],\n    'SPECIAL': ['HEADER', 'FILTER', 'CUSTOM'],\n    undefined: []\n};\n\nclass Lookup {\n    byKey = new Map();\n    byIndex = new Map(); // TODO: Should this be removed?\n    byLabel = new Map();\n    byMatch = new Map();\n}\n\nexport default class RulesLookup {\n    lookup = new Lookup();\n    hasRules = false;\n\n    addRule(column, row, rule) {\n        this.hasRules = true;\n\n        if (Array.isArray(column)) {\n            for (const c of column)\n                this.addRule(c, row, rule);\n            return;\n        }\n\n        if (Array.isArray(row)) {\n            for (const r of row)\n                this.addRule(column, r, rule);\n            return;\n        }\n\n        column = column\n            ? 'id' in column\n                ? { key: stringifyId(column.id) }\n                : column\n            : { match: 'DATA' };\n        row = row\n            ? 'id' in row\n                ? { key: stringifyId(row.id) }\n                : row\n            : { match: 'DATA' };\n\n        function addRowRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, []);\n\n            lookup.get(key).push(rule);\n        }\n\n        function addColumnRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, new Lookup());\n\n            if ('key' in row)\n                addRowRule(lookup.get(key).byKey, row.key);\n            if ('index' in row)\n                addRowRule(lookup.get(key).byIndex, row.index);\n            if ('label' in row)\n                addRowRule(lookup.get(key).byLabel, row.label);\n            for (const match of matchMapping[row.match])\n                addRowRule(lookup.get(key).byMatch, match);\n        }\n\n        if ('key' in column)\n            addColumnRule(this.lookup.byKey, column.key);\n        if ('index' in column)\n            addColumnRule(this.lookup.byIndex, column.index);\n        if ('label' in column)\n            addColumnRule(this.lookup.byLabel, column.label);\n        for (const match of matchMapping[column.match])\n            addColumnRule(this.lookup.byMatch, match);\n    }\n\n    getRules(column, row) {\n        const rules = [];\n\n        if (!this.hasRules)\n            return rules;\n\n        function gatherRules(newRules) {\n            for (const rule of newRules)\n                rules.push(rule);\n        }\n\n        function gatherRowRules(lookup) {\n            if (lookup.byKey.has(row.key))\n                gatherRules(lookup.byKey.get(row.key));\n            if (lookup.byIndex.has(row.index))\n                gatherRules(lookup.byIndex.get(row.index));\n            if (lookup.byMatch.has(row.type))\n                gatherRules(lookup.byMatch.get(row.type));\n            for (const label of row.labels) {\n                if (lookup.byLabel.has(label))\n                    gatherRules(lookup.byLabel.get(label));\n            }\n        }\n\n        if (this.lookup.byKey.has(column.key))\n            gatherRowRules(this.lookup.byKey.get(column.key));\n        if (this.lookup.byIndex.has(column.index))\n            gatherRowRules(this.lookup.byIndex.get(column.index));\n        if (this.lookup.byMatch.has(column.type))\n            gatherRowRules(this.lookup.byMatch.get(column.type));\n        for (const label of column.labels) {\n            if (this.lookup.byLabel.has(label))\n                gatherRowRules(this.lookup.byLabel.get(label));\n        }\n\n        return rules;\n    }\n};",
-        "import { defaultPadding } from \"../core-utils/defaults.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst borderTypes = ['borderTop', 'borderRight', 'borderBottom', 'borderLeft'];\n// TODO: better handle default validate for toggle edit\nconst defaultEdit = { validate: () => true, parse: string => string };\n\n// TODO: Don't recreate styles if they haven't changed\nfunction indexBorders(style, index) {\n    const newStyle = { ...style };\n\n    if ('border' in newStyle) {\n        for (const borderType of borderTypes)\n            newStyle[borderType] = newStyle.border;\n        delete newStyle.border;\n    }\n\n    for (const borderType of borderTypes)\n        if (borderType in newStyle)\n            newStyle[borderType] = { ...newStyle[borderType], index };\n\n    return newStyle;\n}\n\nfunction getText(context) {\n    if ('text' in context)\n        return context.text;\n    if (context.value !== undefined)\n        return `${context.value}`;\n    return '';\n}\n\n// TODO: Rename to FormatResolver\n// TODO: Optimize by not searching using keys that don't have correlated match rules\n// TODO: Accept both a function and an object as a style (where the object is a resolved style)\n// TODO: Consider removing index from the lookup\nexport default class FormattingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const [index, rule] of rules.entries()) {\n            const entry = { index };\n\n            if ('condition' in rule)\n                entry.condition = rule.condition;\n            if ('style' in rule)\n                entry.style = typeof rule.style === 'function' ? rule.style : () => rule.style;\n            if ('value' in rule)\n                entry.value = typeof rule.value === 'function' ? rule.value : () => rule.value;\n            if ('text' in rule)\n                entry.text = typeof rule.text === 'function' ? rule.text : () => rule.text;\n            if ('padding' in rule)\n                entry.padding = typeof rule.padding === 'function' ? rule.padding : () => rule.padding;\n            if ('edit' in rule)\n                entry.edit = rule.edit;\n            if ('draw' in rule)\n                entry.draw = rule.draw;\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, edition) {\n        const rules = this.rulesLookup\n            .getRules(column, row)\n            .sort((a, b) => a.index - b.index)\n            .filter((value, index, array) => value.index !== array[index - 1]?.index);\n\n        let context = { data, rows, columns, row, column };\n        let style = {};\n        let draw = undefined;\n        let visible = true;\n        let padding = defaultPadding;\n\n        if (edition.hasValueByKey(row.key, column.key))\n            context = { ...context, newValue: edition.getValueByKey(row.key, column.key) };\n\n        for (const rule of rules) {\n            if ('condition' in rule && !rule.condition(context))\n                continue;\n\n            // TODO: Don't actually add things like `edit` to the context\n            if ('value' in rule)\n                context = { ...context, value: rule.value(context) };\n            if ('style' in rule)\n                style = { ...style, ...indexBorders(rule.style(context), rule.index) };\n            if ('text' in rule)\n                context = { ...context, text: rule.text(context) };\n            if ('padding' in rule)\n                padding = { ...padding, ...rule.padding(context) };\n            if ('edit' in rule)\n                context = { ...context, edit: rule.edit && 'edit' in context ? { ...context.edit, ...rule.edit } : { ...defaultEdit, ...rule.edit } };\n            if ('draw' in rule) {\n                const currentContext = context;\n                draw = (ctx) => rule.draw({ ...currentContext, ctx });\n            }\n\n            // TODO: Add StopPropagation\n        }\n\n        const text = getText(context);\n        const result = {\n            style,\n            visible,\n            text,\n            padding\n        };\n\n        if ('value' in context)\n            result.value = context.value;\n        if ('edit' in context)\n            result.edit = context.edit;\n        if (draw !== undefined)\n            result.draw = draw;\n        if ('text' in context)\n            result.text = context.text;\n\n        return result;\n    }\n}",
+        "const defaultFont = '12px Calibri';\nconst defaultPadding = { top: 2, right: 5, bottom: 2, left: 5 };\n\nexport { defaultFont, defaultPadding };",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\n\nconst typeMapping = {\n    'HEADER': ['HEADER'],\n    'FILTER': ['FILTER'],\n    'DATA': ['DATA'],\n    'CUSTOM': ['CUSTOM'],\n    'ANY': ['HEADER', 'DATA', 'FILTER', 'CUSTOM'],\n    'SPECIAL': ['HEADER', 'FILTER', 'CUSTOM'],\n    undefined: []\n};\n\nclass Lookup {\n    byKey = new Map();\n    byIndex = new Map(); // TODO: Should this be removed?\n    byLabel = new Map();\n    byType = new Map();\n}\n\nexport default class RulesLookup {\n    lookup = new Lookup();\n    hasRules = false;\n\n    addRule(column, row, rule) {\n        this.hasRules = true;\n\n        if (Array.isArray(column)) {\n            for (const c of column)\n                this.addRule(c, row, rule);\n            return;\n        }\n\n        if (Array.isArray(row)) {\n            for (const r of row)\n                this.addRule(column, r, rule);\n            return;\n        }\n\n        column = column\n            ? 'id' in column\n                ? { key: stringifyId(column.id) }\n                : column\n            : { type: 'DATA' };\n        row = row\n            ? 'id' in row\n                ? { key: stringifyId(row.id) }\n                : row\n            : { type: 'DATA' };\n\n        function addRowRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, []);\n\n            lookup.get(key).push(rule);\n        }\n\n        function addColumnRule(lookup, key) {\n            if (!lookup.has(key))\n                lookup.set(key, new Lookup());\n\n            if ('key' in row)\n                addRowRule(lookup.get(key).byKey, row.key);\n            if ('index' in row)\n                addRowRule(lookup.get(key).byIndex, row.index);\n            if ('label' in row)\n                addRowRule(lookup.get(key).byLabel, row.label);\n            for (const type of typeMapping[row.type])\n                addRowRule(lookup.get(key).byType, type);\n        }\n\n        if ('key' in column)\n            addColumnRule(this.lookup.byKey, column.key);\n        if ('index' in column)\n            addColumnRule(this.lookup.byIndex, column.index);\n        if ('label' in column)\n            addColumnRule(this.lookup.byLabel, column.label);\n        for (const type of typeMapping[column.type])\n            addColumnRule(this.lookup.byType, type);\n    }\n\n    getRules(column, row) {\n        const rules = [];\n\n        if (!this.hasRules)\n            return rules;\n\n        function gatherRules(newRules) {\n            for (const rule of newRules)\n                rules.push(rule);\n        }\n\n        function gatherRowRules(lookup) {\n            if (lookup.byKey.has(row.key))\n                gatherRules(lookup.byKey.get(row.key));\n            if (lookup.byIndex.has(row.index))\n                gatherRules(lookup.byIndex.get(row.index));\n            if (lookup.byType.has(row.type))\n                gatherRules(lookup.byType.get(row.type));\n            for (const label of row.labels) {\n                if (lookup.byLabel.has(label))\n                    gatherRules(lookup.byLabel.get(label));\n            }\n        }\n\n        if (this.lookup.byKey.has(column.key))\n            gatherRowRules(this.lookup.byKey.get(column.key));\n        if (this.lookup.byIndex.has(column.index))\n            gatherRowRules(this.lookup.byIndex.get(column.index));\n        if (this.lookup.byType.has(column.type))\n            gatherRowRules(this.lookup.byType.get(column.type));\n        for (const label of column.labels) {\n            if (this.lookup.byLabel.has(label))\n                gatherRowRules(this.lookup.byLabel.get(label));\n        }\n\n        return rules;\n    }\n};",
+        "import { defaultFont, defaultPadding } from \"../core-utils/defaults.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst borderTypes = ['borderTop', 'borderRight', 'borderBottom', 'borderLeft'];\n// TODO: better handle default validate for toggle edit\nconst defaultEdit = { validate: () => true, parse: ({ string }) => string };\n\n// TODO: Don't recreate styles if they haven't changed\nfunction indexBorders(style, index) {\n    const newStyle = { ...style };\n\n    if ('border' in newStyle) {\n        for (const borderType of borderTypes)\n            newStyle[borderType] = newStyle.border;\n        delete newStyle.border;\n    }\n\n    for (const borderType of borderTypes)\n        if (borderType in newStyle)\n            newStyle[borderType] = { ...newStyle[borderType], index };\n\n    return newStyle;\n}\n\nfunction getText(context) {\n    if ('text' in context)\n        return `${context.text}`;\n    if ('newValue' in context)\n        return `${context.newValue}`;\n    if (context.value !== undefined)\n        return `${context.value}`;\n    return '';\n}\n\nfunction getEdit(rule, context) {\n    if (rule.edit === false)\n        return undefined;\n    if (rule.edit === true)\n        return 'edit' in context ? context.edit : defaultEdit;\n    if ('edit' in context)\n        return { ...context.edit, ...rule.edit };\n    return { ...defaultEdit, ...rule.edit };\n}\n\n// TODO: Rename to FormatResolver\n// TODO: Optimize by not searching using keys that don't have correlated type rules\n// TODO: Accept both a function and an object as a style (where the object is a resolved style)\n// TODO: Consider removing index from the lookup\nexport default class FormattingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const [index, rule] of rules.entries()) {\n            const entry = { index };\n\n            if ('condition' in rule)\n                entry.condition = rule.condition;\n            if ('style' in rule)\n                entry.style = typeof rule.style === 'function' ? rule.style : () => rule.style;\n            if ('value' in rule)\n                entry.value = typeof rule.value === 'function' ? rule.value : () => rule.value;\n            if ('text' in rule)\n                entry.text = typeof rule.text === 'function' ? rule.text : () => rule.text;\n            if ('font' in rule)\n                entry.font = typeof rule.font === 'function' ? rule.font : () => rule.font;\n            if ('padding' in rule)\n                entry.padding = typeof rule.padding === 'function' ? rule.padding : () => rule.padding;\n            if ('edit' in rule)\n                entry.edit = rule.edit;\n            if ('draw' in rule)\n                entry.draw = rule.draw;\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, edition) {\n        const rules = this.rulesLookup\n            .getRules(column, row)\n            .sort((a, b) => a.index - b.index)\n            .filter((value, index, array) => value.index !== array[index - 1]?.index);\n\n        let context = { data, rows, columns, row, column };\n        let style = {};\n        let draw = undefined;\n        let visible = true;\n        let padding = defaultPadding;\n        let font = defaultFont;\n\n        if (edition.hasValueByKey(row.key, column.key))\n            context = { ...context, newValue: edition.getValueByKey(row.key, column.key) };\n\n        for (const rule of rules) {\n            if ('condition' in rule && !rule.condition(context))\n                continue;\n\n            // TODO: Don't actually add things like `edit` to the context\n            if ('value' in rule)\n                context = { ...context, value: rule.value(context) };\n            if ('style' in rule)\n                style = { ...style, ...indexBorders(rule.style(context), rule.index) };\n            if ('text' in rule)\n                context = { ...context, text: rule.text(context) };\n            if ('font' in rule)\n                font = rule.font(context);\n            if ('padding' in rule)\n                padding = { ...padding, ...rule.padding(context) };\n            if ('edit' in rule)\n                context = { ...context, edit: getEdit(rule, context) };\n            if ('draw' in rule) {\n                const currentContext = context;\n                draw = (ctx) => rule.draw({ ...currentContext, ctx });\n            }\n\n            // TODO: Add StopPropagation\n        }\n\n        const text = getText(context);\n        const result = {\n            style,\n            visible,\n            text,\n            padding,\n            font\n        };\n\n        if ('value' in context)\n            result.value = context.value;\n        if ('edit' in context && context.edit !== undefined)\n            result.edit = context.edit;\n        if (draw !== undefined)\n            result.draw = draw;\n\n        return result;\n    }\n}",
         "import FormattingRules from \"../types/FormattingRules.js\";\n\nexport default function getFormattingRules(dataFormatting) {\n    return new FormattingRules(dataFormatting);\n}\n",
         "export default class FormatResolver {\n    constructor(formattingRules, data, rows, columns, edition) {\n        this.formattingRules = formattingRules;\n        this.data = data;\n        this.rows = rows;\n        this.columns = columns;\n        this.edition = edition;\n    }\n\n    resolve(row, column) {\n        return this.formattingRules.resolve(\n            this.data,\n            this.rows,\n            this.columns,\n            row,\n            column,\n            this.edition);\n    }\n}",
         "import FormatResolver from \"../types/FormatResolver.js\";\n\nexport default function getFormatResolver(formattingRules, data, rows, columns, edition) {\n    return new FormatResolver(formattingRules, data, rows, columns, edition);\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction getFilterLookup(filters, primaryKey, secondaryKey) {\n    const filterLookup = new Map();\n    for (const cell of filters) {\n        const primary = stringifyId(cell[primaryKey]);\n        const secondary = stringifyId(cell[secondaryKey]);\n\n        if (!filterLookup.has(primary))\n            filterLookup.set(primary, new Map());\n\n        filterLookup.get(primary).set(secondary, cell.expression);\n    }\n    return filterLookup;\n}\n\nexport function getFilteredRows(filters, filteringRules, formattingRules, data, rows, columns, edition) {\n    if (filters.length === 0)\n        return rows;\n\n    const filterLookup = getFilterLookup(filters, 'columnId', 'rowId');\n    const filteredColumns = columns.filter(column => column.type !== 'FILTER' && filterLookup.has(column.key));\n\n    if (filteredColumns.length === 0)\n        return rows;\n\n    return rows.filter(row => {\n        for (const column of filteredColumns) {\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const columnFilters = filterLookup.get(column.key);\n            const visible = filteringRules.resolve(data, rows, columns, row, column, cell.value, cell.text, columnFilters);\n\n            if (!visible)\n                return false;\n        }\n        return true;\n    });\n}\n\nexport function getFilteredColumns(filters, filteringRules, formattingRules, data, rows, columns, edition) {\n    if (filters.length === 0)\n        return columns;\n\n    const filterLookup = getFilterLookup(filters, 'rowId', 'columnId');\n    const filteredRows = rows.filter(row => row.type !== 'FILTER' && filterLookup.has(row.key));\n\n    if (filteredRows.length === 0)\n        return columns;\n\n    return columns.filter(column => {\n        for (const row of filteredRows) {\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const rowFilters = filterLookup.get(row.key);\n            const visible = filteringRules.resolve(data, rows, columns, row, column, cell.value, cell.text, rowFilters);\n\n            if (!visible)\n                return false;\n        }\n        return true;\n    });\n}",
         "export default function getFixedSize(top, bottom, left, right) {\n    return {\n        top: top,\n        bottom: bottom,\n        left: left,\n        right: right\n    };\n}\n",
         "export default function getTotalSize(columns, rows) {\n    return {\n        width: columns.length ? columns.at(-1).rightWithBorder : 0,\n        height: rows.length ? rows.at(-1).bottomWithBorder : 0\n    };\n}\n",
-        "import { defaultFont } from \"../core-utils/defaults.js\";\n\nexport default class TextResolver\n{\n    constructor() {\n        this.canvas = document.createElement('canvas');\n        this.context = this.canvas.getContext('2d');\n        this.fontMetrics = new Map();\n    }\n\n    measureWidth(text, font) {\n        const ctx = this.context;\n\n        ctx.font = font || defaultFont;\n\n        const textMetrics = ctx.measureText(text);\n\n        return textMetrics.width;\n    }\n\n    measureHeight(text, font) {\n        let lines = 1;\n        for (const char of text) {\n            if (char === '\\n')\n                lines++;\n        }\n\n        return lines * this.getFontMetrics(font).height;\n    }\n\n    getFontMetrics(font) {\n        const key = font;\n\n        if (this.fontMetrics.has(key))\n            return this.fontMetrics.get(key);\n\n        const ctx = this.context;\n\n        // TODO: Set other font properties\n        ctx.font = font || defaultFont;\n\n        const textMetrics = ctx.measureText('X');\n\n        const middle = (textMetrics.actualBoundingBoxDescent - textMetrics.actualBoundingBoxAscent) / 2;\n        const topOffset = middle + textMetrics.fontBoundingBoxAscent;\n        const bottomOffset = textMetrics.fontBoundingBoxDescent - middle;\n        const height = textMetrics.fontBoundingBoxAscent + textMetrics.fontBoundingBoxDescent;\n\n        const fontMetrics = {\n            topOffset: topOffset,\n            middle: -middle,\n            bottomOffset: bottomOffset,\n            height: height\n        };\n\n        this.fontMetrics.set(key, fontMetrics);\n\n        return fontMetrics;\n    }\n}",
+        "import { defaultFont } from \"../core-utils/defaults.js\";\n\nexport default class TextResolver {\n    constructor() {\n        this.canvas = document.createElement('canvas');\n        this.context = this.canvas.getContext('2d');\n        this.fontMetrics = new Map();\n    }\n\n    measureWidth(text, font) {\n        if (!text)\n            return 0;\n\n        const ctx = this.context;\n        ctx.font = font || defaultFont;\n        const textMetrics = ctx.measureText(text);\n\n        return textMetrics.width;\n    }\n\n    measureHeight(text, font) {\n        let lines = 1;\n        for (const char of text) {\n            if (char === '\\n')\n                lines++;\n        }\n\n        return lines * this.getFontMetrics(font).height;\n    }\n\n    getFontMetrics(font) {\n        const key = font;\n\n        if (this.fontMetrics.has(key))\n            return this.fontMetrics.get(key);\n\n        const ctx = this.context;\n\n        // TODO: Set other font properties\n        ctx.font = font || defaultFont;\n\n        const textMetrics = ctx.measureText('X');\n\n        const middle = (textMetrics.actualBoundingBoxDescent - textMetrics.actualBoundingBoxAscent) / 2;\n        const topOffset = middle + textMetrics.fontBoundingBoxAscent;\n        const bottomOffset = textMetrics.fontBoundingBoxDescent - middle;\n        const height = textMetrics.fontBoundingBoxAscent + textMetrics.fontBoundingBoxDescent;\n\n        const fontMetrics = {\n            topOffset: topOffset,\n            middle: -middle,\n            bottomOffset: bottomOffset,\n            height: height\n        };\n\n        this.fontMetrics.set(key, fontMetrics);\n\n        return fontMetrics;\n    }\n}",
         "import TextResolver from \"../types/TextResolver.js\";\n\nexport default function getTextResolver() {\n    return new TextResolver();\n}\n",
         "export function contains(bounds, rect) {\n    return (\n        rect.top >= bounds.top &&\n        rect.left >= bounds.left &&\n        rect.top + rect.height <= bounds.top + bounds.height &&\n        rect.left + rect.width <= bounds.left + bounds.width\n    );\n}\n\nexport function clip(bounds, rect) {\n    const newRect = {\n        top: Math.max(bounds.top, rect.top),\n        left: Math.max(bounds.left, rect.left),\n        width: Math.min(bounds.left + bounds.width, rect.left + rect.width) - Math.max(bounds.left, rect.left),\n        height: Math.min(bounds.top + bounds.height, rect.top + rect.height) - Math.max(bounds.top, rect.top)\n    };\n\n    if (newRect.width >= 0 && newRect.height >= 0)\n        return newRect;\n\n    return {\n        top: bounds.top,\n        left: bounds.left,\n        width: 0,\n        height: 0\n    }\n}\n\nexport function expand(rect, margin) {\n    return {\n        top: rect.top - margin,\n        left: rect.left - margin,\n        width: rect.width + margin * 2,\n        height: rect.height + margin * 2\n    };\n}\n\nexport function area(rect) {\n    return rect.width * rect.height;\n}\n\nexport function subtract(rect, margin) {\n    return {\n        top: rect.top,\n        left: rect.left,\n        width: Math.max(0, rect.width - margin.left - margin.right),\n        height: Math.max(0, rect.height - margin.top - margin.bottom)\n    };\n}",
         "import { area, clip, contains, expand, subtract } from \"../core-utils/rect.js\";\n\nconst requiredMargin = 200;\nconst preloadedMargin = 400;\nconst emptyRect = {\n    left: 0,\n    top: 0,\n    width: 0,\n    height: 0\n};\n\nexport default function getScrollRect(previous, totalSize, fixedSize, element) {\n    // TODO: Is it optimal to use getBoundingClientRect()?\n    const size = {\n        width: element.getBoundingClientRect().width,\n        height: element.getBoundingClientRect().height\n    };\n    const scrollOffset = {\n        left: element.scrollLeft,\n        top: element.scrollTop\n    };\n\n    const prevScrollRect = previous || emptyRect;\n\n    const totalRect = { left: 0, top: 0, ...totalSize };\n    const bounds = subtract(totalRect, fixedSize);\n    const scrollRect = subtract({ ...scrollOffset, ...size }, fixedSize);\n    const requiredScrollRect = clip(bounds, expand(scrollRect, requiredMargin));\n    const preloadedScrollRect = clip(bounds, expand(scrollRect, preloadedMargin));\n\n    if (!contains(bounds, prevScrollRect))\n        return preloadedScrollRect;\n\n    if (!contains(prevScrollRect, requiredScrollRect))\n        return preloadedScrollRect;\n\n    if (area(prevScrollRect) > 2 * area(preloadedScrollRect))\n        return preloadedScrollRect;\n\n    return prevScrollRect;\n}\n",
+        "export default function getInternalPosition(element, position, fixedSize, totalSize) {\n  // TODO: sometimes mousePosition is outside of bounds and it crashes the click events\n  const x = position.x;\n  const y = position.y;\n\n  const scrollOffset = {\n    left: element.scrollLeft,\n    top: element.scrollTop\n  };\n\n  const clientSize = {\n    width: element.clientWidth,\n    height: element.clientHeight\n  };\n\n  return {\n    x: x <= fixedSize.left\n      ? x\n      : x >= clientSize.width // TODO: This will not work for resizing columns pinned to the right\n        ? x + scrollOffset.left\n        : x >= clientSize.width - fixedSize.right\n          ? totalSize.width - clientSize.width + x\n          : x + scrollOffset.left,\n    y: y <= fixedSize.top\n      ? y\n      : y >= clientSize.height // TODO: This will not work for resizing rows pinned to the bottom\n        ? y + scrollOffset.top\n        : y >= clientSize.height - fixedSize.bottom\n          ? totalSize.height - clientSize.height + y\n          : y + scrollOffset.top\n  };\n}",
         "export default function getLookup(elements) {\n    return elements.reduce((lookup, element) => lookup.set(element.key, element), new Map());\n}\n",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nexport default function getHighlightedCells(isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup) {\n    if (!isMouseDown)\n        return [];\n    if (isResizing)\n        return [];\n    if (!hoveredCell)\n        return [];\n    if (!focusedCell)\n        return [];\n\n    const focusedColumnKey = stringifyId(focusedCell.columnId);\n    const focusedRowKey = stringifyId(focusedCell.rowId);\n    const hoveredColumnKey = stringifyId(hoveredCell.columnId);\n    const hoveredRowKey = stringifyId(hoveredCell.rowId);\n\n    if (!columnLookup.has(focusedColumnKey))\n        return [];\n    if (!rowLookup.has(focusedRowKey))\n        return [];\n    if (!columnLookup.has(hoveredColumnKey))\n        return [];\n    if (!rowLookup.has(hoveredRowKey))\n        return [];\n\n    const minColumnIndex = Math.min(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const maxColumnIndex = Math.max(columnLookup.get(focusedColumnKey).index, columnLookup.get(hoveredColumnKey).index);\n    const minRowIndex = Math.min(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n    const maxRowIndex = Math.max(rowLookup.get(focusedRowKey).index, rowLookup.get(hoveredRowKey).index);\n\n    return columns.slice(minColumnIndex, maxColumnIndex + 1).flatMap(column => {\n        return rows.slice(minRowIndex, maxRowIndex + 1).map(row => {\n            return {\n                rowId: row.id,\n                columnId: column.id\n            };\n        });\n    });\n}\n",
         "function getVerticalSection(row) {\n    if (row.pinned === \"BEGIN\")\n        return \"top\";\n    if (row.pinned === \"END\")\n        return \"bottom\";\n    return \"middle\";\n}\n\nfunction getHorizontalSection(column) {\n    if (column.pinned === \"BEGIN\")\n        return \"left\";\n    if (column.pinned === \"END\")\n        return \"right\";\n    return \"center\";\n}\n\nexport default function getCellSection(column, row) {\n    const verticalSection = getVerticalSection(row);\n    const horizontalSection = getHorizontalSection(column);\n\n    return `${verticalSection}-${horizontalSection}`;\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getCellSection from \"./getCellSection.js\";\n\nexport default function getInputPlacement(editableCells, focusedCell, columnLookup, rowLookup, sections) {\n    if (!focusedCell)\n        return null;\n\n    const focusedColumnKey = stringifyId(focusedCell.columnId);\n    const focusedRowKey = stringifyId(focusedCell.rowId);\n\n    if (!columnLookup.has(focusedColumnKey))\n        return null;\n    if (!rowLookup.has(focusedRowKey))\n        return null;\n\n    const column = columnLookup.get(focusedColumnKey);\n    const row = rowLookup.get(focusedRowKey);\n\n    if (editableCells.length === 0)\n        return null;\n\n    const position = {\n        width: column.width,\n        height: row.height,\n        section: getCellSection(column, row)\n    };\n\n    switch (row.pinned) {\n        case \"BEGIN\":\n            position.top = row.top;\n            break;\n        case \"END\":\n            position.bottom = sections.top.height + sections.middle.height + sections.bottom.height - row.top - row.height;\n            break;\n        default:\n            position.marginTop = row.top - sections.top.height;\n    }\n\n    switch (column.pinned) {\n        case \"BEGIN\":\n            position.left = column.left;\n            break;\n        case \"END\":\n            position.right = sections.left.width + sections.center.width + sections.right.width - column.left - column.width;\n            break;\n        default:\n            position.marginLeft = column.left - sections.left.width;\n    }\n\n    return position;\n}\n",
         "export default function getIsTextValid(text, editableCells) {\n    return editableCells.every(cell => cell.edit.validate({ string: text }));\n}\n",
         "function getDefaultIds(elements) {\n    if (!Array.isArray(elements))\n        return Object.keys(elements);\n\n    return elements.map((_, index) => index);\n}\n\nfunction getDefaultRowIds(data) {\n    return getDefaultIds(data);\n}\n\nfunction getDefaultColumnIds(data) {\n    const keys = new Set();\n\n    if (Array.isArray(data)) {\n        for (const element of data) {\n            for (const id of getDefaultIds(element))\n                keys.add(id);\n        }\n    } else {\n        for (const key in data) {\n            for (const id of getDefaultIds(data[key]))\n                keys.add(id);\n        }\n    }\n\n    return [...keys];\n}\n\nexport function getUnfoldedColumns(columns, data) {\n    const hasDataBlocks = columns.some(column => column.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return columns;\n\n    const unfoldedColumns = [];\n\n    for (const column of columns) {\n        if (column.type === 'DATA-BLOCK') {\n            const ids = 'selector' in column\n                ? column.selector(data)\n                : getDefaultColumnIds(data);\n\n            for (const id of ids) {\n                unfoldedColumns.push({\n                    ...column,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedColumns.push(column);\n        }\n    }\n\n    return unfoldedColumns;\n}\n\nexport function getUnfoldedRows(rows, data) {\n    const hasDataBlocks = rows.some(row => row.type === 'DATA-BLOCK');\n\n    if (!hasDataBlocks)\n        return rows;\n\n    const unfoldedRows = [];\n\n    for (const row of rows) {\n        if (row.type === 'DATA-BLOCK') {\n            const ids = 'selector' in row\n                ? row.selector(data)\n                : getDefaultRowIds(data);\n\n            for (const id of ids) {\n                unfoldedRows.push({\n                    ...row,\n                    id,\n                    type: 'DATA'\n                });\n            }\n        } else {\n            unfoldedRows.push(row);\n        }\n    }\n\n    return unfoldedRows;\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport RulesLookup from \"./RulesLookup.js\";\n\nconst defaultCondition = ({ text, expression }) => text.includes(expression);\n\nexport default class FilteringRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'FILTER'),\n                condition: rule.condition || defaultCondition\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(data, rows, columns, row, column, value, text, filterLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return true;\n            if (column.type !== 'DATA')\n                return true;\n            if (!filterLookup.has('\"FILTER\"'))\n                return true;\n\n            return defaultCondition({ text, expression: filterLookup.get('\"FILTER\"') });\n        }\n\n        let context = { data, rows, columns, row, column, value, text };\n\n        for (const rule of rules) {\n            if (!filterLookup.has(rule.by))\n                continue;\n\n            const filterContext = { ...context, expression: filterLookup.get(rule.by) };\n\n            if (!rule.condition(filterContext))\n                return false;\n        }\n\n        return true;\n    }\n}",
         "import FilteringRules from \"../types/FilteringRules.js\";\n\nexport default function getFilteringRules(filtering) {\n    return new FilteringRules(filtering);\n}",
-        "export default function getFilterFormatting(formatting) {\n    return formatting;\n}",
-        "export default function getMeasureFormatting(formatting) {\n    return formatting;\n}",
-        "import { defaultPadding } from \"../core-utils/defaults.js\";\n\n// TODO: add expand and expand-data\n\nexport function getMeasuredColumns(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (columns.every(column => typeof column.width === 'number'))\n        return columns;\n\n    const measureColumn = column => {\n        const requestedWidth = 'width' in column ? column.width : 'fit-once';\n\n        if (typeof requestedWidth === 'number')\n            return requestedWidth;\n\n        if (measuringCache.has(column.key)) {\n            const cached = measuringCache.get(column.key);\n\n            if (requestedWidth === 'fit-once' && !cached.dataOnly)\n                return cached.width;\n            if (requestedWidth === 'fit-data-once' && cached.dataOnly)\n                return cached.width;\n        }\n\n        let width = 0;\n        for (const row of rows) {\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data-once')\n                continue;\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.left + cell.padding.right;\n\n            const cellWidth = textResolver.measureWidth(text, font) + padding;\n\n            width = Math.max(width, cellWidth);\n        }\n\n        measuringCache.set(column.key, {\n            width,\n            dataOnly: requestedWidth === 'fit-data-once'\n        });\n\n        return width;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return columns.map(column => ({\n        ...column,\n        width: measureColumn(column)\n    }));\n}\n\nexport function getMeasuredRows(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (rows.every(row => typeof row.height === 'number'))\n        return rows;\n\n    const measureRow = row => {\n        const requestedHeight = 'height' in row ? row.height : 'fit-once';\n\n        if (typeof requestedHeight === 'number')\n            return requestedHeight;\n\n        if (measuringCache.has(row.key)) {\n            const cached = measuringCache.get(row.key);\n\n            if (requestedHeight === 'fit-once' && !cached.dataOnly)\n                return cached.height;\n            if (requestedHeight === 'fit-data-once' && cached.dataOnly)\n                return cached.height;\n        }\n\n        let height = 0;\n        for (const column of columns) {\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data-once')\n                continue;\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.top + cell.padding.bottom;\n\n            const cellHeight = textResolver.measureHeight(text, font) + padding;\n\n            height = Math.max(height, cellHeight);\n        }\n\n        measuringCache.set(row.key, {\n            height,\n            dataOnly: requestedHeight === 'fit-data-once'\n        });\n\n        return height;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return rows.map(row => ({\n        ...row,\n        height: measureRow(row)\n    }));\n}",
+        "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getFilterFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text']);\n}",
+        "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getMeasureFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text', 'font', 'padding']);\n}",
+        "import { defaultPadding } from \"../core-utils/defaults.js\";\n\n// TODO: add expand and expand-data\n\nexport function getMeasuredColumns(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (columns.every(column => typeof column.width === 'number'))\n        return columns;\n\n    const measureColumn = column => {\n        const requestedWidth = column.width;\n\n        if (typeof requestedWidth === 'number')\n            return requestedWidth;\n\n        if (measuringCache.has(column.key)) {\n            const cached = measuringCache.get(column.key);\n\n            if (requestedWidth === 'fit-once' && !cached.dataOnly)\n                return cached.width;\n            if (requestedWidth === 'fit-data-once' && cached.dataOnly)\n                return cached.width;\n        }\n\n        let width = 0;\n        for (const row of rows) {\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data-once')\n                continue;\n            if (row.type !== 'DATA' && requestedWidth === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.left + cell.padding.right;\n\n            const cellWidth = textResolver.measureWidth(text, font) + padding;\n\n            width = Math.max(width, cellWidth);\n        }\n\n        measuringCache.set(column.key, {\n            width,\n            dataOnly: requestedWidth === 'fit-data-once'\n        });\n\n        return width;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return columns.map(column => ({\n        ...column,\n        width: measureColumn(column)\n    }));\n}\n\nexport function getMeasuredRows(columns, rows, textResolver, formatResolver, measuringCache, presentKeys) {\n    if (rows.every(row => typeof row.height === 'number'))\n        return rows;\n\n    const measureRow = row => {\n        const requestedHeight = row.height;\n\n        if (typeof requestedHeight === 'number')\n            return requestedHeight;\n\n        if (measuringCache.has(row.key)) {\n            const cached = measuringCache.get(row.key);\n\n            if (requestedHeight === 'fit-once' && !cached.dataOnly)\n                return cached.height;\n            if (requestedHeight === 'fit-data-once' && cached.dataOnly)\n                return cached.height;\n        }\n\n        let height = 0;\n        for (const column of columns) {\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data-once')\n                continue;\n            if (column.type !== 'DATA' && requestedHeight === 'fit-data')\n                continue;\n\n            const cell = formatResolver.resolve(row, column);\n            const text = cell.text;\n            const font = cell.font;\n            const padding = cell.padding.top + cell.padding.bottom;\n\n            const cellHeight = textResolver.measureHeight(text, font) + padding;\n\n            height = Math.max(height, cellHeight);\n        }\n\n        measuringCache.set(row.key, {\n            height,\n            dataOnly: requestedHeight === 'fit-data-once'\n        });\n\n        return height;\n    }\n\n    for (const key of measuringCache.keys()) {\n        if (!presentKeys.has(key))\n            measuringCache.delete(key);\n    }\n\n    return rows.map(row => ({\n        ...row,\n        height: measureRow(row)\n    }));\n}",
         "export default function getKeys(entries) {\n    return new Set(entries.map(entry => entry.key));\n}\n",
-        "export default function getSortingFormatting(formatting) {\n    return formatting;\n}",
-        "import RulesLookup from \"./RulesLookup.js\";\n\n// const defaultComparatorAsc = (lhs, rhs) => lhs.value < rhs.value;\n// const defaultComparatorDesc = (lhs, rhs) => lhs.value > rhs.value;\n\nfunction defaultComparatorAsc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value < rhs.value;\n}\n\nfunction defaultComparatorDesc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value > rhs.value;\n}\n\nexport default class SortingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'HEADER'),\n                comparatorAsc: rule.comparator || defaultComparatorAsc,\n                comparatorDesc: (lhs, rhs) => -rule.comparator(lhs, rhs) || defaultComparatorDesc\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(column, row, sortByLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return null;\n            if (column.type !== 'DATA')\n                return null;\n            if (!sortByLookup.has('\"HEADER\"'))\n                return null;\n\n            return sortByLookup.get('\"HEADER\"') === 'ASC'\n                ? defaultComparatorAsc\n                : defaultComparatorDesc;\n        }\n\n        if (rules.length > 1)\n            throw new Error('Multiple sorting rules for the same cell'); // TODO: add more context\n\n        const rule = rules[0];\n\n        return sortByLookup.get(rule.by) === 'ASC'\n            ? rule.comparatorAsc\n            : rule.comparatorDesc;\n    }\n}",
+        "import getReducedFormatting from \"./getReducedFormatting.js\";\n\nexport default function getSortingFormatting(formatting) {\n    return getReducedFormatting(formatting, ['value', 'text']);\n}",
+        "import RulesLookup from \"./RulesLookup.js\";\nimport stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction defaultComparatorAsc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value < rhs.value;\n}\n\nfunction defaultComparatorDesc(lhs, rhs) {\n    if (lhs.value == undefined)\n        return false;\n    if (rhs.value == undefined)\n        return true;\n    return lhs.value > rhs.value;\n}\n\nexport default class SortingRules {\n    constructor(rules) {\n        this.rulesLookup = new RulesLookup();\n\n        for (const rule of rules) {\n            const comparatorAsc = rule.comparator\n                ? (lhs, rhs) => rule.comparator(lhs, rhs)\n                : (lhs, rhs) => defaultComparatorAsc(lhs, rhs);\n            const comparatorDesc = rule.comparator\n                ? (lhs, rhs) => !rule.comparator(lhs, rhs)\n                : (lhs, rhs) => defaultComparatorDesc(lhs, rhs);\n\n            const entry = {\n                by: stringifyId('by' in rule ? rule.by : 'HEADER'),\n                comparatorAsc: comparatorAsc,\n                comparatorDesc: comparatorDesc\n            };\n\n            this.rulesLookup.addRule(rule.column, rule.row, entry);\n        }\n    }\n\n    resolve(column, row, sortByLookup) {\n        const rules = this.rulesLookup.getRules(column, row);\n\n        if (rules.length === 0) {\n            if (row.type !== 'DATA')\n                return null;\n            if (column.type !== 'DATA')\n                return null;\n            if (!sortByLookup.has('\"HEADER\"'))\n                return null;\n\n            return sortByLookup.get('\"HEADER\"') === 'ASC'\n                ? defaultComparatorAsc\n                : defaultComparatorDesc;\n        }\n\n        if (rules.length > 1)\n            throw new Error('Multiple sorting rules for the same cell'); // TODO: add more context\n\n        const rule = rules[0];\n\n        if (!sortByLookup.has(rule.by))\n            return null;\n\n        return sortByLookup.get(rule.by) === 'ASC'\n            ? rule.comparatorAsc\n            : rule.comparatorDesc;\n    }\n}",
         "import SortingRules from \"../types/SortingRules.js\";\n\nexport default function getSortingRules(sorting) {\n    return new SortingRules(sorting);\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\n\nfunction getSortByLookup(sortBy, primaryKey, secondaryKey) {\n    const sortByLookup = new Map();\n    for (const cell of sortBy) {\n        const primary = stringifyId(cell[primaryKey]);\n        const secondary = stringifyId(cell[secondaryKey]);\n\n        if (!sortByLookup.has(primary))\n            sortByLookup.set(primary, new Map());\n\n        sortByLookup.get(primary).set(secondary, cell.direction);\n    }\n    return sortByLookup;\n}\n\nfunction flush(temp, result) {\n    temp.sort((lhs, rhs) => {\n        const result = lhs.comparator(lhs.cell, rhs.cell);\n        if (typeof result === 'number')\n            return result;\n        return result ? -1 : 1;\n    });\n    result.push(...temp.map(entry => entry.entity));\n    temp.length = 0;\n}\n\nexport function getSortedRows(sortBy, sortingRules, formattingRules, data, rows, columns, edition) {\n    if (sortBy.length === 0)\n        return rows;\n\n    const sortByLookup = getSortByLookup(sortBy, 'columnId', 'rowId');\n    const columnLookup = new Map(columns.map(column => [column.key, column]));\n    const sortedColumns = sortBy\n        .map(cell => stringifyId(cell.columnId))\n        .filter(key => columnLookup.has(key))\n        .map(key => columnLookup.get(key))\n        .reverse();\n\n    if (sortedColumns.length === 0)\n        return rows;\n\n    for (const column of sortedColumns) {\n        const result = [];\n        const temp = [];\n\n        for (const row of rows) {\n            const comparator = sortingRules.resolve(column, row, sortByLookup.get(column.key));\n\n            if (!comparator) {\n                flush(temp, result);\n                result.push(row);\n                continue;\n            }\n\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const entry = { entity: row, comparator, cell };\n\n            if (temp.length === 0) {\n                temp.push(entry);\n                continue;\n            }\n\n            if (temp[0].comparator === comparator) {\n                temp.push(entry);\n                continue;\n            }\n\n            flush(temp, result);\n            temp.push(entry);\n        }\n\n        flush(temp, result);\n        rows = result;\n    }\n\n    return rows;\n}\n\nexport function getSortedColumns(sortBy, sortingRules, formattingRules, data, rows, columns, edition) {\n    if (sortBy.length === 0)\n        return columns;\n\n    const sortByLookup = getSortByLookup(sortBy, 'rowId', 'columnId');\n    const rowLookup = new Map(rows.map(row => [row.key, row]));\n    const sortedRows = sortBy\n        .map(cell => stringifyId(cell.rowId))\n        .filter(key => rowLookup.has(key))\n        .map(key => rowLookup.get(key))\n        .reverse();\n\n    if (sortedRows.length === 0)\n        return columns;\n\n    for (const row of sortedRows) {\n        const result = [];\n        const temp = [];\n\n        for (const column of columns) {\n            const comparator = sortingRules.resolve(column, row, sortByLookup.get(row.key));\n\n            if (!comparator) {\n                flush(temp, result);\n                result.push(column);\n                continue;\n            }\n\n            const cell = formattingRules.resolve(data, rows, columns, row, column, edition);\n            const entry = { entity: column, comparator, cell };\n\n            if (temp.length === 0) {\n                temp.push(entry);\n                continue;\n            }\n\n            if (temp[0].comparator === comparator) {\n                temp.push(entry);\n                continue;\n            }\n\n            flush(temp, result);\n            temp.push(entry);\n        }\n\n        flush(temp, result);\n        columns = result;\n    }\n\n    return columns;\n}",
-        "import stringifyId from \"../core-utils/stringifyId.js\";\n\nconst grabOffset = 5;\n\n// TODO: not working when scrolled\n\nexport function getResizableColumn(columns, columnLookup, rowLookup, hoveredCell, mousePosition) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n    const x = mousePosition.x;\n\n    if (row.type !== 'HEADER')\n        return null;\n\n    if (x >= column.right - grabOffset && x <= column.right + grabOffset)\n        return column.id;\n\n    if (column.index === 0)\n        return null;\n    if (x < column.left - grabOffset || x > column.left + grabOffset)\n        return null;\n\n    return columns[column.index - 1].id;\n}\n\nexport function getResizableRow(rows, columnLookup, rowLookup, hoveredCell, mousePosition) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n    const y = mousePosition.y;\n\n    if (column.type !== 'HEADER')\n        return null;\n\n    if (y >= row.bottom - grabOffset && y <= row.bottom + grabOffset)\n        return row.id;\n\n    if (row.index === 0)\n        return null;\n    if (y < row.top - grabOffset || y > row.top + grabOffset)\n        return null;\n\n    return rows[row.index - 1].id;\n}",
+        "import stringifyId from \"../core-utils/stringifyId.js\";\nimport getInternalPosition from \"./getInternalPosition.js\";\n\nconst grabOffset = 5;\n\n// TODO: not working when scrolled\n\nexport function getResizableColumn(columns, columnLookup, rowLookup, hoveredCell, element, mousePosition, fixedSize, totalSize) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n\n    if (row.type !== 'HEADER')\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    if (!internalPosition)\n        return null;\n    const x = internalPosition.x;\n\n    if (x >= column.right - grabOffset && x <= column.right + grabOffset)\n        return column.id;\n\n    if (column.index === 0)\n        return null;\n    if (x < column.left - grabOffset || x > column.left + grabOffset)\n        return null;\n\n    return columns[column.index - 1].id;\n}\n\nexport function getResizableRow(rows, columnLookup, rowLookup, hoveredCell, element, mousePosition, fixedSize, totalSize) {\n    if (!hoveredCell)\n        return null;\n\n    const column = columnLookup.get(stringifyId(hoveredCell.columnId));\n    const row = rowLookup.get(stringifyId(hoveredCell.rowId));\n\n    if (column.type !== 'HEADER')\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    if (!internalPosition)\n        return null;\n    const y = internalPosition.y;\n\n    if (y >= row.bottom - grabOffset && y <= row.bottom + grabOffset)\n        return row.id;\n\n    if (row.index === 0)\n        return null;\n    if (y < row.top - grabOffset || y > row.top + grabOffset)\n        return null;\n\n    return rows[row.index - 1].id;\n}",
         "export default function getResolvedSortBy(sortBy) {\n    return sortBy.map(sort => ({\n        columnId: 'columnId' in sort ? sort.columnId : 'HEADER',\n        rowId: 'rowId' in sort ? sort.rowId : 'HEADER',\n        direction: sort.direction\n    }));\n}",
         "export default function getResolvedFilters(filters) {\n    return filters.map(filter => ({\n        columnId: 'columnId' in filter ? filter.columnId : 'FILTER',\n        rowId: 'rowId' in filter ? filter.rowId : 'FILTER',\n        expression: filter.expression\n    }));\n}",
         "function getActive(entries, callback) {\n    const ids = entries\n        .filter(entry => entry.type === 'DATA')\n        .map(entry => entry.id);\n\n    callback(ids);\n\n    return ids;\n}\n\nexport function getActiveColumns(columns, callback) {\n    return getActive(columns, callback);\n}\n\nexport function getActiveRows(rows, callback) {\n    return getActive(rows, callback);\n}",
-        "import getEditableCells from \"../state-utils/getEditableCells.js\";\nimport getDataFormatting from \"../state-utils/getDataFormatting.js\";\nimport getInputFormatting from \"../state-utils/getInputFormatting.js\";\nimport getRenderFormatting from \"../state-utils/getRenderFormatting.js\";\nimport getSections from \"../state-utils/getSections.js\";\nimport getEditedCellsAndFilters from \"../state-utils/getEditedCellsAndFilters.js\";\nimport getEdition from \"../state-utils/getEdition.js\";\nimport getSelection from \"../state-utils/getSelection.js\";\nimport getInvoked from \"../state-utils/getInvoked.js\";\nimport { getResolvedColumns, getResolvedRows } from \"../state-utils/getResolved.js\";\nimport { getPlacedColumns, getPlacedRows } from \"../state-utils/getPlaced.js\";\nimport getFormattingRules from \"../state-utils/getFormattingRules.js\";\nimport getFormatResolver from \"../state-utils/getFormatResolver.js\";\nimport { getFilteredColumns as getFilteredColumns, getFilteredRows as getFilteredRows } from \"../state-utils/getFiltered.js\";\nimport getFixedSize from \"../state-utils/getFixedSize.js\";\nimport getTotalSize from \"../state-utils/getTotalSize.js\";\nimport getTextResolver from \"../state-utils/getTextResolver.js\";\nimport getScrollRect from \"../state-utils/getScrollRect.js\";\nimport getHoveredCell from \"../state-utils/getHoveredCell.js\";\nimport getLookup from \"../state-utils/getLookup.js\";\nimport getHighlightedCells from \"../state-utils/getHighlightedCells.js\";\nimport getInputPlacement from \"../state-utils/getInputPlacement.js\";\nimport getIsTextValid from \"../state-utils/getIsTextValid.js\";\nimport { getUnfoldedColumns, getUnfoldedRows } from \"../state-utils/getUnfolded.js\";\nimport getFilteringRules from \"../state-utils/getFilteringRules.js\";\nimport getFilterFormatting from \"../state-utils/getFilterFormatting.js\";\nimport getMeasureFormatting from \"../state-utils/getMeasureFormatting.js\";\nimport { getMeasuredColumns, getMeasuredRows } from \"../state-utils/getMeasured.js\";\nimport getKeys from \"../state-utils/getKeys.js\";\nimport getSortingFormatting from \"../state-utils/getSortingFormatting.js\";\nimport getSortingRules from \"../state-utils/getSortingRules.js\";\nimport { getSortedColumns, getSortedRows } from \"../state-utils/getSorted.js\";\nimport { getResizableColumn, getResizableRow } from \"../state-utils/getResizable.js\";\nimport getResolvedSortBy from \"../state-utils/getResolvedSortBy.js\";\nimport getResolvedFilters from \"../state-utils/getResolvedFilters.js\";\nimport { getActiveColumns } from \"../state-utils/getActive.js\";\n\n// TODO: write some test to check if the cache is working properly\nfunction updateStateInternal(context) {\n    console.count('updateState');\n\n    const options = { ...context.localOptions, ...context.externalOptions };\n    const memory = context.memory;\n    const previousState = context.state;\n\n    // TODO: Move to utils\n    function cache(key, func, dependencies) {\n        const previousDependencies = memory[key] && memory[key].dependencies;\n        if (!previousDependencies || dependencies.some((dependency, index) => dependency !== previousDependencies[index]))\n            memory[key] = { value: func(...dependencies), dependencies };\n        return memory[key].value;\n    }\n\n    const devicePixelRatio = window.devicePixelRatio; // TODO: Trigger update on devicePixelRatio change\n    const borderWidth = options.borderWidth / devicePixelRatio;\n    const data = options.data;\n    const text = context.input.value;\n    const sortBy = cache('sortBy', getResolvedSortBy, [options.sortBy]);\n    const filters = cache('filters', getResolvedFilters, [options.filters]);\n    const textResolver = cache('textResolver', getTextResolver, []);\n    const dataFormatting = cache('dataFormatting', getDataFormatting, [options.formatting, options.dataSelector, sortBy]);\n    const editedCellsAndFilters = cache('editedCellsAndFilters', getEditedCellsAndFilters, [options.editedCells, filters]);\n    const edition = cache('edition', getEdition, [editedCellsAndFilters]);\n    const invokedColumns = cache('invokedColumns', getInvoked, [options.columns, data]);\n    const invokedRows = cache('invokedRows', getInvoked, [options.rows, data]);\n    // TODO: throw on duplicate ids\n    // TODO: throw on duplicate row/column filter ids\n    const unfoldedColumns = cache('unfoldedColumns', getUnfoldedColumns, [invokedColumns, data]);\n    const unfoldedRows = cache('unfoldedRows', getUnfoldedRows, [invokedRows, data]);\n    const unfilteredColumns = cache('unfilteredColumns', getResolvedColumns, [unfoldedColumns, options.pinnedLeft, options.pinnedRight, options.columnWidths]);\n    const unfilteredRows = cache('unfilteredRows', getResolvedRows, [unfoldedRows, options.pinnedTop, options.pinnedBottom, options.rowHeights]);\n    const unfilteredColumnKeys = cache('unfilteredColumnKeys', getKeys, [unfilteredColumns]);\n    const unfilteredRowKeys = cache('unfilteredRowKeys', getKeys, [unfilteredRows]);\n\n    // Filtering\n    const filterFormatting = cache('filterFormatting', getFilterFormatting, [dataFormatting]);\n    const filterFormattingRules = cache('filterFormattingRules', getFormattingRules, [filterFormatting]);\n    const filteringRules = cache('filteringRules', getFilteringRules, [options.filtering]);\n    const filteredColumns = cache('filteredColumns', getFilteredColumns, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n    const filteredRows = cache('filteredRows', getFilteredRows, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n\n    // Sorting\n    const sortingFormatting = cache('sortingFormatting', getSortingFormatting, [dataFormatting]);\n    const sortingFormattingRules = cache('sortingFormattingRules', getFormattingRules, [sortingFormatting]);\n    const sortingRules = cache('sortingRules', getSortingRules, [options.sorting]);\n    const sortedColumns = cache('sortedColumns', getSortedColumns, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n    const sortedRows = cache('sortedRows', getSortedRows, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n\n    // Shaping\n    const shapedColumns = sortedColumns;\n    const shapedRows = sortedRows;\n\n    // Measuring\n    const measureFormatting = cache('measureFormatting', getMeasureFormatting, [dataFormatting]);\n    const measureFormattingRules = cache('measureFormattingRules', getFormattingRules, [measureFormatting]);\n    const measureFormatResolver = cache('measureFormatResolver', getFormatResolver, [measureFormattingRules, data, shapedRows, shapedColumns, edition]);\n    const columnWidthCache = context.columnWidthCache;\n    const rowHeightCache = context.rowHeightCache;\n    const measuredColumns = cache('measuredColumns', getMeasuredColumns, [shapedColumns, shapedRows, textResolver, measureFormatResolver, columnWidthCache, unfilteredColumnKeys]);\n    const measuredRows = cache('measuredRows', getMeasuredRows, [shapedColumns, shapedRows, textResolver, measureFormatResolver, rowHeightCache, unfilteredRowKeys]);\n\n    // Placement\n    const columns = cache('columns', getPlacedColumns, [measuredColumns, devicePixelRatio, borderWidth]);\n    const rows = cache('rows', getPlacedRows, [measuredRows, devicePixelRatio, borderWidth]);\n    const columnLookup = cache('columnLookup', getLookup, [columns]);\n    const rowLookup = cache('rowLookup', getLookup, [rows]);\n    const focusedCell = options.focusedCell;\n    const sections = cache('sections', getSections, [columns, rows]);\n    const selectedCells = options.selectedCells;\n    const fixedSize = cache('fixedSize', getFixedSize, [sections.top.height, sections.bottom.height, sections.left.width, sections.right.width]);\n    const totalSize = cache('totalSize', getTotalSize, [columns, rows]);\n    // TODO: do some proper caching, so that if value is not changed, the old value is returned (currently not working because of scrolling)\n    const hoveredCell = getHoveredCell(context.element, context.mousePosition, rows, columns, fixedSize, totalSize);\n    const resizableColumn = context.resizingColumn || cache('resizableColumn', getResizableColumn, [columns, columnLookup, rowLookup, hoveredCell, context.mousePosition]);\n    const resizableRow = context.resizingRow || cache('resizableRow', getResizableRow, [rows, columnLookup, rowLookup, hoveredCell, context.mousePosition]);\n    const isMouseDown = context.isMouseDown;\n    const isResizing = !!resizableColumn || !!resizableRow;\n    const highlightedCells = cache('highlightedCells', getHighlightedCells, [isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup]);\n    const selection = cache('selection', getSelection, [selectedCells]);\n    const highlight = cache('highlight', getSelection, [highlightedCells]);\n    // TODO: addDataFormattingRules and addRenderFormattingRules should remove unnecessary rules\n    const renderFormatting = cache('renderFormatting', getRenderFormatting, [dataFormatting, hoveredCell, focusedCell, selection, highlight, edition, resizableColumn, resizableRow]);\n    const renderFormattingRules = cache('renderFormattingRules', getFormattingRules, [renderFormatting]);\n    const renderFormatResolver = cache('renderFormatResolver', getFormatResolver, [renderFormattingRules, data, rows, columns, edition]);\n    const inputFormatting = cache('inputFormatting', getInputFormatting, [dataFormatting]);\n    const inputFormattingRules = cache('inputFormattingRules', getFormattingRules, [inputFormatting]);\n    const inputFormatResolver = cache('inputFormatResolver', getFormatResolver, [inputFormattingRules, data, rows, columns, edition]);\n    const editableCells = cache('editableCells', getEditableCells, [selectedCells, inputFormatResolver, columnLookup, rowLookup]);\n    const inputPlacement = cache('inputPlacement', getInputPlacement, [editableCells, focusedCell, columnLookup, rowLookup, sections]);\n    const isTextValid = cache('isTextValid', getIsTextValid, [text, editableCells]);\n\n    // cache result, but not call\n    const scrollRect = getScrollRect(previousState?.scrollRect, totalSize, fixedSize, context.element);\n\n    // callbacks\n    cache('activeColumns', getActiveColumns, [columns, options.onActiveColumnsChange]);\n    cache('activeRows', getActiveColumns, [rows, options.onActiveRowsChange]);\n\n    context.state = {\n        options,\n        devicePixelRatio,\n        borderWidth,\n        data,\n        dataFormatting,\n        edition,\n        filteredColumns,\n        filteredRows,\n        columns,\n        rows,\n        sections,\n        selectedCells,\n        selection,\n        highlight,\n        hoveredCell,\n        focusedCell,\n        renderFormatting,\n        renderFormatResolver,\n        inputFormatting,\n        inputFormatResolver,\n        fixedSize,\n        totalSize,\n        textResolver,\n        scrollRect,\n        highlightedCells,\n        inputPlacement,\n        columnLookup,\n        rowLookup,\n        text,\n        isTextValid,\n        resizableColumn,\n        resizableRow,\n    };\n}\n\nexport default function updateState(context) {\n    if (!context.error) {\n        try {\n            updateStateInternal(context);\n        } catch (error) {\n            context.error = error;\n        }\n    }\n}",
-        "import getColumnIndex from \"./getColumnIndex.js\";\nimport getRowIndex from \"./getRowIndex.js\";\n\nexport default function getHoveredCell(element, mousePosition, rows, columns, fixedSize, totalSize) {\n    // TODO: sometimes mousePosition is outside of bounds and it crashes the click events\n\n    if (!mousePosition)\n        return null;\n    if (mousePosition.x < 0 || mousePosition.y < 0 || mousePosition.x > totalSize.width || mousePosition.y > totalSize.height)\n        return null;\n\n    const scrollOffset = {\n        left: element.scrollLeft,\n        top: element.scrollTop\n    };\n\n    const clientSize = {\n        width: element.clientWidth,\n        height: element.clientHeight\n    };\n\n    const x = mousePosition.x <= fixedSize.left\n        ? mousePosition.x\n        : mousePosition.x >= clientSize.width - fixedSize.right\n            ? totalSize.width - clientSize.width + mousePosition.x\n            : mousePosition.x + scrollOffset.left;\n    const y = mousePosition.y <= fixedSize.top\n        ? mousePosition.y\n        : mousePosition.y >= clientSize.height - fixedSize.bottom\n            ? totalSize.height - clientSize.height + mousePosition.y\n            : mousePosition.y + scrollOffset.top;\n\n    const hoverRowIndex = getRowIndex(rows, y);\n    const hoverColumnIndex = getColumnIndex(columns, x);\n\n    if (hoverRowIndex === -1 || hoverColumnIndex === -1)\n        return null;\n\n    return {\n        rowId: rows[hoverRowIndex].id,\n        columnId: columns[hoverColumnIndex].id\n    };\n}\n",
+        "import getEditableCells from \"../state-utils/getEditableCells.js\";\nimport getDataFormatting from \"../state-utils/getDataFormatting.js\";\nimport getInputFormatting from \"../state-utils/getInputFormatting.js\";\nimport getRenderFormatting from \"../state-utils/getRenderFormatting.js\";\nimport getSections from \"../state-utils/getSections.js\";\nimport getEditedCellsAndFilters from \"../state-utils/getEditedCellsAndFilters.js\";\nimport getEdition from \"../state-utils/getEdition.js\";\nimport getSelection from \"../state-utils/getSelection.js\";\nimport getInvoked from \"../state-utils/getInvoked.js\";\nimport { getResolvedColumns, getResolvedRows } from \"../state-utils/getResolved.js\";\nimport { getPlacedColumns, getPlacedRows } from \"../state-utils/getPlaced.js\";\nimport getFormattingRules from \"../state-utils/getFormattingRules.js\";\nimport getFormatResolver from \"../state-utils/getFormatResolver.js\";\nimport { getFilteredColumns as getFilteredColumns, getFilteredRows as getFilteredRows } from \"../state-utils/getFiltered.js\";\nimport getFixedSize from \"../state-utils/getFixedSize.js\";\nimport getTotalSize from \"../state-utils/getTotalSize.js\";\nimport getTextResolver from \"../state-utils/getTextResolver.js\";\nimport getScrollRect from \"../state-utils/getScrollRect.js\";\nimport getHoveredCell from \"../state-utils/getHoveredCell.js\";\nimport getLookup from \"../state-utils/getLookup.js\";\nimport getHighlightedCells from \"../state-utils/getHighlightedCells.js\";\nimport getInputPlacement from \"../state-utils/getInputPlacement.js\";\nimport getIsTextValid from \"../state-utils/getIsTextValid.js\";\nimport { getUnfoldedColumns, getUnfoldedRows } from \"../state-utils/getUnfolded.js\";\nimport getFilteringRules from \"../state-utils/getFilteringRules.js\";\nimport getFilterFormatting from \"../state-utils/getFilterFormatting.js\";\nimport getMeasureFormatting from \"../state-utils/getMeasureFormatting.js\";\nimport { getMeasuredColumns, getMeasuredRows } from \"../state-utils/getMeasured.js\";\nimport getKeys from \"../state-utils/getKeys.js\";\nimport getSortingFormatting from \"../state-utils/getSortingFormatting.js\";\nimport getSortingRules from \"../state-utils/getSortingRules.js\";\nimport { getSortedColumns, getSortedRows } from \"../state-utils/getSorted.js\";\nimport { getResizableColumn, getResizableRow } from \"../state-utils/getResizable.js\";\nimport getResolvedSortBy from \"../state-utils/getResolvedSortBy.js\";\nimport getResolvedFilters from \"../state-utils/getResolvedFilters.js\";\nimport { getActiveColumns } from \"../state-utils/getActive.js\";\n\n// TODO: write some test to check if the cache is working properly\nfunction updateStateInternal(context) {\n    console.count('updateState');\n\n    const options = { ...context.localOptions, ...context.externalOptions };\n    const memory = context.memory;\n    const previousState = context.state;\n    const element = context.element;\n\n    // TODO: Move to utils\n    function cache(key, func, dependencies) {\n        const previousDependencies = memory[key] && memory[key].dependencies;\n        if (!previousDependencies || dependencies.some((dependency, index) => dependency !== previousDependencies[index]))\n            memory[key] = { value: func(...dependencies), dependencies };\n        return memory[key].value;\n    }\n\n    const devicePixelRatio = window.devicePixelRatio; // TODO: Trigger update on devicePixelRatio change\n    const borderWidth = options.borderWidth / devicePixelRatio;\n    const data = options.data;\n    const text = context.input.value;\n    const sortBy = cache('sortBy', getResolvedSortBy, [options.sortBy]);\n    const filters = cache('filters', getResolvedFilters, [options.filters]);\n    const textResolver = cache('textResolver', getTextResolver, []);\n    const dataFormatting = cache('dataFormatting', getDataFormatting, [options.formatting, options.dataSelector, sortBy]);\n    const editedCellsAndFilters = cache('editedCellsAndFilters', getEditedCellsAndFilters, [options.editedCells, filters]);\n    const edition = cache('edition', getEdition, [editedCellsAndFilters]);\n    const invokedColumns = cache('invokedColumns', getInvoked, [options.columns, data]);\n    const invokedRows = cache('invokedRows', getInvoked, [options.rows, data]);\n    // TODO: throw on duplicate ids\n    // TODO: throw on duplicate row/column filter ids\n    const unfoldedColumns = cache('unfoldedColumns', getUnfoldedColumns, [invokedColumns, data]);\n    const unfoldedRows = cache('unfoldedRows', getUnfoldedRows, [invokedRows, data]);\n    const unfilteredColumns = cache('unfilteredColumns', getResolvedColumns, [unfoldedColumns, options.pinnedLeft, options.pinnedRight, options.columnWidths]);\n    const unfilteredRows = cache('unfilteredRows', getResolvedRows, [unfoldedRows, options.pinnedTop, options.pinnedBottom, options.rowHeights]);\n    const unfilteredColumnKeys = cache('unfilteredColumnKeys', getKeys, [unfilteredColumns]);\n    const unfilteredRowKeys = cache('unfilteredRowKeys', getKeys, [unfilteredRows]);\n\n    // Filtering\n    const filterFormatting = cache('filterFormatting', getFilterFormatting, [dataFormatting]);\n    const filterFormattingRules = cache('filterFormattingRules', getFormattingRules, [filterFormatting]);\n    const filteringRules = cache('filteringRules', getFilteringRules, [options.filtering]);\n    const filteredColumns = cache('filteredColumns', getFilteredColumns, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n    const filteredRows = cache('filteredRows', getFilteredRows, [filters, filteringRules, filterFormattingRules, data, unfilteredRows, unfilteredColumns, edition]);\n\n    // Sorting\n    const sortingFormatting = cache('sortingFormatting', getSortingFormatting, [dataFormatting]);\n    const sortingFormattingRules = cache('sortingFormattingRules', getFormattingRules, [sortingFormatting]);\n    const sortingRules = cache('sortingRules', getSortingRules, [options.sorting]);\n    const sortedColumns = cache('sortedColumns', getSortedColumns, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n    const sortedRows = cache('sortedRows', getSortedRows, [sortBy, sortingRules, sortingFormattingRules, data, filteredRows, filteredColumns, edition]);\n\n    // Shaping\n    const shapedColumns = sortedColumns;\n    const shapedRows = sortedRows;\n\n    // Measuring\n    const measureFormatting = cache('measureFormatting', getMeasureFormatting, [dataFormatting]);\n    const measureFormattingRules = cache('measureFormattingRules', getFormattingRules, [measureFormatting]);\n    const measureFormatResolver = cache('measureFormatResolver', getFormatResolver, [measureFormattingRules, data, shapedRows, shapedColumns, edition]);\n    const columnWidthCache = context.columnWidthCache;\n    const rowHeightCache = context.rowHeightCache;\n    const measuredColumns = cache('measuredColumns', getMeasuredColumns, [shapedColumns, shapedRows, textResolver, measureFormatResolver, columnWidthCache, unfilteredColumnKeys]);\n    const measuredRows = cache('measuredRows', getMeasuredRows, [shapedColumns, shapedRows, textResolver, measureFormatResolver, rowHeightCache, unfilteredRowKeys]);\n\n    // Placement\n    const columns = cache('columns', getPlacedColumns, [measuredColumns, devicePixelRatio, borderWidth]);\n    const rows = cache('rows', getPlacedRows, [measuredRows, devicePixelRatio, borderWidth]);\n    const columnLookup = cache('columnLookup', getLookup, [columns]);\n    const rowLookup = cache('rowLookup', getLookup, [rows]);\n    const focusedCell = options.focusedCell;\n    const sections = cache('sections', getSections, [columns, rows]);\n    const selectedCells = options.selectedCells;\n    const fixedSize = cache('fixedSize', getFixedSize, [sections.top.height, sections.bottom.height, sections.left.width, sections.right.width]);\n    const totalSize = cache('totalSize', getTotalSize, [columns, rows]);\n    // TODO: do some proper caching, so that if value is not changed, the old value is returned (currently not working because of scrolling)\n    const hoveredCell = getHoveredCell(element, context.mousePosition, rows, columns, fixedSize, totalSize);\n    const resizableColumn = context.resizingColumn || cache('resizableColumn', getResizableColumn, [columns, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, fixedSize, totalSize]);\n    const resizableRow = context.resizingRow || cache('resizableRow', getResizableRow, [rows, columnLookup, rowLookup, hoveredCell, element, context.mousePosition, fixedSize, totalSize]);\n    const isMouseDown = context.isMouseDown;\n    const isResizing = !!resizableColumn || !!resizableRow;\n    const highlightedCells = cache('highlightedCells', getHighlightedCells, [isMouseDown, isResizing, focusedCell, hoveredCell, columns, rows, columnLookup, rowLookup]);\n    const selection = cache('selection', getSelection, [selectedCells]);\n    const highlight = cache('highlight', getSelection, [highlightedCells]);\n    // TODO: addDataFormattingRules and addRenderFormattingRules should remove unnecessary rules\n    const renderFormatting = cache('renderFormatting', getRenderFormatting, [dataFormatting, hoveredCell, focusedCell, selection, highlight, edition, sortBy, resizableColumn, resizableRow, options.borderWidth]);\n    const renderFormattingRules = cache('renderFormattingRules', getFormattingRules, [renderFormatting]);\n    const renderFormatResolver = cache('renderFormatResolver', getFormatResolver, [renderFormattingRules, data, rows, columns, edition]);\n    const inputFormatting = cache('inputFormatting', getInputFormatting, [dataFormatting]);\n    const inputFormattingRules = cache('inputFormattingRules', getFormattingRules, [inputFormatting]);\n    const inputFormatResolver = cache('inputFormatResolver', getFormatResolver, [inputFormattingRules, data, rows, columns, edition]);\n    const editableCells = cache('editableCells', getEditableCells, [selectedCells, inputFormatResolver, columnLookup, rowLookup]);\n    const inputPlacement = cache('inputPlacement', getInputPlacement, [editableCells, focusedCell, columnLookup, rowLookup, sections]);\n    const isTextValid = cache('isTextValid', getIsTextValid, [text, editableCells]);\n\n    // cache result, but not call\n    const scrollRect = getScrollRect(previousState?.scrollRect, totalSize, fixedSize, element);\n\n    // callbacks\n    cache('activeColumns', getActiveColumns, [columns, options.onActiveColumnsChange]);\n    cache('activeRows', getActiveColumns, [rows, options.onActiveRowsChange]);\n\n    context.state = {\n        options,\n        devicePixelRatio,\n        borderWidth,\n        data,\n        dataFormatting,\n        edition,\n        filteredColumns,\n        filteredRows,\n        columns,\n        rows,\n        sections,\n        selectedCells,\n        selection,\n        highlight,\n        hoveredCell,\n        focusedCell,\n        renderFormatting,\n        renderFormatResolver,\n        inputFormatting,\n        inputFormatResolver,\n        fixedSize,\n        totalSize,\n        textResolver,\n        scrollRect,\n        highlightedCells,\n        inputPlacement,\n        columnLookup,\n        rowLookup,\n        text,\n        isTextValid,\n        resizableColumn,\n        resizableRow,\n    };\n}\n\nexport default function updateState(context) {\n    if (!context.error) {\n        try {\n            updateStateInternal(context);\n        } catch (error) {\n            context.error = error;\n        }\n    }\n}",
+        "import getColumnIndex from \"./getColumnIndex.js\";\nimport getInternalPosition from \"./getInternalPosition.js\";\nimport getRowIndex from \"./getRowIndex.js\";\n\nexport default function getHoveredCell(element, mousePosition, rows, columns, fixedSize, totalSize) {\n    if (!mousePosition)\n        return null;\n    if (mousePosition.x < 0 || mousePosition.y < 0 || mousePosition.x > totalSize.width || mousePosition.y > totalSize.height)\n        return null;\n\n    const internalPosition = getInternalPosition(element, mousePosition, fixedSize, totalSize);\n    const hoverRowIndex = getRowIndex(rows, internalPosition.y);\n    const hoverColumnIndex = getColumnIndex(columns, internalPosition.x);\n\n    if (hoverRowIndex === -1 || hoverColumnIndex === -1)\n        return null;\n\n    return {\n        rowId: rows[hoverRowIndex].id,\n        columnId: columns[hoverColumnIndex].id\n    };\n}\n",
         "export default function getRowIndex(rows, y) {\n    if (rows.length === 0)\n        return -1;\n    if (y < rows[0].topWithBorder)\n        return -1;\n    if (y > rows[rows.length - 1].bottomWithBorder)\n        return -1;\n\n    let iterA = 0;\n    let iterC = rows.length - 1;\n\n    while (iterA <= iterC) {\n        const iterB = Math.floor((iterA + iterC) / 2);\n\n        if (y < rows[iterB].topWithBorder)\n            iterC = iterB - 1;\n        else if (y > rows[iterB].bottomWithBorder)\n            iterA = iterB + 1;\n\n        else\n            return iterB;\n    }\n\n    return -1;\n}\n",
         "export default function getColumnIndex(columns, x) {\n    if (columns.length === 0)\n        return -1;\n    if (x < columns[0].leftWithBorder)\n        return -1;\n    if (x > columns[columns.length - 1].rightWithBorder)\n        return -1;\n\n    let iterA = 0;\n    let iterC = columns.length - 1;\n\n    while (iterA <= iterC) {\n        const iterB = Math.floor((iterA + iterC) / 2);\n\n        if (x < columns[iterB].leftWithBorder)\n            iterC = iterB - 1;\n        else if (x > columns[iterB].rightWithBorder)\n            iterA = iterB + 1;\n\n        else\n            return iterB;\n    }\n\n    return -1;\n}\n",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getCombinedCells(previousCells, newCells) {\n    const selection = new Selection(newCells);\n    return [...newCells, ...previousCells.filter(cell => !selection.isIdSelected(cell.rowId, cell.columnId))];\n}\n",
         "import Selection from \"../types/Selection.js\";\n\nexport default function getReducedCells(previousCells, cellsToRemove) {\n    const selection = new Selection(cellsToRemove);\n    return previousCells.filter(cell => !selection.isIdSelected(cell.rowId, cell.columnId));\n}\n",
         "export default function getMousePosition(event) {\n    const element = event.currentTarget;\n    const rect = element.getBoundingClientRect();\n    return {\n        x: event.clientX - rect.left,\n        y: event.clientY - rect.top\n    };\n}",
-        "import getEditableCells from \"./state-utils/getEditableCells.js\";\nimport stringifyId from \"./core-utils/stringifyId.js\";\nimport render from \"./core/render.js\";\nimport updateState from \"./core/state.js\";\nimport getCombinedCells from \"./state-utils/getCombinedCells.js\";\nimport getReducedCells from \"./state-utils/getReducedCells.js\";\nimport getMousePosition from \"./state-utils/getMousePosition.js\";\nimport getNewSortBy from \"./state-utils/getNewSortBy.js\";\nimport getClipboardData from \"./state-utils/getClipboardData.js\";\nimport getToggledValue from \"./state-utils/getToggledValue.js\";\nimport getCellType from \"./state-utils/getCellType.js\";\n\nfunction initialize(element) {\n    if ('spread-grid-context' in element) return;\n\n    console.log('initialize');\n\n    const canvases = {\n        'top-left': document.createElement('canvas'),\n        'top-center': document.createElement('canvas'),\n        'top-right': document.createElement('canvas'),\n        'middle-left': document.createElement('canvas'),\n        'middle-center': document.createElement('canvas'),\n        'middle-right': document.createElement('canvas'),\n        'bottom-left': document.createElement('canvas'),\n        'bottom-center': document.createElement('canvas'),\n        'bottom-right': document.createElement('canvas')\n    };\n    const input = document.createElement('input');\n\n    element.setAttribute('tabindex', '0');\n    element.setAttribute('style', 'max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;');\n    element.classList.add('spread-grid');\n    canvases['top-left'].setAttribute('style', 'position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;');\n    canvases['top-center'].setAttribute('style', 'position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;');\n    canvases['top-right'].setAttribute('style', 'position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;');\n    canvases['middle-left'].setAttribute('style', 'position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;');\n    canvases['middle-center'].setAttribute('style', 'grid-row: 2; grid-column: 2; z-index: 0;');\n    canvases['middle-right'].setAttribute('style', 'position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;');\n    canvases['bottom-left'].setAttribute('style', 'position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;');\n    canvases['bottom-center'].setAttribute('style', 'position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;');\n    canvases['bottom-right'].setAttribute('style', 'position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;');\n    input.setAttribute('style', 'position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;');\n\n    const context = {\n        externalOptions: {},\n        state: null,\n        memory: {},\n        element: element,\n        canvases: canvases,\n        input: input,\n        renderRequested: false,\n        mousePosition: null,\n        isMouseDown: false,\n        columnWidthCache: new Map(),\n        rowHeightCache: new Map(),\n    };\n\n    context.requestNewRender = () => {\n        if (context.renderRequested) return;\n        context.renderRequested = true;\n        requestAnimationFrame(() => {\n            context.renderRequested = false;\n            updateState(context);\n            render(context);\n        });\n    };\n\n    context.addEventListener = (element, type, listener) => {\n        element.addEventListener(type, (event) => {\n            try {\n                listener(event);\n            }\n            catch (error) {\n                error.message = `[${type} event]: ${error.message}`;\n                context.error = error;\n                context.requestNewRender();\n            }\n        });\n    }\n\n    context.localOptions = {\n        data: [],\n        columns: [{ type: 'DATA-BLOCK' }],\n        rows: [{ type: 'HEADER' }, { type: 'DATA-BLOCK' }],\n        formatting: [],\n        filtering: [],\n        sorting: [],\n        dataSelector: ({ data, row, column }) => data[row.id][column.id],\n        pinnedTop: 0,\n        pinnedBottom: 0,\n        pinnedLeft: 0,\n        pinnedRight: 0,\n        borderWidth: 1,\n        focusedCell: null,\n        onFocusedCellChange: (focusedCell) => {\n            context.localOptions.focusedCell = focusedCell;\n            context.requestNewRender();\n        },\n        selectedCells: [],\n        onSelectedCellsChange: (selectedCells) => {\n            context.localOptions.selectedCells = selectedCells;\n            context.requestNewRender();\n        },\n        highlightedCells: [],\n        editedCells: [],\n        onEditedCellsChange: (editedCells) => {\n            // TODO: optimize by coalescing\n            context.localOptions.editedCells = editedCells;\n            context.requestNewRender();\n        },\n        filters: [],\n        onFiltersChange: (filters) => {\n            context.localOptions.filters = filters;\n            context.requestNewRender();\n        },\n        sortBy: [],\n        onSortByChange: (sortBy) => {\n            context.localOptions.sortBy = sortBy;\n            context.requestNewRender();\n        },\n        onCellClick: () => { },\n        onCustomCellClick: () => { },\n        columnWidths: [],\n        onColumnWidthsChange: (columnWidths) => {\n            context.localOptions.columnWidths = columnWidths;\n            context.requestNewRender();\n        },\n        rowHeights: [],\n        onRowHeightsChange: (rowHeights) => {\n            context.localOptions.rowHeights = rowHeights;\n            context.requestNewRender();\n        },\n        onActiveColumnsChange: () => { },\n        onActiveRowsChange: () => { },\n    };\n\n    element['spread-grid-context'] = context;\n\n    const setText = (text) => {\n        input.value = text;\n        input.dispatchEvent(new Event('input'));\n    }\n\n    const accept = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const text = context.state.text;\n        const isTextValid = context.state.isTextValid;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const addEditedCells = (cells) => setEditedCells(getCombinedCells(context.state.options.editedCells, cells));\n        const addFilters = (cells) => setFilters(getCombinedCells(context.state.options.filters, cells));\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (text === '')\n            return;\n        if (!isTextValid)\n            return;\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        const dataCells = editableCells.filter(cell => cell.type === 'DATA');\n        const filterCells = editableCells.filter(cell => cell.type === 'FILTER');\n\n        addEditedCells(dataCells.map(cell => ({ ...cell.cell, value: cell.edit.parse({ string: text }) })));\n        addFilters(filterCells.map(cell => ({ ...cell.cell, expression: cell.edit.parse({ string: text }) })));\n\n        if (!autoCommit)\n            setText('');\n    };\n\n    const clear = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const removeEditedCells = (cells) => setEditedCells(getReducedCells(context.state.options.editedCells, cells));\n        const removeFilters = (cells) => setFilters(getReducedCells(context.state.options.filters, cells));\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        removeEditedCells(selectedCells);\n        removeFilters(selectedCells);\n    }\n\n    // TODO: Move other input functions here as well\n\n    context.addEventListener(element, 'scroll', (event) => {\n        // TODO: only request new render if scroll position changed outside of the scope\n        // TODO: how to: calculate the new scrollRect here and compare it to the one in the state\n        // TODO: Also don't forget to check if the highlighted cell did change\n        // TODO: Consider forcing a new render when visible scrollRect changes (without waiting for the next render frame)\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseenter', (event) => {\n        context.mousePosition = getMousePosition(event);\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mousemove', (event) => {\n        context.mousePosition = getMousePosition(event);\n\n        if (context.resizingColumn) {\n            const column = context.state.columnLookup.get(stringifyId(context.resizingColumn));\n            const columnWidth = column.width;\n            const columnRight = column.right;\n            const mousePosition = context.mousePosition.x;\n            const newColumnWidth = Math.max(10, mousePosition - columnRight + columnWidth);\n            const previousColumnWidths = context.state.options.columnWidths;\n            const newColumnWidths = previousColumnWidths\n                .filter(columnWidth => stringifyId(columnWidth.columnId) !== column.key)\n                .concat([{ columnId: column.id, width: newColumnWidth }]);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n        }\n        if (context.resizingRow) {\n            const row = context.state.rowLookup.get(stringifyId(context.resizingRow));\n            const rowHeight = row.height;\n            const rowBottom = row.bottom;\n            const mousePosition = context.mousePosition.y;\n            const newRowHeight = Math.max(10, mousePosition - rowBottom + rowHeight);\n            const previousRowHeights = context.state.options.rowHeights;\n            const newRowHeights = previousRowHeights\n                .filter(rowHeight => stringifyId(rowHeight.rowId) !== row.key)\n                .concat([{ rowId: row.id, height: newRowHeight }]);\n            context.state.options.onRowHeightsChange(newRowHeights);\n        }\n\n        // TODO: only request new render if hovered cell changed\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseleave', () => {\n        context.mousePosition = null;\n        context.requestNewRender();\n    });\n\n    // TODO: update mouse position on resize\n\n    context.addEventListener(element, 'mousedown', (event) => {\n        updateState(context);\n        setText('');\n\n        context.isMouseDown = true;\n        context.mouseDownPosition = context.mousePosition;\n        context.mouseDownCell = context.state.hoveredCell;\n\n        if (context.state.resizableColumn) {\n            context.resizingColumn = context.state.resizableColumn;\n        }\n        if (context.state.resizableRow) {\n            context.resizingRow = context.state.resizableRow;\n        }\n        if (!context.state.resizableColumn && !context.state.resizableRow) {\n            context.state.options.onFocusedCellChange(context.state.hoveredCell);\n        }\n\n        if (!event.ctrlKey)\n            context.state.options.onSelectedCellsChange([]);\n\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseup', (event) => {\n        updateState(context);\n\n        context.isMouseDown = false;\n        context.resizingColumn = null;\n        context.resizingRow = null;\n\n        context.state.options.onSelectedCellsChange(getCombinedCells(context.state.options.selectedCells, context.state.highlightedCells));\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'pointerdown', (event) => {\n        context.element.setPointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'pointerup', (event) => {\n        context.element.releasePointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'click', (event) => {\n        updateState(context);\n\n        const cell = context.state.hoveredCell;\n        const mouseDownCell = context.mouseDownCell;\n\n        if (context.state.resizableColumn || context.state.resizableRow)\n            return;\n        if (cell === null)\n            return;\n        if (stringifyId(cell.columnId) !== stringifyId(mouseDownCell.columnId))\n            return;\n        if (stringifyId(cell.rowId) !== stringifyId(mouseDownCell.rowId))\n            return;\n\n        const column = context.state.columnLookup.get(stringifyId(cell.columnId));\n        const row = context.state.rowLookup.get(stringifyId(cell.rowId));\n        const sortBy = context.state.options.sortBy;\n        const formatResolver = context.state.inputFormatResolver;\n        const cellData = formatResolver.resolve(row, column);\n\n        if (cellData.edit?.toggle) {\n            const edition = context.state.edition;\n            const newValue = getToggledValue(cellData, column, row, edition);\n            const cellType = getCellType(column, row);\n            if (cellType === 'DATA')\n                context.state.options.onEditedCellsChange(getCombinedCells(context.state.options.editedCells, [{ ...cell, value: newValue }]));\n            if (cellType === 'FILTER')\n                context.state.options.onFiltersChange(getCombinedCells(context.state.options.filters, [{ ...cell, expression: newValue }]));\n        } else if (column.type === 'DATA' && row.type === 'DATA') {\n            context.state.options.onCellClick(context.state.hoveredCell);\n        } else if (column.type === 'CUSTOM' || row.type === 'CUSTOM') {\n            context.state.options.onCustomCellClick(context.state.hoveredCell);\n        } else if (column.type === 'HEADER' || row.type === 'HEADER') {\n            const newSortBy = getNewSortBy(sortBy, column, row, event.ctrlKey);\n            context.state.options.onSortByChange(newSortBy);\n            context.state.options.onSelectedCellsChange([]);\n        }\n    });\n\n    context.addEventListener(element, 'dblclick', (event) => {\n        updateState(context);\n\n        if (context.state.resizableColumn) {\n            const resizableColumnKey = stringifyId(context.state.resizableColumn);\n            const newColumnWidths = context.state.options.columnWidths.filter(columnWidth => stringifyId(columnWidth.columnId) !== resizableColumnKey);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n            context.columnWidthCache.delete(resizableColumnKey);\n        }\n        if (context.state.resizableRow) {\n            const resizableRowKey = stringifyId(context.state.resizableRow);\n            const newRowHeights = context.state.options.rowHeights.filter(rowHeight => stringifyId(rowHeight.rowId) !== resizableRowKey);\n            context.state.options.onRowHeightsChange(newRowHeights);\n            context.rowHeightCache.delete(resizableRowKey);\n        }\n\n        const focusedCell = context.state.focusedCell;\n        if (focusedCell === null)\n            return;\n\n        const focusedColumnKey = stringifyId(focusedCell.columnId);\n        const focusedRowKey = stringifyId(focusedCell.rowId);\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const formatResolver = context.state.inputFormatResolver;\n\n        if (!columnLookup.has(focusedColumnKey))\n            return;\n        if (!rowLookup.has(focusedRowKey))\n            return;\n\n        const column = columnLookup.get(focusedColumnKey);\n        const row = rowLookup.get(focusedRowKey);\n        const cell = formatResolver.resolve(row, column);\n        const text = cell.text; // TODO: Make it configurable\n\n        if (!cell.edit)\n            return;\n        if (cell.edit.toggle)\n            return;\n\n        setText(text);\n        input?.select();\n    });\n\n    context.addEventListener(element, 'focus', () => {\n        if (input.parentElement)\n            input.focus({ preventScroll: true });\n    });\n\n    context.addEventListener(element, 'keydown', (event) => {\n        // TODO: make sure it's not invoked on keydown of the input\n        updateState(context);\n\n        const focusedCell = context.state.focusedCell;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const selectedCells = context.state.options.selectedCells;\n        const setSelectedCells = context.state.options.onSelectedCellsChange;\n        const addSelectedCells = (cells) => setSelectedCells(getCombinedCells(selectedCells, cells));\n        const setFocusedCell = context.state.options.onFocusedCellChange;\n        const editedCells = context.state.options.editedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const columns = context.state.columns;\n        const rows = context.state.rows;\n        const text = context.state.text;\n        const inputFormatResolver = context.state.inputFormatResolver;\n\n        const arrowTo = (cell, event) => {\n            setFocusedCell(cell);\n\n            if (event.shiftKey)\n                addSelectedCells([cell]);\n            else\n                setSelectedCells([cell]);\n        };\n\n        const arrowHorizontally = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedColumnKey = stringifyId(focusedCell.columnId);\n            if (!columnLookup.has(focusedColumnKey))\n                return;\n\n            const focusedColumnIndex = columnLookup.get(focusedColumnKey).index;\n            const newColumnIndex = Math.max(0, Math.min(columns.length - 1, focusedColumnIndex + offset));\n            if (newColumnIndex === focusedColumnIndex)\n                return;\n\n            const newFocusedCell = { rowId: focusedCell.rowId, columnId: columns[newColumnIndex].id };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const arrowVertically = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedRowKey = stringifyId(focusedCell.rowId);\n            if (!rowLookup.has(focusedRowKey))\n                return;\n\n            const focusedRowIndex = rowLookup.get(focusedRowKey).index;\n            const newRowIndex = Math.max(0, Math.min(rows.length - 1, focusedRowIndex + offset));\n            if (newRowIndex === focusedRowIndex)\n                return;\n\n            const newFocusedCell = { rowId: rows[newRowIndex].id, columnId: focusedCell.columnId };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const preventDefault = () => {\n            event.preventDefault();\n            event.stopPropagation();\n        };\n\n        const cancel = () => {\n            if (text !== '') {\n                setText('');\n            }\n            else if (selectedCells.length > 1) {\n                setSelectedCells([focusedCell]);\n            }\n            else if (editedCells.length > 0) {\n                setEditedCells([]);\n            }\n            else {\n                setFocusedCell(null);\n                setSelectedCells([]);\n            }\n        };\n\n        const copyToClipboard = (event) => {\n            if (!event.ctrlKey)\n                return;\n\n            const clipboardData = getClipboardData(selectedCells, columns, rows, inputFormatResolver);\n\n            if (navigator.clipboard) {\n                navigator.clipboard.writeText(clipboardData);\n            } else {\n                const textArea = document.createElement('textarea');\n                textArea.value = clipboardData;\n                document.body.appendChild(textArea);\n                textArea.select();\n                document.execCommand('copy');\n                document.body.removeChild(textArea);\n            }\n        }\n\n        switch (event.key) {\n            case 'Escape':\n                cancel();\n                break;\n            case 'Enter':\n                accept();\n                break;\n            case 'ArrowUp':\n                // TODO: When ctrl and shift are pressed together, select all cells between the focused cell and the new cell\n                // TODO: When shift is pressed, expand the current rect selection instead of moving the focused cell\n                preventDefault();\n                arrowVertically(event.ctrlKey ? -rows.length : -1, event);\n                break;\n            case 'ArrowDown':\n                preventDefault();\n                arrowVertically(event.ctrlKey ? rows.length : 1, event);\n                break;\n            case 'ArrowLeft':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? -columns.length : -1, event);\n                break;\n            case 'ArrowRight':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? columns.length : 1, event);\n                break;\n            case 'Delete':\n            case 'Backspace':\n                clear();\n                break;\n            case 'c':\n                copyToClipboard(event);\n                break;\n            default:\n                break;\n        }\n    });\n\n    new ResizeObserver(() => {\n        context.requestNewRender();\n    }).observe(element);\n\n    context.addEventListener(input, 'input', (event) => {\n        // TODO: check performance of this (if it's ok to update the state on every input event)\n        updateState(context);\n\n        if (event.target.value) {\n            accept(true);\n\n            input.style.opacity = 1;\n            input.style.pointerEvents = 'auto';\n        }\n        else {\n            if (event.isTrusted)\n                clear(true);\n\n            input.style.opacity = 0;\n            input.style.pointerEvents = 'none';\n        }\n    });\n\n    context.addEventListener(input, 'click', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'dblclick', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'mousedown', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'keydown', (event) => {\n        switch (event.key) {\n            case 'Enter':\n            case 'Escape':\n                break;\n            case 'Delete':\n            case 'Backspace':\n            case 'ArrowUp':\n            case 'ArrowDown':\n            case 'ArrowLeft':\n            case 'ArrowRight':\n                if (input.value !== '') {\n                    event.stopPropagation();\n                    context.requestNewRender();\n                }\n                break;\n            default:\n                event.stopPropagation();\n                // TODO: maybe only check if the new text is valid\n                context.requestNewRender();\n                break;\n        }\n    });\n}\n\nexport default function createGrid(element, options) {\n    console.log('createGrid');\n\n    initialize(element);\n\n    const context = element['spread-grid-context'];\n    context.externalOptions = options;\n\n    if (context.state === null) {\n        updateState(context);\n        // TODO: only render if the state has sufficiently changed\n        render(context);\n    }\n    else {\n        context.requestNewRender();\n    }\n}",
+        "export function getWithAssumedId(cells, defaultId) {\n    return cells.map(cell => ({\n        ...cell,\n        columnId: 'id' in cell ? cell.id : defaultId,\n        rowId: 'id' in cell ? cell.id : defaultId\n    }));\n}",
+        "import getEditableCells from \"./state-utils/getEditableCells.js\";\nimport stringifyId from \"./core-utils/stringifyId.js\";\nimport render from \"./core/render.js\";\nimport updateState from \"./core/state.js\";\nimport getCombinedCells from \"./state-utils/getCombinedCells.js\";\nimport getReducedCells from \"./state-utils/getReducedCells.js\";\nimport getMousePosition from \"./state-utils/getMousePosition.js\";\nimport getNewSortBy from \"./state-utils/getNewSortBy.js\";\nimport getClipboardData from \"./state-utils/getClipboardData.js\";\nimport getToggledValue from \"./state-utils/getToggledValue.js\";\nimport getCellEditType from \"./state-utils/getCellEditType.js\";\nimport getInternalPosition from \"./state-utils/getInternalPosition.js\";\nimport { getWithAssumedId } from \"./state-utils/getWithAssumedId.js\";\n\nfunction initialize(element) {\n    if ('spread-grid-context' in element) return;\n\n    console.log('initialize');\n\n    const canvases = {\n        'top-left': document.createElement('canvas'),\n        'top-center': document.createElement('canvas'),\n        'top-right': document.createElement('canvas'),\n        'middle-left': document.createElement('canvas'),\n        'middle-center': document.createElement('canvas'),\n        'middle-right': document.createElement('canvas'),\n        'bottom-left': document.createElement('canvas'),\n        'bottom-center': document.createElement('canvas'),\n        'bottom-right': document.createElement('canvas')\n    };\n    const input = document.createElement('input');\n\n    element.setAttribute('tabindex', '0');\n    element.setAttribute('style', 'max-width: 100vw; max-height: 100vh; overflow: auto; display: grid; position: relative; grid-template-columns: fit-content(0) fit-content(0) fit-content(0); grid-template-rows: fit-content(0) fit-content(0) fit-content(0); outline: none; user-select: none;');\n    element.classList.add('spread-grid');\n    canvases['top-left'].setAttribute('style', 'position: sticky; left: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 1;');\n    canvases['top-center'].setAttribute('style', 'position: sticky; top: 0; z-index: 1; grid-row: 1; grid-column: 2;');\n    canvases['top-right'].setAttribute('style', 'position: sticky; right: 0; top: 0; z-index: 2; grid-row: 1; grid-column: 3;');\n    canvases['middle-left'].setAttribute('style', 'position: sticky; left: 0; z-index: 1; grid-row: 2; grid-column: 1;');\n    canvases['middle-center'].setAttribute('style', 'grid-row: 2; grid-column: 2; z-index: 0;');\n    canvases['middle-right'].setAttribute('style', 'position: sticky; right: 0; z-index: 1; grid-row: 2; grid-column: 3;');\n    canvases['bottom-left'].setAttribute('style', 'position: sticky; left: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 1;');\n    canvases['bottom-center'].setAttribute('style', 'position: sticky; bottom: 0; z-index: 1; grid-row: 3; grid-column: 2;');\n    canvases['bottom-right'].setAttribute('style', 'position: sticky; right: 0; bottom: 0; z-index: 2; grid-row: 3; grid-column: 3;');\n    input.setAttribute('style', 'position: sticky; z-index: 3; outline: none; border: none; box-shadow: none; padding: 0 5px; font-size: 12px; font-family: Calibri; background-color: white; box-sizing: border-box; opacity: 0; pointer-events: none;');\n\n    const context = {\n        externalOptions: {},\n        state: null,\n        memory: {},\n        element: element,\n        canvases: canvases,\n        input: input,\n        renderRequested: false,\n        mousePosition: null,\n        isMouseDown: false,\n        columnWidthCache: new Map(),\n        rowHeightCache: new Map(),\n    };\n\n    context.requestNewRender = () => {\n        if (context.renderRequested) return;\n        context.renderRequested = true;\n        requestAnimationFrame(() => {\n            context.renderRequested = false;\n            updateState(context);\n            render(context);\n        });\n    };\n\n    context.addEventListener = (element, type, listener) => {\n        element.addEventListener(type, (event) => {\n            try {\n                listener(event);\n            }\n            catch (error) {\n                error.message = `[${type} event]: ${error.message}`;\n                context.error = error;\n                context.requestNewRender();\n            }\n        });\n    }\n\n    context.localOptions = {\n        data: [],\n        columns: [{ type: 'DATA-BLOCK' }],\n        rows: [{ type: 'HEADER' }, { type: 'DATA-BLOCK' }],\n        formatting: [],\n        filtering: [],\n        sorting: [],\n        dataSelector: ({ data, row, column }) => data?.[row.id]?.[column.id],\n        pinnedTop: 0,\n        pinnedBottom: 0,\n        pinnedLeft: 0,\n        pinnedRight: 0,\n        borderWidth: 1,\n        focusedCell: null,\n        onFocusedCellChange: (focusedCell) => {\n            context.localOptions.focusedCell = focusedCell;\n            context.requestNewRender();\n        },\n        selectedCells: [],\n        onSelectedCellsChange: (selectedCells) => {\n            context.localOptions.selectedCells = selectedCells;\n            context.requestNewRender();\n        },\n        highlightedCells: [],\n        editedCells: [],\n        onEditedCellsChange: (editedCells) => {\n            // TODO: optimize by coalescing\n            context.localOptions.editedCells = editedCells;\n            context.requestNewRender();\n        },\n        filters: [],\n        onFiltersChange: (filters) => {\n            context.localOptions.filters = filters;\n            context.requestNewRender();\n        },\n        sortBy: [],\n        onSortByChange: (sortBy) => {\n            context.localOptions.sortBy = sortBy;\n            context.requestNewRender();\n        },\n        onCellClick: () => { },\n        onCustomCellClick: () => { },\n        columnWidths: [],\n        onColumnWidthsChange: (columnWidths) => {\n            context.localOptions.columnWidths = columnWidths;\n            context.requestNewRender();\n        },\n        rowHeights: [],\n        onRowHeightsChange: (rowHeights) => {\n            context.localOptions.rowHeights = rowHeights;\n            context.requestNewRender();\n        },\n        onActiveColumnsChange: () => { },\n        onActiveRowsChange: () => { },\n    };\n\n    element['spread-grid-context'] = context;\n\n    const setText = (text) => {\n        input.value = text;\n        input.dispatchEvent(new Event('input'));\n    }\n\n    const accept = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const text = context.state.text;\n        const isTextValid = context.state.isTextValid;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const addEditedCells = (cells) => setEditedCells(getCombinedCells(context.state.options.editedCells, cells));\n        const addFilters = (cells) => setFilters(getCombinedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (text === '')\n            return;\n        if (!isTextValid)\n            return;\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        const dataCells = editableCells.filter(cell => cell.type === 'DATA');\n        const filterCells = editableCells.filter(cell => cell.type === 'FILTER');\n\n        addEditedCells(dataCells.map(cell => ({ ...cell.cell, value: cell.edit.parse({ string: text }) })));\n        addFilters(filterCells.map(cell => ({ ...cell.cell, expression: cell.edit.parse({ string: text }) })));\n\n        if (!autoCommit)\n            setText('');\n    };\n\n    const clear = (autoCommit) => {\n        const selectedCells = context.state.options.selectedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const setFilters = context.state.options.onFiltersChange;\n        const removeEditedCells = (cells) => setEditedCells(getReducedCells(context.state.options.editedCells, cells));\n        const removeFilters = (cells) => setFilters(getReducedCells(getWithAssumedId(context.state.options.filters, 'FILTER'), cells));\n        const formatResolver = context.state.inputFormatResolver;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const editableCells = getEditableCells(selectedCells, formatResolver, columnLookup, rowLookup);\n\n        if (autoCommit && !editableCells.every(cell => cell.edit.autoCommit))\n            return;\n\n        removeEditedCells(selectedCells);\n        removeFilters(selectedCells);\n    }\n\n    // TODO: Move other input functions here as well\n\n    context.addEventListener(element, 'scroll', (event) => {\n        // TODO: only request new render if scroll position changed outside of the scope\n        // TODO: how to: calculate the new scrollRect here and compare it to the one in the state\n        // TODO: Also don't forget to check if the highlighted cell did change\n        // TODO: Consider forcing a new render when visible scrollRect changes (without waiting for the next render frame)\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseenter', (event) => {\n        context.mousePosition = getMousePosition(event);\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mousemove', (event) => {\n        context.mousePosition = getMousePosition(event);\n\n        if (context.resizingColumn) {\n            const column = context.state.columnLookup.get(stringifyId(context.resizingColumn));\n            const columnWidth = column.width;\n            const columnRight = column.right;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newColumnWidth = Math.max(10, internalPosition.x - columnRight + columnWidth);\n            const previousColumnWidths = context.state.options.columnWidths;\n            const newColumnWidths = previousColumnWidths\n                .filter(columnWidth => stringifyId(columnWidth.columnId) !== column.key)\n                .concat([{ columnId: column.id, width: newColumnWidth }]);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n        }\n        if (context.resizingRow) {\n            const row = context.state.rowLookup.get(stringifyId(context.resizingRow));\n            const rowHeight = row.height;\n            const rowBottom = row.bottom;\n            const internalPosition = getInternalPosition(element, context.mousePosition, context.state.fixedSize, context.state.totalSize);\n            const newRowHeight = Math.max(10, internalPosition.y - rowBottom + rowHeight);\n            const previousRowHeights = context.state.options.rowHeights;\n            const newRowHeights = previousRowHeights\n                .filter(rowHeight => stringifyId(rowHeight.rowId) !== row.key)\n                .concat([{ rowId: row.id, height: newRowHeight }]);\n            context.state.options.onRowHeightsChange(newRowHeights);\n        }\n\n        // TODO: only request new render if hovered cell changed\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseleave', () => {\n        context.mousePosition = null;\n        context.requestNewRender();\n    });\n\n    // TODO: update mouse position on resize\n\n    context.addEventListener(element, 'mousedown', (event) => {\n        updateState(context);\n        setText('');\n\n        context.isMouseDown = true;\n        context.mouseDownPosition = context.mousePosition;\n        context.mouseDownCell = context.state.hoveredCell;\n\n        if (context.state.resizableColumn) {\n            context.resizingColumn = context.state.resizableColumn;\n        }\n        if (context.state.resizableRow) {\n            context.resizingRow = context.state.resizableRow;\n        }\n        if (!context.state.resizableColumn && !context.state.resizableRow) {\n            context.state.options.onFocusedCellChange(context.state.hoveredCell);\n        }\n\n        if (!event.ctrlKey)\n            context.state.options.onSelectedCellsChange([]);\n\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'mouseup', (event) => {\n        updateState(context);\n\n        context.isMouseDown = false;\n        context.resizingColumn = null;\n        context.resizingRow = null;\n\n        context.state.options.onSelectedCellsChange(getCombinedCells(context.state.options.selectedCells, context.state.highlightedCells));\n        context.requestNewRender();\n    });\n\n    context.addEventListener(element, 'pointerdown', (event) => {\n        context.element.setPointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'pointerup', (event) => {\n        context.element.releasePointerCapture(event.pointerId);\n    });\n\n    context.addEventListener(element, 'click', (event) => {\n        updateState(context);\n\n        const cell = context.state.hoveredCell;\n        const mouseDownCell = context.mouseDownCell;\n\n        if (context.state.resizableColumn || context.state.resizableRow)\n            return;\n        if (cell === null)\n            return;\n        if (stringifyId(cell.columnId) !== stringifyId(mouseDownCell.columnId))\n            return;\n        if (stringifyId(cell.rowId) !== stringifyId(mouseDownCell.rowId))\n            return;\n\n        const column = context.state.columnLookup.get(stringifyId(cell.columnId));\n        const row = context.state.rowLookup.get(stringifyId(cell.rowId));\n        const sortBy = context.state.options.sortBy;\n        const formatResolver = context.state.inputFormatResolver;\n        const cellData = formatResolver.resolve(row, column);\n\n        if (cellData.edit?.toggle) {\n            const edition = context.state.edition;\n            const newValue = getToggledValue(cellData, column, row, edition);\n            const cellType = getCellEditType(column, row);\n            if (cellType === 'DATA')\n                context.state.options.onEditedCellsChange(getCombinedCells(context.state.options.editedCells, [{ ...cell, value: newValue }]));\n            if (cellType === 'FILTER')\n                context.state.options.onFiltersChange(getCombinedCells(context.state.options.filters, [{ ...cell, expression: newValue }]));\n        } else if (column.type === 'DATA' && row.type === 'DATA') {\n            context.state.options.onCellClick(context.state.hoveredCell);\n        } else if (column.type === 'CUSTOM' || row.type === 'CUSTOM') {\n            context.state.options.onCustomCellClick(context.state.hoveredCell);\n        } else if (column.type === 'HEADER' || row.type === 'HEADER') {\n            const newSortBy = getNewSortBy(sortBy, column, row, event.ctrlKey);\n            context.state.options.onSortByChange(newSortBy);\n            context.state.options.onSelectedCellsChange([]);\n        }\n    });\n\n    context.addEventListener(element, 'dblclick', (event) => {\n        updateState(context);\n\n        if (context.state.resizableColumn) {\n            const resizableColumnKey = stringifyId(context.state.resizableColumn);\n            const newColumnWidths = context.state.options.columnWidths.filter(columnWidth => stringifyId(columnWidth.columnId) !== resizableColumnKey);\n            context.state.options.onColumnWidthsChange(newColumnWidths);\n            context.columnWidthCache.delete(resizableColumnKey);\n        }\n        if (context.state.resizableRow) {\n            const resizableRowKey = stringifyId(context.state.resizableRow);\n            const newRowHeights = context.state.options.rowHeights.filter(rowHeight => stringifyId(rowHeight.rowId) !== resizableRowKey);\n            context.state.options.onRowHeightsChange(newRowHeights);\n            context.rowHeightCache.delete(resizableRowKey);\n        }\n\n        const focusedCell = context.state.focusedCell;\n        if (focusedCell === null)\n            return;\n\n        const focusedColumnKey = stringifyId(focusedCell.columnId);\n        const focusedRowKey = stringifyId(focusedCell.rowId);\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const formatResolver = context.state.inputFormatResolver;\n\n        if (!columnLookup.has(focusedColumnKey))\n            return;\n        if (!rowLookup.has(focusedRowKey))\n            return;\n\n        const column = columnLookup.get(focusedColumnKey);\n        const row = rowLookup.get(focusedRowKey);\n        const cell = formatResolver.resolve(row, column);\n        const text = cell.text; // TODO: Make it configurable\n\n        if (!cell.edit)\n            return;\n        if (cell.edit.toggle)\n            return;\n\n        setText(text);\n        input?.select();\n    });\n\n    context.addEventListener(element, 'focus', () => {\n        if (input.parentElement)\n            input.focus({ preventScroll: true });\n    });\n\n    context.addEventListener(element, 'keydown', (event) => {\n        // TODO: make sure it's not invoked on keydown of the input\n        updateState(context);\n\n        const focusedCell = context.state.focusedCell;\n        const columnLookup = context.state.columnLookup;\n        const rowLookup = context.state.rowLookup;\n        const selectedCells = context.state.options.selectedCells;\n        const setSelectedCells = context.state.options.onSelectedCellsChange;\n        const addSelectedCells = (cells) => setSelectedCells(getCombinedCells(selectedCells, cells));\n        const setFocusedCell = context.state.options.onFocusedCellChange;\n        const editedCells = context.state.options.editedCells;\n        const setEditedCells = context.state.options.onEditedCellsChange;\n        const columns = context.state.columns;\n        const rows = context.state.rows;\n        const text = context.state.text;\n        const inputFormatResolver = context.state.inputFormatResolver;\n\n        const arrowTo = (cell, event) => {\n            setFocusedCell(cell);\n\n            if (event.shiftKey)\n                addSelectedCells([cell]);\n            else\n                setSelectedCells([cell]);\n        };\n\n        const arrowHorizontally = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedColumnKey = stringifyId(focusedCell.columnId);\n            if (!columnLookup.has(focusedColumnKey))\n                return;\n\n            const focusedColumnIndex = columnLookup.get(focusedColumnKey).index;\n            const newColumnIndex = Math.max(0, Math.min(columns.length - 1, focusedColumnIndex + offset));\n            if (newColumnIndex === focusedColumnIndex)\n                return;\n\n            const newFocusedCell = { rowId: focusedCell.rowId, columnId: columns[newColumnIndex].id };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const arrowVertically = (offset, event) => {\n            if (!focusedCell)\n                return;\n\n            const focusedRowKey = stringifyId(focusedCell.rowId);\n            if (!rowLookup.has(focusedRowKey))\n                return;\n\n            const focusedRowIndex = rowLookup.get(focusedRowKey).index;\n            const newRowIndex = Math.max(0, Math.min(rows.length - 1, focusedRowIndex + offset));\n            if (newRowIndex === focusedRowIndex)\n                return;\n\n            const newFocusedCell = { rowId: rows[newRowIndex].id, columnId: focusedCell.columnId };\n\n            arrowTo(newFocusedCell, event);\n        }\n\n        const preventDefault = () => {\n            event.preventDefault();\n            event.stopPropagation();\n        };\n\n        const cancel = () => {\n            if (text !== '') {\n                setText('');\n            }\n            else if (selectedCells.length > 1) {\n                setSelectedCells([focusedCell]);\n            }\n            else if (editedCells.length > 0) {\n                setEditedCells([]);\n            }\n            else {\n                setFocusedCell(null);\n                setSelectedCells([]);\n            }\n        };\n\n        const copyToClipboard = (event) => {\n            if (!event.ctrlKey)\n                return;\n\n            const clipboardData = getClipboardData(selectedCells, columns, rows, inputFormatResolver);\n\n            if (navigator.clipboard) {\n                navigator.clipboard.writeText(clipboardData);\n            } else {\n                const textArea = document.createElement('textarea');\n                textArea.value = clipboardData;\n                document.body.appendChild(textArea);\n                textArea.select();\n                document.execCommand('copy');\n                document.body.removeChild(textArea);\n            }\n        }\n\n        switch (event.key) {\n            case 'Escape':\n                cancel();\n                break;\n            case 'Enter':\n                accept();\n                break;\n            case 'ArrowUp':\n                // TODO: When ctrl and shift are pressed together, select all cells between the focused cell and the new cell\n                // TODO: When shift is pressed, expand the current rect selection instead of moving the focused cell\n                preventDefault();\n                arrowVertically(event.ctrlKey ? -rows.length : -1, event);\n                break;\n            case 'ArrowDown':\n                preventDefault();\n                arrowVertically(event.ctrlKey ? rows.length : 1, event);\n                break;\n            case 'ArrowLeft':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? -columns.length : -1, event);\n                break;\n            case 'ArrowRight':\n                preventDefault();\n                arrowHorizontally(event.ctrlKey ? columns.length : 1, event);\n                break;\n            case 'Delete':\n            case 'Backspace':\n                clear();\n                break;\n            case 'c':\n                copyToClipboard(event);\n                break;\n            default:\n                break;\n        }\n    });\n\n    new ResizeObserver(() => {\n        context.requestNewRender();\n    }).observe(element);\n\n    context.addEventListener(input, 'input', (event) => {\n        // TODO: check performance of this (if it's ok to update the state on every input event)\n        updateState(context);\n\n        if (event.target.value) {\n            accept(true);\n\n            input.style.opacity = 1;\n            input.style.pointerEvents = 'auto';\n        }\n        else {\n            if (event.isTrusted)\n                clear(true);\n\n            input.style.opacity = 0;\n            input.style.pointerEvents = 'none';\n        }\n    });\n\n    context.addEventListener(input, 'click', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'dblclick', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'mousedown', (event) => {\n        event.stopPropagation();\n    });\n\n    context.addEventListener(input, 'keydown', (event) => {\n        switch (event.key) {\n            case 'Enter':\n            case 'Escape':\n                break;\n            case 'Delete':\n            case 'Backspace':\n            case 'ArrowUp':\n            case 'ArrowDown':\n            case 'ArrowLeft':\n            case 'ArrowRight':\n                if (input.value !== '') {\n                    event.stopPropagation();\n                    context.requestNewRender();\n                }\n                break;\n            default:\n                event.stopPropagation();\n                // TODO: maybe only check if the new text is valid\n                context.requestNewRender();\n                break;\n        }\n    });\n}\n\nexport default function createGrid(element, options) {\n    console.log('createGrid');\n\n    initialize(element);\n\n    const context = element['spread-grid-context'];\n    context.externalOptions = options;\n\n    if (context.state === null) {\n        updateState(context);\n        // TODO: only render if the state has sufficiently changed\n        render(context);\n    }\n    else {\n        context.requestNewRender();\n    }\n}",
         "export default function getToggledValue(cell, column, row, edition) {\n    const value = edition.hasValueByKey(row.key, column.key)\n        ? edition.getValueByKey(row.key, column.key)\n        : cell.value;\n    const toggle = cell.edit.toggle;\n\n    if (typeof toggle === 'function')\n        return toggle({value}); // TODO: expand by context\n\n    return toggle[(toggle.indexOf(value) + 1) % toggle.length];\n}",
-        "import stringifyId from '../core-utils/stringifyId.js';\n\nexport default function getNewSortBy(sortBy, column, row, ctrlKey) {\n    // TODO: better support for multi-row sorting\n\n    function isCurrentRule(rule) {\n        return column.key === stringifyId(rule.columnId || 'HEADER') && row.key === stringifyId(rule.rowId || 'HEADER');\n    }\n\n    const directionLoop = ['ASC', 'DESC', undefined];\n    const currentRule = sortBy.find(isCurrentRule);\n    const directionIndex = directionLoop.indexOf(currentRule?.direction);\n    const newDirection = directionLoop[(directionIndex + 1) % directionLoop.length];\n    const isLastRule = sortBy.indexOf(currentRule) === sortBy.length - 1;\n    const shouldKeepOld = ctrlKey && (isLastRule || !currentRule);\n    const rulesToKeep = shouldKeepOld ? sortBy.filter(rule => !isCurrentRule(rule)) : [];\n    const newRules = newDirection ? [{ columnId: column.id, rowId: row.id, direction: newDirection }] : [];\n\n    return [...rulesToKeep, ...newRules];\n}",
+        "import stringifyId from '../core-utils/stringifyId.js';\n\nexport default function getNewSortBy(sortBy, column, row, ctrlKey) {\n    // TODO: better support for multi-row sorting\n\n    function isCurrentRule(rule) {\n        const columnId = 'columnId' in rule ? rule.columnId : 'HEADER';\n        const rowId = 'rowId' in rule ? rule.rowId : 'HEADER';\n\n        return column.key === stringifyId(columnId) && row.key === stringifyId(rowId);\n    }\n\n    function isConflictingWithCurrentRule(rule) {\n        const columnId = 'columnId' in rule ? rule.columnId : 'HEADER';\n        const rowId = 'rowId' in rule ? rule.rowId : 'HEADER';\n\n        return column.type === 'HEADER' && column.key === stringifyId(columnId)\n            || row.type === 'HEADER' && row.key === stringifyId(rowId);\n    }\n\n    const directionLoop = ['ASC', 'DESC', undefined];\n    const currentRule = sortBy.find(isCurrentRule);\n    const directionIndex = directionLoop.indexOf(currentRule?.direction);\n    const newDirection = directionLoop[(directionIndex + 1) % directionLoop.length];\n    const isLastRule = sortBy.indexOf(currentRule) === sortBy.length - 1;\n    const shouldKeepOld = ctrlKey && (isLastRule || !currentRule);\n    const rulesToKeep = shouldKeepOld\n        ? sortBy.filter(rule => !isCurrentRule(rule))\n        : sortBy.filter(rule => !isConflictingWithCurrentRule(rule));\n    const newRules = newDirection ? [{ columnId: column.id, rowId: row.id, direction: newDirection }] : [];\n\n    return [...rulesToKeep, ...newRules];\n}",
         "import stringifyId from \"../core-utils/stringifyId.js\";\nimport Selection from \"../types/Selection.js\";\n\nexport default function getClipboardData(selectedCells, columns, rows, formatResolver) {\n    const columnLookup = new Map(columns.map(column => [column.key, column]));\n    const rowLookup = new Map(rows.map(row => [row.key, row]));\n    const selectedCellKeys = selectedCells.map(cell => ({\n        columnKey: stringifyId(cell.columnId),\n        rowKey: stringifyId(cell.rowId)\n    })).filter(cell => columnLookup.has(cell.columnKey) && rowLookup.has(cell.rowKey));\n    const selectedColumns = new Set(selectedCellKeys.map(cell => cell.columnKey));\n    const selectedRows = new Set(selectedCellKeys.map(cell => cell.rowKey));\n\n    if (selectedCellKeys.length === 0)\n        return '';\n\n    const selection = new Selection(selectedCells);\n    const minColumnIndex = Math.min(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const maxColumnIndex = Math.max(...selectedCellKeys.map(cell => columnLookup.get(cell.columnKey).index));\n    const minRowIndex = Math.min(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n    const maxRowIndex = Math.max(...selectedCellKeys.map(cell => rowLookup.get(cell.rowKey).index));\n\n    const stringBuilder = [];\n\n    for (let rowIndex = minRowIndex; rowIndex <= maxRowIndex; rowIndex++) {\n        const row = rows[rowIndex];\n        const rowKey = row.key;\n\n        if (!selectedRows.has(rowKey))\n            continue;\n\n        for (let columnIndex = minColumnIndex; columnIndex <= maxColumnIndex; columnIndex++) {\n            const column = columns[columnIndex];\n            const columnKey = column.key;\n\n            if (!selectedColumns.has(columnKey))\n                continue;\n\n            if (selection.isKeySelected(rowKey, columnKey)) {\n                const cellData = formatResolver.resolve(row, column).text;\n                stringBuilder.push(cellData);\n            }\n\n            if (columnIndex < maxColumnIndex)\n                stringBuilder.push('\\t');\n        }\n\n        if (rowIndex < maxRowIndex)\n            stringBuilder.push('\\n');\n    }\n\n    return stringBuilder.join('');\n}",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\t// no module.id needed\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_9m1712685293\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_1m1716626761\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n"
     ],
     "version": 3
 }
```

### Comparing `dash_spread_grid-0.0.9/dash_spread_grid/metadata.json` & `dash_spread_grid-0.1.1/dash_spread_grid/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'src/lib/components/DashSpreadGrid.jsx'": "{'props': {'data_selector': OrderedDict([('type', "*

 * *                                            "OrderedDict([('name', 'string')])), ('required', "*

 * *                                            "False), ('description', ''), ('defaultValue', "*

 * *                                            "OrderedDict([('value', "*

 * *                                            '\'"data[row.id][column.id]"\'), (\'computed\', '*

 * *                                            "False)]))]), 'sel […]*

```diff
@@ -88,26 +88,26 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "any"
                 }
             },
-            "dataSelector": {
+            "data_selector": {
                 "defaultValue": {
                     "computed": false,
                     "value": "\"data[row.id][column.id]\""
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "string"
                 }
             },
-            "editedCells": {
+            "edited_cells": {
                 "defaultValue": {
                     "computed": false,
                     "value": "[]"
                 },
                 "description": "",
                 "required": false,
                 "type": {
@@ -238,15 +238,15 @@
                 },
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "array"
                 }
             },
-            "selectedCells": {
+            "selected_cells": {
                 "defaultValue": {
                     "computed": false,
                     "value": "[]"
                 },
                 "description": "",
                 "required": false,
                 "type": {
@@ -256,15 +256,15 @@
             "setProps": {
                 "description": "",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
-            "sortBy": {
+            "sort_by": {
                 "defaultValue": {
                     "computed": false,
                     "value": "[]"
                 },
                 "description": "",
                 "required": false,
                 "type": {
```

### Comparing `dash_spread_grid-0.0.9/dash_spread_grid/package-info.json` & `dash_spread_grid-0.1.1/dash_spread_grid/package-info.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9017857142857143%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/TomaszRewak/js-spread-grid/issues'}",*

 * * "'homepage'": "'https://spread-grid.tomasz-rewak.com'",*

 * * "'repository'": "{'url': 'https://github.com/TomaszRewak/js-spread-grid.git'}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "author": "Tomasz Rewak <tomasz.rewak@gmail.com>",
     "bugs": {
-        "url": "https://github.com/https://github.com/TomaszRewak/js-spread-grid/dash-spread-grid/issues"
+        "url": "https://github.com/TomaszRewak/js-spread-grid/issues"
     },
     "dependencies": {
         "js-spread-grid": "file:../lib",
         "ramda": "^0.26.1"
     },
     "description": "Fast grid for Dash applications",
     "devDependencies": {
@@ -34,34 +34,34 @@
         "webpack-cli": "^5.1.1",
         "webpack-dev-server": "^4.15.0"
     },
     "engines": {
         "node": ">=8.11.0",
         "npm": ">=6.1.0"
     },
-    "homepage": "https://github.com/https://github.com/TomaszRewak/js-spread-grid/dash-spread-grid",
+    "homepage": "https://spread-grid.tomasz-rewak.com",
     "license": "MIT",
     "main": "build/index.js",
     "name": "dash_spread_grid",
     "repository": {
         "type": "git",
-        "url": "git://github.com/https://github.com/TomaszRewak/js-spread-grid/dash-spread-grid.git"
+        "url": "https://github.com/TomaszRewak/js-spread-grid.git"
     },
     "scripts": {
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components dash_spread_grid -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.0.9",
+    "version": "0.1.1",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

### Comparing `dash_spread_grid-0.0.9/package.json` & `dash_spread_grid-0.1.1/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9017857142857143%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/TomaszRewak/js-spread-grid/issues'}",*

 * * "'homepage'": "'https://spread-grid.tomasz-rewak.com'",*

 * * "'repository'": "{'url': 'https://github.com/TomaszRewak/js-spread-grid.git'}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "author": "Tomasz Rewak <tomasz.rewak@gmail.com>",
     "bugs": {
-        "url": "https://github.com/https://github.com/TomaszRewak/js-spread-grid/dash-spread-grid/issues"
+        "url": "https://github.com/TomaszRewak/js-spread-grid/issues"
     },
     "dependencies": {
         "js-spread-grid": "file:../lib",
         "ramda": "^0.26.1"
     },
     "description": "Fast grid for Dash applications",
     "devDependencies": {
@@ -34,34 +34,34 @@
         "webpack-cli": "^5.1.1",
         "webpack-dev-server": "^4.15.0"
     },
     "engines": {
         "node": ">=8.11.0",
         "npm": ">=6.1.0"
     },
-    "homepage": "https://github.com/https://github.com/TomaszRewak/js-spread-grid/dash-spread-grid",
+    "homepage": "https://spread-grid.tomasz-rewak.com",
     "license": "MIT",
     "main": "build/index.js",
     "name": "dash_spread_grid",
     "repository": {
         "type": "git",
-        "url": "git://github.com/https://github.com/TomaszRewak/js-spread-grid/dash-spread-grid.git"
+        "url": "https://github.com/TomaszRewak/js-spread-grid.git"
     },
     "scripts": {
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components dash_spread_grid -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py",
         "watch": "npm-watch"
     },
-    "version": "0.0.9",
+    "version": "0.1.1",
     "watch": {
         "build": {
             "patterns": [
                 "../lib/**/*",
                 "./src/lib/**/*"
             ]
         }
```

