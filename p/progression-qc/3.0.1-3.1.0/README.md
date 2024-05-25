# Comparing `tmp/progression_qc-3.0.1.tar.gz` & `tmp/progression_qc-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progression_qc-3.0.1.tar", last modified: Thu Apr  4 21:19:46 2024, max compression
+gzip compressed data, was "progression_qc-3.1.0.tar", last modified: Sat May 25 01:27:33 2024, max compression
```

## Comparing `progression_qc-3.0.1.tar` & `progression_qc-3.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.041484 progression_qc-3.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    35074 2024-01-22 02:39:15.000000 progression_qc-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      655 2024-04-04 21:19:46.041484 progression_qc-3.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.037484 progression_qc-3.0.1/progression_qc/
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-04 21:19:33.000000 progression_qc-3.0.1/progression_qc/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      456 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1146 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     7377 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/progression_qc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.037484 progression_qc-3.0.1/progression_qc/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 21:19:34.000000 progression_qc-3.0.1/progression_qc/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/question_base.py
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/question_prog.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/question_sys.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/rétroactions.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/test_prog.py
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-01-22 02:39:15.000000 progression_qc-3.0.1/progression_qc/schemas/test_sys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.041484 progression_qc-3.0.1/progression_qc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      655 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      645 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:19:46.000000 progression_qc-3.0.1/progression_qc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:19:46.041484 progression_qc-3.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      866 2024-04-04 21:19:14.000000 progression_qc-3.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:19:46.037484 progression_qc-3.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6462 2024-01-22 02:39:15.000000 progression_qc-3.0.1/tests/test_progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 01:27:33.216645 progression_qc-3.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35074 2024-05-25 01:24:50.000000 progression_qc-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      655 2024-05-25 01:27:33.216645 progression_qc-3.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 01:27:33.216645 progression_qc-3.1.0/progression_qc/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      456 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7624 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/progression_qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 01:27:33.216645 progression_qc-3.1.0/progression_qc/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-25 01:27:18.000000 progression_qc-3.1.0/progression_qc/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      919 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/schemas/question_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/schemas/question_prog.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/schemas/question_seq.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/schemas/question_sys.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/schemas/rétroactions.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/schemas/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/schemas/test_prog.py
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-05-25 01:24:50.000000 progression_qc-3.1.0/progression_qc/schemas/test_sys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 01:27:33.216645 progression_qc-3.1.0/progression_qc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      655 2024-05-25 01:27:33.000000 progression_qc-3.1.0/progression_qc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2024-05-25 01:27:33.000000 progression_qc-3.1.0/progression_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 01:27:33.000000 progression_qc-3.1.0/progression_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-25 01:27:33.000000 progression_qc-3.1.0/progression_qc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 01:27:33.000000 progression_qc-3.1.0/progression_qc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 01:27:33.216645 progression_qc-3.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-05-25 01:24:50.000000 progression_qc-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 01:27:33.216645 progression_qc-3.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7330 2024-05-25 01:24:50.000000 progression_qc-3.1.0/tests/test_progression_qc.py
```

### Comparing `progression_qc-3.0.1/LICENSE` & `progression_qc-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `progression_qc-3.0.1/PKG-INFO` & `progression_qc-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progression_qc
-Version: 3.0.1
+Version: 3.1.0
 Summary: progression_qc est un compilateur/validateur pour la production de d'exercices pour Progression. progression_qc reçoit sur l'entrée standard ou en paramètre un fichier YAML contenant la description d'une question et reproduit sur la sortie standard le résultat traité et validé.
 Home-page: https://git.dti.crosemont.quebec/progression/validateur
 Author: Patrick Lafrance
 Author-email: plafrance@crosemont.qc.ca
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `progression_qc-3.0.1/progression_qc/__main__.py` & `progression_qc-3.1.0/progression_qc/__main__.py`

 * *Files identical despite different names*

### Comparing `progression_qc-3.0.1/progression_qc/progression_qc.py` & `progression_qc-3.1.0/progression_qc/progression_qc.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,25 @@
         "question_prog",
         eval(pkg_resources.read_text(schemas, "question_prog.py")),
     )
     schema_registry.add(
         "question_sys",
         eval(pkg_resources.read_text(schemas, "question_sys.py")),
     )
+    schema_registry.add(
+        "question_seq",
+        eval(pkg_resources.read_text(schemas, "question_seq.py")),
+    )
 
     if "type" in contenu_fichier and contenu_fichier["type"].lower() == "prog":
         schemas_à_valider = "question_prog"
     elif "type" in contenu_fichier and contenu_fichier["type"].lower() == "sys":
         schemas_à_valider = "question_sys"
+    elif "type" in contenu_fichier and contenu_fichier["type"].lower() == "seq":
+        schemas_à_valider = "question_seq"
     else:
         schemas_à_valider = "question_base"
 
     return traiter_validation_question_yaml(contenu_fichier, schemas_à_valider)
 
 
 def get_readers():
```

### Comparing `progression_qc-3.0.1/progression_qc/schemas/question_base.py` & `progression_qc-3.1.0/progression_qc/schemas/question_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {
-    "type": {"required": True, "type": "string", "regex": "(?i)^(prog|sys)$"},
+    "type": {"required": True, "type": "string", "regex": "(?i)^(prog|sys|seq)$"},
     "niveau": {"required": False, "type": "string"},
     "titre": {"required": False, "type": "string"},
     "objectif": {"required": False, "type": "string"},
     "description": {"required": False, "type": "string"},
     "énoncé": {
         "required": False,
         "type": ["string", "list"],
```

### Comparing `progression_qc-3.0.1/progression_qc/schemas/question_sys.py` & `progression_qc-3.1.0/progression_qc/schemas/question_sys.py`

 * *Files identical despite different names*

### Comparing `progression_qc-3.0.1/progression_qc.egg-info/PKG-INFO` & `progression_qc-3.1.0/progression_qc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progression_qc
-Version: 3.0.1
+Version: 3.1.0
 Summary: progression_qc est un compilateur/validateur pour la production de d'exercices pour Progression. progression_qc reçoit sur l'entrée standard ou en paramètre un fichier YAML contenant la description d'une question et reproduit sur la sortie standard le résultat traité et validé.
 Home-page: https://git.dti.crosemont.quebec/progression/validateur
 Author: Patrick Lafrance
 Author-email: plafrance@crosemont.qc.ca
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `progression_qc-3.0.1/progression_qc.egg-info/SOURCES.txt` & `progression_qc-3.1.0/progression_qc.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 progression_qc.egg-info/SOURCES.txt
 progression_qc.egg-info/dependency_links.txt
 progression_qc.egg-info/requires.txt
 progression_qc.egg-info/top_level.txt
 progression_qc/schemas/__init__.py
 progression_qc/schemas/question_base.py
 progression_qc/schemas/question_prog.py
+progression_qc/schemas/question_seq.py
 progression_qc/schemas/question_sys.py
 progression_qc/schemas/rétroactions.py
 progression_qc/schemas/test_base.py
 progression_qc/schemas/test_prog.py
 progression_qc/schemas/test_sys.py
 tests/test_progression_qc.py
```

### Comparing `progression_qc-3.0.1/setup.py` & `progression_qc-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `progression_qc-3.0.1/tests/test_progression_qc.py` & `progression_qc-3.1.0/tests/test_progression_qc.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,7 +154,32 @@
     from question_prog_avec_ébauches_et_tests_vides import question
 
     résultat = progression_qc.valider_schema_yaml_infos_question(question)
 
     assert résultat == {"avertissements": {},
                         'erreurs': {'tests': ['empty values not allowed'],
                                     'ébauches': ['empty values not allowed']}}
+
+def test_valider_question_seq_minimale():
+    from question_seq_minimale import question
+
+    résultat = progression_qc.valider_schema_yaml_infos_question(question)
+
+    assert résultat == {"avertissements":{}, "erreurs":{}}
+
+def test_valider_question_seq_sans_séquence():
+    from question_seq_sans_séquence import question
+
+    résultat = progression_qc.valider_schema_yaml_infos_question(question)
+
+    assert résultat == {"avertissements":{},
+                        "erreurs": {
+                            'séquence': ['required field']}}
+
+def test_valider_question_seq_vide():
+    from question_seq_vide import question
+
+    résultat = progression_qc.valider_schema_yaml_infos_question(question)
+
+    assert résultat == {"avertissements":{},
+                        "erreurs": {
+                            'séquence': ['empty values not allowed']}}
```

