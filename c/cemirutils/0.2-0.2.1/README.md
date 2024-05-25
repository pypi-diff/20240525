# Comparing `tmp/cemirutils-0.2.tar.gz` & `tmp/cemirutils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cemirutils-0.2.tar", last modified: Sat May 25 13:45:14 2024, max compression
+gzip compressed data, was "cemirutils-0.2.1.tar", last modified: Sat May 25 13:46:45 2024, max compression
```

## Comparing `cemirutils-0.2.tar` & `cemirutils-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 13:45:14.138779 cemirutils-0.2/
--rw-rw-rw-   0        0        0        0 2024-05-25 12:03:29.000000 cemirutils-0.2/LICENSE
--rw-rw-rw-   0        0        0     2064 2024-05-25 13:45:14.137779 cemirutils-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1477 2024-05-25 13:43:44.000000 cemirutils-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 13:45:14.131776 cemirutils-0.2/cemirutils/
--rw-rw-rw-   0        0        0      146 2024-05-25 12:05:50.000000 cemirutils-0.2/cemirutils/__init__.py
--rw-rw-rw-   0        0        0    16151 2024-05-25 13:42:52.000000 cemirutils-0.2/cemirutils/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-25 13:45:14.136778 cemirutils-0.2/cemirutils.egg-info/
--rw-rw-rw-   0        0        0     2064 2024-05-25 13:45:14.000000 cemirutils-0.2/cemirutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-25 13:45:14.000000 cemirutils-0.2/cemirutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 13:45:14.000000 cemirutils-0.2/cemirutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-25 13:45:14.000000 cemirutils-0.2/cemirutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 13:45:14.138779 cemirutils-0.2/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-05-25 13:44:22.000000 cemirutils-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:46:45.953407 cemirutils-0.2.1/
+-rw-rw-rw-   0        0        0        0 2024-05-25 12:03:29.000000 cemirutils-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1975 2024-05-25 13:46:45.952407 cemirutils-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1503 2024-05-25 13:46:37.000000 cemirutils-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 13:46:45.946404 cemirutils-0.2.1/cemirutils/
+-rw-rw-rw-   0        0        0      146 2024-05-25 12:05:50.000000 cemirutils-0.2.1/cemirutils/__init__.py
+-rw-rw-rw-   0        0        0    16151 2024-05-25 13:42:52.000000 cemirutils-0.2.1/cemirutils/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 13:46:45.951406 cemirutils-0.2.1/cemirutils.egg-info/
+-rw-rw-rw-   0        0        0     1975 2024-05-25 13:46:45.000000 cemirutils-0.2.1/cemirutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-25 13:46:45.000000 cemirutils-0.2.1/cemirutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 13:46:45.000000 cemirutils-0.2.1/cemirutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-25 13:46:45.000000 cemirutils-0.2.1/cemirutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 13:46:45.953407 cemirutils-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-25 13:46:43.000000 cemirutils-0.2.1/setup.py
```

### Comparing `cemirutils-0.2/PKG-INFO` & `cemirutils-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 Metadata-Version: 2.1
 Name: cemirutils
-Version: 0.2
+Version: 0.2.1
 Summary: Basit veri işleme yardımcıları
 Home-page: https://github.com/cememir/cemirutils
 Author: Cem Emir / Muslu Yüksektepe
 Author-email: musluyuksektepe@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<meta charset="UTF-8">
+
 # CemirUtils
 
-CemirUtils, basit veri iÅŸleme iÅŸlevlerini iÃ§eren bir Python yardÄ±mcÄ± kÃ¼tÃ¼phanesidir.
+CemirUtils, basit veri işleme işlevlerini içeren bir Python yardımcı kütüphanesidir.
 
 ## Kurulum
 
-Ã–ncelikle CemirUtils kÃ¼tÃ¼phanesini Python projesine eklemek iÃ§in aÅŸaÄŸÄ±daki adÄ±mlarÄ± izleyin:
+Öncelikle CemirUtils kütüphanesini Python projesine eklemek için aşağıdaki adımları izleyin:
 
 ```bash
 pip install cemirutils
 ````
 
 
-## KullanÄ±m
+## Kullanım
 
-KÃ¼tÃ¼phane, farklÄ± veri iÅŸleme iÅŸlevlerini saÄŸlayan `CemirUtils` sÄ±nÄ±fÄ±nÄ± iÃ§erir. Ã–rneÄŸin:
+Kütüphane, farklı veri işleme işlevlerini sağlayan `CemirUtils` sınıfını içerir. Örneğin:
 
 
 ```python
 from cemirutils import CemirUtils
 
-# Mevcut tÃ¼m metodlarÄ±n isimlerini yazdÄ±r
+# Mevcut tüm metodların isimlerini yazdır
 cemir_utils = CemirUtils(None)
 print(cemir_utils.getmethods())
 
-# Veri listesindeki her bir elemanÄ± verilen skaler deÄŸer ile Ã§arpar.
+# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar.
 ceml = CemirUtils([1, 2, 3])
 ceml.multiply_by_scalar(2)  # Output: [2, 4, 6]
 
 
 ceml = CemirUtils([1, 2, 3])
-# Veri listesindeki her bir elemanÄ± verilen skaler deÄŸer ile Ã§arpar
+# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar
 result = ceml.multiply_by_scalar(2)
 print(result)  # Output: [2, 4, 6]
 
 
 ceml = CemirUtils([1, 2, 3])
-# Veri listesindeki en bÃ¼yÃ¼k deÄŸeri dÃ¶ner.
+# Veri listesindeki en büyük değeri döner.
 ceml.get_max_value()  # Output: 3
 
 
 ceml = CemirUtils([1, 2, 2, 3])
-# Verilen deÄŸerin veri listesinde kaÃ§ kez geÃ§tiÄŸini sayar.
+# Verilen değerin veri listesinde kaç kez geçtiğini sayar.
 result = ceml.get_frequency(2)
 print(result)  # Output: 2
 
 
 cemd = CemirUtils({'a': 1, 'b': 2, 'c': 3})
-# SÃ¶zlÃ¼kteki veya sÃ¶zlÃ¼k listesindeki anahtarlarÄ± dÃ¶ndÃ¼rÃ¼r.
+# Sözlükteki veya sözlük listesindeki anahtarları döndürür.
 cemd.get_keys()  # Output: ['a', 'b', 'c']
 
 
 ceml = CemirUtils([[1, 2], [3, 4], [5]])
-# Ã‡ok katmanlÄ± listeyi tek katmana indirger.
+# Çok katmanlı listeyi tek katmana indirger.
 ceml.flatten_list()  # Output: [1, 2, 3, 4, 5]
 
 ````
```

### Comparing `cemirutils-0.2/README.md` & `cemirutils-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<meta charset="UTF-8">
+
 # CemirUtils
 
 CemirUtils, basit veri işleme işlevlerini içeren bir Python yardımcı kütüphanesidir.
 
 ## Kurulum
 
 Öncelikle CemirUtils kütüphanesini Python projesine eklemek için aşağıdaki adımları izleyin:
```

### Comparing `cemirutils-0.2/cemirutils/utils.py` & `cemirutils-0.2.1/cemirutils/utils.py`

 * *Files identical despite different names*

### Comparing `cemirutils-0.2/cemirutils.egg-info/PKG-INFO` & `cemirutils-0.2.1/cemirutils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 Metadata-Version: 2.1
 Name: cemirutils
-Version: 0.2
+Version: 0.2.1
 Summary: Basit veri işleme yardımcıları
 Home-page: https://github.com/cememir/cemirutils
 Author: Cem Emir / Muslu Yüksektepe
 Author-email: musluyuksektepe@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<meta charset="UTF-8">
+
 # CemirUtils
 
-CemirUtils, basit veri iÅŸleme iÅŸlevlerini iÃ§eren bir Python yardÄ±mcÄ± kÃ¼tÃ¼phanesidir.
+CemirUtils, basit veri işleme işlevlerini içeren bir Python yardımcı kütüphanesidir.
 
 ## Kurulum
 
-Ã–ncelikle CemirUtils kÃ¼tÃ¼phanesini Python projesine eklemek iÃ§in aÅŸaÄŸÄ±daki adÄ±mlarÄ± izleyin:
+Öncelikle CemirUtils kütüphanesini Python projesine eklemek için aşağıdaki adımları izleyin:
 
 ```bash
 pip install cemirutils
 ````
 
 
-## KullanÄ±m
+## Kullanım
 
-KÃ¼tÃ¼phane, farklÄ± veri iÅŸleme iÅŸlevlerini saÄŸlayan `CemirUtils` sÄ±nÄ±fÄ±nÄ± iÃ§erir. Ã–rneÄŸin:
+Kütüphane, farklı veri işleme işlevlerini sağlayan `CemirUtils` sınıfını içerir. Örneğin:
 
 
 ```python
 from cemirutils import CemirUtils
 
-# Mevcut tÃ¼m metodlarÄ±n isimlerini yazdÄ±r
+# Mevcut tüm metodların isimlerini yazdır
 cemir_utils = CemirUtils(None)
 print(cemir_utils.getmethods())
 
-# Veri listesindeki her bir elemanÄ± verilen skaler deÄŸer ile Ã§arpar.
+# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar.
 ceml = CemirUtils([1, 2, 3])
 ceml.multiply_by_scalar(2)  # Output: [2, 4, 6]
 
 
 ceml = CemirUtils([1, 2, 3])
-# Veri listesindeki her bir elemanÄ± verilen skaler deÄŸer ile Ã§arpar
+# Veri listesindeki her bir elemanı verilen skaler değer ile çarpar
 result = ceml.multiply_by_scalar(2)
 print(result)  # Output: [2, 4, 6]
 
 
 ceml = CemirUtils([1, 2, 3])
-# Veri listesindeki en bÃ¼yÃ¼k deÄŸeri dÃ¶ner.
+# Veri listesindeki en büyük değeri döner.
 ceml.get_max_value()  # Output: 3
 
 
 ceml = CemirUtils([1, 2, 2, 3])
-# Verilen deÄŸerin veri listesinde kaÃ§ kez geÃ§tiÄŸini sayar.
+# Verilen değerin veri listesinde kaç kez geçtiğini sayar.
 result = ceml.get_frequency(2)
 print(result)  # Output: 2
 
 
 cemd = CemirUtils({'a': 1, 'b': 2, 'c': 3})
-# SÃ¶zlÃ¼kteki veya sÃ¶zlÃ¼k listesindeki anahtarlarÄ± dÃ¶ndÃ¼rÃ¼r.
+# Sözlükteki veya sözlük listesindeki anahtarları döndürür.
 cemd.get_keys()  # Output: ['a', 'b', 'c']
 
 
 ceml = CemirUtils([[1, 2], [3, 4], [5]])
-# Ã‡ok katmanlÄ± listeyi tek katmana indirger.
+# Çok katmanlı listeyi tek katmana indirger.
 ceml.flatten_list()  # Output: [1, 2, 3, 4, 5]
 
 ````
```

### Comparing `cemirutils-0.2/setup.py` & `cemirutils-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='cemirutils',
-    version='0.2',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[],
     author='Cem Emir / Muslu Yüksektepe',
     author_email='musluyuksektepe@gmail.com',
     description='Basit veri işleme yardımcıları',
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/cememir/cemirutils',  # GitHub repo URL'si
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

