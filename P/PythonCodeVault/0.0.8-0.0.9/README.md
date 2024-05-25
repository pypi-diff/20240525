# Comparing `tmp/PythonCodeVault-0.0.8.tar.gz` & `tmp/PythonCodeVault-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonCodeVault-0.0.8.tar", last modified: Thu Mar 21 08:49:23 2024, max compression
+gzip compressed data, was "PythonCodeVault-0.0.9.tar", last modified: Mon Mar 25 12:24:52 2024, max compression
```

## Comparing `PythonCodeVault-0.0.8.tar` & `PythonCodeVault-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 08:49:23.977898 PythonCodeVault-0.0.8/
--rw-rw-rw-   0        0        0      544 2024-03-21 08:49:23.976897 PythonCodeVault-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-21 08:49:23.963901 PythonCodeVault-0.0.8/PythonCodeVault/
--rw-rw-rw-   0        0        0     4708 2024-03-21 08:45:53.000000 PythonCodeVault-0.0.8/PythonCodeVault/KerasDatasets.py
--rw-rw-rw-   0        0        0     8715 2024-03-07 09:59:09.000000 PythonCodeVault-0.0.8/PythonCodeVault/TrainTestValSplitter.py
--rw-rw-rw-   0        0        0      102 2024-03-01 08:00:08.000000 PythonCodeVault-0.0.8/PythonCodeVault/__init__.py
--rw-rw-rw-   0        0        0      791 2024-03-07 09:59:01.000000 PythonCodeVault-0.0.8/PythonCodeVault/onnxConverter.py
-drwxrwxrwx   0        0        0        0 2024-03-21 08:49:23.973897 PythonCodeVault-0.0.8/PythonCodeVault.egg-info/
--rw-rw-rw-   0        0        0      544 2024-03-21 08:49:23.000000 PythonCodeVault-0.0.8/PythonCodeVault.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-03-21 08:49:23.000000 PythonCodeVault-0.0.8/PythonCodeVault.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 08:49:23.000000 PythonCodeVault-0.0.8/PythonCodeVault.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-21 08:49:23.000000 PythonCodeVault-0.0.8/PythonCodeVault.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-21 08:49:23.000000 PythonCodeVault-0.0.8/PythonCodeVault.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       17 2024-03-01 07:29:29.000000 PythonCodeVault-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-21 08:49:23.977898 PythonCodeVault-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      952 2024-03-21 08:49:09.000000 PythonCodeVault-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-25 12:24:52.783036 PythonCodeVault-0.0.9/
+-rw-rw-rw-   0        0        0      544 2024-03-25 12:24:52.781770 PythonCodeVault-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-03-25 12:24:52.765214 PythonCodeVault-0.0.9/PythonCodeVault/
+-rw-rw-rw-   0        0        0     4871 2024-03-25 12:22:54.000000 PythonCodeVault-0.0.9/PythonCodeVault/KerasDatasets.py
+-rw-rw-rw-   0        0        0     8715 2024-03-07 09:59:09.000000 PythonCodeVault-0.0.9/PythonCodeVault/TrainTestValSplitter.py
+-rw-rw-rw-   0        0        0      102 2024-03-01 08:00:08.000000 PythonCodeVault-0.0.9/PythonCodeVault/__init__.py
+-rw-rw-rw-   0        0        0      791 2024-03-07 09:59:01.000000 PythonCodeVault-0.0.9/PythonCodeVault/onnxConverter.py
+drwxrwxrwx   0        0        0        0 2024-03-25 12:24:52.779782 PythonCodeVault-0.0.9/PythonCodeVault.egg-info/
+-rw-rw-rw-   0        0        0      544 2024-03-25 12:24:52.000000 PythonCodeVault-0.0.9/PythonCodeVault.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-03-25 12:24:52.000000 PythonCodeVault-0.0.9/PythonCodeVault.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-25 12:24:52.000000 PythonCodeVault-0.0.9/PythonCodeVault.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-03-25 12:24:52.000000 PythonCodeVault-0.0.9/PythonCodeVault.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-03-25 12:24:52.000000 PythonCodeVault-0.0.9/PythonCodeVault.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       17 2024-03-01 07:29:29.000000 PythonCodeVault-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-25 12:24:52.783036 PythonCodeVault-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      952 2024-03-25 12:24:39.000000 PythonCodeVault-0.0.9/setup.py
```

### Comparing `PythonCodeVault-0.0.8/PKG-INFO` & `PythonCodeVault-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonCodeVault
-Version: 0.0.8
+Version: 0.0.9
 Summary: My Python Functions
 Author: Kevin Fischer
 Author-email: <kevinfischer1611@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PythonCodeVault-0.0.8/PythonCodeVault/KerasDatasets.py` & `PythonCodeVault-0.0.9/PythonCodeVault/KerasDatasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,22 +75,29 @@
         self.pass_tuples = [(img, targets[1]) for img in self.pass_images]
 
         self.data = self.fail_tuples + self.pass_tuples
         
         self.batch_size = batch_size
         self.augmentations = augmentations
 
+        self.counter = 0
+
 
     def __len__(self):
         return len(self.data) // self.batch_size
 
     def shuffle(self):
         random.shuffle(self.data)        
 
     def __getitem__(self, idx):
+        self.counter += 1
+        if self.counter == self.__len__() + 1:
+            self.counter = 0
+            self.shuffle()
+
         data_tuples = self.data[idx * self.batch_size:(idx + 1) * self.batch_size]
 
         batch_x = [i[0] for i in data_tuples]
         batch_y = [i[1] for i in data_tuples]
 
         if self.augmentations: 
             return np.array([self.augmentations(image=x.astype(self.dtype))["image"] for x in batch_x]), np.array(batch_y).astype(self.dtype)
```

### Comparing `PythonCodeVault-0.0.8/PythonCodeVault/TrainTestValSplitter.py` & `PythonCodeVault-0.0.9/PythonCodeVault/TrainTestValSplitter.py`

 * *Files identical despite different names*

### Comparing `PythonCodeVault-0.0.8/PythonCodeVault/onnxConverter.py` & `PythonCodeVault-0.0.9/PythonCodeVault/onnxConverter.py`

 * *Files identical despite different names*

### Comparing `PythonCodeVault-0.0.8/PythonCodeVault.egg-info/PKG-INFO` & `PythonCodeVault-0.0.9/PythonCodeVault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonCodeVault
-Version: 0.0.8
+Version: 0.0.9
 Summary: My Python Functions
 Author: Kevin Fischer
 Author-email: <kevinfischer1611@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PythonCodeVault-0.0.8/setup.py` & `PythonCodeVault-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.8'   # https://github.com/fischi1611/CodeVault/blob/main/Coding/Python/PyPI/Publish_Package.md
+VERSION = '0.0.9'   # https://github.com/fischi1611/CodeVault/blob/main/Coding/Python/PyPI/Publish_Package.md
 DESCRIPTION = 'My Python Functions'
 LONG_DESCRIPTION = 'My Python Functions - long Description'
 
 # Setting up
 setup(
     name="PythonCodeVault",
     version=VERSION,
```

