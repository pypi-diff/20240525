# Comparing `tmp/python_esios-0.1.7.tar.gz` & `tmp/python_esios-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_esios-0.1.7.tar", last modified: Tue May 21 15:51:22 2024, max compression
+gzip compressed data, was "python_esios-0.2.1.tar", last modified: Sat May 25 20:45:38 2024, max compression
```

## Comparing `python_esios-0.1.7.tar` & `python_esios-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.057422 python_esios-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-21 15:51:14.000000 python_esios-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 15:51:22.057422 python_esios-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 15:51:14.000000 python_esios-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.053422 python_esios-0.1.7/esios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.053422 python_esios-0.1.7/esios/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.053422 python_esios-0.1.7/esios/endpoints/archives/
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/archives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.057422 python_esios-0.1.7/esios/endpoints/archives/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/archives/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.057422 python_esios-0.1.7/esios/endpoints/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-05-21 15:51:14.000000 python_esios-0.1.7/esios/endpoints/indicators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:51:22.057422 python_esios-0.1.7/python_esios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 15:51:22.000000 python_esios-0.1.7/python_esios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:51:22.057422 python_esios-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-21 15:51:14.000000 python_esios-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:38.182272 python_esios-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-05-25 20:45:30.000000 python_esios-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 20:45:38.182272 python_esios-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-25 20:45:30.000000 python_esios-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:38.178272 python_esios-0.2.1/esios/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 20:45:30.000000 python_esios-0.2.1/esios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-25 20:45:30.000000 python_esios-0.2.1/esios/archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-25 20:45:30.000000 python_esios-0.2.1/esios/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-25 20:45:30.000000 python_esios-0.2.1/esios/indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:45:38.182272 python_esios-0.2.1/python_esios.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 20:45:38.000000 python_esios-0.2.1/python_esios.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-25 20:45:38.000000 python_esios-0.2.1/python_esios.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 20:45:38.000000 python_esios-0.2.1/python_esios.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 20:45:38.000000 python_esios-0.2.1/python_esios.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-25 20:45:38.000000 python_esios-0.2.1/python_esios.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:45:38.182272 python_esios-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-25 20:45:30.000000 python_esios-0.2.1/setup.py
```

### Comparing `python_esios-0.1.7/setup.py` & `python_esios-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 setup(
     name='python-esios',
-    version='0.1.7',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pandas',
     ],
     author="Jesús López",
     author_email="jesus.lopez@datons.ai",
     description="A Python wrapper for the ESIOS API",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/datons/python-esios",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

