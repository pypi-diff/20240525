# Comparing `tmp/VASP2KP-1.1.4.tar.gz` & `tmp/VASP2KP-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VASP2KP-1.1.4.tar", last modified: Tue May 21 07:03:40 2024, max compression
+gzip compressed data, was "VASP2KP-1.1.5.tar", last modified: Sat May 25 15:09:10 2024, max compression
```

## Comparing `VASP2KP-1.1.4.tar` & `VASP2KP-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-05-21 07:03:40.152186 VASP2KP-1.1.4/
--rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.1.4/LICENSE.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-05-21 07:03:40.151936 VASP2KP-1.1.4/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.1.4/README.md
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-05-21 07:03:40.150195 VASP2KP-1.1.4/VASP2KP/
--rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.1.4/VASP2KP/__init__.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    31562 2024-04-15 02:26:54.000000 VASP2KP-1.1.4/VASP2KP/_get_kp_Zeeman.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    64667 2024-04-13 14:49:00.000000 VASP2KP-1.1.4/VASP2KP/_numeric_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    52754 2024-05-20 16:00:24.000000 VASP2KP-1.1.4/VASP2KP/_read_data.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    91476 2024-05-21 07:00:58.000000 VASP2KP-1.1.4/VASP2KP/_standard_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2024-04-13 10:00:38.000000 VASP2KP-1.1.4/VASP2KP/_transform_matrix.py
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-05-21 07:03:40.151666 VASP2KP-1.1.4/VASP2KP.egg-info/
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)      421 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/SOURCES.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/dependency_links.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-16 10:48:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/not-zip-safe
--rw-r--r--   0 shengzhang   (501) staff       (20)       34 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/requires.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        8 2024-05-21 07:03:40.000000 VASP2KP-1.1.4/VASP2KP.egg-info/top_level.txt
--rwxrwxrwx   0 shengzhang   (501) staff       (20)     9688 2024-04-18 02:00:28.000000 VASP2KP-1.1.4/mat2kp
--rw-r--r--   0 shengzhang   (501) staff       (20)       38 2024-05-21 07:03:40.152245 VASP2KP-1.1.4/setup.cfg
--rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2024-05-21 07:03:24.000000 VASP2KP-1.1.4/setup.py
--rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.1.4/vasp2mat.5.3-patch-1.0.1.sh
--rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.1.4/vasp2mat.6.4-patch-1.0.1.sh
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-05-25 15:09:10.141393 VASP2KP-1.1.5/
+-rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.1.5/LICENSE.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-05-25 15:09:10.141132 VASP2KP-1.1.5/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.1.5/README.md
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-05-25 15:09:10.139421 VASP2KP-1.1.5/VASP2KP/
+-rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.1.5/VASP2KP/__init__.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    31562 2024-04-15 02:26:54.000000 VASP2KP-1.1.5/VASP2KP/_get_kp_Zeeman.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    64667 2024-04-13 14:49:00.000000 VASP2KP-1.1.5/VASP2KP/_numeric_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    53107 2024-05-25 15:06:45.000000 VASP2KP-1.1.5/VASP2KP/_read_data.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    91476 2024-05-21 07:00:58.000000 VASP2KP-1.1.5/VASP2KP/_standard_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2024-04-13 10:00:38.000000 VASP2KP-1.1.5/VASP2KP/_transform_matrix.py
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-05-25 15:09:10.140828 VASP2KP-1.1.5/VASP2KP.egg-info/
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-05-25 15:09:10.000000 VASP2KP-1.1.5/VASP2KP.egg-info/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)      421 2024-05-25 15:09:10.000000 VASP2KP-1.1.5/VASP2KP.egg-info/SOURCES.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-05-25 15:09:10.000000 VASP2KP-1.1.5/VASP2KP.egg-info/dependency_links.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-05-25 15:09:10.000000 VASP2KP-1.1.5/VASP2KP.egg-info/not-zip-safe
+-rw-r--r--   0 shengzhang   (501) staff       (20)       34 2024-05-25 15:09:10.000000 VASP2KP-1.1.5/VASP2KP.egg-info/requires.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        8 2024-05-25 15:09:10.000000 VASP2KP-1.1.5/VASP2KP.egg-info/top_level.txt
+-rwxrwxrwx   0 shengzhang   (501) staff       (20)     9347 2024-05-25 14:53:02.000000 VASP2KP-1.1.5/mat2kp
+-rw-r--r--   0 shengzhang   (501) staff       (20)       38 2024-05-25 15:09:10.141452 VASP2KP-1.1.5/setup.cfg
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2024-05-25 15:07:32.000000 VASP2KP-1.1.5/setup.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.1.5/vasp2mat.5.3-patch-1.0.1.sh
+-rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.1.5/vasp2mat.6.4-patch-1.0.1.sh
```

### Comparing `VASP2KP-1.1.4/LICENSE.txt` & `VASP2KP-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.4/PKG-INFO` & `VASP2KP-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.1.4
+Version: 1.1.5
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.1.4/README.md` & `VASP2KP-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.4/VASP2KP/__init__.py` & `VASP2KP-1.1.5/VASP2KP/__init__.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.4/VASP2KP/_get_kp_Zeeman.py` & `VASP2KP-1.1.5/VASP2KP/_get_kp_Zeeman.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.4/VASP2KP/_numeric_kp.py` & `VASP2KP-1.1.5/VASP2KP/_numeric_kp.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.4/VASP2KP/_read_data.py` & `VASP2KP-1.1.5/VASP2KP/_read_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,15 +470,22 @@
     find_flag = False
     for i in range(num_k):
         file.readline()
         kpoints_eig = file.readline().strip().split(' ')
         while '' in kpoints_eig:
             kpoints_eig.remove('')
         kpoints_eig = np.array([eval(l) for l in kpoints_eig[0:3]])
-        dif = np.linalg.norm(kpoints_eig-kpoints)
+        try:
+            dif = np.linalg.norm(kpoints_eig-kpoints)
+        except:
+            if i==0: 
+                print("ERROR: Empty file 'EIGENVAL'!!! You should use the 'EIGENVAL' generated by VASP when computing wavefunction 'WAVECAR' but not the 'EIGENVAL' generated by vasp2mat!")
+            else:
+                print("ERROR: Please check the file 'EIGENVAL'!!!")
+            sys.exit()
         
         if dif < 1e-6:
             find_flag = True
             break
         else:
             for j in range(num_band):
                 file.readline()
```

### Comparing `VASP2KP-1.1.4/VASP2KP/_standard_kp.py` & `VASP2KP-1.1.5/VASP2KP/_standard_kp.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.4/VASP2KP/_transform_matrix.py` & `VASP2KP-1.1.5/VASP2KP/_transform_matrix.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.4/VASP2KP.egg-info/PKG-INFO` & `VASP2KP-1.1.5/VASP2KP.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.1.4
+Version: 1.1.5
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.1.4/mat2kp` & `VASP2KP-1.1.5/mat2kp`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
 
 elif print_flag == 1:
     print(r"Warning!!! Parameter 'print_flag' is set to 1, all the result will be output on console, not into files!")
     
 
 # calculate the result
-try:
+if True:
     if no_vasp_kp:
         result_kp, result_Zeeman = \
         get_std_kp_Zeeman_no_coe(Symmetry, order=order, gfactor=gfactor, print_flag=print_flag, log=log, repr_split = repr_split)
     
     else:
         result_kp, result_Zeeman = \
         get_std_kp_Zeeman(Symmetry, vaspMAT, kpmodel=kpmodel, order=order, gfactor=gfactor, print_flag=print_flag, log=log, acc=acc, repr_split = repr_split)
@@ -249,20 +249,14 @@
 #     if ve == 'mismatched dimensions':
 #         print("ERROR: At least one matrices in 'Symmetry' is not square matrix! Please check and rewrite it!")
 #     else:
 #         print("An exception occurred:", ve)
 #         print("The program unexpectedly encountered an error. We kindly ask you to send us a screenshot of the error and the input files. Email: zhangsheng221@mails.ucas.ac.cn/wzj@iphy.ac.cn")
 #         sys.exit()
     
-except Exception as e:
-    print("An exception occurred:", e)
-    print("The program unexpectedly encountered an error. We kindly ask you to send us a screenshot of the error and the input files. Email: zhangsheng221@mails.ucas.ac.cn/wzj@iphy.ac.cn")
-    sys.exit()
-else:
-    print("Congratulations! The computation of VASP2KP has finished!!!")
 
 
 if gfactor == 1 and (not no_vasp_kp) and mathematica_flag:
     mathematica_file = open("kp-Zeeman.nb",'w')
     mathematica_file.write(r'Clear["Global`*"];')
     mathematica_file.write('\n')
     kp_string = str(sp.simplify(result_kp.evalf()))
```

### Comparing `VASP2KP-1.1.4/setup.py` & `VASP2KP-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup
 
 README = """A tool for computing k.p effective Hamiltonians and Zeeman's coupling under given symmetry constraints from VASP calculations."""
 
 
 setup(name='VASP2KP',
       python_requires=">=3.6",
-      version = "1.1.4",
+      version = "1.1.5",
       long_description=README,
       install_requires=[
         'sympy', 'numpy', 'scipy', 'kdotp_generator'
         ],
       packages=['VASP2KP'],
       author = 'Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang',
       author_email='zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn',
```

### Comparing `VASP2KP-1.1.4/vasp2mat.5.3-patch-1.0.1.sh` & `VASP2KP-1.1.5/vasp2mat.5.3-patch-1.0.1.sh`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.4/vasp2mat.6.4-patch-1.0.1.sh` & `VASP2KP-1.1.5/vasp2mat.6.4-patch-1.0.1.sh`

 * *Files identical despite different names*

