# Comparing `tmp/nicegui_tabulator-0.1.2.tar.gz` & `tmp/nicegui_tabulator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicegui_tabulator-0.1.2.tar", max compression
+gzip compressed data, was "nicegui_tabulator-0.1.3.tar", max compression
```

## Comparing `nicegui_tabulator-0.1.2.tar` & `nicegui_tabulator-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     1094 2024-05-08 17:39:27.737805 nicegui_tabulator-0.1.2/LICENSE
--rw-r--r--   0        0        0      128 2024-05-08 14:53:27.237225 nicegui_tabulator-0.1.2/nicegui_tabulator/__init__.py
--rw-r--r--   0        0        0      298 2024-05-08 17:33:19.252414 nicegui_tabulator-0.1.2/nicegui_tabulator/core/events.py
--rw-r--r--   0        0        0    33593 2024-05-08 15:00:49.017552 nicegui_tabulator-0.1.2/nicegui_tabulator/core/libs/tabulator.min.css
--rw-r--r--   0        0        0   484963 2024-05-08 15:01:02.793045 nicegui_tabulator-0.1.2/nicegui_tabulator/core/libs/tabulator.min.js
--rw-r--r--   0        0        0     2698 2024-05-15 07:17:16.265715 nicegui_tabulator-0.1.2/nicegui_tabulator/core/tabulator.js
--rw-r--r--   0        0        0     6796 2024-05-15 07:34:12.484761 nicegui_tabulator-0.1.2/nicegui_tabulator/core/tabulator.py
--rw-r--r--   0        0        0      824 2024-05-15 07:23:00.814564 nicegui_tabulator-0.1.2/nicegui_tabulator/core/utils.py
--rw-r--r--   0        0        0       97 2024-05-08 14:40:20.875090 nicegui_tabulator-0.1.2/nicegui_tabulator/version.py
--rw-r--r--   0        0        0      584 2024-05-15 07:36:27.229719 nicegui_tabulator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2411 2024-05-15 07:17:14.855234 nicegui_tabulator-0.1.2/README.md
--rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 nicegui_tabulator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-08 17:39:27.737805 nicegui_tabulator-0.1.3/LICENSE
+-rw-r--r--   0        0        0      184 2024-05-25 11:11:37.557614 nicegui_tabulator-0.1.3/nicegui_tabulator/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-08 17:33:19.252414 nicegui_tabulator-0.1.3/nicegui_tabulator/core/events.py
+-rw-r--r--   0        0        0    33593 2024-05-08 15:00:49.017552 nicegui_tabulator-0.1.3/nicegui_tabulator/core/libs/tabulator.min.css
+-rw-r--r--   0        0        0   484963 2024-05-08 15:01:02.793045 nicegui_tabulator-0.1.3/nicegui_tabulator/core/libs/tabulator.min.js
+-rw-r--r--   0        0        0     3101 2024-05-25 11:11:37.567812 nicegui_tabulator-0.1.3/nicegui_tabulator/core/tabulator.js
+-rw-r--r--   0        0        0    12832 2024-05-25 16:01:18.529668 nicegui_tabulator-0.1.3/nicegui_tabulator/core/tabulator.py
+-rw-r--r--   0        0        0      247 2024-05-25 11:11:37.578058 nicegui_tabulator-0.1.3/nicegui_tabulator/core/teleport.js
+-rw-r--r--   0        0        0      306 2024-05-25 11:11:37.578058 nicegui_tabulator-0.1.3/nicegui_tabulator/core/teleport.py
+-rw-r--r--   0        0        0      531 2024-05-25 11:11:37.578058 nicegui_tabulator-0.1.3/nicegui_tabulator/core/types.py
+-rw-r--r--   0        0        0      824 2024-05-21 02:05:10.120626 nicegui_tabulator-0.1.3/nicegui_tabulator/core/utils.py
+-rw-r--r--   0        0        0       97 2024-05-08 14:40:20.875090 nicegui_tabulator-0.1.3/nicegui_tabulator/version.py
+-rw-r--r--   0        0        0      584 2024-05-25 16:31:06.124306 nicegui_tabulator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4382 2024-05-25 16:30:32.734617 nicegui_tabulator-0.1.3/README.md
+-rw-r--r--   0        0        0     4885 1970-01-01 00:00:00.000000 nicegui_tabulator-0.1.3/PKG-INFO
```

### Comparing `nicegui_tabulator-0.1.2/LICENSE` & `nicegui_tabulator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.2/nicegui_tabulator/core/libs/tabulator.min.css` & `nicegui_tabulator-0.1.3/nicegui_tabulator/core/libs/tabulator.min.css`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.2/nicegui_tabulator/core/libs/tabulator.min.js` & `nicegui_tabulator-0.1.3/nicegui_tabulator/core/libs/tabulator.min.js`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.2/nicegui_tabulator/core/tabulator.js` & `nicegui_tabulator-0.1.3/nicegui_tabulator/core/tabulator.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -2,14 +2,19 @@
     loadResource
 } from "../../static/utils/resources.js";
 import {
     convertDynamicProperties
 } from "../../static/utils/dynamic_properties.js";
 
 
+const completedEvents = new Set([
+    'tableBuilding',
+    'tableBuilt',
+]);
+
 const eventArgsExtractor = new Map([
     ['dataFiltering', filters => ({
         filters
     })],
     ['dataFiltered', (filters, rows) => ({
         filters,
         rows: rows.map(row => row.getData())
@@ -74,25 +79,29 @@
         await this.$nextTick(); // NOTE: wait for window.path_prefix to be set
         await Promise.all([
             loadResource(window.path_prefix + `${this.resource_path}/tabulator.min.css`),
         ]);
 
         convertDynamicProperties(this.options, true);
         this.table = new Tabulator(this.$el, this.options);
-
     },
 
     methods: {
         onEvent(eventName) {
-            this.table.on(eventName, (...args) => {
+            const orgEventName = eventName.replace(/^table:/, '');
+
+            // These events have already been completed at this moment
+            if (completedEvents.has(orgEventName)) {
+                this.$emit(eventName);
+                return;
+            }
+
+            this.table.on(orgEventName, (...args) => {
                 const eventArgs = extractEventArg(eventName, args);
-                this.$emit('table-event', {
-                    eventName,
-                    args: eventArgs
-                });
+                this.$emit(eventName, eventArgs);
 
                 if (eventName === 'rowContext' || eventName === 'groupContext') {
                     args[0].preventDefault();
                 }
             });
         },
         run_table_method(name, ...args) {
@@ -109,9 +118,17 @@
         },
 
         updateColumnDefinition(field, definition) {
             convertDynamicProperties(definition, true);
             this.table.updateColumnDefinition(field, definition);
         },
 
+        updateCellSlot(field, rowNumber) {
+            this.$emit('updateCellSlot', {
+                field,
+                rowNumber
+            })
+        },
+
+
     },
 };
```

### Comparing `nicegui_tabulator-0.1.2/nicegui_tabulator/core/utils.py` & `nicegui_tabulator-0.1.3/nicegui_tabulator/core/utils.py`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.2/pyproject.toml` & `nicegui_tabulator-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nicegui-tabulator"
-version = "0.1.2"
+version = "0.1.3"
 description = "This is a Python package that provides a simple way to create tables using the Tabulator library. It is built on top of the NiceGUI library."
 authors = ["CrystalWindSnake <568166495@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nicegui = "^1.4.24"
```

