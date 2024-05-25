# Comparing `tmp/pyfancytranslator-1.0.6.tar.gz` & `tmp/pyfancytranslator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfancytranslator-1.0.6.tar", last modified: Fri May 17 14:26:27 2024, max compression
+gzip compressed data, was "pyfancytranslator-1.1.0.tar", last modified: Fri May 24 19:50:43 2024, max compression
```

## Comparing `pyfancytranslator-1.0.6.tar` & `pyfancytranslator-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 14:26:27.477558 pyfancytranslator-1.0.6/
-drwxrwxrwx   0        0        0        0 2024-05-17 14:26:27.469076 pyfancytranslator-1.0.6/FancyTranslator/
--rw-rw-rw-   0        0        0      175 2024-05-04 12:18:43.000000 pyfancytranslator-1.0.6/FancyTranslator/__init__.py
--rw-rw-rw-   0        0        0     6412 2024-05-17 14:26:15.000000 pyfancytranslator-1.0.6/FancyTranslator/classes.py
--rw-rw-rw-   0        0        0     2596 2024-05-17 14:26:27.476553 pyfancytranslator-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2001 2024-05-03 13:55:21.000000 pyfancytranslator-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 14:26:27.475059 pyfancytranslator-1.0.6/pyfancytranslator.egg-info/
--rw-rw-rw-   0        0        0     2596 2024-05-17 14:26:27.000000 pyfancytranslator-1.0.6/pyfancytranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-17 14:26:27.000000 pyfancytranslator-1.0.6/pyfancytranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 14:26:27.000000 pyfancytranslator-1.0.6/pyfancytranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-17 14:26:27.000000 pyfancytranslator-1.0.6/pyfancytranslator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      716 2024-05-17 14:26:15.000000 pyfancytranslator-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 14:26:27.477558 pyfancytranslator-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:50:43.508242 pyfancytranslator-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-24 19:50:43.495051 pyfancytranslator-1.1.0/FancyTranslator/
+-rw-rw-rw-   0        0        0      233 2024-05-23 14:10:09.000000 pyfancytranslator-1.1.0/FancyTranslator/__init__.py
+-rw-rw-rw-   0        0        0     6190 2024-05-24 19:49:22.000000 pyfancytranslator-1.1.0/FancyTranslator/classes.py
+-rw-rw-rw-   0        0        0     3438 2024-05-24 19:49:22.000000 pyfancytranslator-1.1.0/FancyTranslator/methods.py
+-rw-rw-rw-   0        0        0     2596 2024-05-24 19:50:43.507244 pyfancytranslator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2001 2024-05-03 13:55:21.000000 pyfancytranslator-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 19:50:43.505249 pyfancytranslator-1.1.0/pyfancytranslator.egg-info/
+-rw-rw-rw-   0        0        0     2596 2024-05-24 19:50:43.000000 pyfancytranslator-1.1.0/pyfancytranslator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-24 19:50:43.000000 pyfancytranslator-1.1.0/pyfancytranslator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 19:50:43.000000 pyfancytranslator-1.1.0/pyfancytranslator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-24 19:50:43.000000 pyfancytranslator-1.1.0/pyfancytranslator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      716 2024-05-23 14:10:09.000000 pyfancytranslator-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 19:50:43.508242 pyfancytranslator-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-05-03 13:27:10.000000 pyfancytranslator-1.1.0/setup.py
```

### Comparing `pyfancytranslator-1.0.6/FancyTranslator/classes.py` & `pyfancytranslator-1.1.0/FancyTranslator/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import os
 import re
 from configparser import ConfigParser
 from typing import Optional, Type, TypeVar, Union
 
+from FancyTranslator.methods import handle_placeholder
+
 
 class Parser:
     """
     Class which holds the data to be accessed by "Language" class
     WARNING: This class is not intended to be modified by users.
     """
 
@@ -18,15 +20,15 @@
         section_dict = self.data.setdefault(section, {})
         section_dict[option] = value
 
     def get(self, section, option):
         return self.data.get(section, {}).get(option, None)
 
 
-class Language:
+class Translation:
     """
     Class which handles the translation for a language.
     Parameters:
         :param parser (Parser): Parser instance, aka the data holder
         :param code (str): Language code, aka the language file name
         :param name (str): Language name, read from the langauge file, section "Translation", key "name"
         :param logger (logging.Logger): The child logger of translator logger for this language
@@ -100,43 +102,36 @@
         # returns "This is an example with a nested placeholder: Nested"
         ```
         """
         text = self.read(section, key, default)
         if not isinstance(text, str):
             return text
 
-        for placeholder in re.findall('%(\\w+(\\.\\w+)*)%', text):
-            path = placeholder[0].split('.')
-            obj: None | object = kwargs.get(path.pop(0), None)
-            while obj is not None and len(path) > 0:
-                if isinstance(obj, dict):
-                    obj = obj.get(path.pop(0), None)
-                else:
-                    obj = getattr(obj, path.pop(0), None)
-
+        for placeholder in re.findall('%(.*)%', text):
+            obj = handle_placeholder(placeholder, self, kwargs)
             text = text.replace(f'%{placeholder}%', str(obj) if obj is not None else f'None({placeholder})')
 
         return text
 
 
-_TL = TypeVar('_TL', bound=Language)
+_TL = TypeVar('_TL', bound=Translation)
 
 
 class Translator:
     """
     Class holding all languages in the translation folder given.
     Parameters:
         :param path (str): The path to look for all translation files. Does not support nested folders.
         :param language_class (Type[Language]): The custom language class if needed.
         :param logger (Logger | str): Change the logger if needed.
 
     """
     def __init__(self, path: str = None, *, language_class: Type[_TL] = None, logger: Union[logging.Logger, str] = None):
-        language_class = language_class or Language
-        if not issubclass(language_class, Language):
+        language_class = language_class or Translation
+        if not issubclass(language_class, Translation):
             raise TypeError('"language_class" must be a subclass of Language')
 
         self.path = path or './'
         self.languages = {}
         self.logger = logging.getLogger('Translator') if logger is None else logging.getLogger(logger) if isinstance(logger, str) else logger
 
         for filename in os.listdir(self.path):
```

### Comparing `pyfancytranslator-1.0.6/PKG-INFO` & `pyfancytranslator-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.6
+Version: 1.1.0
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfancytranslator-1.0.6/README.md` & `pyfancytranslator-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfancytranslator-1.0.6/pyfancytranslator.egg-info/PKG-INFO` & `pyfancytranslator-1.1.0/pyfancytranslator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfancytranslator
-Version: 1.0.6
+Version: 1.1.0
 Summary: A well built translator with placeholders
 Author-email: Ashenguard <ashenguard@agmstudio.xyz>
 Project-URL: Homepage, https://github.com/agm-studio/fancytranslator
 Project-URL: Bug Tracker, https://github.com/agm-studio/fancytranslator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyfancytranslator-1.0.6/pyproject.toml` & `pyfancytranslator-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyfancytranslator"
-version = "1.0.6"
+version = "1.1.0"
 authors = [
     { name = "Ashenguard", email = "ashenguard@agmstudio.xyz" },
 ]
 description = "A well built translator with placeholders"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

