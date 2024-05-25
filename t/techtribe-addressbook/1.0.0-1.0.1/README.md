# Comparing `tmp/techtribe_addressbook-1.0.0.tar.gz` & `tmp/techtribe_addressbook-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techtribe_addressbook-1.0.0.tar", last modified: Sat May 25 17:59:27 2024, max compression
+gzip compressed data, was "techtribe_addressbook-1.0.1.tar", last modified: Sat May 25 18:56:12 2024, max compression
```

## Comparing `techtribe_addressbook-1.0.0.tar` & `techtribe_addressbook-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,14 @@
-drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 17:59:27.077660 techtribe_addressbook-1.0.0/
--rw-r--r--   0 graf       (501) staff       (20)     1081 2024-05-25 17:12:03.000000 techtribe_addressbook-1.0.0/LICENSE
--rw-r--r--   0 graf       (501) staff       (20)     4109 2024-05-25 17:59:27.077417 techtribe_addressbook-1.0.0/PKG-INFO
--rw-r--r--   0 graf       (501) staff       (20)     2429 2024-05-24 19:04:04.000000 techtribe_addressbook-1.0.0/README.md
-drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 17:59:27.074318 techtribe_addressbook-1.0.0/dialogs/
--rw-r--r--   0 graf       (501) staff       (20)      136 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/dialogs/__init__.py
--rw-r--r--   0 graf       (501) staff       (20)     1296 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/dialogs/ask_command_dialog.py
--rw-r--r--   0 graf       (501) staff       (20)      407 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/dialogs/ask_dialog_usage.py
--rw-r--r--   0 graf       (501) staff       (20)      370 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/dialogs/print_text.py
-drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 17:59:27.076005 techtribe_addressbook-1.0.0/models/
--rw-r--r--   0 graf       (501) staff       (20)      162 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/models/__init__.py
--rw-r--r--   0 graf       (501) staff       (20)     7164 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/models/address_book.py
--rw-r--r--   0 graf       (501) staff       (20)      381 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/models/colors.py
--rw-r--r--   0 graf       (501) staff       (20)    10798 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/models/commands.py
--rw-r--r--   0 graf       (501) staff       (20)      386 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/models/field.py
--rw-r--r--   0 graf       (501) staff       (20)     3108 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/models/fields.py
--rw-r--r--   0 graf       (501) staff       (20)     3192 2024-05-24 18:50:51.000000 techtribe_addressbook-1.0.0/models/record.py
--rw-r--r--   0 graf       (501) staff       (20)      647 2024-05-25 17:52:56.000000 techtribe_addressbook-1.0.0/pyproject.toml
--rw-r--r--   0 graf       (501) staff       (20)       38 2024-05-25 17:59:27.077718 techtribe_addressbook-1.0.0/setup.cfg
--rw-r--r--   0 graf       (501) staff       (20)      503 2024-05-25 17:58:27.000000 techtribe_addressbook-1.0.0/setup.py
-drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 17:59:27.077109 techtribe_addressbook-1.0.0/techtribe_addressbook.egg-info/
--rw-r--r--   0 graf       (501) staff       (20)     4109 2024-05-25 17:59:27.000000 techtribe_addressbook-1.0.0/techtribe_addressbook.egg-info/PKG-INFO
--rw-r--r--   0 graf       (501) staff       (20)      541 2024-05-25 17:59:27.000000 techtribe_addressbook-1.0.0/techtribe_addressbook.egg-info/SOURCES.txt
--rw-r--r--   0 graf       (501) staff       (20)        1 2024-05-25 17:59:27.000000 techtribe_addressbook-1.0.0/techtribe_addressbook.egg-info/dependency_links.txt
--rw-r--r--   0 graf       (501) staff       (20)       55 2024-05-25 17:59:27.000000 techtribe_addressbook-1.0.0/techtribe_addressbook.egg-info/entry_points.txt
--rw-r--r--   0 graf       (501) staff       (20)       39 2024-05-25 17:59:27.000000 techtribe_addressbook-1.0.0/techtribe_addressbook.egg-info/requires.txt
--rw-r--r--   0 graf       (501) staff       (20)       15 2024-05-25 17:59:27.000000 techtribe_addressbook-1.0.0/techtribe_addressbook.egg-info/top_level.txt
+drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 18:56:12.919487 techtribe_addressbook-1.0.1/
+-rw-r--r--   0 graf       (501) staff       (20)     1081 2024-05-25 17:12:03.000000 techtribe_addressbook-1.0.1/LICENSE
+-rw-r--r--   0 graf       (501) staff       (20)     4109 2024-05-25 18:56:12.919257 techtribe_addressbook-1.0.1/PKG-INFO
+-rw-r--r--   0 graf       (501) staff       (20)     2429 2024-05-24 19:04:04.000000 techtribe_addressbook-1.0.1/README.md
+-rw-r--r--   0 graf       (501) staff       (20)      647 2024-05-25 18:49:40.000000 techtribe_addressbook-1.0.1/pyproject.toml
+-rw-r--r--   0 graf       (501) staff       (20)       38 2024-05-25 18:56:12.919542 techtribe_addressbook-1.0.1/setup.cfg
+-rw-r--r--   0 graf       (501) staff       (20)      503 2024-05-25 18:31:43.000000 techtribe_addressbook-1.0.1/setup.py
+drwxr-xr-x   0 graf       (501) staff       (20)        0 2024-05-25 18:56:12.918997 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/
+-rw-r--r--   0 graf       (501) staff       (20)     4109 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/PKG-INFO
+-rw-r--r--   0 graf       (501) staff       (20)      313 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/SOURCES.txt
+-rw-r--r--   0 graf       (501) staff       (20)        1 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/dependency_links.txt
+-rw-r--r--   0 graf       (501) staff       (20)       55 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/entry_points.txt
+-rw-r--r--   0 graf       (501) staff       (20)       39 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/requires.txt
+-rw-r--r--   0 graf       (501) staff       (20)        1 2024-05-25 18:56:12.000000 techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/top_level.txt
```

### Comparing `techtribe_addressbook-1.0.0/LICENSE` & `techtribe_addressbook-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `techtribe_addressbook-1.0.0/PKG-INFO` & `techtribe_addressbook-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: techtribe-addressbook
-Version: 1.0.0
+Version: 1.0.1
 Summary: Save your data easy and convenient
 Home-page: https://github.com/Oldestgraf/TechTribe
 License: The MIT License (MIT)
         Copyright © 2024 TechTribe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: techtribe-addressbook Version: 1.0.0 Summary: Save
+Metadata-Version: 2.1 Name: techtribe-addressbook Version: 1.0.1 Summary: Save
 your data easy and convenient Home-page: https://github.com/Oldestgraf/
 TechTribe License: The MIT License (MIT) Copyright Â© 2024 TechTribe Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the âSoftwareâ), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `techtribe_addressbook-1.0.0/README.md` & `techtribe_addressbook-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `techtribe_addressbook-1.0.0/pyproject.toml` & `techtribe_addressbook-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "techtribe-addressbook"
-version = "1.0.0"
+version = "1.0.1"
 description = "Save your data easy and convenient"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `techtribe_addressbook-1.0.0/techtribe_addressbook.egg-info/PKG-INFO` & `techtribe_addressbook-1.0.1/techtribe_addressbook.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: techtribe-addressbook
-Version: 1.0.0
+Version: 1.0.1
 Summary: Save your data easy and convenient
 Home-page: https://github.com/Oldestgraf/TechTribe
 License: The MIT License (MIT)
         Copyright © 2024 TechTribe
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: techtribe-addressbook Version: 1.0.0 Summary: Save
+Metadata-Version: 2.1 Name: techtribe-addressbook Version: 1.0.1 Summary: Save
 your data easy and convenient Home-page: https://github.com/Oldestgraf/
 TechTribe License: The MIT License (MIT) Copyright Â© 2024 TechTribe Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the âSoftwareâ), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

