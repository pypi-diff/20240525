# Comparing `tmp/foscat-3.0.8.tar.gz` & `tmp/foscat-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foscat-3.0.8.tar", last modified: Wed Feb  7 22:56:03 2024, max compression
+gzip compressed data, was "/home/jmdelouis/FOSCAT/dist/.tmp-nkfgctkx/foscat-3.0.9.tar", last modified: Mon Mar 18 16:28:59 2024, max compression
```

## Comparing `foscat-3.0.8.tar` & `foscat-3.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-02-07 22:56:03.397979 foscat-3.0.8/
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     1012 2024-02-07 22:56:03.397979 foscat-3.0.8/PKG-INFO
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     2160 2024-01-29 09:30:16.000000 foscat-3.0.8/README.md
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      107 2024-02-07 22:56:03.399244 foscat-3.0.8/setup.cfg
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     1214 2024-02-07 22:55:38.000000 foscat-3.0.8/setup.py
-drwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-02-07 22:56:03.356703 foscat-3.0.8/src/
-drwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-02-07 22:56:03.387632 foscat-3.0.8/src/foscat/
--rwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)     1682 2024-01-29 13:09:21.000000 foscat-3.0.8/src/foscat/CircSpline.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    61303 2024-02-07 22:06:00.000000 foscat-3.0.8/src/foscat/FoCUS.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      731 2024-01-29 09:30:16.000000 foscat-3.0.8/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     2709 2024-02-07 09:06:38.000000 foscat-3.0.8/src/foscat/Softmax.py
--rwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)     1234 2024-01-29 13:09:33.000000 foscat-3.0.8/src/foscat/Spline1D.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    12720 2024-02-07 22:06:00.000000 foscat-3.0.8/src/foscat/Synthesis.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-01-29 09:30:16.000000 foscat-3.0.8/src/foscat/__init__.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    20249 2024-02-07 22:06:00.000000 foscat-3.0.8/src/foscat/backend.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     1425 2024-02-07 22:06:00.000000 foscat-3.0.8/src/foscat/loss_backend_tens.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     1425 2024-02-07 22:06:00.000000 foscat-3.0.8/src/foscat/loss_backend_torch.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    59627 2024-01-31 18:15:13.000000 foscat-3.0.8/src/foscat/scat.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    43688 2024-02-07 22:06:00.000000 foscat-3.0.8/src/foscat/scat1D.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      523 2024-01-29 18:07:32.000000 foscat-3.0.8/src/foscat/scat2D.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    97283 2024-02-07 22:06:01.000000 foscat-3.0.8/src/foscat/scat_cov.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    58476 2024-02-07 22:06:01.000000 foscat-3.0.8/src/foscat/scat_cov1D.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      536 2024-01-30 08:35:30.000000 foscat-3.0.8/src/foscat/scat_cov2D.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      577 2024-01-30 07:57:56.000000 foscat-3.0.8/src/foscat/scat_cov_map.py
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      559 2024-01-30 07:56:49.000000 foscat-3.0.8/src/foscat/scat_cov_map2D.py
-drwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-02-07 22:56:03.396649 foscat-3.0.8/src/foscat.egg-info/
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     1012 2024-02-07 22:56:03.000000 foscat-3.0.8/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      636 2024-02-07 22:56:03.000000 foscat-3.0.8/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)        1 2024-02-07 22:56:03.000000 foscat-3.0.8/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)       55 2024-02-07 22:56:03.000000 foscat-3.0.8/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)        7 2024-02-07 22:56:03.000000 foscat-3.0.8/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-03-18 16:28:59.000000 foscat-3.0.9/
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      867 2024-03-18 16:28:59.000000 foscat-3.0.9/PKG-INFO
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     2160 2024-01-29 09:30:16.000000 foscat-3.0.9/README.md
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      107 2024-03-18 16:28:59.000000 foscat-3.0.9/setup.cfg
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     1214 2024-03-18 16:28:42.000000 foscat-3.0.9/setup.py
+drwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-03-18 16:28:59.000000 foscat-3.0.9/src/
+drwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-03-18 16:28:59.000000 foscat-3.0.9/src/foscat/
+-rwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)     1684 2024-02-14 13:48:38.000000 foscat-3.0.9/src/foscat/CircSpline.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    61299 2024-02-14 13:48:38.000000 foscat-3.0.9/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      731 2024-01-29 09:30:16.000000 foscat-3.0.9/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     2709 2024-02-07 09:06:38.000000 foscat-3.0.9/src/foscat/Softmax.py
+-rwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)     1232 2024-02-14 13:48:38.000000 foscat-3.0.9/src/foscat/Spline1D.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    12476 2024-03-18 16:27:35.000000 foscat-3.0.9/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-01-29 09:30:16.000000 foscat-3.0.9/src/foscat/__init__.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    28157 2024-03-18 16:27:35.000000 foscat-3.0.9/src/foscat/backend.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     1667 2024-02-14 13:48:38.000000 foscat-3.0.9/src/foscat/loss_backend_tens.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     1755 2024-02-14 13:48:38.000000 foscat-3.0.9/src/foscat/loss_backend_torch.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    59558 2024-02-14 16:31:27.000000 foscat-3.0.9/src/foscat/scat.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    43608 2024-02-14 13:48:38.000000 foscat-3.0.9/src/foscat/scat1D.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      523 2024-01-29 18:07:32.000000 foscat-3.0.9/src/foscat/scat2D.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)   101194 2024-03-18 16:27:35.000000 foscat-3.0.9/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)    58344 2024-02-14 13:48:38.000000 foscat-3.0.9/src/foscat/scat_cov1D.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      536 2024-01-30 08:35:30.000000 foscat-3.0.9/src/foscat/scat_cov2D.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     2729 2024-02-14 11:20:59.000000 foscat-3.0.9/src/foscat/scat_cov_map.py
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)     2754 2024-02-14 11:21:06.000000 foscat-3.0.9/src/foscat/scat_cov_map2D.py
+drwxr-xr-x   0 jmdelouis  (1000) jmdelouis  (1000)        0 2024-03-18 16:28:59.000000 foscat-3.0.9/src/foscat.egg-info/
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      867 2024-03-18 16:28:59.000000 foscat-3.0.9/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)      636 2024-03-18 16:28:59.000000 foscat-3.0.9/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)        1 2024-03-18 16:28:59.000000 foscat-3.0.9/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)       55 2024-03-18 16:28:59.000000 foscat-3.0.9/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdelouis  (1000) jmdelouis  (1000)        7 2024-03-18 16:28:59.000000 foscat-3.0.9/src/foscat.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `foscat-3.0.8/README.md` & `foscat-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `foscat-3.0.8/setup.py` & `foscat-3.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='3.0.8',
+    version='3.0.9',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n Complete doc can be found at https://foscat-documentation.readthedocs.io/en/latest/index.html. \n\n List of developers : J.-M. Delouis, T. Foulquier, L. Mousset, T. Odaka, F. Paul, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-3.0.8/src/foscat/CircSpline.py` & `foscat-3.0.9/src/foscat/CircSpline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import math
 
 class CircSpline:
-    def __init__(self, nodes, degree):
+    def __init__(self, nodes, degree=3):
         """
         Initialize the circular spline with the given number of nodes and degree.
         """
         self.degree = degree
         self.nodes = nodes
         self.norm = [self._compute_norm(i) for i in range(degree + 1)]
```

### Comparing `foscat-3.0.8/src/foscat/FoCUS.py` & `foscat-3.0.9/src/foscat/FoCUS.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,14 +393,18 @@
             ishape=list(im.shape)
             if len(ishape)<axis+2:
                 print('Use of 2D scat with data that has less than 2D')
                 exit(0)
                 
             if nouty is None:
                 nouty=nout
+                
+            if ishape[axis]==nout and ishape[axis+1]==nouty:
+                return im
+                
             npix=im.shape[axis]
             npiy=im.shape[axis+1]
             odata=1
             if len(ishape)>axis+2:
                 for k in range(axis+2,len(ishape)):
                     odata=odata*ishape[k]
                     
@@ -1001,15 +1005,15 @@
 
             v1=self.backend.bk_reduce_sum(mtmp*vtmp,axis=axis+1)
             v2=self.backend.bk_reduce_sum(mtmp*vtmp*vtmp,axis=axis+1)
             vh=self.backend.bk_reduce_sum(mtmp,axis=axis+1)
 
             res=v1/vh
             if calc_var:
-                if vtmp.dtype=='complex128' or vtmp.dtype=='complex64':
+                if self.backend.bk_is_complex(vtmp):
                     res2=self.backend.bk_complex(self.backend.bk_sqrt(self.backend.bk_real(v2)/self.backend.bk_real(vh)
                                                                       -self.backend.bk_real(res)*self.backend.bk_real(res)), \
                                                  self.backend.bk_sqrt(self.backend.bk_imag(v2)/self.backend.bk_real(vh)
                                                                       -self.backend.bk_imag(res)*self.backend.bk_imag(res)))
                 else:
                     res2=self.backend.bk_sqrt((v2/vh-res*res)/(vh))
                 return res,res2
@@ -1022,15 +1026,15 @@
                 
             v1=self.backend.bk_reduce_sum(l_mask*l_x,axis=axis+1)
             v2=self.backend.bk_reduce_sum(l_mask*l_x*l_x,axis=axis+1)
             vh=self.backend.bk_reduce_sum(l_mask,axis=axis+1)
             
             res=v1/vh
             if calc_var:
-                if l_x.dtype=='complex128' or l_x.dtype=='complex64':
+                if self.backend.bk_is_complex(l_x):
                     res2=self.backend.bk_complex(self.backend.bk_sqrt((self.backend.bk_real(v2)/self.backend.bk_real(vh)
                                                                       -self.backend.bk_real(res)*self.backend.bk_real(res))/self.backend.bk_real(v2)), \
                                                  self.backend.bk_sqrt((self.backend.bk_imag(v2)/self.backend.bk_real(vh)
                                                                       -self.backend.bk_imag(res)*self.backend.bk_imag(res))/self.backend.bk_real(v2)))
                 else:
                     res2=self.backend.bk_sqrt((v2/vh-res*res)/(vh))
                 return res,res2
@@ -1086,15 +1090,15 @@
             #l_image=self.swapaxes(self.bk_reshape(image,oshape),-1,-3)
             l_image=self.backend.bk_reshape(image,oshape)
 
             l_ww=np.zeros([self.KERNELSZ,self.KERNELSZ,ishape,ishape*norient])
             for k in range(ishape):
                 l_ww[:,:,k,k*norient:(k+1)*norient]=ww.reshape(self.KERNELSZ,self.KERNELSZ,norient)
             
-            if l_image.dtype=='complex128' or l_image.dtype=='complex64':
+            if self.backend.bk_is_complex(l_image):
                 r=self.backend.conv2d(self.backend.bk_real(l_image),
                                       l_ww,
                                       strides=[1, 1, 1, 1],
                                       padding=self.padding)
                 i=self.backend.conv2d(self.backend.bk_imag(l_image),
                                       l_ww,
                                       strides=[1, 1, 1, 1],
@@ -1105,15 +1109,15 @@
 
             res=self.backend.bk_reshape(res,[o_shape,shape[axis+1],shape[axis+2],ishape,norient])
         else:
             oshape=[o_shape,shape[axis+1],shape[axis+2],1]
             l_ww=self.backend.bk_reshape(ww,[self.KERNELSZ,self.KERNELSZ,1,norient])
 
             tmp=self.backend.bk_reshape(image,oshape)
-            if tmp.dtype=='complex128' or tmp.dtype=='complex64':
+            if self.backend.bk_is_complex(tmp):
                 r=self.backend.conv2d(self.backend.bk_real(tmp),
                                       l_ww,
                                       strides=[1, 1, 1, 1],
                                       padding=self.padding)
                 i=self.backend.conv2d(self.backend.bk_imag(tmp),
                                          l_ww,
                                          strides=[1, 1, 1, 1],
@@ -1147,16 +1151,16 @@
                     odata=odata*ishape[k]
                     
             ndata=1
             for k in range(axis):
                 ndata=ndata*ishape[k]
 
             tim=self.backend.bk_reshape(self.backend.bk_cast(in_image),[ndata,npix,npiy,odata])
-            
-            if tim.dtype=='complex128' or tim.dtype=='complex64':
+
+            if self.backend.bk_is_complex(tim):
                 rr1=self.backend.conv2d(self.backend.bk_real(tim),self.ww_RealT[odata],strides=[1, 1, 1, 1],padding=self.padding)
                 ii1=self.backend.conv2d(self.backend.bk_real(tim),self.ww_ImagT[odata],strides=[1, 1, 1, 1],padding=self.padding)
                 rr2=self.backend.conv2d(self.backend.bk_imag(tim),self.ww_RealT[odata],strides=[1, 1, 1, 1],padding=self.padding)
                 ii2=self.backend.conv2d(self.backend.bk_imag(tim),self.ww_ImagT[odata],strides=[1, 1, 1, 1],padding=self.padding)
                 res=self.backend.bk_complex(rr1-ii2,ii1+rr2)
             else:
                 rr=self.backend.conv2d(tim,self.ww_RealT[odata],strides=[1, 1, 1, 1],padding=self.padding)
@@ -1272,15 +1276,15 @@
                     
             ndata=1
             for k in range(axis):
                 ndata=ndata*ishape[k]
 
             tim=self.backend.bk_reshape(self.backend.bk_cast(in_image),[ndata,npix,npiy,odata])
 
-            if tim.dtype=='complex128' or tim.dtype=='complex64':
+            if self.backend.bk_is_complex(tim):
                 rr=self.backend.conv2d(self.backend.bk_real(tim),self.ww_SmoothT[odata],strides=[1, 1, 1, 1],padding=self.padding)
                 ii=self.backend.conv2d(self.backend.bk_imag(tim),self.ww_SmoothT[odata],strides=[1, 1, 1, 1],padding=self.padding)
                 res=self.backend.bk_complex(rr,ii)
             else:
                 res=self.backend.conv2d(tim,self.ww_SmoothT[odata],strides=[1, 1, 1, 1],padding=self.padding)
                     
             if axis==0:
```

### Comparing `foscat-3.0.8/src/foscat/GetGPUinfo.py` & `foscat-3.0.9/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-3.0.8/src/foscat/Softmax.py` & `foscat-3.0.9/src/foscat/Softmax.py`

 * *Files identical despite different names*

### Comparing `foscat-3.0.8/src/foscat/Spline1D.py` & `foscat-3.0.9/src/foscat/Spline1D.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 class Spline1D:
-    def __init__(self, nodes, degree):
+    def __init__(self, nodes, degree=3):
         self.degree = degree
         self.nodes = nodes
         self.norm = [0] * (self.degree + 1)
         for i in range(self.degree + 1):
             self.norm[i] = pow(-1, i) * (self.degree + 1) / (self._fact_spline(self.degree + 1 - i) * self._fact_spline(i))
 
     def _fact_spline(self, x):
@@ -18,15 +18,15 @@
         if self.degree == 0:
             if x == 0.0:
                 return 0.5
             else:
                 return 1.0
         return pow(x, self.degree)
 
-    def calc_spline1d(self, x):
+    def calculate(self, x):
         y = [0] * self.nodes
         for i in range(self.nodes):
             tmp = 0
             tx = (self.nodes - 1) * x - i
             if x < 0:
                 tx = -i
             if x > 1.0:
```

### Comparing `foscat-3.0.8/src/foscat/Synthesis.py` & `foscat-3.0.9/src/foscat/Synthesis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#import tensorflow as tf
 import numpy as np
 import time
 import sys
 import os
 from datetime import datetime
 from packaging import version
 from threading import Thread
@@ -23,26 +22,14 @@
         self.args=param
         self.name=name
         self.batch=batch
         self.batch_data=batch_data
         self.batch_update=batch_update
         self.info=info_callback
         
-        if scat_operator.BACKEND=='tensorflow':
-            import  loss_backend_tens as fbk
-            self.bk=fbk.loss_backend(scat_operator)
-            
-        if scat_operator.BACKEND=='torch':
-            import  loss_backend_torch as fbk
-            self.bk=fbk.loss_backend(scat_operator)
-            
-        if scat_operator.BACKEND=='numpy':
-            print('Synthesis does not work with numpy. Please use Torch or Tensorflow')
-            exit(0)
-
     def eval(self,x,batch,return_all=False):
         if self.batch is None:
             if self.info:
                 return self.loss_function(x,self.scat_operator,self.args,return_all=return_all)
             else:
                 return self.loss_function(x,self.scat_operator,self.args)
         else:
@@ -54,16 +41,15 @@
 class Synthesis:
     def __init__(self,
                  loss_list,
                  eta=0.03,
                  beta1=0.9,
                  beta2=0.999,
                  epsilon=1e-7,
-                 decay_rate = 0.999,
-                 MAXNUMLOSS=10):
+                 decay_rate = 0.999):
 
         self.loss_class=loss_list
         self.number_of_loss=len(loss_list)
         self.nlog=0
         self.m_dw, self.v_dw = 0.0, 0.0
         self.beta1 = beta1
         self.beta2 = beta2
@@ -74,16 +60,28 @@
         self.history=np.zeros([10])
         self.curr_gpu=0
         self.event = Event()
         self.operation=loss_list[0].scat_operator
         self.mpi_size=self.operation.mpi_size
         self.mpi_rank=self.operation.mpi_rank
         self.KEEP_TRACK=None
-        self.MAXNUMLOSS=MAXNUMLOSS
+        self.MAXNUMLOSS=len(loss_list)
     
+        if self.operation.BACKEND=='tensorflow':
+            import foscat.loss_backend_tens as fbk
+            self.bk=fbk.loss_backend(self.operation,self.curr_gpu,self.mpi_rank)
+            
+        if self.operation.BACKEND=='torch':
+            import foscat.loss_backend_torch as fbk
+            self.bk=fbk.loss_backend(self.operation,self.curr_gpu,self.mpi_rank)
+            
+        if self.operation.BACKEND=='numpy':
+            print('Synthesis does not work with numpy. Please select Torch or Tensorflow FOSCAT backend')
+            exit(0)
+
     # ---------------------------------------------−---------
     def get_gpu(self,event,delay):
 
         isnvidia=os.system('which nvidia-smi &> /dev/null')
 
         while (1):
             if event.is_set():
@@ -150,31 +148,31 @@
         l_tot=0.0
 
         if self.do_all_noise and self.totalsz>self.batchsz:
             nstep=self.totalsz//self.batchsz
         else:
             nstep=1
 
-        x=self.operation.backend.bk_cast(self.operation.backend.bk_reshape(in_x,self.oshape))
+        x=self.operation.backend.bk_reshape(self.operation.backend.bk_cast(in_x),self.oshape)
         
         self.l_log[self.mpi_rank*self.MAXNUMLOSS:(self.mpi_rank+1)*self.MAXNUMLOSS]=-1.0
         
         for istep in range(nstep):
             
             for k in range(self.number_of_loss):
                 if self.loss_class[k].batch is None:
                     l_batch=None
                 else:
                     l_batch=self.loss_class[k].batch(self.loss_class[k].batch_data,istep)
 
                 if self.KEEP_TRACK is not None:
-                    l,g,linfo=self.bk.loss(x,l_batch,self.loss_class[k])
+                    l,g,linfo=self.bk.loss(x,l_batch,self.loss_class[k],self.KEEP_TRACK)
                     self.last_info=self.KEEP_TRACK(linfo,self.mpi_rank,add=True)
                 else:
-                    l,g=self.bk.loss(x,l_batch,self.loss_class[k])
+                    l,g=self.bk.loss(x,l_batch,self.loss_class[k],self.KEEP_TRACK)
 
                 if g_tot is None:
                     g_tot=g
                 else:
                     g_tot=g_tot+g
 
                 l_tot=l_tot+l.numpy()
@@ -201,16 +199,15 @@
             local_log=(self.l_log).astype('float64')
             self.ltot=np.zeros(self.l_log.shape,dtype='float64')
             self.comm.Allreduce((local_log,self.MPI.DOUBLE),(self.ltot,self.MPI.DOUBLE))
             
         if self.mpi_size==1:
             grad=g_tot
         else:
-            
-            if g_tot.dtype=='complex64' or g_tot.dtype=='complex128':
+            if self.operation.backend.bk_is_complex( g_tot):
                 grad=np.zeros(self.oshape,dtype=gtot.dtype)
 
                 self.comm.Allreduce((g_tot),(grad))
             else:
                 grad=np.zeros(self.oshape,dtype='float64')
 
                 self.comm.Allreduce((g_tot.astype('float64'),self.MPI.DOUBLE),
@@ -223,15 +220,15 @@
 
         l_tot=self.ltot[self.ltot!=-1].mean()
         
         self.history[self.nlog]=l_tot
 
         g_tot=grad.flatten()
 
-        if g_tot.dtype=='complex64' or g_tot.dtype=='complex128':
+        if self.operation.backend.bk_is_complex( g_tot):
             return l_tot.astype('float64'),g_tot
         
         return l_tot.astype('float64'),g_tot.astype('float64')
 
     # ---------------------------------------------−---------
     def xtractmap(self,x,axis):
         x=self.operation.backend.bk_reshape(x,self.oshape)
@@ -271,19 +268,14 @@
         self.grd_mask=grd_mask
         self.EVAL_FREQUENCY=EVAL_FREQUENCY
         self.MESSAGE=MESSAGE
         self.SHOWGPU=SHOWGPU
         self.axis=axis
         self.in_x_nshape=in_x.shape[0]
 
-        """
-        if do_lbfgs and (in_x.dtype=='complex64' or in_x.dtype=='complex128'):
-            print('L_BFGS minimisation not yet implemented for acomplex array, use default FOSCAT minimizer or convert your problem to float32 or float64')
-            exit(0)
-        """    
         np.random.seed(self.mpi_rank*7+1234)
             
         x=in_x        
                     
         self.curr_gpu=self.curr_gpu+self.mpi_rank
         
         if self.mpi_size>1:
```

### Comparing `foscat-3.0.8/src/foscat/backend.py` & `foscat-3.0.9/src/foscat/backend.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,15 +20,19 @@
         self._fft_2_orient_C={}
         self._fft_3_orient={}
         self._fft_3_orient_C={}
         
         self.BACKEND=name
         
         if name not in ['tensorflow','torch','numpy']:
-            print('Backend %s not yet implemented')
+            print('Backend "%s" not yet implemented'%(name))
+            print(' Choose inside the next 3 available backends :')
+            print(' - tensorflow')
+            print(' - torch')
+            print(' - numpy (Impossible to do synthesis using numpy)')
             exit(0)
             
         if self.BACKEND=='tensorflow':
             import tensorflow as tf
             
             self.backend=tf
             self.BACKEND=self.TENSORFLOW
@@ -39,14 +43,16 @@
             import torch
             self.BACKEND=self.TORCH
             self.backend=torch
             
         if self.BACKEND=='numpy':
             self.BACKEND=self.NUMPY
             self.backend=np
+            import scipy as scipy
+            self.scipy=scipy
             
         self.float64=self.backend.float64
         self.float32=self.backend.float32
         self.int64=self.backend.int64
         self.int32=self.backend.int32
         self.complex64=self.backend.complex128
         self.complex128=self.backend.complex64
@@ -116,73 +122,142 @@
                 tmp[j*norient+(j+i)%norient,i]=0.25
                 
         self._iso_orient[norient]=self.constant(self.bk_cast(tmp))
         self._iso_orient_T[norient]=self.constant(self.bk_cast(4*tmp.T))
         self._iso_orient_C[norient]=self.bk_complex(self._iso_orient[norient],0*self._iso_orient[norient])
         self._iso_orient_C_T[norient]=self.bk_complex(self._iso_orient_T[norient],0*self._iso_orient_T[norient])
         
-    def calc_fft_orient(self,norient,nharm):
+    def calc_fft_orient(self,norient,nharm,imaginary):
 
         x=np.arange(norient)/norient*2*np.pi
         
-        tmp=np.zeros([norient,1+nharm])
-        for k in range(nharm+1):
-            tmp[:,k]=np.cos(x*k)
+        if imaginary:
+            tmp=np.zeros([norient,1+nharm*2])
+            tmp[:,0]=1.0
+            for k in range(nharm):
+                tmp[:,k*2+1]=np.cos(x*(k+1))
+                tmp[:,k*2+2]=np.sin(x*(k+1))
             
-        self._fft_1_orient[(norient,nharm)]=self.constant(self.bk_cast(tmp))
-        self._fft_1_orient_C[(norient,nharm)]=self.bk_complex(self._fft_1_orient[(norient,nharm)],0*self._fft_1_orient[(norient,nharm)])
+            self._fft_1_orient[(norient,nharm,imaginary)]=self.bk_cast(self.constant(tmp))
+            self._fft_1_orient_C[(norient,nharm,imaginary)]=self.bk_complex(self._fft_1_orient[(norient,nharm,imaginary)],0*self._fft_1_orient[(norient,nharm,imaginary)])
+        else:
+            tmp=np.zeros([norient,1+nharm])
+            for k in range(nharm+1):
+                tmp[:,k]=np.cos(x*k)
+            
+            self._fft_1_orient[(norient,nharm,imaginary)]=self.bk_cast(self.constant(tmp))
+            self._fft_1_orient_C[(norient,nharm,imaginary)]=self.bk_complex(self._fft_1_orient[(norient,nharm,imaginary)],0*self._fft_1_orient[(norient,nharm,imaginary)])
 
         x=np.repeat(x,norient).reshape(norient,norient)
+
+        if imaginary:
+            tmp=np.zeros([norient,norient,(1+nharm*2),(1+nharm*2)])
+            tmp[:,:,0,0]=1.0
+            for k in range(nharm):
+                tmp[:,:,k*2+1,0]=np.cos(x*(k+1))
+                tmp[:,:,k*2+2,0]=np.sin(x*(k+1))
+                tmp[:,:,0,k*2+1]=np.cos((x.T)*(k+1))
+                tmp[:,:,0,k*2+2]=np.sin((x.T)*(k+1))
+                for l in range(nharm):
+                    tmp[:,:,k*2+1,l*2+1]=np.cos(x*(k+1))*np.cos((x.T)*(l+1))
+                    tmp[:,:,k*2+2,l*2+1]=np.sin(x*(k+1))*np.cos((x.T)*(l+1))
+                    tmp[:,:,k*2+1,l*2+2]=np.cos(x*(k+1))*np.sin((x.T)*(l+1))
+                    tmp[:,:,k*2+2,l*2+2]=np.sin(x*(k+1))*np.sin((x.T)*(l+1))
+            
+            self._fft_2_orient[(norient,nharm,imaginary)]=self.bk_cast(self.constant(tmp.reshape(norient*norient,(1+2*nharm)*(1+2*nharm))))
+            self._fft_2_orient_C[(norient,nharm,imaginary)]=self.bk_complex(self._fft_2_orient[(norient,nharm,imaginary)],0*self._fft_2_orient[(norient,nharm,imaginary)])
+        else:
+            tmp=np.zeros([norient,norient,(1+nharm),(1+nharm)])
         
-        tmp=np.zeros([norient,norient,(1+nharm),(1+nharm)])
-        
-        for k in range(nharm+1):
-            for l in range(nharm+1):
-                tmp[:,:,k,l]=np.cos(x*k)*np.cos((x.T)*l)
+            for k in range(nharm+1):
+                for l in range(nharm+1):
+                    tmp[:,:,k,l]=np.cos(x*k)*np.cos((x.T)*l)
         
-        self._fft_2_orient[(norient,nharm)]=self.constant(self.bk_cast(tmp.reshape(norient*norient,(1+nharm)*(1+nharm))))
-        self._fft_2_orient_C[(norient,nharm)]=self.bk_complex(self._fft_2_orient[(norient,nharm)],0*self._fft_2_orient[(norient,nharm)])
+            self._fft_2_orient[(norient,nharm,imaginary)]=self.bk_cast(self.constant(tmp.reshape(norient*norient,(1+nharm)*(1+nharm))))
+            self._fft_2_orient_C[(norient,nharm,imaginary)]=self.bk_complex(self._fft_2_orient[(norient,nharm,imaginary)],0*self._fft_2_orient[(norient,nharm,imaginary)])
 
-        tmp=np.zeros([norient,norient,norient,(1+nharm),(1+nharm),(1+nharm)])
         x=np.arange(norient)/norient*2*np.pi
         xx=np.zeros([norient,norient,norient])
         yy=np.zeros([norient,norient,norient])
         zz=np.zeros([norient,norient,norient])
         for i in range(norient):
             for j in range(norient):
                 xx[:,i,j]=x
                 yy[i,:,j]=x
                 zz[i,j,:]=x
+                
+        if imaginary:
+            tmp=np.ones([norient,norient,norient,(1+nharm*2),(1+nharm*2),(1+nharm*2)])
+            
+            for k in range(nharm):
+                tmp[:,:,:,k*2+1,0,0]=np.cos(xx*(k+1))
+                tmp[:,:,:,0,k*2+1,0]=np.cos(yy*(k+1))
+                tmp[:,:,:,0,0,k*2+1]=np.cos(zz*(k+1))
+                
+                tmp[:,:,:,k*2+2,0,0]=np.sin(xx*(k+1))
+                tmp[:,:,:,0,k*2+2,0]=np.sin(yy*(k+1))
+                tmp[:,:,:,0,0,k*2+2]=np.sin(zz*(k+1))
+                for l in range(nharm):
+                    tmp[:,:,:,k*2+1,l*2+1,0]=np.cos(xx*(k+1))*np.cos(yy*(l+1))
+                    tmp[:,:,:,k*2+1,l*2+2,0]=np.cos(xx*(k+1))*np.sin(yy*(l+1))
+                    tmp[:,:,:,k*2+2,l*2+1,0]=np.sin(xx*(k+1))*np.cos(yy*(l+1))
+                    tmp[:,:,:,k*2+2,l*2+2,0]=np.sin(xx*(k+1))*np.sin(yy*(l+1))
+                    
+                    tmp[:,:,:,k*2+1,0,l*2+1]=np.cos(xx*(k+1))*np.cos(zz*(l+1))
+                    tmp[:,:,:,k*2+1,0,l*2+2]=np.cos(xx*(k+1))*np.sin(zz*(l+1))
+                    tmp[:,:,:,k*2+2,0,l*2+1]=np.sin(xx*(k+1))*np.cos(zz*(l+1))
+                    tmp[:,:,:,k*2+2,0,l*2+2]=np.sin(xx*(k+1))*np.sin(zz*(l+1))
+                    
+                    tmp[:,:,:,0,k*2+1,l*2+1]=np.cos(yy*(k+1))*np.cos(zz*(l+1))
+                    tmp[:,:,:,0,k*2+1,l*2+2]=np.cos(yy*(k+1))*np.sin(zz*(l+1))
+                    tmp[:,:,:,0,k*2+2,l*2+1]=np.sin(yy*(k+1))*np.cos(zz*(l+1))
+                    tmp[:,:,:,0,k*2+2,l*2+2]=np.sin(yy*(k+1))*np.sin(zz*(l+1))
+                    
+                    for m in range(nharm):
+                        tmp[:,:,:,k*2+1,l*2+1,m*2+1]=np.cos(xx*(k+1))*np.cos(yy*(l+1))*np.cos(zz*(m+1))
+                        tmp[:,:,:,k*2+1,l*2+1,m*2+2]=np.cos(xx*(k+1))*np.cos(yy*(l+1))*np.sin(zz*(m+1))
+                        tmp[:,:,:,k*2+1,l*2+2,m*2+1]=np.cos(xx*(k+1))*np.sin(yy*(l+1))*np.cos(zz*(m+1))
+                        tmp[:,:,:,k*2+1,l*2+2,m*2+2]=np.cos(xx*(k+1))*np.sin(yy*(l+1))*np.sin(zz*(m+1))
+                        tmp[:,:,:,k*2+2,l*2+1,m*2+1]=np.sin(xx*(k+1))*np.cos(yy*(l+1))*np.cos(zz*(m+1))
+                        tmp[:,:,:,k*2+2,l*2+1,m*2+2]=np.sin(xx*(k+1))*np.cos(yy*(l+1))*np.sin(zz*(m+1))
+                        tmp[:,:,:,k*2+2,l*2+2,m*2+1]=np.sin(xx*(k+1))*np.sin(yy*(l+1))*np.cos(zz*(m+1))
+                        tmp[:,:,:,k*2+2,l*2+2,m*2+2]=np.sin(xx*(k+1))*np.sin(yy*(l+1))*np.sin(zz*(m+1))
+                    
+
+            self._fft_3_orient[(norient,nharm,imaginary)]=self.bk_cast(self.constant(tmp.reshape(norient*norient*norient,(1+nharm*2)*(1+nharm*2)*(1+nharm*2))))
+            self._fft_3_orient_C[(norient,nharm,imaginary)]=self.bk_complex(self._fft_3_orient[(norient,nharm,imaginary)],0*self._fft_3_orient[(norient,nharm,imaginary)])
+        else:
+            tmp=np.zeros([norient,norient,norient,(1+nharm),(1+nharm),(1+nharm)])
         
-        for k in range(nharm+1):
-            for l in range(nharm+1):
-                for m in range(nharm+1):
-                    tmp[:,:,:,k,l,m]=np.cos(xx*k)*np.cos(yy*l)*np.cos(zz*m)
+            for k in range(nharm+1):
+                for l in range(nharm+1):
+                    for m in range(nharm+1):
+                        tmp[:,:,:,k,l,m]=np.cos(xx*k)*np.cos(yy*l)*np.cos(zz*m)
 
-        self._fft_3_orient[(norient,nharm)]=self.constant(self.bk_cast(tmp.reshape(norient*norient*norient,(1+nharm)*(1+nharm)*(1+nharm))))
-        self._fft_3_orient_C[(norient,nharm)]=self.bk_complex(self._fft_3_orient[(norient,nharm)],0*self._fft_3_orient[(norient,nharm)])
+            self._fft_3_orient[(norient,nharm,imaginary)]=self.bk_cast(self.constant(tmp.reshape(norient*norient*norient,(1+nharm)*(1+nharm)*(1+nharm))))
+            self._fft_3_orient_C[(norient,nharm,imaginary)]=self.bk_complex(self._fft_3_orient[(norient,nharm,imaginary)],0*self._fft_3_orient[(norient,nharm,imaginary)])
         
     # ---------------------------------------------−---------
     # --             BACKEND DEFINITION                    --
     # ---------------------------------------------−---------
     def bk_SparseTensor(self,indice,w,dense_shape=[]):
         if self.BACKEND==self.TENSORFLOW:
             return(self.backend.SparseTensor(indice,w,dense_shape=dense_shape))
         if self.BACKEND==self.TORCH:
             return(self.backend.sparse_coo_tensor(indice.T,w,dense_shape))
         if self.BACKEND==self.NUMPY:
-            return np.sparse_matrix(indice,w,dense_shape=dense_shape)
-
+            return self.scipy.sparse.coo_matrix((w,(indice[:,0],indice[:,1])),shape=dense_shape)
+        
     def bk_sparse_dense_matmul(self,smat,mat):
         if self.BACKEND==self.TENSORFLOW:
             return self.backend.sparse.sparse_dense_matmul(smat,mat) 
         if self.BACKEND==self.TORCH:
             return smat.matmul(mat)
         if self.BACKEND==self.NUMPY:
-            return np.sparse.sparse_dense_matmul(smat,mat)
+            return smat.dot(mat)
 
     def conv2d(self,x,w,strides=[1, 1, 1, 1],padding='SAME'):
         if self.BACKEND==self.TENSORFLOW:
                 return self.backend.nn.conv2d(x,w,
                                                strides=strides,
                                                padding=padding)
         # to be written!!!
@@ -210,35 +285,37 @@
         
     def bk_device(self,device_name):
         return self.backend.device(device_name)
         
     def bk_ones(self,shape,dtype=None):
         if dtype is None:
             dtype=self.all_type
+        if self.BACKEND==self.TORCH:
+            return self.bk_cast(np.ones(shape))
         return(self.backend.ones(shape,dtype=dtype))
     
     def bk_conv1d(self,x,w):
         if self.BACKEND==self.TENSORFLOW:
             return self.backend.nn.conv1d(x,w, stride=[1,1,1], padding='SAME')
         if self.BACKEND==self.TORCH:
             return self.backend.nn.conv1d(x,w, stride=1, padding='SAME')
         if self.BACKEND==self.NUMPY:
             return self.backend.nn.conv1d(x,w, stride=1, padding='SAME')
-        
+
     def bk_flattenR(self,x):
         if self.BACKEND==self.TENSORFLOW or self.BACKEND==self.TORCH:
-            if x.dtype=='complex32' or x.dtype=='complex64':
+            if self.bk_is_complex(x):
                 rr=self.backend.reshape(self.bk_real(x),[np.prod(np.array(list(x.shape)))])
                 ii=self.backend.reshape(self.bk_imag(x),[np.prod(np.array(list(x.shape)))])
                 return self.bk_concat([rr,ii],axis=0) 
             else:
                 return self.backend.reshape(x,[np.prod(np.array(list(x.shape)))])
             
         if self.BACKEND==self.NUMPY:
-            if x.dtype=='complex32' or x.dtype=='complex64':
+            if self.bk_is_complex(x):
                 return np.concatenate([x.real.flatten(),x.imag.flatten()],0)
             else:
                 return x.flatten()
         
     def bk_flatten(self,x):
         if self.BACKEND==self.TENSORFLOW:
             return self.backend.reshape(x,[np.prod(np.array(list(x.shape)))])
@@ -246,16 +323,23 @@
             return self.backend.reshape(x,[np.prod(np.array(list(x.shape)))])
         if self.BACKEND==self.NUMPY:
             return x.flatten()
         
     def bk_resize_image(self,x,shape):
         if self.BACKEND==self.TENSORFLOW:
             return self.bk_cast(self.backend.image.resize(x,shape, method='bilinear'))
+        
         if self.BACKEND==self.TORCH:
-            return self.bk_cast(self.backend.image.resize(x,shape, method='bilinear'))
+            print(x.shape)
+            tmp=self.backend.nn.functional.interpolate(x,
+                                                       size=shape,
+                                                       mode='bilinear',
+                                                       align_corners=False)
+            print(tmp.shape)
+            return self.bk_cast(tmp)
         if self.BACKEND==self.NUMPY:
             return self.bk_cast(self.backend.image.resize(x,shape, method='bilinear'))
         
     def bk_L1(self,x):
         if x.dtype==self.all_cbk_type:
             xr=self.bk_real(x)
             xi=self.bk_imag(x)
@@ -291,27 +375,93 @@
                 return(self.backend.reduce_sum(data,axis=axis))
             if self.BACKEND==self.TORCH:
                 return(self.backend.sum(data,axis))
             if self.BACKEND==self.NUMPY:
                 return(np.sum(data,axis))
         
     # ---------------------------------------------−---------
-    def check_dense(self,data,datasz):
-        if self.BACKEND==self.TENSORFLOW:
-            if isinstance(data, tf.Tensor):
-                return data
-        
-            idx=tf.cast(data.indices, tf.int32)
-            data=tf.math.bincount(idx,weights=data.values,
-                                  minlength=datasz)
-            return data
+    
+    def iso_mean(self,x,use_2D=False):
+        shape=list(x.shape)
         
-        return data
+        i_orient=2
+        if use_2D:
+            i_orient=3
+        norient=shape[i_orient]
+
+        if len(shape)==i_orient+1:
+            return self.bk_reduce_mean(x,-1)
+            
+        if norient not in self._iso_orient:
+            self.calc_iso_orient(norient)
+
+        if self.bk_is_complex(x):
+            lmat   = self._iso_orient_C[norient]
+            lmat_T = self._iso_orient_C_T[norient]
+        else:
+            lmat   = self._iso_orient[norient]
+            lmat_T = self._iso_orient_T[norient]
+
+        oshape=shape[0]
+        for k in range(1,len(shape)-2):
+            oshape*=shape[k]
+            
+        oshape2=[shape[k] for k in range(0,len(shape)-1)]
         
+        return self.bk_reshape(self.backend.matmul(
+            self.bk_reshape(x,[oshape,norient*norient]),lmat),oshape2)
+
     
+    def fft_ang(self,x,nharm=1,imaginary=False,use_2D=False):
+        shape=list(x.shape)
+
+        i_orient=2
+        if use_2D:
+            i_orient=3
+        
+        norient=shape[i_orient]
+        nout=1+nharm
+        
+        oshape_1=shape[0]
+        for k in range(1,i_orient):
+            oshape_1*=shape[k]
+        oshape_2=norient
+        for k in range(i_orient,len(shape)-1):
+            oshape_2*=shape[k]
+        oshape=[oshape_1,oshape_2]
+        
+        
+        if imaginary:
+            nout=1+nharm*2
+            
+        oshape2=[shape[k] for k in range(0,i_orient)]+[nout for k in range(i_orient,len(shape))]
+        
+        if (norient,nharm) not in self._fft_1_orient:
+            self.calc_fft_orient(norient,nharm,imaginary)
+
+        if len(shape)==i_orient+1:
+            if self.bk_is_complex(x):
+                lmat   = self._fft_1_orient_C[(norient,nharm,imaginary)]
+            else:
+                lmat   = self._fft_1_orient[(norient,nharm,imaginary)]
+        
+        if len(shape)==i_orient+2:
+            if self.bk_is_complex(x):
+                lmat   = self._fft_2_orient_C[(norient,nharm,imaginary)]
+            else:
+                lmat   = self._fft_2_orient[(norient,nharm,imaginary)]
+        
+        if len(shape)==i_orient+3:
+            if self.bk_is_complex(x):
+                lmat   = self._fft_3_orient_C[(norient,nharm,imaginary)]
+            else:
+                lmat   = self._fft_3_orient[(norient,nharm,imaginary)]
+                
+        return self.bk_reshape(self.backend.matmul(self.bk_reshape(x,oshape),lmat),oshape2)
+        
     def constant(self,data):
         
         if self.BACKEND==self.TENSORFLOW:
             return(self.backend.constant(data))
         return(data)
 
     def bk_reduce_mean(self,data,axis=None):
@@ -353,20 +503,28 @@
         
         return(self.backend.sqrt(self.backend.abs(data)))
     
     def bk_abs(self,data):
         return(self.backend.abs(data))
 
     def bk_is_complex(self,data):
+        
         if self.BACKEND==self.TENSORFLOW:
-            return data.dtype==self.all_cbk_type
+            if isinstance(data,np.ndarray):
+                return (data.dtype=='complex64' or data.dtype=='complex128')
+            return data.dtype.is_complex
+        
         if self.BACKEND==self.TORCH:
-            return data.dtype==self.all_cbk_type
+            if isinstance(data,np.ndarray):
+                return (data.dtype=='complex64' or data.dtype=='complex128')
+            
+            return data.dtype.is_complex
+        
         if self.BACKEND==self.NUMPY:
-            return data.dtype==self.all_cbk_type
+            return (data.dtype=='complex64' or data.dtype=='complex128')
         
     def bk_norm(self,data):
         if self.bk_is_complex(data):
             res=self.bk_square(self.bk_real(data))+self.bk_square(self.bk_imag(data))
             return self.bk_sqrt(res)
 
         else:
@@ -407,15 +565,15 @@
         
     def bk_complex(self,real,imag):
         if self.BACKEND==self.TENSORFLOW:
             return(self.backend.dtypes.complex(real,imag))
         if self.BACKEND==self.TORCH:
             return(self.backend.complex(real,imag))
         if self.BACKEND==self.NUMPY:
-            return(np.complex(real,imag))
+            return real+1J*imag
 
     def bk_exp(self,data):
         
         return(self.backend.exp(data))
     
     def bk_min(self,data):
         
@@ -434,14 +592,18 @@
         return(self.backend.reduce_max(data))
     
     def bk_argmax(self,data):
         
         return(self.backend.argmax(data))
     
     def bk_reshape(self,data,shape):
+        if self.BACKEND==self.TORCH:
+            if isinstance(data,np.ndarray):
+                return data.reshape(shape)
+            
         return(self.backend.reshape(data,shape))
     
     def bk_repeat(self,data,nn,axis=0):
         return(self.backend.repeat(data,nn,axis=axis))
     
     def bk_tile(self,data,nn,axis=0):
         return(self.backend.tile(data,nn))
@@ -465,18 +627,24 @@
         if self.BACKEND==self.TORCH:
             return(self.backend.transpose(data,thelist))
         if self.BACKEND==self.NUMPY:
             return(np.transpose(data,thelist))
 
     def bk_concat(self,data,axis=None):
                 
-        if axis is None:
-            return(self.backend.concat(data))
+        if self.BACKEND==self.TENSORFLOW or self.BACKEND==self.TORCH:
+            if axis is None:
+                return(self.backend.concat(data))
+            else:
+                return(self.backend.concat(data,axis=axis))
         else:
-            return(self.backend.concat(data,axis=axis))
+            if axis is None:
+                return np.concatenate(data,axis=0)
+            else:
+                return np.concatenate(data,axis=axis)
 
     
     def bk_conjugate(self,data):
                 
         if self.BACKEND==self.TENSORFLOW:
             return self.backend.math.conj(data)
         if self.BACKEND==self.TORCH:
@@ -521,15 +689,15 @@
                 return(x)
         if isinstance(x,np.float32):
             if self.all_bk_type=='float64':
                 return(np.float64(x))
             else:
                 return(x)
 
-        if x.dtype=='complex128' or x.dtype=='complex64':
+        if self.bk_is_complex(x):
             out_type=self.all_cbk_type
         else:
             out_type=self.all_bk_type
             
         if self.BACKEND==self.TENSORFLOW:
             return self.backend.cast(x,out_type)
```

### Comparing `foscat-3.0.8/src/foscat/loss_backend_tens.py` & `foscat-3.0.9/src/foscat/loss_backend_tens.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 import tensorflow as tf
 import numpy as np
+import sys
 
 class loss_backend:
     
-    def __init__(self,backend):
+    def __init__(self,backend,curr_gpu,mpi_rank):
         
         self.bk=backend
+        self.curr_gpu=curr_gpu
+        self.mpi_rank=mpi_rank
+
+    
+    def check_dense(self,data,datasz):
+        if isinstance(data, tf.Tensor):
+            return data
+        
+        return data.to_dense()
+        
     # ---------------------------------------------−---------
     
     @tf.function
-    def loss(self,x,batch,loss_function):
+    def loss(self,x,batch,loss_function,KEEP_TRACK):
 
         operation=loss_function.scat_operator
 
         nx=1
         if len(x.shape)>1:
             nx=x.shape[0]
             
@@ -30,20 +41,20 @@
             """
             
             if nx==1:    
                 ndata=x.shape[0]
             else:
                 ndata=x.shape[0]*x.shape[1]
                 
-            if self.KEEP_TRACK is not None:
+            if KEEP_TRACK is not None:
                 l,linfo=loss_function.eval(l_x,batch,return_all=True)
             else:
                 l=loss_function.eval(l_x,batch)
                 
             g=tf.gradients(l,x)[0]
-            g=self.backend.check_dense(g,ndata)
+            g=self.check_dense(g,ndata)
             self.curr_gpu=self.curr_gpu+1   
             
-        if self.KEEP_TRACK is not None:
+        if KEEP_TRACK is not None:
             return l,g,linfo
         else:
             return l,g
```

### Comparing `foscat-3.0.8/src/foscat/loss_backend_torch.py` & `foscat-3.0.9/src/foscat/loss_backend_torch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,64 @@
-import tensorflow as tf
+import torch
+from torch.autograd import grad
 import numpy as np
+import sys
 
 class loss_backend:
     
-    def __init__(self,backend):
+    def __init__(self,backend,curr_gpu,mpi_rank):
         
         self.bk=backend
-    # ---------------------------------------------−---------
+        self.curr_gpu=curr_gpu
+        self.mpi_rank=mpi_rank
+
     
-    @tf.function
-    def loss(self,x,batch,loss_function):
+    def check_dense(self,data,datasz):
+        if isinstance(data, torch.Tensor):
+            return data
+        """
+        idx=tf.cast(data.indices, tf.int32)
+        data=tf.math.bincount(idx,weights=data.values,
+                              minlength=datasz)
+        """
+        return data
+        
+    # ---------------------------------------------−---------
+
+    def loss(self,x,batch,loss_function,KEEP_TRACK):
 
         operation=loss_function.scat_operator
 
         nx=1
         if len(x.shape)>1:
             nx=x.shape[0]
-            
-        with tf.device(operation.gpulist[(operation.gpupos+self.curr_gpu)%operation.ngpu]):
-            print('%s Run [PROC=%04d] on GPU %s'%(loss_function.name,self.mpi_rank,
-                                      operation.gpulist[(operation.gpupos+self.curr_gpu)%operation.ngpu]))
-            sys.stdout.flush()
-
-            l_x=x
-            """
-            if nx>1:
-                l_x={}
-            for i in range(nx):
-            """
+
+        with torch.cuda.device((operation.gpupos+self.curr_gpu)%operation.ngpu):
+            #print('%s Run [PROC=%04d] on GPU %s'%(loss_function.name,self.mpi_rank,
+            #                          operation.gpulist[(operation.gpupos+self.curr_gpu)%operation.ngpu]))
+            #sys.stdout.flush()
+
+            l_x=x.clone().detach().requires_grad_(True)
             
             if nx==1:    
                 ndata=x.shape[0]
             else:
                 ndata=x.shape[0]*x.shape[1]
                 
-            if self.KEEP_TRACK is not None:
+            if KEEP_TRACK is not None:
                 l,linfo=loss_function.eval(l_x,batch,return_all=True)
             else:
                 l=loss_function.eval(l_x,batch)
-                
-            g=tf.gradients(l,x)[0]
-            g=self.backend.check_dense(g,ndata)
+
+            l.backward()
+            
+            g=l_x.grad
+
+            print(g)
+            
             self.curr_gpu=self.curr_gpu+1   
             
-        if self.KEEP_TRACK is not None:
-            return l,g,linfo
+        if KEEP_TRACK is not None:
+            return l.detach(),g,linfo
         else:
-            return l,g
+            return l.detach(),g
+
```

### Comparing `foscat-3.0.8/src/foscat/scat.py` & `foscat-3.0.9/src/foscat/scat.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,42 +54,45 @@
                     self.backend.constant(self.S2L ), \
                     self.j1  , \
                     self.j2  ,backend=self.backend)
 
     def domult(self,x,y):
         if x.dtype==y.dtype:
             return x*y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)*y,self.backend.bk_imag(x)*y)
         else:
             return self.backend.bk_complex(self.backend.bk_real(y)*x,self.backend.bk_imag(y)*x)
         
     def dodiv(self,x,y):
         if x.dtype==y.dtype:
             return x/y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)/y,self.backend.bk_imag(x)/y)
         else:
             return self.backend.bk_complex(x/self.backend.bk_real(y),x/self.backend.bk_imag(y))
         
     def domin(self,x,y):
         if x.dtype==y.dtype:
             return x-y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)-y,self.backend.bk_imag(x)-y)
         else:
             return self.backend.bk_complex(x-self.backend.bk_real(y),x-self.backend.bk_imag(y))
         
     def doadd(self,x,y):
         if x.dtype==y.dtype:
             return x+y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)+y,self.backend.bk_imag(x)+y)
         else:
             return self.backend.bk_complex(x+self.backend.bk_real(y),x+self.backend.bk_imag(y))
         
     def relu(self):
         
@@ -271,15 +274,15 @@
                         (self.S1* other), \
                         (self.S2* other), \
                         (self.S2L* other), \
                         self.j1,self.j2,backend=self.backend)
 
     def l1_abs(self,x):
         y=self.get_np(x)
-        if y.dtype=='complex64' or y.dtype=='complex128':
+        if self.backend.bk_is_complex(y):
             tmp=y.real*y.real+y.imag*y.imag
             tmp=np.sign(tmp)*np.sqrt(np.fabs(tmp))
             y=tmp
         
         return(y)
     
     def plot(self,name=None,hold=True,color='blue',lw=1,legend=True):
@@ -595,15 +598,15 @@
             P00=self.backend.bk_reshape(self.backend.bk_repeat(P00,shape[2],1),self.S1.shape)
         else:
             P00=self.backend.bk_expand_dims(P00,-1)
 
         if norient not in self.backend._iso_orient:
             self.backend.calc_iso_orient(norient)
         
-        if self.S2.dtype=='complex128' or self.S2.dtype=='complex64':
+        if self.backend.bk_is_complex(self.S2):
             lmat   = self.backend._iso_orient_C[norient]
             lmat_T = self.backend._iso_orient_C_T[norient]
         else:
             lmat   = self.backend._iso_orient[norient]
             lmat_T = self.backend._iso_orient_T[norient]
         
         S2=self.backend.bk_reshape(
@@ -624,46 +627,50 @@
         else:
             S2=self.backend.bk_expand_dims(S2,-1)
             S2L=self.backend.bk_expand_dims(S2L,-1)
 
         return scat(P00,self.S0,S1,S2,S2L,self.j1,self.j2,backend=self.backend)
 
     
-    def fft_ang(self,nharm=1):
+    def fft_ang(self,nharm=1,imaginary=False):
         shape=list(self.S2.shape)
         norient=self.S1.shape[2]
 
+        nout=1+nharm
+        if imaginary:
+            nout=1+nharm*2
+            
         if (norient,nharm) not in self.backend._fft_1_orient:
-            self.backend.calc_fft_orient(norient,nharm)
+            self.backend.calc_fft_orient(norient,nharm,imaginary)
             
-        if self.S1.dtype=='complex128' or self.S1.dtype=='complex64':
-            lmat   = self.backend._fft_1_orient_C[(norient,nharm)]
+        if self.backend.bk_is_complex(self.S1):
+            lmat   = self.backend._fft_1_orient_C[(norient,nharm,imaginary)]
         else:
-            lmat   = self.backend._fft_1_orient[(norient,nharm)]
+            lmat   = self.backend._fft_1_orient[(norient,nharm,imaginary)]
             
         S1=self.backend.bk_reshape(
             self.backend.backend.matmul(self.backend.bk_reshape(self.S1,[self.S1.shape[0],self.S1.shape[1],norient]),lmat),
-            [self.S1.shape[0],self.S1.shape[1],1+nharm])
+            [self.S1.shape[0],self.S1.shape[1],nout])
             
         P00=self.backend.bk_reshape(
             self.backend.backend.matmul(self.backend.bk_reshape(self.P00,[self.S1.shape[0],self.S1.shape[1],norient]),lmat),
-            [self.S1.shape[0],self.S1.shape[1],1+nharm])
+            [self.S1.shape[0],self.S1.shape[1],nout])
             
         
-        if self.S2.dtype=='complex128' or self.S2.dtype=='complex64':
-            lmat   = self.backend._fft_2_orient_C[(norient,nharm)]
+        if self.backend.bk_is_complex(self.S2):
+            lmat   = self.backend._fft_2_orient_C[(norient,nharm,imaginary)]
         else:
-            lmat   = self.backend._fft_2_orient[(norient,nharm)]
+            lmat   = self.backend._fft_2_orient[(norient,nharm,imaginary)]
         
         S2=self.backend.bk_reshape(
             self.backend.backend.matmul(self.backend.bk_reshape(self.S2,[shape[0],shape[1],norient*norient]),lmat),
-            [shape[0],shape[1],1+nharm,1+nharm])
+            [shape[0],shape[1],nout,nout])
         S2L=self.backend.bk_reshape(
             self.backend.backend.matmul(self.backend.bk_reshape(self.S2L,[shape[0],shape[1],norient*norient]),lmat),
-            [shape[0],shape[1],1+nharm,1+nharm])
+            [shape[0],shape[1],nout,nout])
 
         return scat(P00,self.S0,S1,S2,S2L,self.j1,self.j2,backend=self.backend)
 
 
     def iso_std(self,repeat=False):
 
         val=(self-self.iso_mean(repeat=True)).square_comp()
@@ -1083,15 +1090,14 @@
         else:
             vmask = self.backend.bk_cast(mask)  # [Nmask, Npix]
 
         if self.KERNELSZ>3:
             if self.KERNELSZ==5:
                 # if the kernel size is bigger than 3 increase the binning before smoothing
                 if self.use_2D:
-                    print(axis,image1.shape)
                     l_image1=self.up_grade(I1,I1.shape[axis]*2,axis=axis,nouty=I1.shape[axis+1]*2)
                     vmask=self.up_grade(vmask,I1.shape[axis]*2,axis=1,nouty=I1.shape[axis+1]*2)
                 else:
                     l_image1=self.up_grade(I1,nside*2,axis=axis)
                     vmask=self.up_grade(vmask,nside*2,axis=1)
                 
                 if cross:
@@ -1128,24 +1134,24 @@
         if cross and Auto==False:
             if calc_var:
                 s02,vs02=self.masked_mean(l_image2,vmask,axis=axis,calc_var=True)
             else:
                 s02=self.masked_mean(l_image2,vmask,axis=axis)
                 
             if len(image1.shape)==1 or (len(image1.shape)==2 and self.use_2D):
-                if s0.dtype!='complex64' and s0.dtype!='complex128':
+                if self.backend.bk_is_complex(s0):
                     s0 = self.backend.bk_complex(s0,s02+s0_off)
                     if calc_var:
                         vs0 = self.backend.bk_complex(vs0,vs02)
                 else:
                     s0 = self.backend.bk_concat([s0,s02],axis=0)
                     if calc_var:
                         vs0 = self.backend.bk_concat([vs0,vs02],axis=0)
             else:
-                if s0.dtype!='complex64' and s0.dtype!='complex128':
+                if self.backend.bk_is_complex(s0):
                     s0 = self.backend.bk_complex(s0,s02+s0_off)
                     if calc_var:
                         vs0 = self.backend.bk_complex(vs0,vs02)
                 else:
                     s0 = self.backend.bk_concat([s0,s02],axis=0)
                     if calc_var:
                         vs0 = self.backend.bk_concat([vs0,vs02],axis=0)
```

### Comparing `foscat-3.0.8/src/foscat/scat1D.py` & `foscat-3.0.9/src/foscat/scat1D.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,42 +49,42 @@
                     self.backend.constant(self.S2L ), \
                     self.j1  , \
                     self.j2  ,backend=self.backend)
 
     def domult(self,x,y):
         if x.dtype==y.dtype:
             return x*y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)*y,self.backend.bk_imag(x)*y)
         else:
             return self.backend.bk_complex(self.backend.bk_real(y)*x,self.backend.bk_imag(y)*x)
         
     def dodiv(self,x,y):
         if x.dtype==y.dtype:
             return x/y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)/y,self.backend.bk_imag(x)/y)
         else:
             return self.backend.bk_complex(x/self.backend.bk_real(y),x/self.backend.bk_imag(y))
         
     def domin(self,x,y):
         if x.dtype==y.dtype:
             return x-y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)-y,self.backend.bk_imag(x)-y)
         else:
             return self.backend.bk_complex(x-self.backend.bk_real(y),x-self.backend.bk_imag(y))
         
     def doadd(self,x,y):
         if x.dtype==y.dtype:
             return x+y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)+y,self.backend.bk_imag(x)+y)
         else:
             return self.backend.bk_complex(x+self.backend.bk_real(y),x+self.backend.bk_imag(y))
         
     def relu(self):
         
@@ -266,15 +266,15 @@
                         (self.S1* other), \
                         (self.S2* other), \
                         (self.S2L* other), \
                         self.j1,self.j2,backend=self.backend)
 
     def l1_abs(self,x):
         y=self.get_np(x)
-        if y.dtype=='complex64' or y.dtype=='complex128':
+        if self.backend.bk_is_complex(y):
             tmp=y.real*y.real+y.imag*y.imag
             tmp=np.sign(tmp)*np.sqrt(np.fabs(tmp))
             y=tmp
         
         return(y)
     
     def plot(self,name=None,hold=True,color='blue',lw=1,legend=True):
```

### Comparing `foscat-3.0.8/src/foscat/scat2D.py` & `foscat-3.0.9/src/foscat/scat2D.py`

 * *Files identical despite different names*

### Comparing `foscat-3.0.8/src/foscat/scat_cov.py` & `foscat-3.0.9/src/foscat/scat_cov.py`

 * *Files 3% similar despite different names*

```diff
@@ -256,15 +256,17 @@
         return self.C10
 
     def get_C11(self):
         return self.C11
 
     def get_j_idx(self):
         shape=list(self.P00.shape)
-        if len(shape)==4:
+        if len(shape)==3:
+            nscale=shape[2]
+        elif len(shape)==4:
             nscale=shape[2]
         else:
             nscale=shape[3]
 
         n=nscale*(nscale+1)//2
         j1=np.zeros([n],dtype='int')
         j2=np.zeros([n],dtype='int')
@@ -379,28 +381,28 @@
         if self.S1 is None:
             s1 = None
         else:
             if isinstance(other, scat_cov):
                 if other.S1 is None:
                     s1 = None
                 else:
-                    s1 = self.S1 / other.S1
+                    s1 = self.dodiv(self.S1 , other.S1)
             else:
-                s1 = self.S1 / other
+                s1 = self.dodiv(self.S1 , other)
 
         if self.C10 is None:
             c10 = None
         else:
             if isinstance(other, scat_cov):
                 if other.C10 is None:
                     c10 = None
                 else:
                     c10 = self.dodiv(self.C10 , other.C10)
             else:
-                c10 = self.C10 / other
+                c10 = self.dodiv(self.C10 , other)
                 
         if self.C11 is None:
             c11 = None
         else:
             if isinstance(other, scat_cov):
                 if other.C11 is None:
                     c11 = None
@@ -408,15 +410,15 @@
                     c11 = self.dodiv(self.C11, other.C11 )
             else:
                 c11 = self.C11/other 
 
         if isinstance(other, scat_cov):
             return scat_cov(self.dodiv(self.S0,other.S0),
                             self.dodiv(self.P00,other.P00),
-                            (self.C01 / other.C01),
+                            self.dodiv(self.C01,other.C01),
                             c11,s1=s1, c10=c10,backend=self.backend)
         else:
             return scat_cov((self.S0 / other),
                             (self.P00 / other),
                             (self.C01 / other),
                             c11,s1=s1, c10=c10,backend=self.backend)
 
@@ -563,42 +565,43 @@
                             (self.C01 - other),
                             c11,
                             s1=s1, c10=c10,backend=self.backend)
         
     def domult(self,x,y):
         if x.dtype==y.dtype:
             return x*y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)*y,self.backend.bk_imag(x)*y)
         else:
             return self.backend.bk_complex(self.backend.bk_real(y)*x,self.backend.bk_imag(y)*x)
-        
+
     def dodiv(self,x,y):
         if x.dtype==y.dtype:
             return x/y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)/y,self.backend.bk_imag(x)/y)
         else:
             return self.backend.bk_complex(x/self.backend.bk_real(y),x/self.backend.bk_imag(y))
         
     def domin(self,x,y):
         if x.dtype==y.dtype:
             return x-y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)-y,self.backend.bk_imag(x)-y)
         else:
             return self.backend.bk_complex(x-self.backend.bk_real(y),x-self.backend.bk_imag(y))
         
     def doadd(self,x,y):
         if x.dtype==y.dtype:
             return x+y
-        if x.dtype=='complex64' or x.dtype=='complex128':
+        if self.backend.bk_is_complex(x):
             
             return self.backend.bk_complex(self.backend.bk_real(x)+y,self.backend.bk_imag(x)+y)
         else:
             return self.backend.bk_complex(x+self.backend.bk_real(y),x+self.backend.bk_imag(y))
                 
             
     def __mul__(self, other):
@@ -735,38 +738,56 @@
         if hold:
             plt.figure(figsize=(16, 8))
 
         if self.S1 is not None:
             plt.subplot(2, 2, 1)
             tmp=abs(self.get_np(self.S1))
             test=None
-            for k in range(tmp.shape[3]):
+            if len(tmp.shape)>3:
+                for k in range(tmp.shape[3]):
+                    for i1 in range(tmp.shape[0]):
+                        for i2 in range(tmp.shape[0]):
+                            if test is None:
+                                test=1
+                                plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $S_1$' % (name), lw=lw)
+                            else:
+                                plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
+            else:
                 for i1 in range(tmp.shape[0]):
                     for i2 in range(tmp.shape[0]):
                         if test is None:
                             test=1
-                            plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $S_1$' % (name), lw=lw)
+                            plt.plot(tmp[i1,i2,:],color=color, label=r'%s $S_1$' % (name), lw=lw)
                         else:
-                            plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
+                            plt.plot(tmp[i1,i2,:],color=color, lw=lw)
             plt.yscale('log')
             plt.legend()
             plt.ylabel('S1')
             plt.xlabel(r'$j_{1}$')
 
         test=None
         plt.subplot(2, 2, 2)
         tmp=abs(self.get_np(self.P00))
-        for k in range(tmp.shape[3]):
+        if len(tmp.shape)>3:
+            for k in range(tmp.shape[3]):
+                for i1 in range(tmp.shape[0]):
+                    for i2 in range(tmp.shape[0]):
+                        if test is None:
+                            test=1
+                            plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $P_{00}$' % (name), lw=lw)
+                        else:
+                            plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
+        else:
             for i1 in range(tmp.shape[0]):
                 for i2 in range(tmp.shape[0]):
                     if test is None:
                         test=1
-                        plt.plot(tmp[i1,i2,:,k],color=color, label=r'%s $P_{00}$' % (name), lw=lw)
+                        plt.plot(tmp[i1,i2,:],color=color, label=r'%s $P_{00}$' % (name), lw=lw)
                     else:
-                        plt.plot(tmp[i1,i2,:,k],color=color, lw=lw)
+                        plt.plot(tmp[i1,i2,:],color=color, lw=lw)
         plt.yscale('log')
         plt.ylabel('P00')
         plt.xlabel(r'$j_{1}$')
         plt.legend()
 
         ax1=plt.subplot(2, 2, 3)
         ax2 = ax1.twiny()
@@ -779,36 +800,57 @@
             lname=r'%s $C_{10}$' % (name)
             ax1.set_ylabel(r'$C_{10}$')
         test=None
         tabx=[]
         tabnx=[]
         tab2x=[]
         tab2nx=[]
-        
-        for i0 in range(tmp.shape[0]):
-            for i1 in range(tmp.shape[1]):
-                for i2 in range(j1.max()+1):
-                    for i3 in range(tmp.shape[3]):
-                        for i4 in range(tmp.shape[4]):
-                            if j2[j1==i2].shape[0]==1:
-                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4],'.', \
+        if len(tmp.shape)>4:
+            for i0 in range(tmp.shape[0]):
+                for i1 in range(tmp.shape[1]):
+                    for i2 in range(j1.max()+1):
+                        for i3 in range(tmp.shape[3]):
+                            for i4 in range(tmp.shape[4]):
+                                if j2[j1==i2].shape[0]==1:
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4],'.', \
+                                                 color=color, lw=lw)
+                                else:
+                                    if legend and test is None:
+                                        ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                                 color=color, label=lname, lw=lw)
+                                        test=1
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
                                              color=color, lw=lw)
+                        tabnx=tabnx+[r'%d'%(k) for k in j2[j1==i2]]
+                        tabx=tabx+[k+n for k in j2[j1==i2]]
+                        tab2x=tab2x+[(j2[j1==i2]+n).mean()]
+                        tab2nx=tab2nx+['%d'%(i2)]
+                        ax1.axvline((j2[j1==i2]+n).max()+0.5,ls=':',color='gray') 
+                        n=n+j2[j1==i2].shape[0]-1
+        else:
+            for i0 in range(tmp.shape[0]):
+                for i1 in range(tmp.shape[1]):
+                    for i2 in range(j1.max()+1):
+                        for i3 in range(tmp.shape[3]):
+                            if j2[j1==i2].shape[0]==1:
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3],'.', \
+                                         color=color, lw=lw)
                             else:
                                 if legend and test is None:
-                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                    ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3], \
                                              color=color, label=lname, lw=lw)
                                     test=1
-                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3,i4], \
+                                ax1.plot(j2[j1==i2]+n,tmp[i0,i1,j1==i2,i3], \
                                          color=color, lw=lw)
-                    tabnx=tabnx+[r'%d'%(k) for k in j2[j1==i2]]
-                    tabx=tabx+[k+n for k in j2[j1==i2]]
-                    tab2x=tab2x+[(j2[j1==i2]+n).mean()]
-                    tab2nx=tab2nx+['%d'%(i2)]
-                    ax1.axvline((j2[j1==i2]+n).max()+0.5,ls=':',color='gray') 
-                    n=n+j2[j1==i2].shape[0]-1
+                        tabnx=tabnx+[r'%d'%(k) for k in j2[j1==i2]]
+                        tabx=tabx+[k+n for k in j2[j1==i2]]
+                        tab2x=tab2x+[(j2[j1==i2]+n).mean()]
+                        tab2nx=tab2nx+['%d'%(i2)]
+                        ax1.axvline((j2[j1==i2]+n).max()+0.5,ls=':',color='gray') 
+                        n=n+j2[j1==i2].shape[0]-1
         plt.yscale('log')
         ax1.set_xlim(0,n+2)
         ax1.set_xticks(tabx)
         ax1.set_xticklabels(tabnx,fontsize=6)
         ax1.set_xlabel(r"$j_{2}$",fontsize=6)
         
         # Move twinned axis ticks and label from top to bottom
@@ -839,39 +881,64 @@
         tmp=abs(self.get_np(self.C11))
         lname=r'%s $C_{11}$' % (name)
         test=None
         tabx=[]
         tabnx=[]
         tab2x=[]
         tab2nx=[]
-        for i0 in range(tmp.shape[0]):
-            for i1 in range(tmp.shape[1]):
-                for i2 in range(j1.max()+1):
-                    nprev=n
-                    for i2b in range(j2[j1==i2].max()+1):
-                        idx=np.where((j1==i2)*(j2==i2b))[0]
-                        for i3 in range(tmp.shape[3]):
-                            for i4 in range(tmp.shape[4]):
-                                for i5 in range(tmp.shape[5]):
-                                    if len(idx)==1:
-                                        ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3,i4,i5],'.', \
-                                                 color=color, lw=lw)
-                                    else:
-                                        if legend and test is None:
+        if len(tmp.shape)>4:
+            for i0 in range(tmp.shape[0]):
+                for i1 in range(tmp.shape[1]):
+                    for i2 in range(j1.max()+1):
+                        nprev=n
+                        for i2b in range(j2[j1==i2].max()+1):
+                            idx=np.where((j1==i2)*(j2==i2b))[0]
+                            for i3 in range(tmp.shape[3]):
+                                for i4 in range(tmp.shape[4]):
+                                    for i5 in range(tmp.shape[5]):
+                                        if len(idx)==1:
+                                            ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3,i4,i5],'.', \
+                                                     color=color, lw=lw)
+                                        else:
+                                            if legend and test is None:
+                                                ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3,i4,i5], \
+                                                         color=color, label=lname, lw=lw)
+                                                test=1
                                             ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3,i4,i5], \
-                                                     color=color, label=lname, lw=lw)
-                                            test=1
-                                        ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3,i4,i5], \
-                                                 color=color, lw=lw)
-                        tabnx=tabnx+[r'%d,%d'%(j2[k],j3[k]) for k in idx]
-                        tabx=tabx+[k+n for k in range(len(idx))]
-                        n=n+idx.shape[0]
-                    tab2x=tab2x+[(n+nprev-1)/2]
-                    tab2nx=tab2nx+['%d'%(i2)]
-                    ax1.axvline(n-0.5,ls=':',color='gray') 
+                                                     color=color, lw=lw)
+                            tabnx=tabnx+[r'%d,%d'%(j2[k],j3[k]) for k in idx]
+                            tabx=tabx+[k+n for k in range(len(idx))]
+                            n=n+idx.shape[0]
+                        tab2x=tab2x+[(n+nprev-1)/2]
+                        tab2nx=tab2nx+['%d'%(i2)]
+                        ax1.axvline(n-0.5,ls=':',color='gray')
+        else:
+            for i0 in range(tmp.shape[0]):
+                for i1 in range(tmp.shape[1]):
+                    for i2 in range(j1.max()+1):
+                        nprev=n
+                        for i2b in range(j2[j1==i2].max()+1):
+                            idx=np.where((j1==i2)*(j2==i2b))[0]
+                            for i3 in range(tmp.shape[3]):
+                                if len(idx)==1:
+                                    ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3],'.', \
+                                             color=color, lw=lw)
+                                else:
+                                    if legend and test is None:
+                                        ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3], \
+                                                 color=color, label=lname, lw=lw)
+                                        test=1
+                                    ax1.plot(np.arange(len(idx))+n,tmp[i0,i1,idx,i3], \
+                                             color=color, lw=lw)
+                            tabnx=tabnx+[r'%d,%d'%(j2[k],j3[k]) for k in idx]
+                            tabx=tabx+[k+n for k in range(len(idx))]
+                            n=n+idx.shape[0]
+                        tab2x=tab2x+[(n+nprev-1)/2]
+                        tab2nx=tab2nx+['%d'%(i2)]
+                        ax1.axvline(n-0.5,ls=':',color='gray')
         plt.yscale('log')
         ax1.set_ylabel(r'$C_{11}$')
         ax1.set_xticks(tabx)
         ax1.set_xticklabels(tabnx,fontsize=6)
         ax1.set_xlabel(r"$j_{2},j_{3}$",fontsize=6)
         ax1.set_xlim(0,n)
         
@@ -1037,15 +1104,15 @@
 
         if norient not in self.backend._iso_orient:
             self.backend.calc_iso_orient(norient)
 
         
         shape=list(self.C01.shape)
         if self.C01 is not None:
-            if self.C01.dtype=='complex128' or self.C01.dtype=='complex64':
+            if self.backend.bk_is_complex(self.C01):
                 lmat   = self.backend._iso_orient_C[norient]
                 lmat_T = self.backend._iso_orient_C_T[norient]
             else:
                 lmat   = self.backend._iso_orient[norient]
                 lmat_T = self.backend._iso_orient_T[norient]
                 
             C01=self.backend.bk_reshape(
@@ -1058,15 +1125,15 @@
                     self.backend.backend.matmul(
                         self.backend.bk_reshape(C01,[shape[0]*shape[1]*shape[2],norient]),
                         lmat_T),
                     [shape[0],shape[1],shape[2],norient,norient])
                 
         C10=self.C10
         if self.C10 is not None:
-            if self.C10.dtype=='complex128' or self.C10.dtype=='complex64':
+            if self.backend.bk_is_complex(self.C10):
                 lmat   = self.backend._iso_orient_C[norient]
                 lmat_T = self.backend._iso_orient_C_T[norient]
             else:
                 lmat   = self.backend._iso_orient[norient]
                 lmat_T = self.backend._iso_orient_T[norient]
                     
             C10=self.backend.bk_reshape(
@@ -1079,104 +1146,111 @@
                     self.backend.backend.matmul(
                         self.backend.bk_reshape(C10,[shape[0]*shape[1]*shape[2],norient]),
                         lmat_T),
                     [shape[0],shape[1],shape[2],norient,norient])
 
         C11=self.C11
         if self.C11 is not None:
-            if self.C11.dtype=='complex128' or self.C11.dtype=='complex64':
+            if self.backend.bk_is_complex(self.C11):
                 lmat   = self.backend._iso_orient_C[norient]
                 lmat_T = self.backend._iso_orient_C_T[norient]
             else:
                 lmat   = self.backend._iso_orient[norient]
                 lmat_T = self.backend._iso_orient_T[norient]
                     
             shape=list(self.C11.shape)
             C11=self.backend.bk_reshape(
                 self.backend.backend.matmul(
                     self.backend.bk_reshape(self.C11,[shape[0]*shape[1]*shape[2]*norient,norient*norient]),
                     lmat),
                 [shape[0],shape[1],shape[2],norient,norient])
+            C11=self.backend.bk_reduce_mean(C11,3)
             if repeat:
                 C11=self.backend.bk_reshape(
-                    self.backend.backend.matmul(
-                        self.backend.bk_reshape(C11,[shape[0]*shape[1]*shape[2]*norient,norient]),
-                        lmat_T),
+                    self.backend.bk_repeat(
+                        self.backend.bk_reshape(C11,[shape[0]*shape[1]*shape[2],norient]),
+                        norient,axis=0),
+                    [shape[0]*shape[1]*shape[2]*norient,norient])
+                C11=self.backend.bk_reshape(
+                    self.backend.backend.matmul(C11,lmat_T),
                     [shape[0],shape[1],shape[2],norient,norient,norient])
 
         return scat_cov(self.S0,P00, C01, C11, s1=S1, c10=C10,backend=self.backend)
 
 
-    def fft_ang(self,nharm=1):
+    def fft_ang(self,nharm=1,imaginary=False):
         shape=list(self.P00.shape)
         norient=shape[3]
 
         if (norient,nharm) not in self.backend._fft_1_orient:
-            self.backend.calc_fft_orient(norient,nharm)
+            self.backend.calc_fft_orient(norient,nharm,imaginary)
             
+        nout=1+nharm
+        if imaginary:
+            nout=1+nharm*2
             
         S1=self.S1
         if self.S1 is not None:
-            if self.S1.dtype=='complex128' or self.S1.dtype=='complex64':
-                lmat   = self.backend._fft_1_orient_C[(norient,nharm)]
+            if self.backend.bk_is_complex(self.S1):
+                lmat   = self.backend._fft_1_orient_C[(norient,nharm,imaginary)]
             else:
-                lmat   = self.backend._fft_1_orient[(norient,nharm)]
+                lmat   = self.backend._fft_1_orient[(norient,nharm,imaginary)]
             S1=self.backend.bk_reshape(
                 self.backend.backend.matmul(self.backend.bk_reshape(self.S1,[shape[0]*shape[1]*shape[2],norient]),lmat),
-                [shape[0],shape[1],shape[2],1+nharm])
+                [shape[0],shape[1],shape[2],nout])
             
-        if self.P00.dtype=='complex128' or self.P00.dtype=='complex64':
-            lmat   = self.backend._fft_1_orient_C[(norient,nharm)]
+        if self.backend.bk_is_complex(self.P00):
+            lmat   = self.backend._fft_1_orient_C[(norient,nharm,imaginary)]
         else:
-            lmat   = self.backend._fft_1_orient[(norient,nharm)]
+            lmat   = self.backend._fft_1_orient[(norient,nharm,imaginary)]
             
         P00=self.backend.bk_reshape(
             self.backend.backend.matmul(self.backend.bk_reshape(self.P00,[shape[0]*shape[1]*shape[2],norient]),lmat),
-                [shape[0],shape[1],shape[2],1+nharm])
+                [shape[0],shape[1],shape[2],nout])
             
         C01=self.C01
         shape=list(self.C01.shape)
         if self.C01 is not None:
-            if self.C01.dtype=='complex128' or self.C01.dtype=='complex64':
-                lmat   = self.backend._fft_2_orient_C[(norient,nharm)]
+            if self.backend.bk_is_complex(self.C01):
+                lmat   = self.backend._fft_2_orient_C[(norient,nharm,imaginary)]
             else:
-                lmat   = self.backend._fft_2_orient[(norient,nharm)]
+                lmat   = self.backend._fft_2_orient[(norient,nharm,imaginary)]
                 
             C01=self.backend.bk_reshape(
                 self.backend.backend.matmul(
                     self.backend.bk_reshape(self.C01,[shape[0]*shape[1]*shape[2],norient*norient]),
                     lmat),
-                [shape[0],shape[1],shape[2],1+nharm,1+nharm])
+                [shape[0],shape[1],shape[2],nout,nout])
                 
         C10=self.C10
         if self.C10 is not None:
-            if self.C10.dtype=='complex128' or self.C10.dtype=='complex64':
-                lmat   = self.backend._fft_2_orient_C[(norient,nharm)]
+            if self.backend.bk_is_complex(self.C10):
+                lmat   = self.backend._fft_2_orient_C[(norient,nharm,imaginary)]
             else:
-                lmat   = self.backend._fft_2_orient[(norient,nharm)]
+                lmat   = self.backend._fft_2_orient[(norient,nharm,imaginary)]
                 
             C10=self.backend.bk_reshape(
                 self.backend.backend.matmul(
                     self.backend.bk_reshape(self.C10,[shape[0]*shape[1]*shape[2],norient*norient]),
                     lmat),
-                [shape[0],shape[1],shape[2],1+nharm,1+nharm])
+                [shape[0],shape[1],shape[2],nout,nout])
 
         C11=self.C11
         if self.C11 is not None:
-            if self.C01.dtype=='complex128' or self.C01.dtype=='complex64':
-                lmat   = self.backend._fft_3_orient_C[(norient,nharm)]
+            if self.backend.bk_is_complex(self.C01):
+                lmat   = self.backend._fft_3_orient_C[(norient,nharm,imaginary)]
             else:
-                lmat   = self.backend._fft_3_orient[(norient,nharm)]
+                lmat   = self.backend._fft_3_orient[(norient,nharm,imaginary)]
                     
             shape=list(self.C11.shape)
             C11=self.backend.bk_reshape(
                 self.backend.backend.matmul(
                     self.backend.bk_reshape(self.C11,[shape[0]*shape[1]*shape[2],norient*norient*norient]),
                     lmat),
-                [shape[0],shape[1],shape[2],1+nharm,1+nharm,1+nharm])
+                [shape[0],shape[1],shape[2],nout,nout,nout])
 
         return scat_cov(self.S0,P00, C01, C11, s1=S1, c10=C10,backend=self.backend)
     
     def iso_std(self,repeat=False):
 
         val=(self-self.iso_mean(repeat=True)).square_comp()
         return (val.iso_mean(repeat=repeat)).L1()
@@ -2228,17 +2302,17 @@
                                 x.domult(sig.C01,x.C01)*x.domult(sig.C01,x.C01),
                                 x.domult(sig.C11,x.C11)*x.domult(sig.C11,x.C11),
                                 backend=self.backend)
         return(self.NORIENT)
     """
     @tf.function
     """
-    def eval_comp_fast(self, image1, image2=None,mask=None,norm=None, Auto=True,Add_R45=False):
+    def eval_comp_fast(self, image1, image2=None,mask=None,norm=None, Auto=True):
 
-        res=self.eval(image1, image2=image2,mask=mask,Auto=Auto,Add_R45=Add_R45)
+        res=self.eval(image1, image2=image2,mask=mask,Auto=Auto)
         return res.S0,res.P00,res.S1,res.C01,res.C11,res.C10
 
-    def eval_fast(self, image1, image2=None,mask=None,norm=None, Auto=True,Add_R45=False):
-        s0,p0,s1,c01,c11,c10=self.eval_comp_fast(image1, image2=image2,mask=mask,Auto=Auto,Add_R45=Add_R45)
+    def eval_fast(self, image1, image2=None,mask=None,norm=None, Auto=True):
+        s0,p0,s1,c01,c11,c10=self.eval_comp_fast(image1, image2=image2,mask=mask,Auto=Auto)
         return scat_cov(s0, p0,  c01, c11, s1=s1,c10=c10,backend=self.backend)
```

### Comparing `foscat-3.0.8/src/foscat/scat_cov1D.py` & `foscat-3.0.9/src/foscat/scat_cov1D.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,43 +364,43 @@
                             (self.C01 - other),
                             c11,
                             s1=s1, c10=c10,backend=self.backend)
         
     def domult(self,x,y):
         if x.dtype==y.dtype:
             return x*y
-        if x.dtype=='complex64' or x.dtype=='complex128':
-            
+        
+        if self.backend.bk_is_complex(x):
             return self.backend.bk_complex(self.backend.bk_real(x)*y,self.backend.bk_imag(x)*y)
         else:
             return self.backend.bk_complex(self.backend.bk_real(y)*x,self.backend.bk_imag(y)*x)
         
     def dodiv(self,x,y):
         if x.dtype==y.dtype:
             return x/y
-        if x.dtype=='complex64' or x.dtype=='complex128':
-            
+        
+        if self.backend.bk_is_complex(x):
             return self.backend.bk_complex(self.backend.bk_real(x)/y,self.backend.bk_imag(x)/y)
         else:
             return self.backend.bk_complex(x/self.backend.bk_real(y),x/self.backend.bk_imag(y))
         
     def domin(self,x,y):
         if x.dtype==y.dtype:
             return x-y
-        if x.dtype=='complex64' or x.dtype=='complex128':
             
+        if self.backend.bk_is_complex(x):
             return self.backend.bk_complex(self.backend.bk_real(x)-y,self.backend.bk_imag(x)-y)
         else:
             return self.backend.bk_complex(x-self.backend.bk_real(y),x-self.backend.bk_imag(y))
         
     def doadd(self,x,y):
         if x.dtype==y.dtype:
             return x+y
-        if x.dtype=='complex64' or x.dtype=='complex128':
             
+        if self.backend.bk_is_complex(x):
             return self.backend.bk_complex(self.backend.bk_real(x)+y,self.backend.bk_imag(x)+y)
         else:
             return self.backend.bk_complex(x+self.backend.bk_real(y),x+self.backend.bk_imag(y))
                 
             
     def __mul__(self, other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
@@ -1071,15 +1071,15 @@
             M1_dic[j3] = M1
 
             if not cross:  # Auto
                 M1_square=self.backend.bk_real(M1_square)
                 
                 ### P00_auto = < M1^2 >_pix
                 # Apply the mask [Nmask, Npix_j3] and average over pixels
-                if M1_square.dtype=='complex64' or M1_square.dtype=='complex128':
+                if self.backend.bk_is_complex(M1_square):
                     p00 = self.backend.bk_reduce_sum(M1_square[:, None, :]*self.backend.bk_complex(vmask[None,:, :],0*vmask[None,:, :]), axis=2)
                 else:
                     p00 = self.backend.bk_reduce_sum(M1_square[:, None, :]*vmask[None,:, :], axis=2)
                     
                 if cond_init_P1_dic:
                     # We fill P1_dic with P00 for normalisation of C01 and C11
                     P1_dic[j3] = p00  # [Nbatch, Nmask, Norient3]
@@ -1091,15 +1091,15 @@
                     P00 = p00[:, :, None]  # Add a dimension for NP00
                 else:
                     P00 = self.backend.bk_concat([P00, p00[:, :, None]], axis=axis+2)
 
                 #### S1_auto computation
                 ### Image 1 : S1 = < M1 >_pix
                 # Apply the mask [Nmask, Npix_j3] and average over pixels
-                if M1.dtype=='complex64' or M1.dtype=='complex128':
+                if self.backend.bk_is_complex(M1):
                     s1 = self.backend.bk_reduce_sum(M1[:, None, :]*self.backend.bk_complex(vmask[None,:, :],0*vmask[None,:, :]), axis=2)
                 else:
                     s1 = self.backend.bk_reduce_sum(M1[:, None, :]*vmask[None,:, :], axis=2)
                     
                 ### Normalize S1
                 if norm is not None:
                     s1 /= (P1_dic[j3]) ** 0.5
@@ -1147,15 +1147,15 @@
                     P00 = p00[:,:,None,:]  # Add a dimension for NP00
                 else:
                     P00 = self.backend.bk_concat([P00, p00[:,:,None,:]], axis=2)
                     
                 #### S1_auto computation
                 ### Image 1 : S1 = < M1 >_pix
                 # Apply the mask [Nmask, Npix_j3] and average over pixels
-                if tmp.dtype=='complex64' or tmp.dtype=='complex128':
+                if self.backend.bk_is_complex(s1):
                     s1 = self.backend.bk_reduce_sum(tmp[:, None, :]*self.backend.bk_complex(vmask[None,:, :],0*vmask[None,:, :]), axis=2)
                 else:
                     s1 = self.backend.bk_reduce_sum(tmp[:, None, :]*vmask[None,:, :], axis=2)
                     
                 ### Normalize S1
                 if norm is not None:
                     s1 /= (P1_dic[j3]) ** 0.5
```

### Comparing `foscat-3.0.8/src/foscat/scat_cov2D.py` & `foscat-3.0.9/src/foscat/scat_cov2D.py`

 * *Files identical despite different names*

### Comparing `foscat-3.0.8/src/foscat.egg-info/SOURCES.txt` & `foscat-3.0.9/src/foscat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

