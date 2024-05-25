# Comparing `tmp/magyar-3.1.1.tar.gz` & `tmp/magyar-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-3.1.1.tar", last modified: Tue May 16 20:00:51 2023, max compression
+gzip compressed data, was "magyar-4.0.0.tar", last modified: Sat May 25 18:00:05 2024, max compression
```

## Comparing `magyar-3.1.1.tar` & `magyar-4.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-16 20:00:51.859305 magyar-3.1.1/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6839 2023-05-16 20:00:51.859305 magyar-3.1.1/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     6429 2023-05-16 20:00:36.000000 magyar-3.1.1/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-16 20:00:51.859305 magyar-3.1.1/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6839 2023-05-16 20:00:51.000000 magyar-3.1.1/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-16 20:00:51.000000 magyar-3.1.1/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-16 20:00:51.000000 magyar-3.1.1/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-16 20:00:51.000000 magyar-3.1.1/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)   179728 2023-05-16 19:38:59.000000 magyar-3.1.1/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-16 20:00:51.859305 magyar-3.1.1/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-16 19:46:03.000000 magyar-3.1.1/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-25 18:00:05.846459 magyar-4.0.0/
+-rw-r--r--   0 bela      (1000) bela      (1000)     6940 2024-05-25 18:00:05.846459 magyar-4.0.0/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6530 2024-05-25 17:42:38.000000 magyar-4.0.0/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-25 18:00:05.846459 magyar-4.0.0/magyar.egg-info/
+-rw-r--r--   0 bela      (1000) bela      (1000)     6940 2024-05-25 18:00:05.000000 magyar-4.0.0/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-25 18:00:05.000000 magyar-4.0.0/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-25 18:00:05.000000 magyar-4.0.0/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-25 18:00:05.000000 magyar-4.0.0/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)   349737 2024-05-25 17:42:38.000000 magyar-4.0.0/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-25 18:00:05.846459 magyar-4.0.0/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      627 2024-05-25 17:56:35.000000 magyar-4.0.0/setup.py
```

### Comparing `magyar-3.1.1/PKG-INFO` & `magyar-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.1.1
+Version: 4.0.0
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,19 +46,15 @@
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
 
 ## Listában Tuple:
 1. Magyarország összes települése + megye **telepules_megye**
-<br>
-
-![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/tuple.png)
-<br>
-
+2. Magyarország összes települése + megye + geo koordináták **telepules_megye_koordinata**
 
 1. Last names =  magyar.**vezeteknev**
 2. Female first names = magyar.**keresztnev_n**
 3. Male first names  = magyar.**keresztnev_f**
 4. Street names = magyar.**utca**
 5. City names = magyar.**telepules**
 6. Names of counties = magyar.**megye**
@@ -86,14 +82,15 @@
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
 
 Tuple in List:
 1. All settlements in Hungary + county. = magyar.telepules_megye
+2. All settlements in Hungary + county + geo coordinates = magyar.telepules_megye_koordinata
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators.
```

### Comparing `magyar-3.1.1/README.md` & `magyar-4.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,19 +34,15 @@
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
 
 ## Listában Tuple:
 1. Magyarország összes települése + megye **telepules_megye**
-<br>
-
-![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/tuple.png)
-<br>
-
+2. Magyarország összes települése + megye + geo koordináták **telepules_megye_koordinata**
 
 1. Last names =  magyar.**vezeteknev**
 2. Female first names = magyar.**keresztnev_n**
 3. Male first names  = magyar.**keresztnev_f**
 4. Street names = magyar.**utca**
 5. City names = magyar.**telepules**
 6. Names of counties = magyar.**megye**
@@ -74,14 +70,15 @@
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
 
 Tuple in List:
 1. All settlements in Hungary + county. = magyar.telepules_megye
+2. All settlements in Hungary + county + geo coordinates = magyar.telepules_megye_koordinata
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators.
```

### Comparing `magyar-3.1.1/magyar.egg-info/PKG-INFO` & `magyar-4.0.0/magyar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.1.1
+Version: 4.0.0
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -46,19 +46,15 @@
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
 
 ## Listában Tuple:
 1. Magyarország összes települése + megye **telepules_megye**
-<br>
-
-![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/tuple.png)
-<br>
-
+2. Magyarország összes települése + megye + geo koordináták **telepules_megye_koordinata**
 
 1. Last names =  magyar.**vezeteknev**
 2. Female first names = magyar.**keresztnev_n**
 3. Male first names  = magyar.**keresztnev_f**
 4. Street names = magyar.**utca**
 5. City names = magyar.**telepules**
 6. Names of counties = magyar.**megye**
@@ -86,14 +82,15 @@
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
 
 Tuple in List:
 1. All settlements in Hungary + county. = magyar.telepules_megye
+2. All settlements in Hungary + county + geo coordinates = magyar.telepules_megye_koordinata
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators.
```

### Comparing `magyar-3.1.1/setup.py` & `magyar-4.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="3.1.1",
+    version="4.0.0",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

