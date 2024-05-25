# Comparing `tmp/citeman-0.1.tar.gz` & `tmp/citeman-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citeman-0.1.tar", last modified: Mon May  6 09:09:33 2024, max compression
+gzip compressed data, was "citeman-0.2.tar", last modified: Sat May 25 21:28:08 2024, max compression
```

## Comparing `citeman-0.1.tar` & `citeman-0.2.tar`

### file list

```diff
@@ -1,29 +1,43 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-06 09:09:33.321187 citeman-0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3298 2024-05-06 08:16:23.000000 citeman-0.1/.gitignore
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35148 2024-05-05 19:02:21.000000 citeman-0.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2423 2024-05-06 09:09:33.321187 citeman-0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1695 2024-05-06 08:14:29.000000 citeman-0.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1089 2024-05-06 09:07:17.000000 citeman-0.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-06 09:09:33.321187 citeman-0.1/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-06 09:09:33.317187 citeman-0.1/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-06 09:09:33.317187 citeman-0.1/src/citeman/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-05 18:20:04.000000 citeman-0.1/src/citeman/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       67 2024-05-06 06:35:49.000000 citeman-0.1/src/citeman/__main__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      462 2024-05-06 08:33:49.000000 citeman-0.1/src/citeman/bibliography.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3092 2024-05-06 07:19:09.000000 citeman-0.1/src/citeman/library.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4569 2024-05-05 19:50:31.000000 citeman-0.1/src/citeman/logo
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7522 2024-05-06 07:32:27.000000 citeman-0.1/src/citeman/processor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2882 2024-05-05 22:20:12.000000 citeman-0.1/src/citeman/query.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7396 2024-05-06 08:49:19.000000 citeman-0.1/src/citeman/ui.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       87 2024-05-06 06:35:49.000000 citeman-0.1/src/citeman/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-06 09:09:33.321187 citeman-0.1/src/citeman.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     2423 2024-05-06 09:09:33.000000 citeman-0.1/src/citeman.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2024-05-06 09:09:33.000000 citeman-0.1/src/citeman.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-06 09:09:33.000000 citeman-0.1/src/citeman.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       55 2024-05-06 09:09:33.000000 citeman-0.1/src/citeman.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2024-05-06 09:09:33.000000 citeman-0.1/src/citeman.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-06 09:09:33.321187 citeman-0.1/static/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   668097 2024-05-06 08:01:54.000000 citeman-0.1/static/citeman.gif
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   103324 2024-05-05 19:28:01.000000 citeman-0.1/static/logo.png
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    33119 2024-05-05 19:28:00.000000 citeman-0.1/static/logo.svg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12466 2024-05-05 19:50:51.000000 citeman-0.1/static/logo_ascii.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:28:08.913449 citeman-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:28:08.905449 citeman-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:28:08.905449 citeman-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-25 21:28:01.000000 citeman-0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-25 21:28:01.000000 citeman-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-25 21:28:01.000000 citeman-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-25 21:28:08.913449 citeman-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-25 21:28:01.000000 citeman-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-25 21:28:01.000000 citeman-0.2/RELEASE-NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-25 21:28:01.000000 citeman-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:28:08.913449 citeman-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:28:08.905449 citeman-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:28:08.909449 citeman-0.2/src/citeman/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/logo
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/ui_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/ui_notice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/ui_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/ui_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/ui_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/ui_show.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-25 21:28:01.000000 citeman-0.2/src/citeman/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:28:08.913449 citeman-0.2/src/citeman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-25 21:28:08.000000 citeman-0.2/src/citeman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-25 21:28:08.000000 citeman-0.2/src/citeman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:28:08.000000 citeman-0.2/src/citeman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-25 21:28:08.000000 citeman-0.2/src/citeman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 21:28:08.000000 citeman-0.2/src/citeman.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:28:08.913449 citeman-0.2/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   668097 2024-05-25 21:28:01.000000 citeman-0.2/static/citeman.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   103324 2024-05-25 21:28:01.000000 citeman-0.2/static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33119 2024-05-25 21:28:01.000000 citeman-0.2/static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-05-25 21:28:01.000000 citeman-0.2/static/logo_ascii.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:28:08.913449 citeman-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-25 21:28:01.000000 citeman-0.2/tests/test_utils.py
```

### Comparing `citeman-0.1/.gitignore` & `citeman-0.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Project-specific
+*.bib
+*.p
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `citeman-0.1/LICENSE` & `citeman-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citeman-0.1/PKG-INFO` & `citeman-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citeman
-Version: 0.1
+Version: 0.2
 Summary: A simple command line citation manager for your academic manuscript.
 Author-email: "Dylan Russell, MD" <dyl.russell@gmail.com>
 Maintainer-email: "Dylan Russell, MD" <dyl.russell@gmail.com>
 Project-URL: Homepage, https://github.com/dylanrussellmd/pycite
 Project-URL: Issues, https://github.com/dylanrussellmd/pycite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `citeman-0.1/README.md` & `citeman-0.2/README.md`

 * *Files identical despite different names*

### Comparing `citeman-0.1/pyproject.toml` & `citeman-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `citeman-0.1/src/citeman/library.py` & `citeman-0.2/src/citeman/entry.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+from typing import List
 from bibtexparser.splitter import Splitter
-from bibtexparser.model import Entry
+from bibtexparser.model import Entry, Field
+from bibtexparser.writer import BibtexFormat, VAL_SEP, _val_intent_string
 from bibtexparser.exceptions import BlockAbortedException, ParserStateException
 import logging
 import re
 
 # Overwriting bibtexparser.Splitter to return an Entry.
 class EntrySplitter(Splitter):
-    def __init__(self, bibstr: str):
-        super().__init__(bibstr)
 
     def split(self) -> Entry:      
 
         self._markiter = re.finditer(
             r"(?<!\\)[\{\}\",=\n]|@[\w]*( |\t)*(?={)", self.bibstr, re.MULTILINE
         )
 
@@ -73,8 +73,28 @@
 
         # Check if there's an implicit comment at the EOF
         if self._implicit_comment_start is not None:
             comment = self._end_implicit_comment(len(self.bibstr))
             if comment is not None:
                 pass
 
-        return entry
+        return entry
+
+# Taken from https://github.com/sciunto-org/python-bibtexparser/blob/main/bibtexparser/writer.py#L41
+# Modified slightly to use here without having to specify a bibtex_format as in the original and 
+# to return a concatenated string at the end.
+def getEntryRaw(block: Entry) -> List[str]:
+    res = ["@", block.entry_type, "{", block.key, ",\n"]
+    bibtex_format = BibtexFormat()
+    field: Field
+    for i, field in enumerate(block.fields):
+        res.append(bibtex_format.indent)
+        res.append(field.key)
+        res.append(_val_intent_string(bibtex_format, field.key))
+        res.append(VAL_SEP)
+        res.append(field.value)
+        if bibtex_format.trailing_comma or i < len(block.fields) - 1:
+            res.append(",")
+        res.append("\n")
+    res.append("}\n")
+    
+    return "".join(res)
```

### Comparing `citeman-0.1/src/citeman/logo` & `citeman-0.2/src/citeman/logo`

 * *Files identical despite different names*

### Comparing `citeman-0.1/src/citeman/processor.py` & `citeman-0.2/src/citeman/processor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from bibtexparser.model import DuplicateBlockKeyBlock
+from bibtexparser.model import DuplicateBlockKeyBlock, Field
+from bibtexparser.entrypoint import write_file
+from pickle import dump
+from .errors import CriticalFieldException, FieldExistsError, FieldMissingError, HistoryEmptyError, KeyExistsError, LibraryEmptyError
+from .entry import getEntryRaw
 from .query import CrossRef, Query
-from .bibliography import write
 from .utils import removeBraces
 
 class Processor():
     """
     A class that represents a processor for handling queries and managing a library.
     All interactions between the user and the Library/.bib file are handled by the Processor.
 
@@ -23,18 +26,37 @@
     """
 
     def __init__(self, library):
         """
         Initializes a Processor object with a library.
 
         Args:
-            library (Library): The library object that stores the blocks.
+            library (Library): The library object that stores the entries.
         """
         self.library = library
-        self.queryHistory = TypedList(Query) 
+        self._queryHistory = list()
+
+    @property
+    def entries(self):
+        if not self.library.entries:
+            raise LibraryEmptyError()
+        return self.library.entries
+
+    @property 
+    def queryHistory(self):
+        if not self._queryHistory:
+            raise HistoryEmptyError()
+        return self._queryHistory
+    
+    def overwriteLibrary(self, library):
+        self.library = library
+
+    def save(self):
+        with open('citeman.p', 'wb') as f:
+            dump(self, f)
 
     def processQuery(self, input):
         """
         Processes a query and adds it to the query history.
 
         Args:
             input (str): The article ID to query.
@@ -42,15 +64,15 @@
         Raises:
             Exception: If an error occurs while processing the query.
             Should only be raising unanticipated exceptions as most have been
             handled in the Query class.
         """
         try:
             query = CrossRef(input)
-            self.queryHistory.append(query)
+            self._queryHistory.append(query)
         except:
             raise
     
     def add(self, block) -> None:
         """
         Adds a block to the library and writes the library to .bib file.
 
@@ -58,82 +80,120 @@
             block (Block): The block to be added to the library.
         """
         try:
             self.library.add(block, fail_on_duplicate_key=True)
         except:
             raise
 
-        self.write()
+        self._write()
+        self.save()
 
     def remove(self, block) -> None:
         """
         Removes a block from the library and writes the library to .bib file.
 
         Args:
             block (Block): The block to be removed from the library.
         """
         self.library.remove(block)
-        self.write()
+        self._write()
+        self.save()
+
+    @staticmethod
+    def updateEntryRaw(block) -> None:
+        block._raw = getEntryRaw(block)
+
+    @staticmethod
+    def checkCriticalField(block, field):
+        try:
+            Processor.fieldMissing(block, field)
+        except:
+            raise CriticalFieldException(field)
+
+    @staticmethod
+    def updateField(block, field, value) -> None:
+        try:
+            Processor.fieldMissing(block, field)
+        except:
+            raise
+        
+        block.set_field(Field(field, value))
+        Processor.updateEntryRaw(block)
+
+    @staticmethod
+    def addField(block, field, value) -> None:
+        try:
+            Processor.fieldExists(block, field)
+        except:
+            raise
+
+        block.set_field(Field(field, value))
+        Processor.updateEntryRaw(block)
 
-    def write(self) -> None:
+    @staticmethod
+    def updateKey(block, key) -> None:
+        """
+        Changes the key of a block in the library.
+
+        Args:
+            block (Block): The block whose key is to be changed.
+            key (str): The new key to assign to the block.
+        """
+        block.key = key
+        block._raw = getEntryRaw(block)
+
+    def _write(self) -> None:
         """
         Writes the library to .bib file.
         """
-        write(self.library)
+        bib = 'bibliography.bib'
+        write_file(bib, self.library)
 
-    def compare(self, query):
+    def idExists(self, query):
         """
         Compares a given article ID with the library.
 
         Args:
             id (str): The article ID to compare.
 
         Returns:
             bool: True if the article ID is in the library, False otherwise.
         """
-        entries = self.library.entries
+        try:
+            entries = self.entries
+        except LibraryEmptyError:
+            return False
         type = query.type
         for entry in entries:
             id = removeBraces(entry.get(type).value)
             if id is not None and id == query.id:
                     return True
             else:
                 return False
-            
-    def incrementKey(self, block):
-        """
-        Increments the key of a block in the library to avoid duplicates.
-
-        Args:
-            key (str): The new key to assign to the block.
-        """
-        key_v = 1
-        new_key = block.key + f"_{key_v}"
-        while self._keyExists(new_key):
-            key_v += 1
-            new_key = block.key + f"_{key_v}"
-        block.key = new_key
-
-    def _keyExists(self, key):
-        """
-        Checks if a key already exists in the library.
-
-        Args:
-            key (str): The key to check.
-
-        Returns:
-            bool: True if the key exists in the library, False otherwise.
-        """
-        entries = self.library.entries
+    
+    def keyExists(self, key):
+        try:
+            entries = self.entries
+        except LibraryEmptyError:
+            return
         for entry in entries:
             if entry.key == key:
-                return True
-            else:
-                return False
-            
+                raise KeyExistsError(key)
+    
+    @staticmethod
+    def fieldExists(block, field):
+        if block.get(field) is not None:
+            raise FieldExistsError(field)
+    
+    @staticmethod
+    def fieldMissing(block, field):
+        if block.get(field) is None:
+            raise FieldMissingError(field)
+    
+    # MIGHT NOT BE NEEDED
     def removeDuplicateBlocks(self):
         """
         Removes duplicate blocks from the library.
         """
         duplicates = [block for block in self.library.blocks if isinstance(block, DuplicateBlockKeyBlock)]
         self.library.remove(duplicates)
 
@@ -152,82 +212,8 @@
     def getLastQuery(self) -> Query:
         """
         Retrieves the last query from the query history.
 
         Returns:
             Query: The last query object in the query history.
         """
-        return self.getQuery(-1)
-    
-class TypedList(list):
-    """
-    A typed list that enforces a specific element type.
-
-    Attributes:
-        element_type (type): The type of elements allowed in the list.
-
-    Methods:
-        __init__(self, element_type, initial_list): Initializes a TypedList object with an element type and an initial list.
-        _validate(self, element): Validates if an element is of the correct type.
-        append(self, element): Appends an element to the list after validating its type.
-        insert(self, index, element): Inserts an element into the list at a specific index after validating its type.
-        extend(self, iterable): Extends the list with elements from an iterable after validating their types.
-    """
-
-    def __init__(self, element_type, initial_list=None):
-        """
-        Initializes a TypedList object with an element type and an initial list.
-
-        Args:
-            element_type (type): The type of elements allowed in the list.
-            initial_list (list, optional): An initial list to populate the TypedList with. Defaults to None.
-        """
-        self.element_type = element_type
-        if initial_list:
-            for element in initial_list:
-                self._validate(element)
-                super().append(element)
-
-    def _validate(self, element):
-        """
-        Validates if an element is of the correct type.
-
-        Args:
-            element: The element to be validated.
-
-        Raises:
-            TypeError: If the element is not of the correct type.
-        """
-        if not isinstance(element, self.element_type):
-            raise TypeError(f"Only {self.element_type.__name__} elements are allowed")
-
-    def append(self, element):
-        """
-        Appends an element to the list after validating its type.
-
-        Args:
-            element: The element to be appended.
-        """
-        self._validate(element)
-        super().append(element)
-
-    def insert(self, index, element):
-        """
-        Inserts an element into the list at a specific index after validating its type.
-
-        Args:
-            index (int): The index at which to insert the element.
-            element: The element to be inserted.
-        """
-        self._validate(element)
-        super().insert(index, element)
-
-    def extend(self, iterable):
-        """
-        Extends the list with elements from an iterable after validating their types.
-
-        Args:
-            iterable (iterable): The iterable containing elements to be added to the list.
-        """
-        for element in iterable:
-            self._validate(element)
-        super().extend(iterable)
+        return self.getQuery(-1)
```

### Comparing `citeman-0.1/src/citeman/query.py` & `citeman-0.2/src/citeman/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABCMeta, abstractmethod
 from enum import Enum
 from typing import Type
 from habanero import cn
 from requests import HTTPError
-from .library import EntrySplitter
+from .entry import EntrySplitter, getEntryRaw
 import re
 import warnings
 import six
 
 # When working with `venv`, to get pylance to work:
 # You have to choose the correct interpreter.
 # Use shortcuts "Ctrl+Shift+P" and type "Python: Select Interperter" to choose the venv.
@@ -15,29 +15,30 @@
 @six.add_metaclass(ABCMeta)
 class Query:
     def __init__(self, id: Type[str]) -> None:
         self.success = True
         self.id = self._handleId(id)
         self.type = self._handleType()
         self.result = self._handleResult()
-        self.block = self._handleBlock() 
+        self.block = self._handleBlock()
+        self.raw = self._handleRaw()
+        self.block._raw = self._handleEntryRaw()
 
     def _fail(self, result):
         self.success = False
         self.result = result
 
     def _handleId(self, id):
         try:
             return self._id(id)
         except TypeError as e:
             self._fail(e)
         return None
 
-    @staticmethod
-    def _id(id):
+    def _id(self, id):
         if isinstance(id, str):
             return id
         elif isinstance(id, list) and all(isinstance(i, str) for i in id):
             warnings.warn("ID is a list of strings. Using the first element.")
             return id[0]
         else:
             raise TypeError("ID must be a string or a list of strings")
@@ -47,18 +48,17 @@
             return None
         try:
             return self._type(self.id)
         except ValueError as e:
             self._fail(e)
         return None
 
-    @staticmethod
-    def _type(id):
+    def _type(self, id):
         for reid in ReID:
-            if re.match(reid.value, id, flags=re.I):
+            if bool(re.search(reid.value, id, flags=re.I)):
                 return reid.name
         raise ValueError("ID is not a valid article identifier")
 
     def _handleResult(self):
         if not self.success:
             return self.result
         try:
@@ -76,29 +76,33 @@
 
     @abstractmethod
     def _result(id):
         pass
 
     def _handleBlock(self):
         if self.success:
-           block = EntrySplitter(self.result).split()
-           self.result = f"Found {self.type} {self.id}"
-           return block
+            block = EntrySplitter(self.result).split()
+            self.result = f"Found {self.type} {self.id}"
+            return block
+        return None
+    
+    def _handleRaw(self):
+        if self.success and self.block is not None:
+            return self.block._raw
         return None
 
+    def _handleEntryRaw(self):
+        if self.success and self.raw is not None:
+            return getEntryRaw(self.block)
+
 class ReID(Enum):
-    DOI = r"^10\.\d{4,9}\/[-._;()/:A-Z0-9]+$"
+    DOI = r"10\.\d{4,9}\/[-._;()/:A-Z0-9]+$"
     PMID = r"^\d+$"
 
-# https://www.crossref.org/blog/dois-and-matching-regular-expressions/
-# Need to review to learn and consolidate.
-# When to use static methods?
-
-# consider allowing different urls/formats for cn.contentnegotiation
 class CrossRef(Query):
-
+   
     @staticmethod
     def _result(id):
         try:
             return cn.content_negotiation(id, format='bibtex', url="https://doi.org")
         except:
             raise
```

### Comparing `citeman-0.1/src/citeman.egg-info/PKG-INFO` & `citeman-0.2/src/citeman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citeman
-Version: 0.1
+Version: 0.2
 Summary: A simple command line citation manager for your academic manuscript.
 Author-email: "Dylan Russell, MD" <dyl.russell@gmail.com>
 Maintainer-email: "Dylan Russell, MD" <dyl.russell@gmail.com>
 Project-URL: Homepage, https://github.com/dylanrussellmd/pycite
 Project-URL: Issues, https://github.com/dylanrussellmd/pycite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `citeman-0.1/static/citeman.gif` & `citeman-0.2/static/citeman.gif`

 * *Files identical despite different names*

### Comparing `citeman-0.1/static/logo.png` & `citeman-0.2/static/logo.png`

 * *Files identical despite different names*

### Comparing `citeman-0.1/static/logo.svg` & `citeman-0.2/static/logo.svg`

 * *Files identical despite different names*

### Comparing `citeman-0.1/static/logo_ascii.svg` & `citeman-0.2/static/logo_ascii.svg`

 * *Files identical despite different names*

