# Comparing `tmp/jftools-0.4.1.tar.gz` & `tmp/jftools-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jftools-0.4.1.tar", last modified: Thu Feb 22 12:03:57 2018, max compression
+gzip compressed data, was "jftools-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jftools-0.4.1.tar` & `jftools-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0       35 2017-05-16 15:32:31.000000 jftools-0.4.1/.gitattributes
--rw-r--r--   0        0        0     1063 2017-05-16 15:32:31.000000 jftools-0.4.1/.gitignore
--rw-r--r--   0        0        0     1071 2016-11-27 23:38:59.000000 jftools-0.4.1/LICENSE
--rw-r--r--   0        0        0      105 2016-11-27 23:38:59.000000 jftools-0.4.1/README.rst
--rw-r--r--   0        0        0        7 2017-05-16 15:32:31.000000 jftools-0.4.1/dev/.gitignore
--rw-r--r--   0        0        0     8226 2017-05-16 15:32:31.000000 jftools-0.4.1/dev/bench_spmv.ipynb
--rw-r--r--   0        0        0     6036 2017-05-16 15:32:31.000000 jftools-0.4.1/dev/check_dvr.ipynb
--rw-r--r--   0        0        0  1088281 2017-11-22 10:12:32.000000 jftools-0.4.1/dev/check_fedvr.ipynb
--rw-r--r--   0        0        0    25235 2017-05-16 15:32:31.000000 jftools-0.4.1/dev/dvrmod.f90
--rw-r--r--   0        0        0    16770 2017-05-16 15:32:31.000000 jftools-0.4.1/dev/test_sil.ipynb
--rw-r--r--   0        0        0      192 2016-11-27 23:38:59.000000 jftools-0.4.1/flit.ini
--rw-r--r--   0        0        0      542 2018-02-22 12:01:46.000000 jftools-0.4.1/jftools/__init__.py
--rw-r--r--   0        0        0    16608 2017-05-16 15:32:31.000000 jftools-0.4.1/jftools/fedvr.py
--rw-r--r--   0        0        0     1028 2017-05-16 15:32:31.000000 jftools-0.4.1/jftools/interpolate.py
--rw-r--r--   0        0        0     4548 2017-05-16 15:32:31.000000 jftools-0.4.1/jftools/ipynbimport.py
--rw-r--r--   0        0        0      382 2017-05-16 15:32:31.000000 jftools-0.4.1/jftools/myjit.py
--rw-r--r--   0        0        0      607 2017-05-16 15:32:31.000000 jftools-0.4.1/jftools/plotting.py
--rw-r--r--   0        0        0     1175 2017-05-16 15:32:31.000000 jftools-0.4.1/jftools/shade_color.py
--rw-r--r--   0        0        0     8804 2018-02-22 11:49:17.000000 jftools-0.4.1/jftools/short_iterative_lanczos.py
--rw-r--r--   0        0        0      204 2017-05-16 15:32:31.000000 jftools-0.4.1/jftools/tictoc.py
--rw-r--r--   0        0        0      843 2017-05-16 15:32:31.000000 jftools-0.4.1/jftools/unroll_phase.py
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 jftools-0.4.1/setup.py
--rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 jftools-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       35 2017-05-16 15:32:31.000000 jftools-0.4.2/.gitattributes
+-rw-r--r--   0        0        0      955 2024-05-24 08:34:57.110763 jftools-0.4.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1063 2017-05-16 15:32:31.000000 jftools-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1081 2024-01-24 16:59:47.451540 jftools-0.4.2/LICENSE
+-rw-r--r--   0        0        0       82 2024-01-24 17:00:48.594916 jftools-0.4.2/README.md
+-rw-r--r--   0        0        0        7 2017-05-16 15:32:31.000000 jftools-0.4.2/dev/.gitignore
+-rw-r--r--   0        0        0     8226 2024-05-25 14:05:09.103777 jftools-0.4.2/dev/bench_spmv.ipynb
+-rw-r--r--   0        0        0     6036 2017-05-16 15:32:31.000000 jftools-0.4.2/dev/check_dvr.ipynb
+-rw-r--r--   0        0        0     8835 2024-05-25 14:05:09.104163 jftools-0.4.2/dev/check_fedvr.ipynb
+-rw-r--r--   0        0        0    25235 2017-05-16 15:32:31.000000 jftools-0.4.2/dev/dvrmod.f90
+-rw-r--r--   0        0        0    16770 2017-05-16 15:32:31.000000 jftools-0.4.2/dev/test_sil.ipynb
+-rw-r--r--   0        0        0      538 2024-05-25 14:04:00.816619 jftools-0.4.2/jftools/__init__.py
+-rw-r--r--   0        0        0    21675 2024-05-24 08:35:29.866190 jftools-0.4.2/jftools/fedvr.py
+-rw-r--r--   0        0        0     1088 2024-05-25 14:01:36.549807 jftools-0.4.2/jftools/interpolate.py
+-rw-r--r--   0        0        0     4592 2024-05-25 13:45:13.172155 jftools-0.4.2/jftools/ipynbimport.py
+-rw-r--r--   0        0        0      398 2024-05-25 13:48:06.486873 jftools-0.4.2/jftools/myjit.py
+-rw-r--r--   0        0        0      616 2024-05-24 08:35:29.865345 jftools-0.4.2/jftools/plotting.py
+-rw-r--r--   0        0        0     1188 2024-05-25 14:01:26.319064 jftools-0.4.2/jftools/shade_color.py
+-rw-r--r--   0        0        0     9128 2024-05-25 14:01:36.550186 jftools-0.4.2/jftools/short_iterative_lanczos.py
+-rw-r--r--   0        0        0      208 2024-05-24 08:35:29.865372 jftools-0.4.2/jftools/tictoc.py
+-rw-r--r--   0        0        0     1040 2024-05-24 08:35:29.865548 jftools-0.4.2/jftools/unroll_phase.py
+-rw-r--r--   0        0        0      648 2024-05-25 13:58:18.756664 jftools-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 08:29:14.226362 jftools-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     2947 2024-05-24 08:35:29.865334 jftools-0.4.2/tests/test_all.py
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 jftools-0.4.2/PKG-INFO
```

### Comparing `jftools-0.4.1/.gitignore` & `jftools-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jftools-0.4.1/LICENSE` & `jftools-0.4.2/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
+The MIT License (MIT)
 
-Copyright (c) 2016 Johannes Feist
+Copyright (c) 2024 Johannes Feist
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `jftools-0.4.1/dev/bench_spmv.ipynb` & `jftools-0.4.2/dev/bench_spmv.ipynb`

 * *Files identical despite different names*

### Comparing `jftools-0.4.1/dev/check_dvr.ipynb` & `jftools-0.4.2/dev/check_dvr.ipynb`

 * *Files identical despite different names*

### Comparing `jftools-0.4.1/dev/dvrmod.f90` & `jftools-0.4.2/dev/dvrmod.f90`

 * *Files identical despite different names*

### Comparing `jftools-0.4.1/dev/test_sil.ipynb` & `jftools-0.4.2/dev/test_sil.ipynb`

 * *Files identical despite different names*

### Comparing `jftools-0.4.1/jftools/__init__.py` & `jftools-0.4.2/jftools/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Collection of small useful helper tools for Python by Johannes Feist."""
 
-__version__ = '0.4.1'
+__version__ = "0.4.2"
 
-__all__ = ['shade_color','tic','toc','ipynbimport_install','unroll_phase',
-           'interp_cmplx','plotcolored','fedvr','short_iterative_lanczos']
+__all__ = ["shade_color", "tic", "toc", "ipynbimport_install", "unroll_phase", "interp_cmplx", "plotcolored", "fedvr", "short_iterative_lanczos"]
 
 from .shade_color import shade_color
 from .tictoc import tic, toc
 from .ipynbimport import install as ipynbimport_install
 from .unroll_phase import unroll_phase
 from .interpolate import interp_cmplx
 from .plotting import plotcolored
```

### Comparing `jftools-0.4.1/jftools/fedvr.py` & `jftools-0.4.2/jftools/fedvr.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,120 +2,124 @@
 
 import scipy.linalg
 import numpy as np
 import math
 
 from .myjit import jit
 
+
 @jit(nopython=True)
 def simpsrule(n):
-    if n%2==0:
-        raise ValueError('n must be odd for simpson rule')
+    if n % 2 == 0:
+        raise ValueError("n must be odd for simpson rule")
     if n <= 1:
         t = np.zeros(1)
-        w = 2.*np.ones(1)
+        w = 2.0 * np.ones(1)
     else:
-        t = np.linspace(-1,1,n)
-        h = t[1]-t[0]
+        t = np.linspace(-1, 1, n)
+        h = t[1] - t[0]
         w = np.ones(n)
         w[1:-1:2] = 4
         w[2:-2:2] = 2
-        w *= h/3
-    return t,w
+        w *= h / 3
+    return t, w
+
 
 @jit(nopython=True)
-def classpol(ikind, n, alpha=0., beta=0.):
+def classpol(ikind, n, alpha=0.0, beta=0.0):
     # this procedure supplies the coefficients a(j), b(j) of the
     # recurrence relation
     #   b p (x) = (x - a ) p   (x) - b   p   (x)
     #    j j            j   j-1       j-1 j-2
     # for the various classical (normalized) orthogonal polynomials,
     # and the zero-th moment
     #   muzero = integral w(x) dx
     # of the given polynomial weight function w(x). since the
     # polynomials are orthonormalized, the tridiagonal matrix is
     # guaranteed to be symmetric.
     # the input parameter alpha is used only for laguerre and
     # jacobi polynomials, and the parameter beta is used only for
     # jacobi polynomials.  the laguerre and jacobi polynomials
     # require the gamma function.
-    if ikind==1:
+    if ikind == 1:
         # ikind = 1=  legendre polynomials p(x)
         # on (-1, +1), w(x) = 1.
-        muzero = 2.
+        muzero = 2.0
         a = np.zeros(n)
-        iis = np.arange(1,n)
-        b = iis/np.sqrt(4*iis**2-1)
-    elif ikind==2:
+        iis = np.arange(1, n)
+        b = iis / np.sqrt(4 * iis**2 - 1)
+    elif ikind == 2:
         # ikind = 2=  chebyshev polynomials of the first ikind t(x)
         # on (-1, +1), w(x) = 1 / sqrt(1 - x*x)
         muzero = np.pi
         a = np.zeros(n)
-        b = 0.5*np.ones(n-1)
+        b = 0.5 * np.ones(n - 1)
         b[0] = np.sqrt(0.5)
-    elif ikind==3:
+    elif ikind == 3:
         # ikind = 3=  chebyshev polynomials of the second ikind u(x)
         # on (-1, +1), w(x) = sqrt(1 - x*x)
-        muzero = np.pi/2.
+        muzero = np.pi / 2.0
         a = np.zeros(n)
-        b = 0.5*np.ones(n-1)
-    elif ikind==4:
+        b = 0.5 * np.ones(n - 1)
+    elif ikind == 4:
         # ikind = 4=  hermite polynomials h(x)
         # on (-infinity,+infinity), w(x) = exp(-x**2)
         muzero = np.sqrt(np.pi)
         a = np.zeros(n)
-        b = np.sqrt(np.arange(1,n)/2)
-    elif ikind==5:
+        b = np.sqrt(np.arange(1, n) / 2)
+    elif ikind == 5:
         # ikind = 5=  jacobi polynomials p(alpha, beta)(x)
         # on (-1, +1), w(x) = (1-x)**alpha + (1+x)**beta,
         # alpha and beta greater than -1
         alpha = float(alpha)
         beta = float(beta)
         ab = alpha + beta
-        abi = 2.+ab
-        muzero = 2.**(ab+1) * math.gamma(alpha+1) * math.gamma(beta+1.) / math.gamma(abi)
+        abi = 2.0 + ab
+        muzero = 2.0 ** (ab + 1) * math.gamma(alpha + 1) * math.gamma(beta + 1.0) / math.gamma(abi)
         a = np.empty(n)
-        b = np.empty(n-1)
-        a[0] = (beta - alpha)/abi
-        b[0] = np.sqrt(4.*(1.+alpha)*(1.+beta)/((abi+1.)*abi**2))
+        b = np.empty(n - 1)
+        a[0] = (beta - alpha) / abi
+        b[0] = np.sqrt(4.0 * (1.0 + alpha) * (1.0 + beta) / ((abi + 1.0) * abi**2))
         a2b2 = beta**2 - alpha**2
-        for ii in range(1,n-1):
+        for ii in range(1, n - 1):
             jj = ii + 1
-            abi = 2.*jj + ab
-            a[ii] = a2b2/((abi-2.)*abi)
-            b[ii] = np.sqrt(4.*jj*(jj+alpha)*(jj+beta)*(jj+ab)/((abi**2-1)*abi**2))
-        abi = 2.*n + ab
-        a[-1] = a2b2/((abi-2.)*abi)
-    elif ikind==6:
+            abi = 2.0 * jj + ab
+            a[ii] = a2b2 / ((abi - 2.0) * abi)
+            b[ii] = np.sqrt(4.0 * jj * (jj + alpha) * (jj + beta) * (jj + ab) / ((abi**2 - 1) * abi**2))
+        abi = 2.0 * n + ab
+        a[-1] = a2b2 / ((abi - 2.0) * abi)
+    elif ikind == 6:
         # ikind = 6=  laguerre polynomials l(alpha)(x)
         # on (0, +infinity), w(x) = exp(-x) * x**alpha, alpha greater than -1.
         alpha = float(alpha)
-        muzero = math.gamma(alpha+1.)
-        iis = np.arange(1,n+1)
-        a = 2*iis - 1 + alpha
-        b = np.sqrt(iis[:-1]*(iis[:-1]+alpha))
+        muzero = math.gamma(alpha + 1.0)
+        iis = np.arange(1, n + 1)
+        a = 2 * iis - 1 + alpha
+        b = np.sqrt(iis[:-1] * (iis[:-1] + alpha))
     return b, a, muzero
 
+
 @jit(nopython=True)
 def gbslve(shift, a, b):
     """this procedure performs elimination to solve for the
     n-th component of the solution delta to the equation
          (jn - shift*identity) * delta  = en,
     where en is the vector of all zeroes except for 1 in
     the n-th position.
     the matrix jn is symmetric tridiagonal, with diagonal
     elements a(i), off-diagonal elements b(i).  this equation
     must be solved to obtain the appropriate changes in the lower
     2 by 2 submatrix of coefficients for orthogonal polynomials."""
     alpha = a[0] - shift
-    for ii in range(1,len(a)-1):
-        alpha = a[ii] - shift - b[ii-1]**2/alpha
-    return 1./alpha
+    for ii in range(1, len(a) - 1):
+        alpha = a[ii] - shift - b[ii - 1] ** 2 / alpha
+    return 1.0 / alpha
+
 
-def gaussq(kind, n, endpts, alpha=0., beta=0.):
+def gaussq(kind, n, endpts, alpha=0.0, beta=0.0):
     #        this set of routines computes the nodes x(i) and weights
     #        c(i) for gaussian-type quadrature rules with pre-assigned
     #        nodes.  these are used when one wishes to approximate
 
     #                 integral (from a to b)  f(x) w(x) dx
 
     #                              n
@@ -135,17 +139,17 @@
     #     input parameters
 
     #        ikind     an integer between 0 and 6 giving the type of
     #                 quadrature rule
 
     #        ikind = 0=  simpson's rule w(x) = 1 on (-1, 1) n must be odd.
     #        ikind = 1=  legendre quadrature, w(x) = 1 on (-1, 1)
-    #        ikind = 2=  chebyshev quadrature of the first ikind
+    #        ikind = 2=  chebyshev quadrature of the first kind
     #                   w(x) = 1/dsqrt(1 - x*x) on (-1, +1)
-    #        ikind = 3=  chebyshev quadrature of the second ikind
+    #        ikind = 3=  chebyshev quadrature of the second kind
     #                   w(x) = dsqrt(1 - x*x) on (-1, 1)
     #        ikind = 4=  hermite quadrature, w(x) = exp(-x*x) on
     #                   (-infinity, +infinity)
     #        ikind = 5=  jacobi quadrature, w(x) = (1-x)**alpha * (1+x)**
     #                   beta on (-1, 1), alpha, beta .gt. -1.
     #                   note= ikind=2 and 3 are a special case of this.
     #        ikind = 6=  generalized laguerre quadrature, w(x) = exp(-x)*
@@ -207,199 +211,302 @@
     #            1969), pp. 221-230.
     #        2.  golub, g. h.,  some modified matrix eigenvalue problems,
     #            siam review 15 (april, 1973), pp. 318-334 (section 7).
     #        3.  stroud and secrest, gaussian quadrature formulas, prentice-
     #            hall, englewood cliffs, n.j., 1966.
 
     #     ..................................................................
-    kinds = ('simpson','legendre','chebyshev-1','chebyshev-2','hermite','jacobi','laguerre')
+    kinds = ("simpson", "legendre", "chebyshev-1", "chebyshev-2", "hermite", "jacobi", "laguerre")
     ikind = kinds.index(kind)
 
-    if ikind==0:
+    if ikind == 0:
         return simpsrule(n)
 
     b, t, muzero = classpol(ikind, n, alpha, beta)
     # the matrix of coefficients is assumed to be symmetric.
     # the array t contains the diagonal elements, the array
     # b the off-diagonal elements.
     # make appropriate changes in the lower right 2 by 2
     # submatrix.
 
-    if len(endpts)==1:
+    if len(endpts) == 1:
         # if kpts=1, only t(n) must be changed
-        t[-1] = gbslve(endpts[0], t, b) * b[-1]**2 + endpts[0]
-    elif len(endpts)==2:
+        t[-1] = gbslve(endpts[0], t, b) * b[-1] ** 2 + endpts[0]
+    elif len(endpts) == 2:
         # if kpts=2, t(n) and b(n-1) must be recomputed
         gam = gbslve(endpts[0], t, b)
         t1 = (endpts[0] - endpts[1]) / (gbslve(endpts[1], t, b) - gam)
         b[-1] = np.sqrt(t1)
-        t[-1] = endpts[0] + gam*t1
+        t[-1] = endpts[0] + gam * t1
 
     # now compute the eigenvalues of the symmetric tridiagonal
     # matrix, which has been modified as necessary.
-    # the method used is a ql-type method with origin shifting
 
     # upper form:
     # *   *   a02 a13 a24 a35
     # *   a01 a12 a23 a34 a45
     # a00 a11 a22 a33 a44 a55
-    A = np.empty((2,n))
-    A[0,1:] = b
-    A[1,:]  = t
+    A = np.empty((2, n))
+    A[0, 1:] = b
+    A[1, :] = t
     t, w = scipy.linalg.eig_banded(A)
-    w = muzero * w[0,:]**2
+    w = muzero * w[0, :] ** 2
     return t, w
 
+
 @jit(nopython=True)
-def lgngr(x,y):
+def lgngr(x, y):
     """Finds Lagrange interpolating polynomials of function of x
-and their first and second derivatives on an arbitrary grid y."""
+    and their first and second derivatives on an arbitrary grid y."""
     nx, ny = len(x), len(y)
-    p   = np.empty((ny,nx))
-    dp  = np.empty_like(p)
+    p = np.empty((ny, nx))
+    dp = np.empty_like(p)
     ddp = np.empty_like(p)
     #     generate polynomials and derivatives with respect to x
     for i in range(ny):
         zerfac = -1
         for j in range(nx):
-            if (abs(y[i]-x[j]) <= 1e-10):
+            if abs(y[i] - x[j]) <= 1e-10:
                 zerfac = j
         for j in range(nx):
-            p[i,j] = 1.
+            p[i, j] = 1.0
             for k in range(nx):
-                if k==j:
+                if k == j:
                     continue
-                p[i,j] *= (y[i]-x[k])/(x[j]-x[k])
-            if abs(p[i,j])>1e-10:
-                sn = 0.
-                ssn = 0.
+                p[i, j] *= (y[i] - x[k]) / (x[j] - x[k])
+            if abs(p[i, j]) > 1e-10:
+                sn = 0.0
+                ssn = 0.0
                 for k in range(nx):
-                    if k==j:
+                    if k == j:
                         continue
-                    fac = 1./(y[i]-x[k])
+                    fac = 1.0 / (y[i] - x[k])
                     sn += fac
                     ssn += fac**2
-                dp[i,j] = sn*p[i,j]
-                ddp[i,j] = sn*dp[i,j] - ssn*p[i,j]
+                dp[i, j] = sn * p[i, j]
+                ddp[i, j] = sn * dp[i, j] - ssn * p[i, j]
             else:
-                sn = 1.
-                ssn = 0.
+                sn = 1.0
+                ssn = 0.0
                 for k in range(nx):
-                    if k in (j,zerfac):
+                    if k in (j, zerfac):
                         continue
-                    fac = 1./(x[j]-x[k])
-                    sn *= fac*(y[i]-x[k])
-                    ssn += 1./(y[i]-x[k])
-                dp[i,j] = sn/(x[j]-x[zerfac])
-                ddp[i,j] = 2.*ssn*dp[i,j]
-    return p,dp,ddp
+                    fac = 1.0 / (x[j] - x[k])
+                    sn *= fac * (y[i] - x[k])
+                    ssn += 1.0 / (y[i] - x[k])
+                dp[i, j] = sn / (x[j] - x[zerfac])
+                ddp[i, j] = 2.0 * ssn * dp[i, j]
+    return p, dp, ddp
+
 
 class fedvr_region:
     # NB: the weight factors wt in each region
     # do NOT include the sum of the two weights
     # wt_n^i + wt_1^i+1 for the bridge functions!!
-    def __init__(self,nfun,bounds):
+    def __init__(self, nfun, bounds):
         self.nfun = nfun
 
         # Find zeros of nfun'th order Legendre quadrature (Gauss-Lobatto)
-        self.x, self.wt = gaussq('legendre',nfun,[-1,1])
+        self.x, self.wt = gaussq("legendre", nfun, [-1, 1])
 
         # Set up rescaled position grid
         xmin, xmax = bounds
-        A = abs(xmax-xmin)/2.
-        B = (xmax+xmin)/2.
-        self.x  = A*self.x + B
-        self.wt = A*self.wt
+        A = abs(xmax - xmin) / 2.0
+        B = (xmax + xmin) / 2.0
+        self.x = A * self.x + B
+        self.wt = A * self.wt
 
         # fix that the ends sometimes do not come out as exactly the given bounds
-        self.x[[0,-1]] = bounds
+        self.x[[0, -1]] = bounds
 
         # Generate Lagrange interpolating polynomials
         # and their first and second derivatives
-        f,self.dx,self.dx2 = lgngr(self.x,self.x)
+        f, self.dx, self.dx2 = lgngr(self.x, self.x)
 
         # Set up kinetic energy matrix
         # ke[function index, point index]
-        self.ke = self.dx2 * self.wt[:,None]
+        self.ke = self.dx2 * self.wt[:, None]
         # add the bloch contributions
-        self.ke[ 0,:] +=  f[ 0, 0]*self.dx[ 0,:]
-        self.ke[-1,:] += -f[-1,-1]*self.dx[-1,:]
+        self.ke[0, :] += f[0, 0] * self.dx[0, :]
+        self.ke[-1, :] += -f[-1, -1] * self.dx[-1, :]
         self.ke *= -0.5
 
+
 class fedvr_grid:
-    def __init__(self,nfun,xels):
+    def __init__(self, nfun, xels):
         from scipy.sparse import csr_matrix
 
         self.nfun = nfun
-        self.Nreg = len(xels)-1
+        self.Nreg = len(xels) - 1
         self.regs = []
-        nx = self.Nreg*(nfun-1)+1
-        self.x  = np.empty(nx)
+        nx = self.Nreg * (nfun - 1) + 1
+        self.x = np.empty(nx)
         # self.wt has to be initialized to zeros!
         self.wt = np.zeros_like(self.x)
         istart = 0
         for ii in range(self.Nreg):
-            reg = fedvr_region(nfun,xels[ii:ii+2])
+            reg = fedvr_region(nfun, xels[ii : ii + 2])
             iend = istart + reg.nfun
             self.regs.append(reg)
-            self.x [istart:iend]  = reg.x
+            self.x[istart:iend] = reg.x
             # the weights are additive (so bridge functions have sum of weights from the two elements)
             self.wt[istart:iend] += reg.wt
             # one grid point overlap
-            istart = iend-1
+            istart = iend - 1
 
-        dx = np.zeros([nx,nx])
+        dx = np.zeros([nx, nx])
         dx2 = np.zeros_like(dx)
         istart = 0
         for reg in self.regs:
-            iend = istart+reg.nfun
+            iend = istart + reg.nfun
+            # we have to multiply by the weights here to take into account that
+            # the bridge function weight is actually different from the element weight
+            wtcorr = 1.0 / np.sqrt(self.wt[istart:iend, None] * self.wt[None, istart:iend])
+            dx[istart:iend, istart:iend] += reg.dx * reg.wt[:, None] * wtcorr
+            # we use the "ke" (kinetic energy) matrix, which treats the second derivatives correctly at the boundaries
+            dx2[istart:iend, istart:iend] += -2 * reg.ke * wtcorr
+            istart = iend - 1
+        # make dx explicitly anti-hermitian (this also set the diagonal to zero)
+        self.dx = csr_matrix(0.5 * (dx - dx.T))
+        # make dx2 explicitly hermitian
+        self.dx2 = csr_matrix(0.5 * (dx2 + dx2.T))
+
+    def __repr__(self):
+        return "FEDVR basis: Rmin=%s, Rmax=%s, nfun=%s, nreg=%s, NR=%s" % (self.x[0], self.x[-1], self.nfun, self.Nreg, len(self.x))
+
+    def project_function(self, f):
+        """Takes a function f(x) and returns the coefficients c_n representing it in the FEDVR basis, f̃ = Σ c_n ϕ_n(x).
+        f must be callable with an array."""
+        return f(self.x) * np.sqrt(self.wt)
+
+    def evaluate_basis(self, cn, xs):
+        """Takes FEDVR basis coefficients c_n and returns the function values at points xs."""
+        fvals = self.get_basis_function_values(xs)
+        return cn.dot(fvals)
+
+    def get_basis_function_values(self, xs):
+        """Returns an array F_ni=f_n(x_i), where f_n(x) are the orthonormalized basis functions we use."""
+        # only interior points
+        xels = [reg.x[0] for reg in self.regs[1:]]
+        # searchsorted returns the index at which to insert into a sorted array to keep the order
+        # this is the same as the finite element number containing the point for us
+        reginds = np.searchsorted(xels, xs)
+        fvals = np.zeros([len(self.x), len(xs)])
+        istart = 0
+        for ireg, reg in enumerate(self.regs):
+            # find xs that are in this region
+            regixs = np.where(ireg == reginds)
+            if len(regixs) == 0:
+                continue
+            # construct basis functions = Lagrange interpolating polynomials with weight,
+            # f_i(x_j) = δ_ij/sqrt(w_i)
+            # f_i(x) = 1/sqrt(w_i) Π_{j≠i} (x-x_j)/(x_i-x_j)
+            for ibas, xbas in enumerate(reg.x, start=istart):
+                # we have to use the _global_ weight self.wt here, which treats the bridge functions correctly
+                fvals[ibas, regixs] = 1.0 / np.sqrt(self.wt[ibas])
+                for ix, xp in enumerate(reg.x, start=istart):
+                    if ibas != ix:
+                        fvals[ibas, regixs] *= (xs[regixs] - xp) / (xbas - xp)
+            # next element starts nfun-1 basis functions later (-1 because of bridge function)
+            istart += reg.nfun - 1
+        return fvals
+
+
+class fedvr_grid_ecs:
+    def __init__(self, nfun, xels, xels_ecs, ecs_angle):
+        from scipy.sparse import csr_matrix
+
+        assert xels[-1] == xels_ecs[0]
+        self.nfun = nfun
+        self.ecs_angle = ecs_angle
+        self.Nreg_real = len(xels) - 1
+        self.Nreg_ecs = len(xels_ecs) - 1
+        self.Nreg = self.Nreg_real + self.Nreg_ecs
+        self.regs = []
+        nx = self.Nreg * (nfun - 1) + 1
+        self.x = np.empty(nx)
+        # self.wt has to be initialized to zeros!
+        self.wt = np.zeros(nx, dtype=complex)
+        istart = 0
+        for ii in range(self.Nreg_real):
+            reg = fedvr_region(nfun, xels[ii : ii + 2])
+            iend = istart + reg.nfun
+            self.regs.append(reg)
+            self.x[istart:iend] = reg.x
+            # the weights are additive (so bridge functions have sum of weights from the two elements)
+            self.wt[istart:iend] += reg.wt
+            # one grid point overlap
+            istart = iend - 1
+
+        for ii in range(self.Nreg_ecs):
+            reg = fedvr_region(nfun, xels_ecs[ii : ii + 2])
+            # do complex rotation
+            reg.ke = reg.ke * np.exp(-1j * ecs_angle)
+            # reg.first_deriv does not get a factor from complex rotation
+            reg.wt = reg.wt * np.exp(1j * ecs_angle)
+            self.regs.append(reg)
+
+            iend = istart + reg.nfun
+            self.x[istart:iend] = reg.x
+            # the weights are additive (so bridge functions have sum of weights from the two elements)
+            self.wt[istart:iend] += reg.wt
+            # one grid point overlap
+            istart = iend - 1
+
+        dx = np.zeros([nx, nx], dtype=complex)
+        dx2 = np.zeros_like(dx)
+        istart = 0
+        for reg in self.regs:
+            iend = istart + reg.nfun
             # we have to multiply by the weights here to take into account that
             # the bridge function weight is actually different from the element weight
-            wtcorr = 1./np.sqrt(self.wt[istart:iend,None]*self.wt[None,istart:iend])
-            dx [istart:iend,istart:iend] += reg.dx*reg.wt[:,None] * wtcorr
+            wtcorr = 1.0 / np.sqrt(self.wt[istart:iend, None] * self.wt[None, istart:iend])
+            dx[istart:iend, istart:iend] += reg.dx * reg.wt[:, None] * wtcorr
             # we use the "ke" (kinetic energy) matrix, which treats the second derivatives correctly at the boundaries
-            dx2[istart:iend,istart:iend] += -2 * reg.ke * wtcorr
-            istart = iend-1
+            dx2[istart:iend, istart:iend] += -2 * reg.ke * wtcorr
+            istart = iend - 1
         # make dx explicitly anti-hermitian (this also set the diagonal to zero)
-        self.dx = csr_matrix(0.5*(dx-dx.T))
+        # self.dx = csr_matrix(0.5*(dx-dx.T))
         # make dx2 explicitly hermitian
-        self.dx2 = csr_matrix(0.5*(dx2+dx2.T))
+        # self.dx2 = csr_matrix(0.5*(dx2+dx2.T))
+        self.dx = csr_matrix(dx)
+        self.dx2 = csr_matrix(dx2)
 
     def __repr__(self):
-        return "FEDVR basis: Rmin=%s, Rmax=%s, nfun=%s, nreg=%s, NR=%s"%(self.x[0], self.x[-1], self.nfun, self.Nreg, len(self.x))
+        return f"FEDVR basis: Rmin={self.x[0]}, Rmax={self.x[-1]}, nfun={self.nfun}, nreg={self.Nreg}, NR={len(self.x)}, Recs={self.reg[self.Nreg_real-1].x[-1]}, θecs={self.ecs_angle}"
 
-    def project_function(self,f):
+    def project_function(self, f):
         """Takes a function f(x) and returns the coefficients c_n representing it in the FEDVR basis, f̃ = Σ c_n ϕ_n(x).
         f must be callable with an array."""
         return f(self.x) * np.sqrt(self.wt)
 
-    def evaluate_basis(self,cn,xs):
+    def evaluate_basis(self, cn, xs):
         """Takes FEDVR basis coefficients c_n and returns the function values at points xs."""
         fvals = self.get_basis_function_values(xs)
         return cn.dot(fvals)
 
-    def get_basis_function_values(self,xs):
+    def get_basis_function_values(self, xs):
         """Returns an array F_ni=f_n(x_i), where f_n(x) are the orthonormalized basis functions we use."""
         # only interior points
         xels = [reg.x[0] for reg in self.regs[1:]]
         # searchsorted returns the index at which to insert into a sorted array to keep the order
         # this is the same as the finite element number containing the point for us
         reginds = np.searchsorted(xels, xs)
-        fvals = np.zeros([len(self.x),len(xs)])
+        fvals = np.zeros([len(self.x), len(xs)])
         istart = 0
-        for ireg,reg in enumerate(self.regs):
+        for ireg, reg in enumerate(self.regs):
             # find xs that are in this region
-            regixs = np.where(ireg==reginds)
-            if len(regixs)==0:
+            regixs = np.where(ireg == reginds)
+            if len(regixs) == 0:
                 continue
             # construct basis functions = Lagrange interpolating polynomials with weight,
             # f_i(x_j) = δ_ij/sqrt(w_i)
             # f_i(x) = 1/sqrt(w_i) Π_{j≠i} (x-x_j)/(x_i-x_j)
-            for ibas, xbas in enumerate(reg.x,start=istart):
+            for ibas, xbas in enumerate(reg.x, start=istart):
                 # we have to use the _global_ weight self.wt here, which treats the bridge functions correctly
-                fvals[ibas,regixs] = 1./np.sqrt(self.wt[ibas])
-                for ix, xp in enumerate(reg.x,start=istart):
-                    if ibas!=ix:
-                        fvals[ibas,regixs] *= (xs[regixs] - xp) / (xbas - xp)
+                fvals[ibas, regixs] = 1.0 / np.sqrt(self.wt[ibas])
+                for ix, xp in enumerate(reg.x, start=istart):
+                    if ibas != ix:
+                        fvals[ibas, regixs] *= (xs[regixs] - xp) / (xbas - xp)
             # next element starts nfun-1 basis functions later (-1 because of bridge function)
-            istart += reg.nfun-1
+            istart += reg.nfun - 1
         return fvals
```

### Comparing `jftools-0.4.1/jftools/ipynbimport.py` & `jftools-0.4.2/jftools/ipynbimport.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,44 +5,50 @@
 # This is made difficult by the fact that Notebooks are not plain Python files,
 # and thus cannot be imported by the regular Python machinery.
 #
 # Fortunately, Python provides some fairly sophisticated [hooks](http://www.python.org/dev/peps/pep-0302/) into the import machinery,
 # so we can actually make IPython notebooks importable without much difficulty,
 # and only using public APIs.
 
-import io, os, sys, types
+import io
+import os
+import sys
+import types
+
 try:
     import nbformat
 except ImportError:
     from IPython import nbformat
 from IPython.core.interactiveshell import InteractiveShell
 
+
 # Import hooks typically take the form of two objects:
 #
 # 1. a Module **Loader**, which takes a module name (e.g. `'IPython.display'`), and returns a Module
 # 2. a Module **Finder**, which figures out whether a module might exist, and tells Python what **Loader** to use
 def find_notebook(fullname, path=None):
     """find a notebook, given its fully qualified name and an optional path
 
     This turns "foo.bar" into "foo/bar.ipynb"
     and tries turning "Foo_Bar" into "Foo Bar" if Foo_Bar
     does not exist.
     """
-    name = fullname.rsplit('.', 1)[-1]
+    name = fullname.rsplit(".", 1)[-1]
     if not path:
-        path = ['']
+        path = [""]
     for d in path:
         nb_path = os.path.join(d, name + ".ipynb")
         if os.path.isfile(nb_path):
             return nb_path
         # let import Notebook_Name find "Notebook Name.ipynb"
         nb_path = nb_path.replace("_", " ")
         if os.path.isfile(nb_path):
             return nb_path
 
+
 ### Notebook Loader
 # Here we have our Notebook Loader.
 # It's actually quite simple - once we figure out the filename of the module,
 # all it does is:
 #
 # 1. load the notebook document into memory
 # 2. create an empty Module
@@ -50,49 +56,49 @@
 #
 # Since IPython cells can have extended syntax,
 # the IPython transform is applied to turn each of these cells into their pure-Python counterparts before executing them.
 # If all of your notebook cells are pure-Python,
 # this step is unnecessary.
 class NotebookLoader(object):
     """Module Loader for IPython Notebooks"""
+
     def __init__(self, path=None):
         self.shell = InteractiveShell.instance()
         self.path = path
 
     def load_module(self, fullname):
         """import a notebook as a module"""
         path = find_notebook(fullname, self.path)
 
-        print ("importing IPython notebook from %s" % path)
+        print("importing IPython notebook from %s" % path)
 
         # load the notebook object
-        with io.open(path, 'r', encoding='utf-8') as f:
+        with io.open(path, "r", encoding="utf-8") as f:
             nb = nbformat.read(f, 4)
 
-
         # create the module and add it to sys.modules
         # if name in sys.modules:
         #    return sys.modules[name]
         mod = types.ModuleType(fullname)
         mod.__file__ = path
         mod.__loader__ = self
         sys.modules[fullname] = mod
 
         # extra work to ensure that magics that would affect the user_ns
         # actually affect the notebook module's ns
         save_user_ns = self.shell.user_ns
         self.shell.user_ns = mod.__dict__
 
         try:
-          for cell in nb.cells:
-            if cell.cell_type == 'code':
-                # transform the input to executable Python
-                code = self.shell.input_transformer_manager.transform_cell(cell.source)
-                # run the code in themodule
-                exec(code, mod.__dict__)
+            for cell in nb.cells:
+                if cell.cell_type == "code":
+                    # transform the input to executable Python
+                    code = self.shell.input_transformer_manager.transform_cell(cell.source)
+                    # run the code in themodule
+                    exec(code, mod.__dict__)
         finally:
             self.shell.user_ns = save_user_ns
         return mod
 
 
 ### The Module Finder
 # The finder is a simple object that tells you whether a name can be imported,
@@ -105,14 +111,15 @@
 #
 # it checks whether `mynotebook.ipynb` exists.
 # If a notebook is found, then it returns a NotebookLoader.
 #
 # Any extra logic is just for resolving paths within packages.
 class NotebookFinder(object):
     """Module finder that locates IPython Notebooks"""
+
     def __init__(self):
         self.loaders = {}
 
     def find_module(self, fullname, path=None):
         nb_path = find_notebook(fullname, path)
         if not nb_path:
             return
@@ -122,11 +129,12 @@
             # lists aren't hashable
             key = os.path.sep.join(path)
 
         if key not in self.loaders:
             self.loaders[key] = NotebookLoader(path)
         return self.loaders[key]
 
+
 ### Register the hook
 # Now we register the `NotebookFinder` with `sys.meta_path`
 def install():
     sys.meta_path.append(NotebookFinder())
```

### Comparing `jftools-0.4.1/jftools/plotting.py` & `jftools-0.4.2/jftools/plotting.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import numpy as np
 import matplotlib as mpl
 from matplotlib.collections import LineCollection
 
-def plotcolored(ax,x,y,c,*,lw=None,cmap=None,norm=None):
+
+def plotcolored(ax, x, y, c, *, lw=None, cmap=None, norm=None):
     if lw is None:
-        lw = mpl.rcParams['lines.linewidth']
+        lw = mpl.rcParams["lines.linewidth"]
     if cmap is None:
-        cmap = mpl.rcParams['image.cmap']
+        cmap = mpl.rcParams["image.cmap"]
     if norm is None:
-        norm = mpl.colors.Normalize(vmin=0,vmax=1)
+        norm = mpl.colors.Normalize(vmin=0, vmax=1)
     points = np.array([x, y]).T.reshape(-1, 1, 2)
     segments = np.concatenate([points[:-1], points[1:]], axis=1)
     lc = LineCollection(segments, cmap=cmap, norm=norm)
     lc.set_array(c)
     lc.set_linewidth(lw)
     ax.add_collection(lc)
     return lc
```

### Comparing `jftools-0.4.1/jftools/shade_color.py` & `jftools-0.4.2/jftools/shade_color.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # taken from https://github.com/matplotlib/matplotlib/pull/2745
 # Copyright (c) 2012- Matplotlib Development Team; All Rights Reserved
 def shade_color(color, percent):
     """
     A color helper utility to either darken or lighten given color.
     This color utility function allows the user to easily darken or lighten a color for
-    plotting purposes.  This function first converts the given color to RGB using 
-    ColorConverter and then to HSL.  The saturation is modified according to the given 
+    plotting purposes.  This function first converts the given color to RGB using
+    ColorConverter and then to HSL.  The saturation is modified according to the given
     percentage and converted back to RGB.
     Parameters
     ----------
     color : string, list, hexvalue
         Any acceptable Matplotlib color value, such as 'red', 'slategrey', '#FFEE11', (1,0,0)
     percent :  the amount by which to brighten or darken the color.
     Returns
     -------
     color : tuple of floats
         tuple representing converted rgb values
     """
     from matplotlib.colors import colorConverter
     from colorsys import rgb_to_hls, hls_to_rgb
     import numpy as np
-    r,g,b = colorConverter.to_rgb(color)
-    h,l,s = rgb_to_hls(r,g,b)
-    l *= 1 + float(percent)/100
-    l = np.clip(l, 0, 1)
-    r,g,b = hls_to_rgb(h,l,s)
-    return r,g,b
+
+    R, G, B = colorConverter.to_rgb(color)
+    H, L, S = rgb_to_hls(R, G, B)
+    L *= 1 + float(percent) / 100
+    L = np.clip(L, 0, 1)
+    R, G, B = hls_to_rgb(H, L, S)
+    return R, G, B
```

### Comparing `jftools-0.4.1/jftools/short_iterative_lanczos.py` & `jftools-0.4.2/jftools/short_iterative_lanczos.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,170 +2,188 @@
 from numpy import einsum, empty, zeros, vdot, log10, exp
 from numpy.linalg import norm
 from scipy.linalg import eig_banded
 import warnings
 
 try:
     import qutip
+
     have_qutip = True
-except:
+except ImportError:
     have_qutip = False
 
+
 class normdotndarray(np.ndarray):
     """extension of numpy array that supports interface for lanczos_timeprop"""
+
     def norm(self):
         return norm(self)
-    def dot(self,other):
-        return vdot(self,other)
+
+    def dot(self, other):
+        return vdot(self, other)
+
 
 def calc_coeff(step, a_band, HT, coeff):
-    vals, vecs = eig_banded(a_band[:,:step],lower=False,overwrite_a_band=False)
+    vals, vecs = eig_banded(a_band[:, :step], lower=False, overwrite_a_band=False)
     # expH(j,k) = vecs(j,i) * exp(vals(i)) * delta(i,l) * transpose(vecs(l,k))
     # expH(j,k) = vecs(j,i) * exp(vals(i)) * vecs(k,i)
-    coeff[:step] = einsum('ji,i,i->j',vecs,vecs[0],exp(-1j*HT*vals))
-    coeff[step:] = 0.
+    coeff[:step] = einsum("ji,i,i->j", vecs, vecs[0], exp(-1j * HT * vals))
+    coeff[step:] = 0.0
     return coeff
 
+
 class lanczos_timeprop:
-    def __init__(self,H,maxsteps,target_convg,debug=0,do_full_order=False):
-        if have_qutip and isinstance(H,qutip.Qobj):
+    def __init__(self, H, maxsteps, target_convg, debug=0, do_full_order=False):
+        if have_qutip and isinstance(H, qutip.Qobj):
             H = H.data
 
         if not callable(H):
             # time-independent operator
             # assume it supports .dot for matrix-vector multiplication
-            def Hfun(t,phi,Hphi):
+            def Hfun(t, phi, Hphi):
                 Hphi[:] = H.dot(phi)
                 return Hphi
+
             self.Hfun = Hfun
         else:
             self.Hfun = H
 
         self.maxsteps = maxsteps
         self.target_convg = target_convg
-        self.prefacs = empty(maxsteps+1)
+        self.prefacs = empty(maxsteps + 1)
         # this is the array that will hold the banded matrix
-        self.a_band = empty((2,maxsteps+1))
+        self.a_band = empty((2, maxsteps + 1))
         self.debug = debug
         self.do_full_order = do_full_order
 
-        self.curr_coeff = zeros(maxsteps+1,dtype=complex)
+        self.curr_coeff = zeros(maxsteps + 1, dtype=complex)
         self.prev_coeff = self.curr_coeff.copy()
 
-    def propagate(self,phi0,ts,maxHT=None):
+    def propagate(self, phi0, ts, maxHT=None):
         ts = np.asarray(ts)
-        assert ts.ndim==1, 'ts must be a 1d array'
+        assert ts.ndim == 1, "ts must be a 1d array"
+
+        def get_phi_out(x):
+            return x.copy()
+
+        if isinstance(phi0, np.ndarray):
+
+            def get_phi_out(x):
+                return x.view(np.ndarray).copy()
 
-        get_phi_out = lambda x: x.copy()
-        if isinstance(phi0,np.ndarray):
-            get_phi_out = lambda x: x.view(np.ndarray).copy()
             phi0 = phi0.view(normdotndarray)
-        elif have_qutip and isinstance(phi0,qutip.Qobj):
+        elif have_qutip and isinstance(phi0, qutip.Qobj):
             outdims = phi0.dims.copy()
             outtype = phi0.type
-            get_phi_out = lambda x: qutip.Qobj(x,dims=outdims,type=outtype)
+
+            def get_phi_out(x):
+                return qutip.Qobj(x, dims=outdims, type=outtype)
+
             phi0 = phi0.full().view(normdotndarray)
 
-        self.phia = [phi0.copy() for _ in range(self.maxsteps+1)]
+        self.phia = [phi0.copy() for _ in range(self.maxsteps + 1)]
 
         ids = np.array([id(x) for x in self.phia])
 
         tt = ts[0]
         phis = [get_phi_out(phi0)]
         for tf in ts[1:]:
-            while tt<tf:
-                HT = tf-tt
+            while tt < tf:
+                HT = tf - tt
                 if maxHT is not None:
-                    HT = min(HT,maxHT)
-                HT_done = self._step(tt,HT)
+                    HT = min(HT, maxHT)
+                HT_done = self._step(tt, HT)
                 tt += HT_done
             phis.append(get_phi_out(self.phia[0]))
 
-        if not np.all(ids==np.array([id(x) for x in self.phia])):
-            warnings.warn('self.phia have not been updated in-place!')
+        if not np.all(ids == np.array([id(x) for x in self.phia])):
+            warnings.warn("self.phia have not been updated in-place!")
 
         return phis
 
-    def _step(self,t,HT):
+    def _step(self, t, HT):
         # create local variables that use the class storage locations
         beta, alpha = self.a_band
         phia = self.phia
         prefacs = self.prefacs
         curr_coeff = self.curr_coeff
         prev_coeff = self.prev_coeff
         debug = self.debug
         Hfun = self.Hfun
 
         HT_done = HT
 
         # initialize norm of starting vector
         phinorm = phia[0].norm()
-        prefacs[0] = 1. / phinorm
+        prefacs[0] = 1.0 / phinorm
 
         # set current solution vector to zero so that it
         # doesn't converge at first step
-        curr_coeff[:] = 0.
+        curr_coeff[:] = 0.0
 
-        for step in range(1, self.maxsteps+1):
+        for step in range(1, self.maxsteps + 1):
             # set |phia(step)> to H|phia(step-1)>
-            phia[step] = Hfun(t,phia[step-1],phia[step])
-            prefacs[step] = prefacs[step-1]
+            phia[step] = Hfun(t, phia[step - 1], phia[step])
+            prefacs[step] = prefacs[step - 1]
             phinorm = prefacs[step] * phia[step].norm()
             # phinorm = sqrt(<q(step-1)|H H|q(step-1)>)
             # build lanczos-matrix
             # it's tridiagonal, so we only need two steps in the loop
             # start with step-1 for numerical reasons - this should ensure better orthogonality by
             # removing the potentially largest part (by a significant amount) first
-            dotpr = prefacs[step-1] * prefacs[step] * phia[step-1].dot(phia[step])
+            dotpr = prefacs[step - 1] * prefacs[step] * phia[step - 1].dot(phia[step])
             # don't use too stringent a criterion here, as the dot product does not contain squares
-            if abs(dotpr.imag) > 1e-9 and debug>3:
-                print('imaginary part of dotpr !=0:', dotpr.imag)
-            alpha[step-1] = dotpr.real
+            if abs(dotpr.imag) > 1e-9 and debug > 3:
+                print("imaginary part of dotpr !=0:", dotpr.imag)
+            alpha[step - 1] = dotpr.real
 
-            phia[step] -= alpha[step-1] * prefacs[step-1]/prefacs[step] * phia[step-1]
+            phia[step] -= alpha[step - 1] * prefacs[step - 1] / prefacs[step] * phia[step - 1]
 
             # phinorm     = sqrt(<q(step-1)|H H|q(step-1)>)
             # alpha(step) = <q(step-1)| H |q(step-1)>
             # abs(phinorm**2 - alpha(step)**2) is deltaH**2, i.e. a measure of how close q(step-1) is
             #   to being an eigenvector of H. if this is a small number, we take another
             #   gram-schmidt step to ensure that we have good orthogonality
-            if abs(phinorm**2-alpha[step-1]**2) < 0.1:
-                dotpr = prefacs[step-1] * prefacs[step] * phia[step-1].dot(phia[step])
-                phia[step] -= dotpr * prefacs[step-1]/prefacs[step] * phia[step-1]
+            if abs(phinorm**2 - alpha[step - 1] ** 2) < 0.1:
+                dotpr = prefacs[step - 1] * prefacs[step] * phia[step - 1].dot(phia[step])
+                phia[step] -= dotpr * prefacs[step - 1] / prefacs[step] * phia[step - 1]
             if step >= 2:
-                phia[step] -= beta[step-1] * prefacs[step-2] / prefacs[step] * phia[step-2]
+                phia[step] -= beta[step - 1] * prefacs[step - 2] / prefacs[step] * phia[step - 2]
 
             # ************ normalize phia(step) to get q_step ***************
             # be careful here: beta should be the norm of the
             # current q_step == prefac * |phi>,
             # i.e. beta = prefac * sqrt(<phi|phi>)
             # after that, we set prefac to _normalize_ the vector |phi>,
             # i.e. to prefac = 1.d0 / sqrt(<phi|phi>)
             phinorm = phia[step].norm()
             beta[step] = prefacs[step] * phinorm
-            prefacs[step] = 1. / phinorm
-            if abs(log10(prefacs[step])) > 4.:
+            prefacs[step] = 1.0 / phinorm
+            if abs(log10(prefacs[step])) > 4.0:
                 phia[step] *= prefacs[step]
-                prefacs[step] = 1.
+                prefacs[step] = 1.0
             if abs(beta[step]) < 1e-2 and debug > 2:
-                print('WARNING! beta[%d]=%g is very small - there seems to be a linearly dependent vector!'%(step,beta[step]))
+                print("WARNING! beta[%d]=%g is very small - there seems to be a linearly dependent vector!" % (step, beta[step]))
             if debug > 1:
                 # check if new vector is orthogonal to all others
                 for ii in range(step):
                     dotpr = prefacs[ii] * prefacs[step] * phia[ii].dot(phia[step])
                 if abs(dotpr) > 1e-12:
-                    print('WARNING! vectors not orthogonal. dotpr(%d,%d) = %g'%(ii,step,dotpr))
+                    print("WARNING! vectors not orthogonal. dotpr(%d,%d) = %g" % (ii, step, dotpr))
 
             # check convergence
             prev_coeff[:] = curr_coeff[:]
             calc_coeff(step, self.a_band, HT_done, curr_coeff)
-            convg = norm(curr_coeff-prev_coeff)
-            if debug > 6: print('prev_coeff:', prev_coeff)
-            if debug > 6: print('curr_coeff:', curr_coeff)
-            if debug > 5: print('convg:', convg)
+            convg = norm(curr_coeff - prev_coeff)
+            if debug > 6:
+                print("prev_coeff:", prev_coeff)
+            if debug > 6:
+                print("curr_coeff:", curr_coeff)
+            if debug > 5:
+                print("convg:", convg)
 
             if not self.do_full_order and convg < self.target_convg:
                 break
 
         if debug > 8:
             print(alpha[0:step])
             print(beta[1:step])
@@ -173,38 +191,42 @@
         # if convergence was reached in lanczos_loop, convg < target_convg, and this loop is never entered
         while convg > self.target_convg:
             # error (~convg) should be O(HT**maxsteps)
             # convg = a * HT**maxsteps
             # target_convg = a * HT_new**maxsteps
             # target_convg/convg = (HT_new/HT)**maxsteps
             # -> HT_new = HT * (target_convg/convg)**(1/maxsteps)
-            scale = 0.95 * (self.target_convg/convg)**(1./step)
+            scale = 0.95 * (self.target_convg / convg) ** (1.0 / step)
             # the 0.95d0 is to get convergence when we're very close
             # and scale would be almost unity
             # to prevent going to much too small steps when very far from convergence, decrease
             # step size by at most one half
-            scale = max(0.5,scale)
+            scale = max(0.5, scale)
             if debug > 3:
-                print('scales HT with scale =', scale)
+                print("scales HT with scale =", scale)
             HT_done = HT_done * scale
-            calc_coeff(step-1, self.a_band, HT_done, prev_coeff)
-            calc_coeff(step  , self.a_band, HT_done, curr_coeff)
-            convg = norm(curr_coeff-prev_coeff)
-            if debug > 6: print('prev_coeff:', abs(prev_coeff)**2)
-            if debug > 6: print('curr_coeff:', abs(curr_coeff)**2)
-            if debug > 5: print('convg:', convg)
+            calc_coeff(step - 1, self.a_band, HT_done, prev_coeff)
+            calc_coeff(step, self.a_band, HT_done, curr_coeff)
+            convg = norm(curr_coeff - prev_coeff)
+            if debug > 6:
+                print("prev_coeff:", abs(prev_coeff) ** 2)
+            if debug > 6:
+                print("curr_coeff:", abs(curr_coeff) ** 2)
+            if debug > 5:
+                print("convg:", convg)
 
-        if debug > 6 and HT_done!=HT:
-            print('did not converge in %d iterations, step size decreased from %g to %g'%(self.maxsteps,HT,HT_done))
+        if debug > 6 and HT_done != HT:
+            print("did not converge in %d iterations, step size decreased from %g to %g" % (self.maxsteps, HT, HT_done))
 
         # build the new vector
         # do NOT include the prefactor prefac[0] into phi - we do not want to normalize it
         phia[0] *= curr_coeff[0]
-        cc = curr_coeff*prefacs/prefacs[0]
-        for ii in range(1,step+1):
+        cc = curr_coeff * prefacs / prefacs[0]
+        for ii in range(1, step + 1):
             phia[0] += cc[ii] * phia[ii]
 
         return HT_done
 
-def sesolve_lanczos(H,phi0,ts,maxsteps,target_convg,maxHT=None,debug=0,do_full_order=False):
-    prop = lanczos_timeprop(H,maxsteps,target_convg,debug,do_full_order)
-    return prop.propagate(phi0,ts,maxHT)
+
+def sesolve_lanczos(H, phi0, ts, maxsteps, target_convg, maxHT=None, debug=0, do_full_order=False):
+    prop = lanczos_timeprop(H, maxsteps, target_convg, debug, do_full_order)
+    return prop.propagate(phi0, ts, maxHT)
```

### Comparing `jftools-0.4.1/jftools/unroll_phase.py` & `jftools-0.4.2/jftools/unroll_phase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from .myjit import jit
 import numpy as np
 
+
 def unroll_phase(phases):
-    return _unroll_phase(np.asarray(phases))
+    # first convert to numpy array
+    phases = np.asarray(phases)
+    # then make sure it is at least float64
+    phases = np.asarray(phases, dtype=np.promote_types(phases.dtype, np.float64))
+    return _unroll_phase(phases)
+
 
 @jit(nopython=True)
 def _unroll_phase(phases):
-    TWOPI = 2*np.pi
+    TWOPI = 2 * np.pi
     # acc_phase keeps track of how many phase jumps by TWOPI we have accumulated
-    acc_phase = 0.
-    for ii in range(1,len(phases)):
+    acc_phase = 0.0
+    for ii in range(1, len(phases)):
         # the phase difference between the previous and current step,
         # including a possible phase jump of +-TWOPI
-        phase_diff = phases[ii] - phases[ii-1] - acc_phase
-        if abs(phase_diff-TWOPI)<abs(phase_diff):
+        phase_diff = phases[ii] - phases[ii - 1] - acc_phase
+        if abs(phase_diff - TWOPI) < abs(phase_diff):
             # if +TWOPI
-            acc_phase  += TWOPI
+            acc_phase += TWOPI
             phase_diff -= TWOPI
-        elif abs(phase_diff+TWOPI)<abs(phase_diff):
+        elif abs(phase_diff + TWOPI) < abs(phase_diff):
             # if -TWOPI
-            acc_phase  -= TWOPI
+            acc_phase -= TWOPI
             phase_diff += TWOPI
-        phases[ii] = phases[ii-1] + phase_diff
+        phases[ii] = phases[ii - 1] + phase_diff
     return phases
```

