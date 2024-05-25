# Comparing `tmp/deepmimov3-0.2.4.tar.gz` & `tmp/deepmimov3-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepmimov3-0.2.4.tar", last modified: Sun May 12 16:00:10 2024, max compression
+gzip compressed data, was "deepmimov3-0.2.5.tar", last modified: Sat May 25 18:02:51 2024, max compression
```

## Comparing `deepmimov3-0.2.4.tar` & `deepmimov3-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-12 16:00:10.403637 deepmimov3-0.2.4/
--rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-12 16:00:10.403637 deepmimov3-0.2.4/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)     3396 2024-05-11 15:36:00.000000 deepmimov3-0.2.4/README.md
--rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-05-12 16:00:10.403637 deepmimov3-0.2.4/setup.cfg
--rw-rw-r--   0 joao      (1000) joao      (1000)      933 2024-05-12 16:00:03.000000 deepmimov3-0.2.4/setup.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-12 16:00:10.403637 deepmimov3-0.2.4/src/
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-12 16:00:10.403637 deepmimov3-0.2.4/src/DeepMIMOv3/
--rw-rw-r--   0 joao      (1000) joao      (1000)      221 2024-05-11 15:36:00.000000 deepmimov3-0.2.4/src/DeepMIMOv3/__init__.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     2034 2024-05-11 15:36:00.000000 deepmimov3-0.2.4/src/DeepMIMOv3/ant_patterns.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    14187 2024-05-12 00:22:18.000000 deepmimov3-0.2.4/src/DeepMIMOv3/construct_deepmimo.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     3362 2024-05-11 15:36:00.000000 deepmimov3-0.2.4/src/DeepMIMOv3/consts.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    14786 2024-05-11 19:36:10.000000 deepmimov3-0.2.4/src/DeepMIMOv3/generator.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     3053 2024-05-11 15:36:00.000000 deepmimov3-0.2.4/src/DeepMIMOv3/params.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     7290 2024-05-11 15:36:00.000000 deepmimov3-0.2.4/src/DeepMIMOv3/raytracing_v2.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     8272 2024-05-11 15:36:00.000000 deepmimov3-0.2.4/src/DeepMIMOv3/raytracing_v3.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     5749 2024-05-11 15:36:00.000000 deepmimov3-0.2.4/src/DeepMIMOv3/sionna_adapter.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    11120 2024-05-12 02:08:27.000000 deepmimov3-0.2.4/src/DeepMIMOv3/utils.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     7316 2024-05-11 23:27:00.000000 deepmimov3-0.2.4/src/DeepMIMOv3/visualization.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-12 16:00:10.403637 deepmimov3-0.2.4/src/DeepMIMOv3.egg-info/
--rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-12 16:00:10.000000 deepmimov3-0.2.4/src/DeepMIMOv3.egg-info/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)      533 2024-05-12 16:00:10.000000 deepmimov3-0.2.4/src/DeepMIMOv3.egg-info/SOURCES.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-05-12 16:00:10.000000 deepmimov3-0.2.4/src/DeepMIMOv3.egg-info/dependency_links.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       28 2024-05-12 16:00:10.000000 deepmimov3-0.2.4/src/DeepMIMOv3.egg-info/requires.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       11 2024-05-12 16:00:10.000000 deepmimov3-0.2.4/src/DeepMIMOv3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 18:02:51.746134 deepmimov3-0.2.5/
+-rw-rw-rw-   0        0        0      470 2024-05-25 18:02:51.744138 deepmimov3-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3413 2022-12-25 16:46:43.000000 deepmimov3-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 18:02:51.746134 deepmimov3-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      963 2024-05-25 17:36:02.000000 deepmimov3-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 18:02:51.681135 deepmimov3-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 18:02:51.712134 deepmimov3-0.2.5/src/DeepMIMOv3/
+-rw-rw-rw-   0        0        0      224 2024-05-25 17:42:56.000000 deepmimov3-0.2.5/src/DeepMIMOv3/__init__.py
+-rw-rw-rw-   0        0        0     2090 2024-03-17 07:24:37.000000 deepmimov3-0.2.5/src/DeepMIMOv3/ant_patterns.py
+-rw-rw-rw-   0        0        0    14498 2024-05-25 08:35:51.000000 deepmimov3-0.2.5/src/DeepMIMOv3/construct_deepmimo.py
+-rw-rw-rw-   0        0        0     3467 2024-03-17 07:24:37.000000 deepmimov3-0.2.5/src/DeepMIMOv3/consts.py
+-rw-rw-rw-   0        0        0    15056 2024-05-25 08:35:51.000000 deepmimov3-0.2.5/src/DeepMIMOv3/generator.py
+-rw-rw-rw-   0        0        0     3128 2024-03-17 07:24:37.000000 deepmimov3-0.2.5/src/DeepMIMOv3/params.py
+-rw-rw-rw-   0        0        0     7453 2024-03-17 07:24:37.000000 deepmimov3-0.2.5/src/DeepMIMOv3/raytracing_v2.py
+-rw-rw-rw-   0        0        0     8454 2024-05-25 17:25:08.000000 deepmimov3-0.2.5/src/DeepMIMOv3/raytracing_v3.py
+-rw-rw-rw-   0        0        0     5876 2024-03-17 07:24:37.000000 deepmimov3-0.2.5/src/DeepMIMOv3/sionna_adapter.py
+-rw-rw-rw-   0        0        0    11412 2024-05-25 08:35:51.000000 deepmimov3-0.2.5/src/DeepMIMOv3/utils.py
+-rw-rw-rw-   0        0        0     7494 2024-05-25 17:49:30.000000 deepmimov3-0.2.5/src/DeepMIMOv3/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-25 18:02:51.743134 deepmimov3-0.2.5/src/DeepMIMOv3.egg-info/
+-rw-rw-rw-   0        0        0      470 2024-05-25 18:02:51.000000 deepmimov3-0.2.5/src/DeepMIMOv3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2024-05-25 18:02:51.000000 deepmimov3-0.2.5/src/DeepMIMOv3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 18:02:51.000000 deepmimov3-0.2.5/src/DeepMIMOv3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-25 18:02:51.000000 deepmimov3-0.2.5/src/DeepMIMOv3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-25 18:02:51.000000 deepmimov3-0.2.5/src/DeepMIMOv3.egg-info/top_level.txt
```

### Comparing `deepmimov3-0.2.4/README.md` & `deepmimov3-0.2.5/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# DeepMIMO: A Generic Deep Learning Dataset for Millimeter Wave and Massive MIMO Applications
-This is a python code package of the DeepMIMO dataset generated using [Remcom Wireless InSite](http://www.remcom.com/wireless-insite) software. The [DeepMIMO dataset](https://deepmimo.net/) is a publicly available parameterized dataset published for deep learning applications in mmWave and massive MIMO systems.
-
-This python code package is related to the following article: 
->Ahmed Alkhateeb, “[DeepMIMO: A Generic Deep Learning Dataset for Millimeter Wave and Massive MIMO Applications](https://arxiv.org/pdf/1902.06435.pdf),” in Proc. of Information Theory and Applications Workshop (ITA), San Diego, CA, Feb. 2019.
-# Abstract of the Article
-Machine learning tools are finding interesting applications in millimeter wave (mmWave) and massive MIMO systems. This is mainly thanks to their powerful capabilities in learning unknown models and tackling hard optimization problems. To advance the machine learning research in mmWave/massive MIMO, however, there is a need for a common dataset. This dataset can be used to evaluate the developed algorithms, reproduce the results, set *benchmarks*, and compare the different solutions. In this work, we introduce the DeepMIMO dataset, which is a generic dataset for mmWave/massive MIMO channels. The DeepMIMO dataset generation framework has two important features. First, the DeepMIMO channels are constructed based on accurate ray-tracing data obtained from Remcom Wireless InSite. The DeepMIMO channels, therefore, capture the dependence on the environment geometry/materials and transmitter/receiver locations, which is essential for several machine learning applications. Second, the DeepMIMO dataset is generic/parameterized as the researcher can adjust a set of system and channel parameters to tailor the generated DeepMIMO dataset for the target machine learning application. The DeepMIMO dataset can then be completely defined by the (i) the adopted ray-tracing scenario and (ii) the set of parameters, which enables the accurate definition and reproduction of the dataset. In this paper, an example DeepMIMO dataset is described based on an outdoor ray-tracing scenario of 18 base stations and more than one million users. The paper also shows how this dataset can be used in an example deep learning application of mmWave beam prediction.
-
-# Installation & Dataset Generation
-**To generate the dataset, please refer to [this website](https://deepmimo.net/versions/v2-python/) for the different dataset options and their generation steps.
-
-If you have any questions regarding the code and used dataset, please contact [Ahmed Alkhateeb](https://www.aalkhateeb.net/).
-
-# License and Referencing
-This code package is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/). If you in any way use this code for research that results in publications, please cite both the original article and the Remcom Wireless InSite website:
-> - A. Alkhateeb, “[DeepMIMO: A Generic Deep Learning Dataset for Millimeter Wave and Massive MIMO Applications](https://arxiv.org/pdf/1902.06435.pdf),” in Proc. of Information Theory and Applications Workshop (ITA), San Diego, CA, Feb. 2019.
-> - Remcom, Wireless insite, “http://www.remcom.com/wireless-insite”
+# DeepMIMO: A Generic Deep Learning Dataset for Millimeter Wave and Massive MIMO Applications
+This is a python code package of the DeepMIMO dataset generated using [Remcom Wireless InSite](http://www.remcom.com/wireless-insite) software. The [DeepMIMO dataset](https://deepmimo.net/) is a publicly available parameterized dataset published for deep learning applications in mmWave and massive MIMO systems.
+
+This python code package is related to the following article: 
+>Ahmed Alkhateeb, “[DeepMIMO: A Generic Deep Learning Dataset for Millimeter Wave and Massive MIMO Applications](https://arxiv.org/pdf/1902.06435.pdf),” in Proc. of Information Theory and Applications Workshop (ITA), San Diego, CA, Feb. 2019.
+# Abstract of the Article
+Machine learning tools are finding interesting applications in millimeter wave (mmWave) and massive MIMO systems. This is mainly thanks to their powerful capabilities in learning unknown models and tackling hard optimization problems. To advance the machine learning research in mmWave/massive MIMO, however, there is a need for a common dataset. This dataset can be used to evaluate the developed algorithms, reproduce the results, set *benchmarks*, and compare the different solutions. In this work, we introduce the DeepMIMO dataset, which is a generic dataset for mmWave/massive MIMO channels. The DeepMIMO dataset generation framework has two important features. First, the DeepMIMO channels are constructed based on accurate ray-tracing data obtained from Remcom Wireless InSite. The DeepMIMO channels, therefore, capture the dependence on the environment geometry/materials and transmitter/receiver locations, which is essential for several machine learning applications. Second, the DeepMIMO dataset is generic/parameterized as the researcher can adjust a set of system and channel parameters to tailor the generated DeepMIMO dataset for the target machine learning application. The DeepMIMO dataset can then be completely defined by the (i) the adopted ray-tracing scenario and (ii) the set of parameters, which enables the accurate definition and reproduction of the dataset. In this paper, an example DeepMIMO dataset is described based on an outdoor ray-tracing scenario of 18 base stations and more than one million users. The paper also shows how this dataset can be used in an example deep learning application of mmWave beam prediction.
+
+# Installation & Dataset Generation
+**To generate the dataset, please refer to [this website](https://deepmimo.net/versions/v2-python/) for the different dataset options and their generation steps.
+
+If you have any questions regarding the code and used dataset, please contact [Ahmed Alkhateeb](https://www.aalkhateeb.net/).
+
+# License and Referencing
+This code package is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/). If you in any way use this code for research that results in publications, please cite both the original article and the Remcom Wireless InSite website:
+> - A. Alkhateeb, “[DeepMIMO: A Generic Deep Learning Dataset for Millimeter Wave and Massive MIMO Applications](https://arxiv.org/pdf/1902.06435.pdf),” in Proc. of Information Theory and Applications Workshop (ITA), San Diego, CA, Feb. 2019.
+> - Remcom, Wireless insite, “http://www.remcom.com/wireless-insite”
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3/ant_patterns.py` & `deepmimov3-0.2.5/src/DeepMIMOv3/ant_patterns.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# -*- coding: utf-8 -*-
-"""
-DeepMIMOv2 Python Implementation
-
-Description: Antenna Radiation Patterns
-
-Authors: Umut Demirhan, Ahmed Alkhateeb
-Date: 3/16/2022
-"""
-
-import DeepMIMOv3.consts as c
-import numpy as np
-
-class AntennaPattern():
-    def __init__(self, tx_pattern, rx_pattern):
-        # Initialize TX Pattern
-        if tx_pattern in c.PARAMSET_ANT_RAD_PAT_VALS:
-            if tx_pattern == c.PARAMSET_ANT_RAD_PAT_VALS[0]:
-                self.tx_pattern_fn = None
-            else:
-                tx_pattern = tx_pattern.replace('-', '_')
-                tx_pattern = 'pattern_' + tx_pattern
-                self.tx_pattern_fn = globals()[tx_pattern]
-        else:
-            raise NotImplementedError('The given \'%s\' antenna radiation pattern is not applicable.' % tx_pattern)
-        
-        
-        # Initialize RX Pattern
-        if rx_pattern in c.PARAMSET_ANT_RAD_PAT_VALS:
-            if rx_pattern == c.PARAMSET_ANT_RAD_PAT_VALS[0]:
-                self.rx_pattern_fn = None
-            else:
-                rx_pattern = rx_pattern.replace('-', '_')
-                rx_pattern = 'pattern_' + rx_pattern
-                self.rx_pattern_fn = globals()[rx_pattern]
-        else:
-            raise NotImplementedError('The given \'%s\' antenna radiation pattern is not applicable.' % rx_pattern)
-    
-    def apply(self, power, doa_theta, doa_phi, dod_theta, dod_phi):
-        pattern = 1.
-        if self.tx_pattern_fn is not None:
-            pattern *= self.tx_pattern_fn(dod_theta, dod_phi)
-        if self.rx_pattern_fn is not None:
-            pattern *= self.rx_pattern_fn(doa_theta, doa_phi)
-            
-        return power * pattern
-
-def pattern_halfwave_dipole(theta, phi):
-    max_gain = 1.6409223769 # Half-wave dipole maximum directivity
-    theta_nonzero = theta.copy()
-    zero_idx = theta_nonzero==0
-    theta_nonzero[zero_idx] = 1e-4 # Approximation of 0 at limit
-    pattern = max_gain * np.cos((np.pi/2)*np.cos(theta))**2 / np.sin(theta)**2
-    pattern[zero_idx] = 0
-    return pattern
-    
+# -*- coding: utf-8 -*-
+"""
+DeepMIMOv2 Python Implementation
+
+Description: Antenna Radiation Patterns
+
+Authors: Umut Demirhan, Ahmed Alkhateeb
+Date: 3/16/2022
+"""
+
+import DeepMIMOv3.consts as c
+import numpy as np
+
+class AntennaPattern():
+    def __init__(self, tx_pattern, rx_pattern):
+        # Initialize TX Pattern
+        if tx_pattern in c.PARAMSET_ANT_RAD_PAT_VALS:
+            if tx_pattern == c.PARAMSET_ANT_RAD_PAT_VALS[0]:
+                self.tx_pattern_fn = None
+            else:
+                tx_pattern = tx_pattern.replace('-', '_')
+                tx_pattern = 'pattern_' + tx_pattern
+                self.tx_pattern_fn = globals()[tx_pattern]
+        else:
+            raise NotImplementedError('The given \'%s\' antenna radiation pattern is not applicable.' % tx_pattern)
+        
+        
+        # Initialize RX Pattern
+        if rx_pattern in c.PARAMSET_ANT_RAD_PAT_VALS:
+            if rx_pattern == c.PARAMSET_ANT_RAD_PAT_VALS[0]:
+                self.rx_pattern_fn = None
+            else:
+                rx_pattern = rx_pattern.replace('-', '_')
+                rx_pattern = 'pattern_' + rx_pattern
+                self.rx_pattern_fn = globals()[rx_pattern]
+        else:
+            raise NotImplementedError('The given \'%s\' antenna radiation pattern is not applicable.' % rx_pattern)
+    
+    def apply(self, power, doa_theta, doa_phi, dod_theta, dod_phi):
+        pattern = 1.
+        if self.tx_pattern_fn is not None:
+            pattern *= self.tx_pattern_fn(dod_theta, dod_phi)
+        if self.rx_pattern_fn is not None:
+            pattern *= self.rx_pattern_fn(doa_theta, doa_phi)
+            
+        return power * pattern
+
+def pattern_halfwave_dipole(theta, phi):
+    max_gain = 1.6409223769 # Half-wave dipole maximum directivity
+    theta_nonzero = theta.copy()
+    zero_idx = theta_nonzero==0
+    theta_nonzero[zero_idx] = 1e-4 # Approximation of 0 at limit
+    pattern = max_gain * np.cos((np.pi/2)*np.cos(theta))**2 / np.sin(theta)**2
+    pattern[zero_idx] = 0
+    return pattern
+
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3/construct_deepmimo.py` & `deepmimov3-0.2.5/src/DeepMIMOv3/construct_deepmimo.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,312 +1,312 @@
-# -*- coding: utf-8 -*-
-"""
-DeepMIMOv2 Python Implementation
-
-Description: MIMO channel generator
-
-Authors: Umut Demirhan, Ahmed Alkhateeb
-Date: 12/10/2021
-"""
-
-import DeepMIMOv3.consts as c
-import numpy as np
-from tqdm import tqdm
-from DeepMIMOv3.ant_patterns import AntennaPattern
-
-# Generates common parameters first. The output is a numpy matrix.
-def generate_MIMO_channel(raydata, params, tx_ant_params, rx_ant_params):
-    
-    bandwidth = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_BW] * c.PARAMSET_OFDM_BW_MULT
-    
-    kd_tx = 2*np.pi*tx_ant_params[c.PARAMSET_ANT_SPACING]
-    kd_rx = 2*np.pi*rx_ant_params[c.PARAMSET_ANT_SPACING]
-    Ts = 1/bandwidth
-    subcarriers = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_SC_SAMP]
-    path_gen = OFDM_PathGenerator(params, subcarriers)
-    antennapattern = AntennaPattern(tx_pattern = tx_ant_params[c.PARAMSET_ANT_RAD_PAT], rx_pattern = rx_ant_params[c.PARAMSET_ANT_RAD_PAT])
-
-    M_tx = np.prod(tx_ant_params[c.PARAMSET_ANT_SHAPE])
-    ant_tx_ind = ant_indices(tx_ant_params[c.PARAMSET_ANT_SHAPE])
-    
-    M_rx = np.prod(rx_ant_params[c.PARAMSET_ANT_SHAPE])
-    ant_rx_ind = ant_indices(rx_ant_params[c.PARAMSET_ANT_SHAPE])
-    
-    if  params[c.PARAMSET_FDTD]:
-        channel = np.zeros((len(raydata), M_rx, M_tx, len(subcarriers)), dtype = np.csingle)
-    else:
-        channel = np.zeros((len(raydata), M_rx, M_tx, params[c.PARAMSET_NUM_PATHS]), dtype = np.csingle)
-    LoS_status = np.zeros((len(raydata)), dtype=np.int8)-2
-        
-    for i in tqdm(range(len(raydata)), desc='Generating channels'):
-        
-        if raydata[i][c.OUT_PATH_NUM]==0:
-            LoS_status[i] = -1
-            continue
-        
-        
-        dod_theta, dod_phi = rotate_angles(rotation = tx_ant_params[c.PARAMSET_ANT_ROTATION],
-                                  theta = raydata[i][c.OUT_PATH_DOD_THETA],
-                                  phi = raydata[i][c.OUT_PATH_DOD_PHI])
-        
-        doa_theta, doa_phi = rotate_angles(rotation = rx_ant_params[c.PARAMSET_ANT_ROTATION][i],
-                                  theta = raydata[i][c.OUT_PATH_DOA_THETA],
-                                  phi = raydata[i][c.OUT_PATH_DOA_PHI])
-        
-        FoV_tx = apply_FoV(tx_ant_params[c.PARAMSET_ANT_FOV], dod_theta, dod_phi)
-        FoV_rx = apply_FoV(rx_ant_params[c.PARAMSET_ANT_FOV], doa_theta, doa_phi)
-        FoV = np.logical_and(FoV_tx, FoV_rx)
-        dod_theta = dod_theta[FoV]
-        dod_phi = dod_phi[FoV]
-        doa_theta = doa_theta[FoV]
-        doa_phi = doa_phi[FoV]
-        
-        for key in raydata[i].keys():
-            if key == 'num_paths':
-                raydata[i][key] = FoV.sum()
-            else:
-                raydata[i][key] = raydata[i][key][FoV]
-        
-        if raydata[i]['num_paths'] == 0:
-            LoS_status[i] = -1
-        else:
-            LoS_status[i] = raydata[i]['LoS'].sum()
-                
-        array_response_TX = array_response(ant_ind = ant_tx_ind, 
-                                           theta = dod_theta, 
-                                           phi = dod_phi, 
-                                           kd = kd_tx)
-        
-        array_response_RX = array_response(ant_ind = ant_rx_ind, 
-                                           theta =  doa_theta, 
-                                           phi = doa_phi,
-                                           kd = kd_rx)
-        
-        power = antennapattern.apply(power = raydata[i][c.OUT_PATH_RX_POW], 
-                                     doa_theta = doa_theta, 
-                                     doa_phi = doa_phi, 
-                                     dod_theta = dod_theta, 
-                                     dod_phi = dod_phi)
-        raydata[i][c.OUT_PATH_RX_POW] = power
-        
-        if  params[c.PARAMSET_FDTD]: # OFDM
-            path_const = path_gen.generate(raydata[i], Ts)
-            
-            # The next step is to be defined
-            if params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_LPF] == 0:
-                channel[i] = np.sum(array_response_RX[:, None, None, :] * array_response_TX[None, :, None, :] * path_const.T[None, None, :, :], axis=3)
-            else:
-                channel[i] = np.sum(array_response_RX[:, None, None, :] * array_response_TX[None, :, None, :] * path_const.T[None, None, :, :], axis=3) @ path_gen.delay_to_OFDM
-        
-        else: # TD channel
-            channel[i, :, :, :raydata[i][c.OUT_PATH_NUM]] = array_response_RX[:, None, :] * array_response_TX[None, :, :] * (np.sqrt(power) * np.exp(1j*np.deg2rad(raydata[i][c.OUT_PATH_PHASE])))[None, None, :]
-
-    return channel, LoS_status
-
-# Generates everything for each rx_ant_params - 
-# necessary for BS-BS channels since different antennas can be defined. 
-# The output is a list.
-def generate_MIMO_channel_rx_ind(raydata, params, tx_ant_params, rx_ant_params):
-    
-    bandwidth = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_BW] * c.PARAMSET_OFDM_BW_MULT
-    
-    Ts = 1/bandwidth
-    subcarriers = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_SC_SAMP]
-    path_gen = OFDM_PathGenerator(params, subcarriers)
-    
-    
-    channel = []
-    LoS_status = []
-        
-    for i in tqdm(range(len(raydata)), desc='Generating channels'):
-        
-        antennapattern = AntennaPattern(tx_pattern = tx_ant_params[c.PARAMSET_ANT_RAD_PAT], rx_pattern = rx_ant_params[i][c.PARAMSET_ANT_RAD_PAT])
-        
-        kd_tx = 2*np.pi*tx_ant_params[c.PARAMSET_ANT_SPACING]
-        kd_rx = 2*np.pi*rx_ant_params[i][c.PARAMSET_ANT_SPACING]
-        
-        M_tx = np.prod(tx_ant_params[c.PARAMSET_ANT_SHAPE])
-        ant_tx_ind = ant_indices(tx_ant_params[c.PARAMSET_ANT_SHAPE])
-        
-        M_rx = np.prod(rx_ant_params[i][c.PARAMSET_ANT_SHAPE])
-        ant_rx_ind = ant_indices(rx_ant_params[i][c.PARAMSET_ANT_SHAPE])
-        
-        if raydata[i][c.OUT_PATH_NUM]==0:
-            channel.append(np.zeros((M_rx, M_tx, len(subcarriers))))
-            LoS_status.append(-1)
-            continue
-    
-        
-        dod_theta, dod_phi = rotate_angles(rotation = tx_ant_params[c.PARAMSET_ANT_ROTATION],
-                                  theta = raydata[i][c.OUT_PATH_DOD_THETA],
-                                  phi = raydata[i][c.OUT_PATH_DOD_PHI])
-        
-        doa_theta, doa_phi = rotate_angles(rotation = rx_ant_params[i][c.PARAMSET_ANT_ROTATION],
-                                  theta = raydata[i][c.OUT_PATH_DOA_THETA],
-                                  phi = raydata[i][c.OUT_PATH_DOA_PHI])
-                
-        FoV_tx = apply_FoV(tx_ant_params[c.PARAMSET_ANT_FOV], dod_theta, dod_phi)
-        FoV_rx = apply_FoV(rx_ant_params[i][c.PARAMSET_ANT_FOV], doa_theta, doa_phi)
-        FoV = np.logical_and(FoV_tx, FoV_rx)
-        dod_theta = dod_theta[FoV]
-        dod_phi = dod_phi[FoV]
-        doa_theta = doa_theta[FoV]
-        doa_phi = doa_phi[FoV]
-        
-        for key in raydata[i].keys():
-            if key == 'num_paths':
-                raydata[i][key] = FoV.sum()
-            else:
-                raydata[i][key] = raydata[i][key][FoV]
-        
-        if raydata[i]['num_paths'] == 0:
-            LoS_status.append(-1)
-        else:
-            LoS_status.append(raydata[i]['LoS'].sum())
-            
-        array_response_TX = array_response(ant_ind = ant_tx_ind, 
-                                           theta = dod_theta, 
-                                           phi = dod_phi, 
-                                           kd = kd_tx)
-        
-        array_response_RX = array_response(ant_ind = ant_rx_ind, 
-                                           theta =  doa_theta, 
-                                           phi = doa_phi,
-                                           kd = kd_rx)
-        
-        power = antennapattern.apply(power = raydata[i][c.OUT_PATH_RX_POW], 
-                                     doa_theta = doa_theta, 
-                                     doa_phi = doa_phi, 
-                                     dod_theta = dod_theta, 
-                                     dod_phi = dod_phi)
-        raydata[i][c.OUT_PATH_RX_POW] = power
-        
-        if  params[c.PARAMSET_FDTD]: # OFDM
-            path_const = path_gen.generate(raydata[i], Ts)
-            
-            # The next step is to be defined
-            if params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_LPF] == 0: # NO LPF
-                channel.append(np.sum(array_response_RX[:, None, None, :] * array_response_TX[None, :, None, :] * path_const.T[None, None, :, :], axis=3))
-            else: # Sinc LPF
-                channel.append(np.sum(array_response_RX[:, None, None, :] * array_response_TX[None, :, None, :] * path_const.T[None, None, :, :], axis=3) @ path_gen.delay_to_OFDM)
-        
-        else: # Time domain
-            channel.append(array_response_RX[:, None, :] * array_response_TX[None, :, :] * (np.sqrt(power) * np.exp(1j*np.deg2rad(raydata[i][c.OUT_PATH_PHASE])))[None, None, :])
-
-    return channel, LoS_status
-
-
-def array_response(ant_ind, theta, phi, kd):        
-    gamma = array_response_phase(theta, phi, kd)
-    return np.exp(ant_ind@gamma.T)
-    
-def array_response_phase(theta, phi, kd):
-    gamma_x = 1j*kd*np.sin(theta)*np.cos(phi)
-    gamma_y = 1j*kd*np.sin(theta)*np.sin(phi)
-    gamma_z = 1j*kd*np.cos(theta)
-    return np.vstack([gamma_x, gamma_y, gamma_z]).T
- 
-def ant_indices(panel_size):
-    gamma_x = np.tile(np.arange(1), panel_size[0]*panel_size[1])
-    gamma_y = np.tile(np.repeat(np.arange(panel_size[0]), 1), panel_size[1])
-    gamma_z = np.repeat(np.arange(panel_size[1]), panel_size[0])
-    return np.vstack([gamma_x, gamma_y, gamma_z]).T
-
-def apply_FoV(FoV, theta, phi):
-    theta = np.mod(theta, 2*np.pi)
-    phi = np.mod(phi, 2*np.pi)
-    FoV = np.deg2rad(FoV)
-    path_inclusion_phi = np.logical_or(phi <= 0+FoV[0]/2, phi >= 2*np.pi-FoV[0]/2)
-    path_inclusion_theta = np.logical_and(theta <= np.pi/2+FoV[1]/2, theta >= np.pi/2-FoV[1]/2)
-    path_inclusion = np.logical_and(path_inclusion_phi, path_inclusion_theta)
-    return path_inclusion
-
-def rotate_angles(rotation, theta, phi): # Input all degrees - output radians
-    theta = np.deg2rad(theta)
-    phi = np.deg2rad(phi)
-
-    if rotation is not None:
-        rotation = np.deg2rad(rotation)
-    
-        sin_alpha = np.sin(phi - rotation[2])
-        sin_beta = np.sin(rotation[1])
-        sin_gamma = np.sin(rotation[0])
-        cos_alpha = np.cos(phi - rotation[2])
-        cos_beta = np.cos(rotation[1])
-        cos_gamma = np.cos(rotation[0])
-        
-        sin_theta = np.sin(theta)
-        cos_theta = np.cos(theta)
-        
-        theta = np.arccos(cos_beta*cos_gamma*cos_theta 
-                              + sin_theta*(sin_beta*cos_gamma*cos_alpha-sin_gamma*sin_alpha)
-                              )
-        phi = np.angle(cos_beta*sin_theta*cos_alpha-sin_beta*cos_theta 
-                           + 1j*(cos_beta*sin_gamma*cos_theta 
-                                 + sin_theta*(sin_beta*sin_gamma*cos_alpha + cos_gamma*sin_alpha))
-                           )
-    return theta, phi
-
-class OFDM_PathGenerator:
-    def __init__(self, params, subcarriers):
-        self.params = params
-        self.OFDM_params = params[c.PARAMSET_OFDM]
-        
-        if self.OFDM_params[c.PARAMSET_OFDM_LPF] == 0: # No Pulse Shaping
-            self.generate = getattr(self, 'no_LPF')
-        else: # Pulse Shaping
-            self.generate = getattr(self, 'with_LPF')
-            
-                
-        self.subcarriers = subcarriers
-        self.total_subcarriers = self.OFDM_params[c.PARAMSET_OFDM_SC_NUM]
-        
-        self.delay_d = np.arange(self.OFDM_params['subcarriers'])
-        self.delay_to_OFDM = np.exp(-1j*2*np.pi/self.total_subcarriers*np.outer(self.delay_d, self.subcarriers))
-        
-    def no_LPF(self, raydata, Ts):
-        power = (raydata[c.OUT_PATH_RX_POW]).reshape(-1, 1)
-        delay_n = (raydata[c.OUT_PATH_TOA]/Ts).reshape(-1, 1)
-        phase = raydata[c.OUT_PATH_PHASE].reshape(-1,1)
-        
-        paths_over_FFT = (delay_n >= self.OFDM_params['subcarriers'])
-        power[paths_over_FFT] = 0
-        delay_n[paths_over_FFT] = self.OFDM_params['subcarriers']
-        
-        path_const = np.sqrt(power/self.total_subcarriers) * np.exp(1j*(np.deg2rad(phase) - (2*np.pi/self.total_subcarriers)*np.outer(delay_n, self.subcarriers) ))
-        
-        if self.params[c.PARAMSET_DOPPLER_EN] and self.params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_DOPPLER_EN]:
-            doppler_vel = raydata[c.OUT_PATH_DOP_VEL].reshape(-1, 1)
-            doppler_acc = raydata[c.OUT_PATH_DOP_ACC].reshape(-1, 1)
-            carr_freq = self.params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_CF]
-            
-            delay = (raydata[c.OUT_PATH_TOA]).reshape(-1, 1)
-            Doppler_phase = np.exp(-1j*2*np.pi*carr_freq*(doppler_vel*delay/c.LIGHTSPEED + doppler_acc*(delay**2)/(2*c.LIGHTSPEED)))
-            path_const *= Doppler_phase
-        
-        return path_const
-    
-    def with_LPF(self, raydata, Ts):
-        power = (raydata[c.OUT_PATH_RX_POW]).reshape(-1, 1)
-        delay_n = (raydata[c.OUT_PATH_TOA]/Ts).reshape(-1, 1)
-        phase = raydata[c.OUT_PATH_PHASE].reshape(-1,1)
-        
-        # Ignore the paths over CP
-        paths_over_FFT = (delay_n >= self.OFDM_params['subcarriers'])
-        power[paths_over_FFT] = 0
-        delay_n[paths_over_FFT] = self.OFDM_params['subcarriers']
-        
-        # Pulse - LPF convolution and channel generation
-        pulse = np.sinc(self.delay_d-delay_n)
-        pulse = pulse * np.sqrt(power/self.total_subcarriers) * np.exp(1j*np.deg2rad(phase)) # Power scaling
-        
-        if self.params[c.PARAMSET_DOPPLER_EN] and self.params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_DOPPLER_EN]:
-            doppler_vel = raydata[c.OUT_PATH_DOP_VEL].reshape(-1, 1)
-            doppler_acc = raydata[c.OUT_PATH_DOP_ACC].reshape(-1, 1)
-            carr_freq = self.params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_CF]
-            
-            delay = Ts * self.delay_d.T
-            Doppler_phase = np.exp(-1j*2*np.pi*carr_freq*(doppler_vel*delay/c.LIGHTSPEED + doppler_acc*(delay**2)/(2*c.LIGHTSPEED)))
-            pulse *= Doppler_phase
-        
-        return pulse
+# -*- coding: utf-8 -*-
+"""
+DeepMIMOv2 Python Implementation
+
+Description: MIMO channel generator
+
+Authors: Umut Demirhan, Ahmed Alkhateeb
+Date: 12/10/2021
+"""
+
+import DeepMIMOv3.consts as c
+import numpy as np
+from tqdm import tqdm
+from DeepMIMOv3.ant_patterns import AntennaPattern
+
+# Generates common parameters first. The output is a numpy matrix.
+def generate_MIMO_channel(raydata, params, tx_ant_params, rx_ant_params):
+    
+    bandwidth = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_BW] * c.PARAMSET_OFDM_BW_MULT
+    
+    kd_tx = 2*np.pi*tx_ant_params[c.PARAMSET_ANT_SPACING]
+    kd_rx = 2*np.pi*rx_ant_params[c.PARAMSET_ANT_SPACING]
+    Ts = 1/bandwidth
+    subcarriers = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_SC_SAMP]
+    path_gen = OFDM_PathGenerator(params, subcarriers)
+    antennapattern = AntennaPattern(tx_pattern = tx_ant_params[c.PARAMSET_ANT_RAD_PAT], rx_pattern = rx_ant_params[c.PARAMSET_ANT_RAD_PAT])
+
+    M_tx = np.prod(tx_ant_params[c.PARAMSET_ANT_SHAPE])
+    ant_tx_ind = ant_indices(tx_ant_params[c.PARAMSET_ANT_SHAPE])
+    
+    M_rx = np.prod(rx_ant_params[c.PARAMSET_ANT_SHAPE])
+    ant_rx_ind = ant_indices(rx_ant_params[c.PARAMSET_ANT_SHAPE])
+    
+    if  params[c.PARAMSET_FDTD]:
+        channel = np.zeros((len(raydata), M_rx, M_tx, len(subcarriers)), dtype = np.csingle)
+    else:
+        channel = np.zeros((len(raydata), M_rx, M_tx, params[c.PARAMSET_NUM_PATHS]), dtype = np.csingle)
+    LoS_status = np.zeros((len(raydata)), dtype=np.int8)-2
+        
+    for i in tqdm(range(len(raydata)), desc='Generating channels'):
+        
+        if raydata[i][c.OUT_PATH_NUM]==0:
+            LoS_status[i] = -1
+            continue
+        
+        
+        dod_theta, dod_phi = rotate_angles(rotation = tx_ant_params[c.PARAMSET_ANT_ROTATION],
+                                  theta = raydata[i][c.OUT_PATH_DOD_THETA],
+                                  phi = raydata[i][c.OUT_PATH_DOD_PHI])
+        
+        doa_theta, doa_phi = rotate_angles(rotation = rx_ant_params[c.PARAMSET_ANT_ROTATION][i],
+                                  theta = raydata[i][c.OUT_PATH_DOA_THETA],
+                                  phi = raydata[i][c.OUT_PATH_DOA_PHI])
+        
+        FoV_tx = apply_FoV(tx_ant_params[c.PARAMSET_ANT_FOV], dod_theta, dod_phi)
+        FoV_rx = apply_FoV(rx_ant_params[c.PARAMSET_ANT_FOV], doa_theta, doa_phi)
+        FoV = np.logical_and(FoV_tx, FoV_rx)
+        dod_theta = dod_theta[FoV]
+        dod_phi = dod_phi[FoV]
+        doa_theta = doa_theta[FoV]
+        doa_phi = doa_phi[FoV]
+        
+        for key in raydata[i].keys():
+            if key == 'num_paths':
+                raydata[i][key] = FoV.sum()
+            else:
+                raydata[i][key] = raydata[i][key][FoV]
+        
+        if raydata[i]['num_paths'] == 0:
+            LoS_status[i] = -1
+        else:
+            LoS_status[i] = raydata[i]['LoS'].sum()
+                
+        array_response_TX = array_response(ant_ind = ant_tx_ind, 
+                                           theta = dod_theta, 
+                                           phi = dod_phi, 
+                                           kd = kd_tx)
+        
+        array_response_RX = array_response(ant_ind = ant_rx_ind, 
+                                           theta =  doa_theta, 
+                                           phi = doa_phi,
+                                           kd = kd_rx)
+        
+        power = antennapattern.apply(power = raydata[i][c.OUT_PATH_RX_POW], 
+                                     doa_theta = doa_theta, 
+                                     doa_phi = doa_phi, 
+                                     dod_theta = dod_theta, 
+                                     dod_phi = dod_phi)
+        raydata[i][c.OUT_PATH_RX_POW] = power
+        
+        if  params[c.PARAMSET_FDTD]: # OFDM
+            path_const = path_gen.generate(raydata[i], Ts)
+            
+            # The next step is to be defined
+            if params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_LPF] == 0:
+                channel[i] = np.sum(array_response_RX[:, None, None, :] * array_response_TX[None, :, None, :] * path_const.T[None, None, :, :], axis=3)
+            else:
+                channel[i] = np.sum(array_response_RX[:, None, None, :] * array_response_TX[None, :, None, :] * path_const.T[None, None, :, :], axis=3) @ path_gen.delay_to_OFDM
+        
+        else: # TD channel
+            channel[i, :, :, :raydata[i][c.OUT_PATH_NUM]] = array_response_RX[:, None, :] * array_response_TX[None, :, :] * (np.sqrt(power) * np.exp(1j*np.deg2rad(raydata[i][c.OUT_PATH_PHASE])))[None, None, :]
+
+    return channel, LoS_status
+
+# Generates everything for each rx_ant_params - 
+# necessary for BS-BS channels since different antennas can be defined. 
+# The output is a list.
+def generate_MIMO_channel_rx_ind(raydata, params, tx_ant_params, rx_ant_params):
+    
+    bandwidth = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_BW] * c.PARAMSET_OFDM_BW_MULT
+    
+    Ts = 1/bandwidth
+    subcarriers = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_SC_SAMP]
+    path_gen = OFDM_PathGenerator(params, subcarriers)
+    
+    
+    channel = []
+    LoS_status = []
+        
+    for i in tqdm(range(len(raydata)), desc='Generating channels'):
+        
+        antennapattern = AntennaPattern(tx_pattern = tx_ant_params[c.PARAMSET_ANT_RAD_PAT], rx_pattern = rx_ant_params[i][c.PARAMSET_ANT_RAD_PAT])
+        
+        kd_tx = 2*np.pi*tx_ant_params[c.PARAMSET_ANT_SPACING]
+        kd_rx = 2*np.pi*rx_ant_params[i][c.PARAMSET_ANT_SPACING]
+        
+        M_tx = np.prod(tx_ant_params[c.PARAMSET_ANT_SHAPE])
+        ant_tx_ind = ant_indices(tx_ant_params[c.PARAMSET_ANT_SHAPE])
+        
+        M_rx = np.prod(rx_ant_params[i][c.PARAMSET_ANT_SHAPE])
+        ant_rx_ind = ant_indices(rx_ant_params[i][c.PARAMSET_ANT_SHAPE])
+        
+        if raydata[i][c.OUT_PATH_NUM]==0:
+            channel.append(np.zeros((M_rx, M_tx, len(subcarriers))))
+            LoS_status.append(-1)
+            continue
+    
+        
+        dod_theta, dod_phi = rotate_angles(rotation = tx_ant_params[c.PARAMSET_ANT_ROTATION],
+                                  theta = raydata[i][c.OUT_PATH_DOD_THETA],
+                                  phi = raydata[i][c.OUT_PATH_DOD_PHI])
+        
+        doa_theta, doa_phi = rotate_angles(rotation = rx_ant_params[i][c.PARAMSET_ANT_ROTATION],
+                                  theta = raydata[i][c.OUT_PATH_DOA_THETA],
+                                  phi = raydata[i][c.OUT_PATH_DOA_PHI])
+                
+        FoV_tx = apply_FoV(tx_ant_params[c.PARAMSET_ANT_FOV], dod_theta, dod_phi)
+        FoV_rx = apply_FoV(rx_ant_params[i][c.PARAMSET_ANT_FOV], doa_theta, doa_phi)
+        FoV = np.logical_and(FoV_tx, FoV_rx)
+        dod_theta = dod_theta[FoV]
+        dod_phi = dod_phi[FoV]
+        doa_theta = doa_theta[FoV]
+        doa_phi = doa_phi[FoV]
+        
+        for key in raydata[i].keys():
+            if key == 'num_paths':
+                raydata[i][key] = FoV.sum()
+            else:
+                raydata[i][key] = raydata[i][key][FoV]
+        
+        if raydata[i]['num_paths'] == 0:
+            LoS_status.append(-1)
+        else:
+            LoS_status.append(raydata[i]['LoS'].sum())
+            
+        array_response_TX = array_response(ant_ind = ant_tx_ind, 
+                                           theta = dod_theta, 
+                                           phi = dod_phi, 
+                                           kd = kd_tx)
+        
+        array_response_RX = array_response(ant_ind = ant_rx_ind, 
+                                           theta =  doa_theta, 
+                                           phi = doa_phi,
+                                           kd = kd_rx)
+        
+        power = antennapattern.apply(power = raydata[i][c.OUT_PATH_RX_POW], 
+                                     doa_theta = doa_theta, 
+                                     doa_phi = doa_phi, 
+                                     dod_theta = dod_theta, 
+                                     dod_phi = dod_phi)
+        raydata[i][c.OUT_PATH_RX_POW] = power
+        
+        if  params[c.PARAMSET_FDTD]: # OFDM
+            path_const = path_gen.generate(raydata[i], Ts)
+            
+            # The next step is to be defined
+            if params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_LPF] == 0: # NO LPF
+                channel.append(np.sum(array_response_RX[:, None, None, :] * array_response_TX[None, :, None, :] * path_const.T[None, None, :, :], axis=3))
+            else: # Sinc LPF
+                channel.append(np.sum(array_response_RX[:, None, None, :] * array_response_TX[None, :, None, :] * path_const.T[None, None, :, :], axis=3) @ path_gen.delay_to_OFDM)
+        
+        else: # Time domain
+            channel.append(array_response_RX[:, None, :] * array_response_TX[None, :, :] * (np.sqrt(power) * np.exp(1j*np.deg2rad(raydata[i][c.OUT_PATH_PHASE])))[None, None, :])
+
+    return channel, LoS_status
+
+
+def array_response(ant_ind, theta, phi, kd):        
+    gamma = array_response_phase(theta, phi, kd)
+    return np.exp(ant_ind@gamma.T)
+    
+def array_response_phase(theta, phi, kd):
+    gamma_x = 1j*kd*np.sin(theta)*np.cos(phi)
+    gamma_y = 1j*kd*np.sin(theta)*np.sin(phi)
+    gamma_z = 1j*kd*np.cos(theta)
+    return np.vstack([gamma_x, gamma_y, gamma_z]).T
+ 
+def ant_indices(panel_size):
+    gamma_x = np.tile(np.arange(1), panel_size[0]*panel_size[1])
+    gamma_y = np.tile(np.repeat(np.arange(panel_size[0]), 1), panel_size[1])
+    gamma_z = np.repeat(np.arange(panel_size[1]), panel_size[0])
+    return np.vstack([gamma_x, gamma_y, gamma_z]).T
+
+def apply_FoV(FoV, theta, phi):
+    theta = np.mod(theta, 2*np.pi)
+    phi = np.mod(phi, 2*np.pi)
+    FoV = np.deg2rad(FoV)
+    path_inclusion_phi = np.logical_or(phi <= 0+FoV[0]/2, phi >= 2*np.pi-FoV[0]/2)
+    path_inclusion_theta = np.logical_and(theta <= np.pi/2+FoV[1]/2, theta >= np.pi/2-FoV[1]/2)
+    path_inclusion = np.logical_and(path_inclusion_phi, path_inclusion_theta)
+    return path_inclusion
+
+def rotate_angles(rotation, theta, phi): # Input all degrees - output radians
+    theta = np.deg2rad(theta)
+    phi = np.deg2rad(phi)
+
+    if rotation is not None:
+        rotation = np.deg2rad(rotation)
+    
+        sin_alpha = np.sin(phi - rotation[2])
+        sin_beta = np.sin(rotation[1])
+        sin_gamma = np.sin(rotation[0])
+        cos_alpha = np.cos(phi - rotation[2])
+        cos_beta = np.cos(rotation[1])
+        cos_gamma = np.cos(rotation[0])
+        
+        sin_theta = np.sin(theta)
+        cos_theta = np.cos(theta)
+        
+        theta = np.arccos(cos_beta*cos_gamma*cos_theta 
+                              + sin_theta*(sin_beta*cos_gamma*cos_alpha-sin_gamma*sin_alpha)
+                              )
+        phi = np.angle(cos_beta*sin_theta*cos_alpha-sin_beta*cos_theta 
+                           + 1j*(cos_beta*sin_gamma*cos_theta 
+                                 + sin_theta*(sin_beta*sin_gamma*cos_alpha + cos_gamma*sin_alpha))
+                           )
+    return theta, phi
+
+class OFDM_PathGenerator:
+    def __init__(self, params, subcarriers):
+        self.params = params
+        self.OFDM_params = params[c.PARAMSET_OFDM]
+        
+        if self.OFDM_params[c.PARAMSET_OFDM_LPF] == 0: # No Pulse Shaping
+            self.generate = getattr(self, 'no_LPF')
+        else: # Pulse Shaping
+            self.generate = getattr(self, 'with_LPF')
+            
+                
+        self.subcarriers = subcarriers
+        self.total_subcarriers = self.OFDM_params[c.PARAMSET_OFDM_SC_NUM]
+        
+        self.delay_d = np.arange(self.OFDM_params['subcarriers'])
+        self.delay_to_OFDM = np.exp(-1j*2*np.pi/self.total_subcarriers*np.outer(self.delay_d, self.subcarriers))
+        
+    def no_LPF(self, raydata, Ts):
+        power = (raydata[c.OUT_PATH_RX_POW]).reshape(-1, 1)
+        delay_n = (raydata[c.OUT_PATH_TOA]/Ts).reshape(-1, 1)
+        phase = raydata[c.OUT_PATH_PHASE].reshape(-1,1)
+        
+        paths_over_FFT = (delay_n >= self.OFDM_params['subcarriers'])
+        power[paths_over_FFT] = 0
+        delay_n[paths_over_FFT] = self.OFDM_params['subcarriers']
+        
+        path_const = np.sqrt(power/self.total_subcarriers) * np.exp(1j*(np.deg2rad(phase) - (2*np.pi/self.total_subcarriers)*np.outer(delay_n, self.subcarriers) ))
+        
+        if self.params[c.PARAMSET_DOPPLER_EN] and self.params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_DOPPLER_EN]:
+            doppler_vel = raydata[c.OUT_PATH_DOP_VEL].reshape(-1, 1)
+            doppler_acc = raydata[c.OUT_PATH_DOP_ACC].reshape(-1, 1)
+            carr_freq = self.params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_CF]
+            
+            delay = (raydata[c.OUT_PATH_TOA]).reshape(-1, 1)
+            Doppler_phase = np.exp(-1j*2*np.pi*carr_freq*(doppler_vel*delay/c.LIGHTSPEED + doppler_acc*(delay**2)/(2*c.LIGHTSPEED)))
+            path_const *= Doppler_phase
+        
+        return path_const
+    
+    def with_LPF(self, raydata, Ts):
+        power = (raydata[c.OUT_PATH_RX_POW]).reshape(-1, 1)
+        delay_n = (raydata[c.OUT_PATH_TOA]/Ts).reshape(-1, 1)
+        phase = raydata[c.OUT_PATH_PHASE].reshape(-1,1)
+        
+        # Ignore the paths over CP
+        paths_over_FFT = (delay_n >= self.OFDM_params['subcarriers'])
+        power[paths_over_FFT] = 0
+        delay_n[paths_over_FFT] = self.OFDM_params['subcarriers']
+        
+        # Pulse - LPF convolution and channel generation
+        pulse = np.sinc(self.delay_d-delay_n)
+        pulse = pulse * np.sqrt(power/self.total_subcarriers) * np.exp(1j*np.deg2rad(phase)) # Power scaling
+        
+        if self.params[c.PARAMSET_DOPPLER_EN] and self.params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_DOPPLER_EN]:
+            doppler_vel = raydata[c.OUT_PATH_DOP_VEL].reshape(-1, 1)
+            doppler_acc = raydata[c.OUT_PATH_DOP_ACC].reshape(-1, 1)
+            carr_freq = self.params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_CF]
+            
+            delay = Ts * self.delay_d.T
+            Doppler_phase = np.exp(-1j*2*np.pi*carr_freq*(doppler_vel*delay/c.LIGHTSPEED + doppler_acc*(delay**2)/(2*c.LIGHTSPEED)))
+            pulse *= Doppler_phase
+        
+        return pulse
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3/consts.py` & `deepmimov3-0.2.5/src/DeepMIMOv3/consts.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-# -*- coding: utf-8 -*-
-"""
-DeepMIMOv2 Python Implementation
-
-Description: Constant file
-
-Authors: Umut Demirhan, Ahmed Alkhateeb
-Date: 12/10/2021
-"""
-
-DICT_UE_IDX = 'user'
-DICT_BS_IDX = 'basestation'
-
-# NAME OF PARAMETER VARIABLES
-PARAMSET_DATASET_FOLDER = 'dataset_folder'
-PARAMSET_SCENARIO = 'scenario'
-PARAMSET_DYNAMIC_SCENES = 'dynamic_scenario_scenes'
-
-PARAMSET_NUM_PATHS = 'num_paths'
-PARAMSET_ACTIVE_BS = 'active_BS'
-PARAMSET_USER_ROWS = 'user_rows'
-# PARAMSET_USER_ROW_FIRST = 'user_row_first'
-# PARAMSET_USER_ROW_LAST = 'user_row_last'
-# PARAMSET_USER_ROW_SUBSAMP = 'row_subsampling'
-PARAMSET_USER_SUBSAMP = 'user_subsampling'
-
-PARAMSET_POLAR_EN = 'enable_dual_polar'
-PARAMSET_DOPPLER_EN = 'enable_doppler'
-
-PARAMSET_BS2BS = 'enable_BS2BS'
-PARAMSET_FDTD = 'OFDM_channels' # TD/OFDM
-
-PARAMSET_OFDM = 'OFDM'
-PARAMSET_OFDM_SC_NUM = 'subcarriers'
-# PARAMSET_OFDM_SC_LIM = 'subcarriers_limit'
-PARAMSET_OFDM_SC_SAMP = 'selected_subcarriers'
-PARAMSET_OFDM_BW = 'bandwidth'
-PARAMSET_OFDM_BW_MULT = 1e9 # Bandwidth input is GHz, multiply by this
-PARAMSET_OFDM_LPF = 'RX_filter'
-
-PARAMSET_ANT_BS = 'bs_antenna'
-PARAMSET_ANT_UE = 'ue_antenna'
-PARAMSET_ANT_SHAPE = 'shape'
-PARAMSET_ANT_SPACING = 'spacing'
-PARAMSET_ANT_ROTATION = 'rotation'
-PARAMSET_ANT_RAD_PAT = 'radiation_pattern'
-PARAMSET_ANT_RAD_PAT_VALS = ['isotropic', 'halfwave-dipole']
-PARAMSET_ANT_FOV = 'FoV'
-
-# INNER VARIABLES
-PARAMSET_ACTIVE_UE = 'active_UE'
-PARAMSET_SCENARIO_FIL = 'scenario_files'
-#PARAMSET_ACTIVE_USERS = 'active_user_idx'
-PARAMSET_ANT_BS_DIFF = 'BS2BS_isnumpy' # Based on this paramater, the BS-BS channels won't be converted from a list of matrices to a single matrix
-
-# SCENARIO PARAMS
-PARAMSET_SCENARIO_PARAMS = 'scenario_params'
-PARAMSET_SCENARIO_PARAMS_CF = 'carrier_freq'
-PARAMSET_SCENARIO_PARAMS_TX_POW = 'tx_power'
-PARAMSET_SCENARIO_PARAMS_NUM_BS = 'num_BS'
-PARAMSET_SCENARIO_PARAMS_USER_GRIDS = 'user_grids'
-PARAMSET_SCENARIO_PARAMS_POLAR_EN = 'dual_polar_available'
-PARAMSET_SCENARIO_PARAMS_DOPPLER_EN = 'doppler_available'
-
-PARAMSET_SCENARIO_PARAMS_PATH = 'scenario_params_path'
-# OUTPUT VARIABLES
-OUT_CHANNEL = 'channel'
-OUT_PATH = 'paths'
-OUT_LOS = 'LoS'
-OUT_LOC = 'location'
-OUT_DIST = 'distance'
-OUT_PL = 'pathloss'
-
-OUT_PATH_NUM = 'num_paths'
-OUT_PATH_DOD_PHI = 'DoD_phi'
-OUT_PATH_DOD_THETA = 'DoD_theta'
-OUT_PATH_DOA_PHI = 'DoA_phi'
-OUT_PATH_DOA_THETA = 'DoA_theta'
-OUT_PATH_PHASE = 'phase'
-OUT_PATH_TOA = 'ToA'
-OUT_PATH_RX_POW = 'power'
-OUT_PATH_LOS = 'LoS'
-OUT_PATH_DOP_VEL = 'Doppler_vel'
-OUT_PATH_DOP_ACC = 'Doppler_acc'
-OUT_PATH_ACTIVE = 'active_paths'
-
-# FILE LISTS - raytracing.load_ray_data()
-LOAD_FILE_EXT = ['DoD', 'DoA', 'CIR', 'LoS', 'PL', 'Loc']
-LOAD_FILE_EXT_FLATTEN =[1, 1, 1, 1, 0, 0]
-LOAD_FILE_EXT_UE = ['DoD.mat', 'DoA.mat', 'CIR.mat', 'LoS.mat', 'PL.mat', 'Loc.mat']
-LOAD_FILE_EXT_BS = ['DoD.BSBS.mat', 'DoA.BSBS.mat', 'CIR.BSBS.mat', 'LoS.BSBS.mat', 'PL.BSBS.mat', 'BSBS.RX_Loc.mat']
-
-# TX LOCATION FILE VARIABLE NAME - load_scenario_params()
-LOAD_FILE_TX_LOC = 'TX_Loc_array_full'
-
-# SCENARIO PARAMS FILE VARIABLE NAMES - load_scenario_params()
-LOAD_FILE_SP_EXT = '.params.mat'
-LOAD_FILE_SP_CF = 'carrier_freq'
-LOAD_FILE_SP_TX_POW = 'transmit_power'
-LOAD_FILE_SP_NUM_BS = 'num_BS'
-LOAD_FILE_SP_USER_GRIDS = 'user_grids'
-LOAD_FILE_SP_DOPPLER = 'doppler_available'
-LOAD_FILE_SP_POLAR = 'dual_polar_available'
-
-# Constants
+# -*- coding: utf-8 -*-
+"""
+DeepMIMOv2 Python Implementation
+
+Description: Constant file
+
+Authors: Umut Demirhan, Ahmed Alkhateeb
+Date: 12/10/2021
+"""
+
+DICT_UE_IDX = 'user'
+DICT_BS_IDX = 'basestation'
+
+# NAME OF PARAMETER VARIABLES
+PARAMSET_DATASET_FOLDER = 'dataset_folder'
+PARAMSET_SCENARIO = 'scenario'
+PARAMSET_DYNAMIC_SCENES = 'dynamic_scenario_scenes'
+
+PARAMSET_NUM_PATHS = 'num_paths'
+PARAMSET_ACTIVE_BS = 'active_BS'
+PARAMSET_USER_ROWS = 'user_rows'
+# PARAMSET_USER_ROW_FIRST = 'user_row_first'
+# PARAMSET_USER_ROW_LAST = 'user_row_last'
+# PARAMSET_USER_ROW_SUBSAMP = 'row_subsampling'
+PARAMSET_USER_SUBSAMP = 'user_subsampling'
+
+PARAMSET_POLAR_EN = 'enable_dual_polar'
+PARAMSET_DOPPLER_EN = 'enable_doppler'
+
+PARAMSET_BS2BS = 'enable_BS2BS'
+PARAMSET_FDTD = 'OFDM_channels' # TD/OFDM
+
+PARAMSET_OFDM = 'OFDM'
+PARAMSET_OFDM_SC_NUM = 'subcarriers'
+# PARAMSET_OFDM_SC_LIM = 'subcarriers_limit'
+PARAMSET_OFDM_SC_SAMP = 'selected_subcarriers'
+PARAMSET_OFDM_BW = 'bandwidth'
+PARAMSET_OFDM_BW_MULT = 1e9 # Bandwidth input is GHz, multiply by this
+PARAMSET_OFDM_LPF = 'RX_filter'
+
+PARAMSET_ANT_BS = 'bs_antenna'
+PARAMSET_ANT_UE = 'ue_antenna'
+PARAMSET_ANT_SHAPE = 'shape'
+PARAMSET_ANT_SPACING = 'spacing'
+PARAMSET_ANT_ROTATION = 'rotation'
+PARAMSET_ANT_RAD_PAT = 'radiation_pattern'
+PARAMSET_ANT_RAD_PAT_VALS = ['isotropic', 'halfwave-dipole']
+PARAMSET_ANT_FOV = 'FoV'
+
+# INNER VARIABLES
+PARAMSET_ACTIVE_UE = 'active_UE'
+PARAMSET_SCENARIO_FIL = 'scenario_files'
+#PARAMSET_ACTIVE_USERS = 'active_user_idx'
+PARAMSET_ANT_BS_DIFF = 'BS2BS_isnumpy' # Based on this paramater, the BS-BS channels won't be converted from a list of matrices to a single matrix
+
+# SCENARIO PARAMS
+PARAMSET_SCENARIO_PARAMS = 'scenario_params'
+PARAMSET_SCENARIO_PARAMS_CF = 'carrier_freq'
+PARAMSET_SCENARIO_PARAMS_TX_POW = 'tx_power'
+PARAMSET_SCENARIO_PARAMS_NUM_BS = 'num_BS'
+PARAMSET_SCENARIO_PARAMS_USER_GRIDS = 'user_grids'
+PARAMSET_SCENARIO_PARAMS_POLAR_EN = 'dual_polar_available'
+PARAMSET_SCENARIO_PARAMS_DOPPLER_EN = 'doppler_available'
+
+PARAMSET_SCENARIO_PARAMS_PATH = 'scenario_params_path'
+# OUTPUT VARIABLES
+OUT_CHANNEL = 'channel'
+OUT_PATH = 'paths'
+OUT_LOS = 'LoS'
+OUT_LOC = 'location'
+OUT_DIST = 'distance'
+OUT_PL = 'pathloss'
+
+OUT_PATH_NUM = 'num_paths'
+OUT_PATH_DOD_PHI = 'DoD_phi'
+OUT_PATH_DOD_THETA = 'DoD_theta'
+OUT_PATH_DOA_PHI = 'DoA_phi'
+OUT_PATH_DOA_THETA = 'DoA_theta'
+OUT_PATH_PHASE = 'phase'
+OUT_PATH_TOA = 'ToA'
+OUT_PATH_RX_POW = 'power'
+OUT_PATH_LOS = 'LoS'
+OUT_PATH_DOP_VEL = 'Doppler_vel'
+OUT_PATH_DOP_ACC = 'Doppler_acc'
+OUT_PATH_ACTIVE = 'active_paths'
+
+# FILE LISTS - raytracing.load_ray_data()
+LOAD_FILE_EXT = ['DoD', 'DoA', 'CIR', 'LoS', 'PL', 'Loc']
+LOAD_FILE_EXT_FLATTEN =[1, 1, 1, 1, 0, 0]
+LOAD_FILE_EXT_UE = ['DoD.mat', 'DoA.mat', 'CIR.mat', 'LoS.mat', 'PL.mat', 'Loc.mat']
+LOAD_FILE_EXT_BS = ['DoD.BSBS.mat', 'DoA.BSBS.mat', 'CIR.BSBS.mat', 'LoS.BSBS.mat', 'PL.BSBS.mat', 'BSBS.RX_Loc.mat']
+
+# TX LOCATION FILE VARIABLE NAME - load_scenario_params()
+LOAD_FILE_TX_LOC = 'TX_Loc_array_full'
+
+# SCENARIO PARAMS FILE VARIABLE NAMES - load_scenario_params()
+LOAD_FILE_SP_EXT = '.params.mat'
+LOAD_FILE_SP_CF = 'carrier_freq'
+LOAD_FILE_SP_TX_POW = 'transmit_power'
+LOAD_FILE_SP_NUM_BS = 'num_BS'
+LOAD_FILE_SP_USER_GRIDS = 'user_grids'
+LOAD_FILE_SP_DOPPLER = 'doppler_available'
+LOAD_FILE_SP_POLAR = 'dual_polar_available'
+
+# Constants
 LIGHTSPEED = 299792458
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3/params.py` & `deepmimov3-0.2.5/src/DeepMIMOv3/params.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# -*- coding: utf-8 -*-
-"""
-DeepMIMOv2 Python Implementation
-
-Description: Parameters file
-
-Authors: Umut Demirhan, Ahmed Alkhateeb
-Date: 12/10/2021
-"""
-
-import numpy as np
-import DeepMIMOv3.consts as c
-
-def default_params():
-    params = {c.PARAMSET_DATASET_FOLDER: './Raytracing_scenarios',
-              c.PARAMSET_SCENARIO:'O1_60',
-              
-              # Dynamic scenario scene selection
-              c.PARAMSET_DYNAMIC_SCENES: np.array([1]),
-              
-              # Maximum # of paths to be loaded
-              c.PARAMSET_NUM_PATHS: 5,
-              
-              # Active Basestation IDs
-              c.PARAMSET_ACTIVE_BS: np.array([1]), # To be implemented
-              
-              # Selected user rows
-              c.PARAMSET_USER_ROWS: np.array([1]),
-              
-              # Subsampling
-              # c.PARAMSET_USER_ROW_SUBSAMP: 1,
-              c.PARAMSET_USER_SUBSAMP: 1,
-              
-              # BS Antenna Parameters
-              c.PARAMSET_ANT_BS: {
-                  c.PARAMSET_ANT_SHAPE: np.array([8, 4]), # Antenna dimensions in X - Y - Z
-                  c.PARAMSET_ANT_SPACING: 0.5,
-                  c.PARAMSET_ANT_ROTATION: np.array([0, 0, 0]), # Rotation around X - Y - Z axes
-                  c.PARAMSET_ANT_FOV: np.array([360, 180]), # Horizontal-Vertical FoV
-                  c.PARAMSET_ANT_RAD_PAT: c.PARAMSET_ANT_RAD_PAT_VALS[0] # 'omni-directional'
-                  },
-              
-              # UE Antenna Parameters
-              c.PARAMSET_ANT_UE: {
-                  c.PARAMSET_ANT_SHAPE: np.array([4, 2]), # Antenna dimensions in X - Y - Z
-                  c.PARAMSET_ANT_SPACING: 0.5,
-                  c.PARAMSET_ANT_ROTATION: np.array([0, 0, 0]), # Rotation around X - Y - Z axes
-                  c.PARAMSET_ANT_FOV: np.array([360, 180]), # Horizontal-Vertical FoV
-                  c.PARAMSET_ANT_RAD_PAT: c.PARAMSET_ANT_RAD_PAT_VALS[0] # 'omni-directional'
-                  },
-              
-              c.PARAMSET_DOPPLER_EN: 0,
-              c.PARAMSET_POLAR_EN: 0,
-              c.PARAMSET_BS2BS: 1,
-              
-              c.PARAMSET_FDTD: 1 , 
-              # OFDM if 1 
-              # Time domain if 0.
-              # In time domain, the channel of 
-              # RX antennas x TX antennas x Number of available paths is generated.
-              # Each matrix of RX ant x TX ant represent the response matrix of that path.
-              
-              # OFDM Parameters
-              c.PARAMSET_OFDM: {
-                  c.PARAMSET_OFDM_SC_NUM: 512, # Number of total subcarriers
-                  c.PARAMSET_OFDM_SC_SAMP: np.arange(1), # Select subcarriers to generate
-                                    
-                  c.PARAMSET_OFDM_BW: 0.05, # GHz
-                  
-                  # Receive Low Pass / ADC Filter
-                  # 0: No Filter - Delta Function 
-                  # 1: Ideal (Rectangular) Low Pass Filter - Sinc Function
-                  c.PARAMSET_OFDM_LPF: 0
-                  }
-              }
+# -*- coding: utf-8 -*-
+"""
+DeepMIMOv2 Python Implementation
+
+Description: Parameters file
+
+Authors: Umut Demirhan, Ahmed Alkhateeb
+Date: 12/10/2021
+"""
+
+import numpy as np
+import DeepMIMOv3.consts as c
+
+def default_params():
+    params = {c.PARAMSET_DATASET_FOLDER: './Raytracing_scenarios',
+              c.PARAMSET_SCENARIO:'O1_60',
+              
+              # Dynamic scenario scene selection
+              c.PARAMSET_DYNAMIC_SCENES: np.array([1]),
+              
+              # Maximum # of paths to be loaded
+              c.PARAMSET_NUM_PATHS: 5,
+              
+              # Active Basestation IDs
+              c.PARAMSET_ACTIVE_BS: np.array([1]), # To be implemented
+              
+              # Selected user rows
+              c.PARAMSET_USER_ROWS: np.array([1]),
+              
+              # Subsampling
+              # c.PARAMSET_USER_ROW_SUBSAMP: 1,
+              c.PARAMSET_USER_SUBSAMP: 1,
+              
+              # BS Antenna Parameters
+              c.PARAMSET_ANT_BS: {
+                  c.PARAMSET_ANT_SHAPE: np.array([8, 4]), # Antenna dimensions in X - Y - Z
+                  c.PARAMSET_ANT_SPACING: 0.5,
+                  c.PARAMSET_ANT_ROTATION: np.array([0, 0, 0]), # Rotation around X - Y - Z axes
+                  c.PARAMSET_ANT_FOV: np.array([360, 180]), # Horizontal-Vertical FoV
+                  c.PARAMSET_ANT_RAD_PAT: c.PARAMSET_ANT_RAD_PAT_VALS[0] # 'omni-directional'
+                  },
+              
+              # UE Antenna Parameters
+              c.PARAMSET_ANT_UE: {
+                  c.PARAMSET_ANT_SHAPE: np.array([4, 2]), # Antenna dimensions in X - Y - Z
+                  c.PARAMSET_ANT_SPACING: 0.5,
+                  c.PARAMSET_ANT_ROTATION: np.array([0, 0, 0]), # Rotation around X - Y - Z axes
+                  c.PARAMSET_ANT_FOV: np.array([360, 180]), # Horizontal-Vertical FoV
+                  c.PARAMSET_ANT_RAD_PAT: c.PARAMSET_ANT_RAD_PAT_VALS[0] # 'omni-directional'
+                  },
+              
+              c.PARAMSET_DOPPLER_EN: 0,
+              c.PARAMSET_POLAR_EN: 0,
+              c.PARAMSET_BS2BS: 1,
+              
+              c.PARAMSET_FDTD: 1 , 
+              # OFDM if 1 
+              # Time domain if 0.
+              # In time domain, the channel of 
+              # RX antennas x TX antennas x Number of available paths is generated.
+              # Each matrix of RX ant x TX ant represent the response matrix of that path.
+              
+              # OFDM Parameters
+              c.PARAMSET_OFDM: {
+                  c.PARAMSET_OFDM_SC_NUM: 512, # Number of total subcarriers
+                  c.PARAMSET_OFDM_SC_SAMP: np.arange(1), # Select subcarriers to generate
+                                    
+                  c.PARAMSET_OFDM_BW: 0.05, # GHz
+                  
+                  # Receive Low Pass / ADC Filter
+                  # 0: No Filter - Delta Function 
+                  # 1: Ideal (Rectangular) Low Pass Filter - Sinc Function
+                  c.PARAMSET_OFDM_LPF: 0
+                  }
+              }
     return params
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3/raytracing_v2.py` & `deepmimov3-0.2.5/src/DeepMIMOv3/raytracing_v2.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-# -*- coding: utf-8 -*-
-"""
-DeepMIMOv3 Python Implementation
-
-Description: Read scenario files
-
-Authors: Umut Demirhan, Ahmed Alkhateeb
-Date: 12/10/2021
-"""
-
-import os
-import numpy as np
-from tqdm import tqdm
-import DeepMIMOv3.consts as c
-from DeepMIMOv3.utils import safe_print, PathVerifier, dbm2pow
-import scipy.io
-
-def read_raytracing(bs_id, params, user=True):
-    
-    scenario_files = os.path.join(params[c.PARAMSET_SCENARIO_FIL], params[c.PARAMSET_SCENARIO])
-    params[c.PARAMSET_SCENARIO_PARAMS] = load_scenario_params(params[c.PARAMSET_SCENARIO_PARAMS_PATH])
-    
-    if user:
-        generation_idx = params[c.PARAMSET_ACTIVE_UE] # Active User IDX
-    else:
-        generation_idx = params[c.PARAMSET_ACTIVE_BS]-1 # Active BS IDX
-        
-    ray_data = load_ray_data(scenario_files, bs_id, user=user)
-    data = extract_data_from_ray(ray_data, generation_idx, params)
-    
-    bs_loc = load_bs_loc(scenario_files, bs_id)
-    return data, bs_loc
-
-# Extracts the information to a dictionary from the loaded data file
-# for the users given in IDs, and with maximum number of paths
-def extract_data_from_ray(ray_data, ids, params):
-    
-    path_verifier = PathVerifier(params)
-    
-    num_channels = len(ids)
-    
-    pointer = 1 # First user ID
-    
-    # Generate empty user array of dictionaries
-    path_dict = {c.OUT_PATH_NUM: 0,
-                 c.OUT_PATH_DOD_PHI: [],
-                 c.OUT_PATH_DOD_THETA: [],
-                 c.OUT_PATH_DOA_PHI: [],
-                 c.OUT_PATH_DOA_THETA: [],
-                 c.OUT_PATH_PHASE: [],
-                 c.OUT_PATH_TOA: [],
-                 c.OUT_PATH_RX_POW: [],
-                 c.OUT_PATH_LOS: []
-                 }
-    data = {c.OUT_PATH: np.array([dict(path_dict) for j in range(len(ids))]),
-            c.OUT_LOS : np.zeros(num_channels, dtype=int),
-            c.OUT_LOC : np.zeros((num_channels, 3)),
-            c.OUT_DIST : np.zeros(num_channels),
-            c.OUT_PL : np.zeros(num_channels)
-            }
-    
-    j = 0
-    for user in tqdm(range(max(ids)+1), desc='Reading ray-tracing'):
-        pointer += 1 # Number of Paths
-        num_paths_available = int(ray_data[c.LOAD_FILE_EXT[0]][pointer]) # DoD file
-        pointer += 1 # First Path
-        if user in ids:
-            num_paths_read = min(num_paths_available, params[c.PARAMSET_NUM_PATHS])
-            path_limited_data_length = num_paths_read*4;
-                
-            if num_paths_available>0:
-                data[c.OUT_PATH][j] = load_variables(num_paths_read=num_paths_read, 
-                                                     path_DoD=ray_data[c.LOAD_FILE_EXT[0]][(pointer):(pointer+path_limited_data_length)], 
-                                                     path_DoA=ray_data[c.LOAD_FILE_EXT[1]][(pointer):(pointer+path_limited_data_length)], 
-                                                     path_CIR=ray_data[c.LOAD_FILE_EXT[2]][(pointer):(pointer+path_limited_data_length)], 
-                                                     LoS_status=ray_data[c.LOAD_FILE_EXT[3]][user+1],
-                                                     path_verifier=path_verifier, 
-                                                     params=params)
-                data[c.OUT_PL][j] = ray_data[c.LOAD_FILE_EXT[4]][user, 1]
-                
-            data[c.OUT_LOS][j] = ray_data[c.LOAD_FILE_EXT[3]][user+1]
-            data[c.OUT_LOC][j] = ray_data[c.LOAD_FILE_EXT[5]][user, 1:4]
-            data[c.OUT_DIST][j] = ray_data[c.LOAD_FILE_EXT[4]][user, 0]
-            j += 1
-            
-        pointer += num_paths_available*4
-        
-    path_verifier.notify()
-    
-    # The reading operation of the raytracing is linear
-    # Therefore, it is re-ordered to return in the same order of user IDs
-    rev_argsort = np.empty(ids.shape, dtype=np.intp)
-    rev_argsort[np.argsort(ids)] = np.arange(len(ids))
-    for dict_key in data.keys():
-        data[dict_key] = data[dict_key][rev_argsort]
-    return data
-
-# Split variables into a dictionary
-def load_variables(num_paths_read, path_DoD, path_DoA, path_CIR, LoS_status, path_verifier, params):
-    user_data = dict()
-    user_data[c.OUT_PATH_NUM] = num_paths_read
-    user_data[c.OUT_PATH_DOD_PHI] = path_DoD[1::4]
-    user_data[c.OUT_PATH_DOD_THETA] = path_DoD[2::4]
-    user_data[c.OUT_PATH_DOA_PHI] = path_DoA[1::4]
-    user_data[c.OUT_PATH_DOA_THETA] = path_DoA[2::4]
-    user_data[c.OUT_PATH_PHASE] = path_CIR[1::4]
-    user_data[c.OUT_PATH_TOA] = path_CIR[2::4]
-    
-    aux = np.zeros_like(user_data[c.OUT_PATH_TOA])
-    aux[0] = LoS_status
-    user_data[c.OUT_PATH_LOS] = aux
-    
-    user_data[c.OUT_PATH_RX_POW] = dbm2pow(path_CIR[3::4] + 30 - params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_TX_POW])
-    path_verifier.verify_path(user_data[c.OUT_PATH_TOA], user_data[c.OUT_PATH_RX_POW])
-    return user_data
-
-
-def load_scenario_params(scenario_params_path):
-    data = scipy.io.loadmat(scenario_params_path)
-    scenario_params = {
-                        c.PARAMSET_SCENARIO_PARAMS_CF: data[c.LOAD_FILE_SP_CF].astype(float).item(),
-                        c.PARAMSET_SCENARIO_PARAMS_TX_POW: data[c.LOAD_FILE_SP_TX_POW].astype(float).item(),
-                        c.PARAMSET_SCENARIO_PARAMS_NUM_BS: data[c.LOAD_FILE_SP_NUM_BS].astype(int).item(),
-                        c.PARAMSET_SCENARIO_PARAMS_USER_GRIDS: data[c.LOAD_FILE_SP_USER_GRIDS].astype(int),
-                        c.PARAMSET_SCENARIO_PARAMS_DOPPLER_EN: 0,
-                        c.PARAMSET_SCENARIO_PARAMS_POLAR_EN: 0
-                      }
-    return scenario_params
-
-def load_bs_loc(scenario_files, bs_id):
-    TX_loc_file = scenario_files + '.TX_Loc.mat'
-    data = scipy.io.loadmat(TX_loc_file)
-    return data[list(data.keys())[3]].astype(float)[bs_id-1, 1:4]
-
-# Loads the user and basestation dataset files
-def load_ray_data(scenario_files, bs_id, user=True):
-    # File Types and Directories
-    file_list = c.LOAD_FILE_EXT
-    file_list_reshape = c.LOAD_FILE_EXT_FLATTEN
-    
-    if user:
-        file_loc = [scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[0], 
-                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[1], 
-                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[2], 
-                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[3],
-                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[4],
-                    scenario_files +  '.' + c.LOAD_FILE_EXT_UE[5]]
-    else: # Basestation
-        file_loc = [scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[0], 
-                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[1], 
-                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[2], 
-                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[3],
-                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[4], 
-                    scenario_files +  '.' + c.LOAD_FILE_EXT_BS[5]]
-    
-    # Load files
-    ray_data = dict.fromkeys(file_list)
-    for i in range(len(file_list)):
-        data = scipy.io.loadmat(file_loc[i])
-        ray_data[file_list[i]] = data[list(data.keys())[3]]
-        if file_list_reshape[i]:
-            ray_data[file_list[i]] = ray_data[file_list[i]].reshape(-1) # 3rd key is the data
-
+# -*- coding: utf-8 -*-
+"""
+DeepMIMOv3 Python Implementation
+
+Description: Read scenario files
+
+Authors: Umut Demirhan, Ahmed Alkhateeb
+Date: 12/10/2021
+"""
+
+import os
+import numpy as np
+from tqdm import tqdm
+import DeepMIMOv3.consts as c
+from DeepMIMOv3.utils import safe_print, PathVerifier, dbm2pow
+import scipy.io
+
+def read_raytracing(bs_id, params, user=True):
+    
+    scenario_files = os.path.join(params[c.PARAMSET_SCENARIO_FIL], params[c.PARAMSET_SCENARIO])
+    params[c.PARAMSET_SCENARIO_PARAMS] = load_scenario_params(params[c.PARAMSET_SCENARIO_PARAMS_PATH])
+    
+    if user:
+        generation_idx = params[c.PARAMSET_ACTIVE_UE] # Active User IDX
+    else:
+        generation_idx = params[c.PARAMSET_ACTIVE_BS]-1 # Active BS IDX
+        
+    ray_data = load_ray_data(scenario_files, bs_id, user=user)
+    data = extract_data_from_ray(ray_data, generation_idx, params)
+    
+    bs_loc = load_bs_loc(scenario_files, bs_id)
+    return data, bs_loc
+
+# Extracts the information to a dictionary from the loaded data file
+# for the users given in IDs, and with maximum number of paths
+def extract_data_from_ray(ray_data, ids, params):
+    
+    path_verifier = PathVerifier(params)
+    
+    num_channels = len(ids)
+    
+    pointer = 1 # First user ID
+    
+    # Generate empty user array of dictionaries
+    path_dict = {c.OUT_PATH_NUM: 0,
+                 c.OUT_PATH_DOD_PHI: [],
+                 c.OUT_PATH_DOD_THETA: [],
+                 c.OUT_PATH_DOA_PHI: [],
+                 c.OUT_PATH_DOA_THETA: [],
+                 c.OUT_PATH_PHASE: [],
+                 c.OUT_PATH_TOA: [],
+                 c.OUT_PATH_RX_POW: [],
+                 c.OUT_PATH_LOS: []
+                 }
+    data = {c.OUT_PATH: np.array([dict(path_dict) for j in range(len(ids))]),
+            c.OUT_LOS : np.zeros(num_channels, dtype=int),
+            c.OUT_LOC : np.zeros((num_channels, 3)),
+            c.OUT_DIST : np.zeros(num_channels),
+            c.OUT_PL : np.zeros(num_channels)
+            }
+    
+    j = 0
+    for user in tqdm(range(max(ids)+1), desc='Reading ray-tracing'):
+        pointer += 1 # Number of Paths
+        num_paths_available = int(ray_data[c.LOAD_FILE_EXT[0]][pointer]) # DoD file
+        pointer += 1 # First Path
+        if user in ids:
+            num_paths_read = min(num_paths_available, params[c.PARAMSET_NUM_PATHS])
+            path_limited_data_length = num_paths_read*4;
+                
+            if num_paths_available>0:
+                data[c.OUT_PATH][j] = load_variables(num_paths_read=num_paths_read, 
+                                                     path_DoD=ray_data[c.LOAD_FILE_EXT[0]][(pointer):(pointer+path_limited_data_length)], 
+                                                     path_DoA=ray_data[c.LOAD_FILE_EXT[1]][(pointer):(pointer+path_limited_data_length)], 
+                                                     path_CIR=ray_data[c.LOAD_FILE_EXT[2]][(pointer):(pointer+path_limited_data_length)], 
+                                                     LoS_status=ray_data[c.LOAD_FILE_EXT[3]][user+1],
+                                                     path_verifier=path_verifier, 
+                                                     params=params)
+                data[c.OUT_PL][j] = ray_data[c.LOAD_FILE_EXT[4]][user, 1]
+                
+            data[c.OUT_LOS][j] = ray_data[c.LOAD_FILE_EXT[3]][user+1]
+            data[c.OUT_LOC][j] = ray_data[c.LOAD_FILE_EXT[5]][user, 1:4]
+            data[c.OUT_DIST][j] = ray_data[c.LOAD_FILE_EXT[4]][user, 0]
+            j += 1
+            
+        pointer += num_paths_available*4
+        
+    path_verifier.notify()
+    
+    # The reading operation of the raytracing is linear
+    # Therefore, it is re-ordered to return in the same order of user IDs
+    rev_argsort = np.empty(ids.shape, dtype=np.intp)
+    rev_argsort[np.argsort(ids)] = np.arange(len(ids))
+    for dict_key in data.keys():
+        data[dict_key] = data[dict_key][rev_argsort]
+    return data
+
+# Split variables into a dictionary
+def load_variables(num_paths_read, path_DoD, path_DoA, path_CIR, LoS_status, path_verifier, params):
+    user_data = dict()
+    user_data[c.OUT_PATH_NUM] = num_paths_read
+    user_data[c.OUT_PATH_DOD_PHI] = path_DoD[1::4]
+    user_data[c.OUT_PATH_DOD_THETA] = path_DoD[2::4]
+    user_data[c.OUT_PATH_DOA_PHI] = path_DoA[1::4]
+    user_data[c.OUT_PATH_DOA_THETA] = path_DoA[2::4]
+    user_data[c.OUT_PATH_PHASE] = path_CIR[1::4]
+    user_data[c.OUT_PATH_TOA] = path_CIR[2::4]
+    
+    aux = np.zeros_like(user_data[c.OUT_PATH_TOA])
+    aux[0] = LoS_status
+    user_data[c.OUT_PATH_LOS] = aux
+    
+    user_data[c.OUT_PATH_RX_POW] = dbm2pow(path_CIR[3::4] + 30 - params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_TX_POW])
+    path_verifier.verify_path(user_data[c.OUT_PATH_TOA], user_data[c.OUT_PATH_RX_POW])
+    return user_data
+
+
+def load_scenario_params(scenario_params_path):
+    data = scipy.io.loadmat(scenario_params_path)
+    scenario_params = {
+                        c.PARAMSET_SCENARIO_PARAMS_CF: data[c.LOAD_FILE_SP_CF].astype(float).item(),
+                        c.PARAMSET_SCENARIO_PARAMS_TX_POW: data[c.LOAD_FILE_SP_TX_POW].astype(float).item(),
+                        c.PARAMSET_SCENARIO_PARAMS_NUM_BS: data[c.LOAD_FILE_SP_NUM_BS].astype(int).item(),
+                        c.PARAMSET_SCENARIO_PARAMS_USER_GRIDS: data[c.LOAD_FILE_SP_USER_GRIDS].astype(int),
+                        c.PARAMSET_SCENARIO_PARAMS_DOPPLER_EN: 0,
+                        c.PARAMSET_SCENARIO_PARAMS_POLAR_EN: 0
+                      }
+    return scenario_params
+
+def load_bs_loc(scenario_files, bs_id):
+    TX_loc_file = scenario_files + '.TX_Loc.mat'
+    data = scipy.io.loadmat(TX_loc_file)
+    return data[list(data.keys())[3]].astype(float)[bs_id-1, 1:4]
+
+# Loads the user and basestation dataset files
+def load_ray_data(scenario_files, bs_id, user=True):
+    # File Types and Directories
+    file_list = c.LOAD_FILE_EXT
+    file_list_reshape = c.LOAD_FILE_EXT_FLATTEN
+    
+    if user:
+        file_loc = [scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[0], 
+                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[1], 
+                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[2], 
+                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[3],
+                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_UE[4],
+                    scenario_files +  '.' + c.LOAD_FILE_EXT_UE[5]]
+    else: # Basestation
+        file_loc = [scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[0], 
+                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[1], 
+                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[2], 
+                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[3],
+                    scenario_files +  '.%i.' % bs_id + c.LOAD_FILE_EXT_BS[4], 
+                    scenario_files +  '.' + c.LOAD_FILE_EXT_BS[5]]
+    
+    # Load files
+    ray_data = dict.fromkeys(file_list)
+    for i in range(len(file_list)):
+        data = scipy.io.loadmat(file_loc[i])
+        ray_data[file_list[i]] = data[list(data.keys())[3]]
+        if file_list_reshape[i]:
+            ray_data[file_list[i]] = ray_data[file_list[i]].reshape(-1) # 3rd key is the data
+
     return ray_data
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3/raytracing_v3.py` & `deepmimov3-0.2.5/src/DeepMIMOv3/raytracing_v3.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-# -*- coding: utf-8 -*-
-"""
-DeepMIMOv3 Python Implementation
-
-Description: Read scenario files
-
-Authors: Umut Demirhan, Ahmed Alkhateeb
-Date: 12/10/2021
-"""
-
-import os
-import numpy as np
-from tqdm import tqdm
-import DeepMIMOv3.consts as c
-from DeepMIMOv3.utils import safe_print, PathVerifier, dbm2pow
-import scipy.io
-import glob
-
-def read_raytracing(bs_id, params, user=True):
-    
-    params[c.PARAMSET_SCENARIO_PARAMS] = load_scenario_params(params[c.PARAMSET_SCENARIO_PARAMS_PATH])
-    
-    if user:
-        generation_idx = params[c.PARAMSET_ACTIVE_UE] # Active User IDX
-    else:
-        generation_idx = params[c.PARAMSET_ACTIVE_BS]-1 # Active BS IDX
-        
-    ray_data, rx_locs, tx_loc = load_ray_data(generation_idx, bs_id, params, user)
-    
-    if params['scenario_params']['dual_polar_available'] and params['enable_dual_polar']:
-        ray_data_out = {}
-        for i, polar_str in enumerate(['VV', 'VH', 'HH', 'HV']):
-            ray_data_out[polar_str] = extract_data_from_ray(ray_data[i], rx_locs, params)
-    else:
-        ray_data_out = extract_data_from_ray(ray_data, rx_locs, params)
-    
-    return ray_data_out, tx_loc
-
-# Extracts the information to a dictionary from the loaded data file
-# for the users given in IDs, and with maximum number of paths
-def extract_data_from_ray(ray_data, rx_locs, params):
-    
-    path_verifier = PathVerifier(params)
-    
-    num_channels = ray_data.shape[0]
-    # Generate empty user array of dictionaries
-    path_dict = {c.OUT_PATH_NUM: 0,
-                 c.OUT_PATH_DOD_PHI: [],
-                 c.OUT_PATH_DOD_THETA: [],
-                 c.OUT_PATH_DOA_PHI: [],
-                 c.OUT_PATH_DOA_THETA: [],
-                 c.OUT_PATH_PHASE: [],
-                 c.OUT_PATH_TOA: [],
-                 c.OUT_PATH_RX_POW: [],
-                 c.OUT_PATH_LOS: []
-                 }
-    if params[c.PARAMSET_SCENARIO_PARAMS][c.LOAD_FILE_SP_DOPPLER]:
-        path_dict[c.OUT_PATH_DOP_VEL] = []
-        path_dict[c.OUT_PATH_DOP_ACC] = []
-    
-    data = {c.OUT_PATH: np.array([dict(path_dict) for j in range(num_channels)]),
-            c.OUT_LOS : np.zeros(num_channels, dtype=int)
-            }
-    if num_channels>0:
-        data[c.OUT_LOC] = rx_locs[:, :3]
-        data[c.OUT_DIST] = rx_locs[:, 3]
-        data[c.OUT_PL] = rx_locs[:, 4]
-    else:
-        data[c.OUT_LOC] = np.zeros((num_channels, 3), dtype=float)
-        data[c.OUT_DIST] = np.zeros(num_channels, dtype=float)
-        data[c.OUT_PL] = np.zeros(num_channels, dtype=float)
-    
-    for user in tqdm(range(num_channels), desc='Reading ray-tracing'):
-        num_paths_available = int(ray_data[user][0].shape[1])
-        if num_paths_available>0:
-            data[c.OUT_PATH][user] = load_variables(ray_data[user][0], path_verifier, params)
-        
-    path_verifier.notify()
-    
-    return data
-
-# Split variables into a dictionary
-def load_variables(path_params, path_verifier, params):
-    num_max_paths = params[c.PARAMSET_NUM_PATHS]
-    user_data = dict()
-    user_data[c.OUT_PATH_NUM] = min(num_mat_paths, path_params.shape[1])
-    user_data[c.OUT_PATH_PHASE] = path_params[0, :num_max_paths]
-    user_data[c.OUT_PATH_TOA] = path_params[1, :num_max_paths]
-    user_data[c.OUT_PATH_RX_POW] = dbm2pow(path_params[2, :num_max_paths] + 30 - params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_TX_POW])
-    user_data[c.OUT_PATH_DOA_PHI] = path_params[3, :num_max_paths]
-    user_data[c.OUT_PATH_DOA_THETA] = path_params[4, :num_max_paths]
-    user_data[c.OUT_PATH_DOD_PHI] = path_params[5, :num_max_paths]
-    user_data[c.OUT_PATH_DOD_THETA] = path_params[6, :num_max_paths]
-    user_data[c.OUT_PATH_LOS] =  path_params[7, :num_max_paths]
-    
-    if params[c.PARAMSET_SCENARIO_PARAMS][c.LOAD_FILE_SP_DOPPLER]:
-        if path_params.shape[0]>8:
-            user_data[c.OUT_PATH_DOP_VEL] =  path_params[8, :num_max_paths]
-            user_data[c.OUT_PATH_DOP_ACC] =  path_params[9, :num_max_paths]
-        else:
-            user_data[c.OUT_PATH_DOP_VEL] =  np.zeros(path_params[7, :num_max_paths].shape)
-            user_data[c.OUT_PATH_DOP_ACC] =  np.zeros(path_params[7, :num_max_paths].shape)
-        
-    path_verifier.verify_path(user_data[c.OUT_PATH_TOA], user_data[c.OUT_PATH_RX_POW])
-    
-    return user_data
-
-
-def load_scenario_params(scenario_params_path):
-    data = scipy.io.loadmat(scenario_params_path)
-    scenario_params = {
-                        c.PARAMSET_SCENARIO_PARAMS_CF: data[c.LOAD_FILE_SP_CF].astype(float).item(),
-                        c.PARAMSET_SCENARIO_PARAMS_TX_POW: data[c.LOAD_FILE_SP_TX_POW].astype(float).item(),
-                        c.PARAMSET_SCENARIO_PARAMS_NUM_BS: data[c.LOAD_FILE_SP_NUM_BS].astype(int).item(),
-                        c.PARAMSET_SCENARIO_PARAMS_USER_GRIDS: data[c.LOAD_FILE_SP_USER_GRIDS].astype(int),
-                        c.PARAMSET_SCENARIO_PARAMS_DOPPLER_EN: data[c.LOAD_FILE_SP_DOPPLER].astype(int).item(),
-                        c.PARAMSET_SCENARIO_PARAMS_POLAR_EN: data[c.LOAD_FILE_SP_POLAR].astype(int).item()
-                      }
-    return scenario_params
-
-# Loads the user and basestation dataset files
-def load_ray_data(generation_idx, bs_id, params, user=True):
-    
-    # File Types and Directories
-    ray_data = []
-    rx_locs = []
-    file_data = None
-    if user:
-        files = glob.glob(os.path.join(params[c.PARAMSET_SCENARIO_FIL], 'BS%i_UE*.mat'%bs_id))
-        for file in files:
-            filename = os.path.splitext(file)[0]
-            user_ids = filename.split('_')[-1]
-            file_start = int(user_ids.split('-')[0])
-            file_end = int(user_ids.split('-')[1])
-            users_in_file = np.logical_and(generation_idx >= file_start, generation_idx<file_end)
-            if np.sum(users_in_file)>0:
-                file_data = scipy.io.loadmat(file)
-                for user in generation_idx[users_in_file]: # May remove this for loop with array indexing
-                    if params['scenario_params']['dual_polar_available']:
-                        if params['enable_dual_polar']:
-                            ray_data.append(file_data['channels_VV'][0][user-file_start][0][0])
-                            ray_data.append(file_data['channels_VH'][0][user-file_start][0][0])
-                            ray_data.append(file_data['channels_HH'][0][user-file_start][0][0])
-                            ray_data.append(file_data['channels_HV'][0][user-file_start][0][0])
-                        else:
-                            ray_data.append(file_data['channels_VV'][0][user-file_start][0][0])
-                            
-                    else:
-                        ray_data.append(file_data['channels'][0][user-file_start][0][0])
-                    rx_locs.append(file_data['rx_locs'][user-file_start])
-    else:
-        file = os.path.join(params[c.PARAMSET_SCENARIO_FIL], 'BS%i_BS.mat'%bs_id)
-        file_data = scipy.io.loadmat(file)
-        for bs_idx in generation_idx:
-            if params['scenario_params']['dual_polar_available']:
-                if params['enable_dual_polar']:
-                    ray_data.append(file_data['channels_VV'][0][bs_idx][0][0])
-                    ray_data.append(file_data['channels_VH'][0][bs_idx][0][0])
-                    ray_data.append(file_data['channels_HH'][0][bs_idx][0][0])
-                    ray_data.append(file_data['channels_HV'][0][bs_idx][0][0])
-                else:
-                    ray_data.append(file_data['channels_VV'][0][bs_idx][0][0])
-                    
-            else:
-                ray_data.append(file_data['channels'][0][bs_idx][0][0])
-            rx_locs.append(file_data['rx_locs'][bs_idx])
-        
-    ray_data = np.array(ray_data)
-    if params['enable_dual_polar'] and params['scenario_params']['dual_polar_available']:
-        ray_data = ray_data.reshape((4, -1))
-        
-    rx_locs = np.array(rx_locs)
-    
-    if file_data is not None and 'tx_loc' in file_data:
-        tx_loc = file_data['tx_loc'].squeeze()
-    # If tx location is not available in the data
-    # pull it from the BS-BS file
-    else:
-        file = os.path.join(params[c.PARAMSET_SCENARIO_FIL], 'BS%i_BS.mat'%bs_id)
-        file_data = scipy.io.loadmat(file)
-        tx_loc = file_data['rx_locs'][bs_id-1][:3]
-    return ray_data, rx_locs, tx_loc
+# -*- coding: utf-8 -*-
+"""
+DeepMIMOv3 Python Implementation
+
+Description: Read scenario files
+
+Authors: Umut Demirhan, Ahmed Alkhateeb
+Date: 12/10/2021
+"""
+
+import os
+import numpy as np
+from tqdm import tqdm
+import DeepMIMOv3.consts as c
+from DeepMIMOv3.utils import safe_print, PathVerifier, dbm2pow
+import scipy.io
+import glob
+
+def read_raytracing(bs_id, params, user=True):
+    
+    params[c.PARAMSET_SCENARIO_PARAMS] = load_scenario_params(params[c.PARAMSET_SCENARIO_PARAMS_PATH])
+    
+    if user:
+        generation_idx = params[c.PARAMSET_ACTIVE_UE] # Active User IDX
+    else:
+        generation_idx = params[c.PARAMSET_ACTIVE_BS]-1 # Active BS IDX
+        
+    ray_data, rx_locs, tx_loc = load_ray_data(generation_idx, bs_id, params, user)
+    
+    if params['scenario_params']['dual_polar_available'] and params['enable_dual_polar']:
+        ray_data_out = {}
+        for i, polar_str in enumerate(['VV', 'VH', 'HH', 'HV']):
+            ray_data_out[polar_str] = extract_data_from_ray(ray_data[i], rx_locs, params)
+    else:
+        ray_data_out = extract_data_from_ray(ray_data, rx_locs, params)
+    
+    return ray_data_out, tx_loc
+
+# Extracts the information to a dictionary from the loaded data file
+# for the users given in IDs, and with maximum number of paths
+def extract_data_from_ray(ray_data, rx_locs, params):
+    
+    path_verifier = PathVerifier(params)
+    
+    num_channels = ray_data.shape[0]
+    # Generate empty user array of dictionaries
+    path_dict = {c.OUT_PATH_NUM: 0,
+                 c.OUT_PATH_DOD_PHI: [],
+                 c.OUT_PATH_DOD_THETA: [],
+                 c.OUT_PATH_DOA_PHI: [],
+                 c.OUT_PATH_DOA_THETA: [],
+                 c.OUT_PATH_PHASE: [],
+                 c.OUT_PATH_TOA: [],
+                 c.OUT_PATH_RX_POW: [],
+                 c.OUT_PATH_LOS: []
+                 }
+    if params[c.PARAMSET_SCENARIO_PARAMS][c.LOAD_FILE_SP_DOPPLER]:
+        path_dict[c.OUT_PATH_DOP_VEL] = []
+        path_dict[c.OUT_PATH_DOP_ACC] = []
+    
+    data = {c.OUT_PATH: np.array([dict(path_dict) for j in range(num_channels)]),
+            c.OUT_LOS : np.zeros(num_channels, dtype=int)
+            }
+    if num_channels>0:
+        data[c.OUT_LOC] = rx_locs[:, :3]
+        data[c.OUT_DIST] = rx_locs[:, 3]
+        data[c.OUT_PL] = rx_locs[:, 4]
+    else:
+        data[c.OUT_LOC] = np.zeros((num_channels, 3), dtype=float)
+        data[c.OUT_DIST] = np.zeros(num_channels, dtype=float)
+        data[c.OUT_PL] = np.zeros(num_channels, dtype=float)
+    
+    for user in tqdm(range(num_channels), desc='Reading ray-tracing'):
+        num_paths_available = int(ray_data[user][0].shape[1])
+        if num_paths_available>0:
+            data[c.OUT_PATH][user] = load_variables(ray_data[user][0], path_verifier, params)
+        
+    path_verifier.notify()
+    
+    return data
+
+# Split variables into a dictionary
+def load_variables(path_params, path_verifier, params):
+    num_max_paths = params[c.PARAMSET_NUM_PATHS]
+    user_data = dict()
+    user_data[c.OUT_PATH_NUM] = min(num_max_paths, path_params.shape[1])
+    user_data[c.OUT_PATH_PHASE] = path_params[0, :num_max_paths]
+    user_data[c.OUT_PATH_TOA] = path_params[1, :num_max_paths]
+    user_data[c.OUT_PATH_RX_POW] = dbm2pow(path_params[2, :num_max_paths] + 30 - params[c.PARAMSET_SCENARIO_PARAMS][c.PARAMSET_SCENARIO_PARAMS_TX_POW])
+    user_data[c.OUT_PATH_DOA_PHI] = path_params[3, :num_max_paths]
+    user_data[c.OUT_PATH_DOA_THETA] = path_params[4, :num_max_paths]
+    user_data[c.OUT_PATH_DOD_PHI] = path_params[5, :num_max_paths]
+    user_data[c.OUT_PATH_DOD_THETA] = path_params[6, :num_max_paths]
+    user_data[c.OUT_PATH_LOS] =  path_params[7, :num_max_paths]
+    
+    if params[c.PARAMSET_SCENARIO_PARAMS][c.LOAD_FILE_SP_DOPPLER]:
+        if path_params.shape[0]>8:
+            user_data[c.OUT_PATH_DOP_VEL] =  path_params[8, :num_max_paths]
+            user_data[c.OUT_PATH_DOP_ACC] =  path_params[9, :num_max_paths]
+        else:
+            user_data[c.OUT_PATH_DOP_VEL] =  np.zeros(path_params[7, :num_max_paths].shape)
+            user_data[c.OUT_PATH_DOP_ACC] =  np.zeros(path_params[7, :num_max_paths].shape)
+        
+    path_verifier.verify_path(user_data[c.OUT_PATH_TOA], user_data[c.OUT_PATH_RX_POW])
+    
+    return user_data
+
+
+def load_scenario_params(scenario_params_path):
+    data = scipy.io.loadmat(scenario_params_path)
+    scenario_params = {
+                        c.PARAMSET_SCENARIO_PARAMS_CF: data[c.LOAD_FILE_SP_CF].astype(float).item(),
+                        c.PARAMSET_SCENARIO_PARAMS_TX_POW: data[c.LOAD_FILE_SP_TX_POW].astype(float).item(),
+                        c.PARAMSET_SCENARIO_PARAMS_NUM_BS: data[c.LOAD_FILE_SP_NUM_BS].astype(int).item(),
+                        c.PARAMSET_SCENARIO_PARAMS_USER_GRIDS: data[c.LOAD_FILE_SP_USER_GRIDS].astype(int),
+                        c.PARAMSET_SCENARIO_PARAMS_DOPPLER_EN: data[c.LOAD_FILE_SP_DOPPLER].astype(int).item(),
+                        c.PARAMSET_SCENARIO_PARAMS_POLAR_EN: data[c.LOAD_FILE_SP_POLAR].astype(int).item()
+                      }
+    return scenario_params
+
+# Loads the user and basestation dataset files
+def load_ray_data(generation_idx, bs_id, params, user=True):
+    
+    # File Types and Directories
+    ray_data = []
+    rx_locs = []
+    file_data = None
+    if user:
+        files = glob.glob(os.path.join(params[c.PARAMSET_SCENARIO_FIL], 'BS%i_UE*.mat'%bs_id))
+        for file in files:
+            filename = os.path.splitext(file)[0]
+            user_ids = filename.split('_')[-1]
+            file_start = int(user_ids.split('-')[0])
+            file_end = int(user_ids.split('-')[1])
+            users_in_file = np.logical_and(generation_idx >= file_start, generation_idx<file_end)
+            if np.sum(users_in_file)>0:
+                file_data = scipy.io.loadmat(file)
+                for user in generation_idx[users_in_file]: # May remove this for loop with array indexing
+                    if params['scenario_params']['dual_polar_available']:
+                        if params['enable_dual_polar']:
+                            ray_data.append(file_data['channels_VV'][0][user-file_start][0][0])
+                            ray_data.append(file_data['channels_VH'][0][user-file_start][0][0])
+                            ray_data.append(file_data['channels_HH'][0][user-file_start][0][0])
+                            ray_data.append(file_data['channels_HV'][0][user-file_start][0][0])
+                        else:
+                            ray_data.append(file_data['channels_VV'][0][user-file_start][0][0])
+                            
+                    else:
+                        ray_data.append(file_data['channels'][0][user-file_start][0][0])
+                    rx_locs.append(file_data['rx_locs'][user-file_start])
+    else:
+        file = os.path.join(params[c.PARAMSET_SCENARIO_FIL], 'BS%i_BS.mat'%bs_id)
+        file_data = scipy.io.loadmat(file)
+        for bs_idx in generation_idx:
+            if params['scenario_params']['dual_polar_available']:
+                if params['enable_dual_polar']:
+                    ray_data.append(file_data['channels_VV'][0][bs_idx][0][0])
+                    ray_data.append(file_data['channels_VH'][0][bs_idx][0][0])
+                    ray_data.append(file_data['channels_HH'][0][bs_idx][0][0])
+                    ray_data.append(file_data['channels_HV'][0][bs_idx][0][0])
+                else:
+                    ray_data.append(file_data['channels_VV'][0][bs_idx][0][0])
+                    
+            else:
+                ray_data.append(file_data['channels'][0][bs_idx][0][0])
+            rx_locs.append(file_data['rx_locs'][bs_idx])
+        
+    ray_data = np.array(ray_data)
+    if params['enable_dual_polar'] and params['scenario_params']['dual_polar_available']:
+        ray_data = ray_data.reshape((4, -1))
+        
+    rx_locs = np.array(rx_locs)
+    
+    if file_data is not None and 'tx_loc' in file_data:
+        tx_loc = file_data['tx_loc'].squeeze()
+    # If tx location is not available in the data
+    # pull it from the BS-BS file
+    else:
+        file = os.path.join(params[c.PARAMSET_SCENARIO_FIL], 'BS%i_BS.mat'%bs_id)
+        file_data = scipy.io.loadmat(file)
+        tx_loc = file_data['rx_locs'][bs_id-1][:3]
+    return ray_data, rx_locs, tx_loc
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3/sionna_adapter.py` & `deepmimov3-0.2.5/src/DeepMIMOv3/sionna_adapter.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Sat Jul 16 10:53:50 2022
-
-@author: Umut Demirhan, Ahmed Alkhateeb
-"""
-import numpy as np
-
-# The DeepMIMO dataset adapter for Sionna
-#
-# Input: DeepMIMO dataset, UE and BS indices to be included
-#
-# For a given 1D vector of BS or UE indices, the generated dataset will be stacked as different samples
-#
-# By default, the adapter will only select the first BS of the DeepMIMO dataset and all UEs
-# The adapter assumes BSs are transmitters and users are receivers. 
-# Uplink channels could be generated using (transpose) reciprocity.
-#
-# For multi-user channels, provide a 2D numpy matrix of size (num_samples x num_rx)
-#
-# Examples:
-# ue_idx = np.array([[0, 1 ,2], [1, 2, 3]]) generates (num_bs x 3 UEs) channels
-# with 2 data samples from the BSs to the UEs [0, 1, 2] and [1, 2, 3], respectively.
-#
-# For single-basestation channels with the data from different basestations stacked,
-# provide a 1D array of basestation indices
-#
-# For multi-BS channels, provide a 2D numpy matrix of (num_samples x num_tx)
-#
-# Examples:
-# bs_idx = np.array([[0, 1], [2, 3], [4, 5]]) generates (2 BSs x num_rx) channels
-# by stacking the data of channels from the basestations (0 and 1), (2 and 3), 
-# and (4 and 5) to the UEs.
-#
-class DeepMIMOSionnaAdapter:
-    def __init__(self, DeepMIMO_dataset, bs_idx = None, ue_idx = None):
-        self.dataset = DeepMIMO_dataset
-        
-        # Set bs_idx based on given parameters
-        # If no input is given, choose the first basestation
-        if bs_idx is None:
-            bs_idx = np.array([[0]])
-        self.bs_idx = self._verify_idx(bs_idx)
-        
-        # Set ue_idx based on given parameters
-        # If no input is given, set all user indices
-        if ue_idx is None:
-            ue_idx = np.arange(DeepMIMO_dataset[0]['user']['channel'].shape[0])
-        self.ue_idx = self._verify_idx(ue_idx)
-        
-        # Extract number of antennas from the DeepMIMO dataset
-        self.num_rx_ant = DeepMIMO_dataset[0]['user']['channel'].shape[1]
-        self.num_tx_ant = DeepMIMO_dataset[0]['user']['channel'].shape[2]
-        
-        # Determine the number of samples based on the given indices
-        self.num_samples_bs = self.bs_idx.shape[0]
-        self.num_samples_ue = self.ue_idx.shape[0]
-        self.num_samples = self.num_samples_bs * self.num_samples_ue
-        
-        # Determine the number of tx and rx elements in each channel sample based on the given indices
-        self.num_rx = self.ue_idx.shape[1]
-        self.num_tx = self.bs_idx.shape[1]
-        
-        # Determine the number of available paths in the DeepMIMO dataset
-        self.num_paths = DeepMIMO_dataset[0]['user']['channel'].shape[-1]
-        self.num_time_steps = 1 # Time step = 1 for static scenarios
-        
-        # The required path power shape for Sionna
-        self.ch_shape = (self.num_rx, 
-                         self.num_rx_ant, 
-                         self.num_tx, 
-                         self.num_tx_ant, 
-                         self.num_paths, 
-                         self.num_time_steps)
-        
-        # The required path delay shape for Sionna
-        self.t_shape = (self.num_rx, self.num_tx, self.num_paths)
-    
-    # Verify the index values given as input
-    def _verify_idx(self, idx):
-        idx = self._idx_to_numpy(idx)
-        idx = self._numpy_size_check(idx)
-        return idx
-    
-    # Convert the possible input types to numpy (integer - range - list)
-    def _idx_to_numpy(self, idx):
-        if isinstance(idx, int): # If the input is an integer - a single ID - convert it to 2D numpy array
-            idx = np.array([[idx]])
-        elif isinstance(idx, list) or isinstance(idx, range): # If the input is a list or range - convert it to a numpy array
-            idx = np.array(idx)
-        elif isinstance(idx, np.ndarray):
-            pass
-        else:
-            raise TypeError('The index input type must be an integer, list, or numpy array!') 
-        return idx
-    
-    # Check the size of the given input and convert it to a 2D matrix of proper shape (num_tx x num_samples) or (num_rx x num_samples)
-    def _numpy_size_check(self, idx):
-        if len(idx.shape) == 1:
-            idx = idx.reshape((-1, 1))
-        elif len(idx.shape) == 2:
-            pass
-        else:
-            raise ValueError('The index input must be integer, vector or 2D matrix!')
-        return idx
-    
-    # Override length of the generator to provide the available number of samples
-    def __len__(self):
-        return self.num_samples
-        
-    # Provide samples each time the generator is called
-    def __call__(self):
-        for i in range(self.num_samples_ue): # For each UE sample
-            for j in range(self.num_samples_bs): # For each BS sample
-                # Generate zero vectors for the Sionna sample
-                a = np.zeros(self.ch_shape, dtype=np.csingle)
-                tau = np.zeros(self.t_shape, dtype=np.single)
-                
-                # Place the DeepMIMO dataset power and delays into the channel sample for Sionna
-                for i_ch in range(self.num_rx): # for each receiver in the sample
-                    for j_ch in range(self.num_tx): # for each transmitter in the sample
-                        i_ue = self.ue_idx[i][i_ch] # UE channel sample i - channel RX i_ch
-                        i_bs = self.bs_idx[j][j_ch] # BS channel sample i - channel TX j_ch
-                        a[i_ch, :, j_ch, :, :, 0] = self.dataset[i_bs]['user']['channel'][i_ue]
-                        tau[i_ch, j_ch, :self.dataset[i_bs]['user']['paths'][i_ue]['num_paths']] = self.dataset[i_bs]['user']['paths'][i_ue]['ToA'] 
-                
-                yield (a, tau) # yield this sample
+# -*- coding: utf-8 -*-
+"""
+Created on Sat Jul 16 10:53:50 2022
+
+@author: Umut Demirhan, Ahmed Alkhateeb
+"""
+import numpy as np
+
+# The DeepMIMO dataset adapter for Sionna
+#
+# Input: DeepMIMO dataset, UE and BS indices to be included
+#
+# For a given 1D vector of BS or UE indices, the generated dataset will be stacked as different samples
+#
+# By default, the adapter will only select the first BS of the DeepMIMO dataset and all UEs
+# The adapter assumes BSs are transmitters and users are receivers. 
+# Uplink channels could be generated using (transpose) reciprocity.
+#
+# For multi-user channels, provide a 2D numpy matrix of size (num_samples x num_rx)
+#
+# Examples:
+# ue_idx = np.array([[0, 1 ,2], [1, 2, 3]]) generates (num_bs x 3 UEs) channels
+# with 2 data samples from the BSs to the UEs [0, 1, 2] and [1, 2, 3], respectively.
+#
+# For single-basestation channels with the data from different basestations stacked,
+# provide a 1D array of basestation indices
+#
+# For multi-BS channels, provide a 2D numpy matrix of (num_samples x num_tx)
+#
+# Examples:
+# bs_idx = np.array([[0, 1], [2, 3], [4, 5]]) generates (2 BSs x num_rx) channels
+# by stacking the data of channels from the basestations (0 and 1), (2 and 3), 
+# and (4 and 5) to the UEs.
+#
+class DeepMIMOSionnaAdapter:
+    def __init__(self, DeepMIMO_dataset, bs_idx = None, ue_idx = None):
+        self.dataset = DeepMIMO_dataset
+        
+        # Set bs_idx based on given parameters
+        # If no input is given, choose the first basestation
+        if bs_idx is None:
+            bs_idx = np.array([[0]])
+        self.bs_idx = self._verify_idx(bs_idx)
+        
+        # Set ue_idx based on given parameters
+        # If no input is given, set all user indices
+        if ue_idx is None:
+            ue_idx = np.arange(DeepMIMO_dataset[0]['user']['channel'].shape[0])
+        self.ue_idx = self._verify_idx(ue_idx)
+        
+        # Extract number of antennas from the DeepMIMO dataset
+        self.num_rx_ant = DeepMIMO_dataset[0]['user']['channel'].shape[1]
+        self.num_tx_ant = DeepMIMO_dataset[0]['user']['channel'].shape[2]
+        
+        # Determine the number of samples based on the given indices
+        self.num_samples_bs = self.bs_idx.shape[0]
+        self.num_samples_ue = self.ue_idx.shape[0]
+        self.num_samples = self.num_samples_bs * self.num_samples_ue
+        
+        # Determine the number of tx and rx elements in each channel sample based on the given indices
+        self.num_rx = self.ue_idx.shape[1]
+        self.num_tx = self.bs_idx.shape[1]
+        
+        # Determine the number of available paths in the DeepMIMO dataset
+        self.num_paths = DeepMIMO_dataset[0]['user']['channel'].shape[-1]
+        self.num_time_steps = 1 # Time step = 1 for static scenarios
+        
+        # The required path power shape for Sionna
+        self.ch_shape = (self.num_rx, 
+                         self.num_rx_ant, 
+                         self.num_tx, 
+                         self.num_tx_ant, 
+                         self.num_paths, 
+                         self.num_time_steps)
+        
+        # The required path delay shape for Sionna
+        self.t_shape = (self.num_rx, self.num_tx, self.num_paths)
+    
+    # Verify the index values given as input
+    def _verify_idx(self, idx):
+        idx = self._idx_to_numpy(idx)
+        idx = self._numpy_size_check(idx)
+        return idx
+    
+    # Convert the possible input types to numpy (integer - range - list)
+    def _idx_to_numpy(self, idx):
+        if isinstance(idx, int): # If the input is an integer - a single ID - convert it to 2D numpy array
+            idx = np.array([[idx]])
+        elif isinstance(idx, list) or isinstance(idx, range): # If the input is a list or range - convert it to a numpy array
+            idx = np.array(idx)
+        elif isinstance(idx, np.ndarray):
+            pass
+        else:
+            raise TypeError('The index input type must be an integer, list, or numpy array!') 
+        return idx
+    
+    # Check the size of the given input and convert it to a 2D matrix of proper shape (num_tx x num_samples) or (num_rx x num_samples)
+    def _numpy_size_check(self, idx):
+        if len(idx.shape) == 1:
+            idx = idx.reshape((-1, 1))
+        elif len(idx.shape) == 2:
+            pass
+        else:
+            raise ValueError('The index input must be integer, vector or 2D matrix!')
+        return idx
+    
+    # Override length of the generator to provide the available number of samples
+    def __len__(self):
+        return self.num_samples
+        
+    # Provide samples each time the generator is called
+    def __call__(self):
+        for i in range(self.num_samples_ue): # For each UE sample
+            for j in range(self.num_samples_bs): # For each BS sample
+                # Generate zero vectors for the Sionna sample
+                a = np.zeros(self.ch_shape, dtype=np.csingle)
+                tau = np.zeros(self.t_shape, dtype=np.single)
+                
+                # Place the DeepMIMO dataset power and delays into the channel sample for Sionna
+                for i_ch in range(self.num_rx): # for each receiver in the sample
+                    for j_ch in range(self.num_tx): # for each transmitter in the sample
+                        i_ue = self.ue_idx[i][i_ch] # UE channel sample i - channel RX i_ch
+                        i_bs = self.bs_idx[j][j_ch] # BS channel sample i - channel TX j_ch
+                        a[i_ch, :, j_ch, :, :, 0] = self.dataset[i_bs]['user']['channel'][i_ue]
+                        tau[i_ch, j_ch, :self.dataset[i_bs]['user']['paths'][i_ue]['num_paths']] = self.dataset[i_bs]['user']['paths'][i_ue]['ToA'] 
+                
+                yield (a, tau) # yield this sample
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3/utils.py` & `deepmimov3-0.2.5/src/DeepMIMOv3/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,292 +1,292 @@
-# -*- coding: utf-8 -*-
-"""
-DeepMIMOv3 Python Implementation
-
-Description: Utilities
-
-Authors: Umut Demirhan, Ahmed Alkhateeb
-Date: 12/10/2021
-"""
-
-import time
-import DeepMIMOv3.consts as c
-from DeepMIMOv3.construct_deepmimo import ant_indices, array_response
-import numpy as np
-
-################################# Internal ####################################
-
-# Sleep between print and tqdm displays
-def safe_print(text, stop_dur=0.3):
-    print(text)
-    time.sleep(stop_dur)
-        
-# Determine active paths with the given configurations
-# (For OFDM, only the paths within DS are activated)
-class PathVerifier:
-    def __init__(self, params):
-        self.params = params
-        if self.params[c.PARAMSET_FDTD]: # IF OFDM
-            Ts = 1 / (params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_BW]*c.PARAMSET_OFDM_BW_MULT)
-            self.FFT_duration = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_SC_NUM] * Ts
-            self.max_ToA = 0
-            self.path_ratio_FFT = []
-    
-    def verify_path(self, ToA, power):
-        if self.params[c.PARAMSET_FDTD]: # OFDM CH
-            m_toa = np.max(ToA)
-            self.max_ToA = max(self.max_ToA, m_toa)
-            
-            if m_toa > self.FFT_duration:
-                violating_paths = ToA > self.FFT_duration
-                self.path_ratio_FFT.append( sum(power[violating_paths])/sum(power) )
-                        
-    def notify(self):
-        if self.params[c.PARAMSET_FDTD]: # IF OFDM
-            avg_ratio_FFT = 0
-            if len(self.path_ratio_FFT) != 0:
-                avg_ratio_FFT = np.mean(self.path_ratio_FFT)*100
-                
-            if self.max_ToA > self.FFT_duration and avg_ratio_FFT >= 1.:
-                safe_print('ToA of some paths of %i channels with an average total power of %.2f%% exceed the useful OFDM symbol duration and are clipped.' % (len(self.path_ratio_FFT), avg_ratio_FFT))
-            
-
-
-
-################################## For User ###################################
-
-def dbm2pow(val):
-    return 10**(val/10 - 3)
-
-def steering_vec(array, phi=0, theta=0, spacing=0.5):
-    """
-    Creates the array steering vector for uniform (linear and rectangular) arrays.
-
-    Parameters
-    ----------
-    array : tuple, list or numpy.ndarray
-        Number of [elements along the horizontal, elements along the vertical]
-    phi : float, optional    
-        Azimuth angle in degrees. 0 azimuth is normal to the array. 
-        Positive azimuth points beams to the right. The default is 0.
-    theta : float, optional
-        Elevation angle in degrees. 0 elevation is horizon (normal to the array). 
-        Positive elevation tilts the beam downards. The default is 0.
-    spacing : flaot, optional
-        Antenna spacing in wavelengths. The default is 0.5.
-
-    Returns
-    -------
-    numpy.ndarray
-        The normalized array response vector.
-
-    """
-    idxs = ant_indices(array)
-    resp = array_response(idxs, phi*np.pi/180, theta*np.pi/180 + np.pi/2, 2*np.pi*spacing)
-    return resp / np.linalg.norm(resp)
-
-# TODO: add info field to dataset (so data like number of users per row doesn't 
-#       need to be read from the webstie). This way, we can make the arguments
-#       of this function defaults based on the dataset
-
-def uniform_sampling(sampling_div, n_rows, users_per_row):
-    """
-    Returns indices of users at uniform steps/intervals.
-    
-    Parameters
-    ----------
-    steps : list
-        Step size along x and y dimensions. The list should have 2 elements only.
-        Examples:
-        [1,1] = indices of all users
-        [1,2] = same number of users across x, one every two users along y. Results: half the users.
-        [2,2] = takes one user every 2 users (step=2), along x and y. Results: 1/4 the total users
-    n_rows : int
-        Number of rows in the generated dataset. Necessary for indexing users.
-    users_per_row : int
-        Number of users per row in the generated dataset. Necessary for indexing users.
-        
-    Returns
-    -------
-    data : list
-        List of undersampled indices.
-    """
-    cols = np.arange(users_per_row, step=sampling_div[0])
-    rows = np.arange(n_rows, step=sampling_div[1])
-    uniform_idxs = np.array([j + i*users_per_row for i in rows for j in cols])
-    
-    return uniform_idxs
-
-
-def trim_by_idx(dataset, idxs):
-    """
-    Returns a DeepMIMO dataset with only the selected user indices.
-
-    Parameters
-    ----------
-    dataset : DeepMIMO dataset (dictionary)
-        A dataset as the output of DeepMIMO.generate_data()
-    idxs : list or array
-        List of selected indices.
-
-    Returns
-    -------
-    dataset_t : DeepMIMO dataset (dictionary)
-        Trimmed dataset.
-    """
-    
-    if len(idxs) == dataset[0]['user']['location'].shape[0]:
-        return dataset
-    
-    dataset_t = []
-    for bs_idx in range(len(dataset)):
-        dataset_t.append({})
-        for key in dataset[bs_idx].keys():
-            dataset_t[bs_idx]['location'] = dataset[bs_idx]['location']
-            dataset_t[bs_idx]['user'] = {}
-            for key in dataset[bs_idx]['user']:
-                dataset_t[bs_idx]['user'][key] = dataset[bs_idx]['user'][key][idxs]
-        
-    return dataset_t
-
-
-
-class LinearPath():
-    def __init__(self, deepmimo_dataset, first_pos, last_pos, res=1, n_steps=False, filter_repeated=True):
-        """
-        Creates a linear path of features. 
-
-        Parameters
-        ----------
-        deepmimo_dataset : DeepMIMO dataset
-            A dataset generated from DeepMIMO.generate_data(parameters).
-        first_pos : numpy.ndarray
-            [x, y, (z)] position of the start of the linear path.
-        last_pos : numpy.ndarray
-            [x, y, (z)] position of the end of the linear path.
-        res : float, optional
-            Resolution [in meters]. The same as providing n_steps. The default is 1.
-        n_steps : int, optional
-            Number of positions / samples between first and last position (including).
-            If False, either uses the resolution parameter <res>. The default is False.
-        filter_repeated : bool, optional
-            Whether to eliminated repeated positions. 
-            Repeated positions happen when a path is oversampled or the closest
-            dataste position repeats for a set of path positions. 
-            If True, the repeated positions are removed. The default is True.
-
-        Returns
-        -------
-        None.
-
-        """
-        
-        if len(first_pos) == 2: # if not given, assume z-coordinate = 0
-            first_pos = np.concatenate((first_pos,[0]))
-            last_pos = np.concatenate((last_pos,[0]))
-            
-        self.first_pos = first_pos
-        self.last_pos = last_pos
-        
-        self.dataset = deepmimo_dataset if type(deepmimo_dataset) != list else deepmimo_dataset[0]
-        self._set_idxs_pos_res_steps(res, n_steps, filter_repeated)
-        self._copy_data_from_dataset()
-        self._extract_features()
-        
-    def _set_idxs_pos_res_steps(self, res, n_steps, filter_repeated):
-        dataset_pos = self.dataset['user']['location']
-        if not n_steps:
-            data_res = np.linalg.norm(dataset_pos[0] - dataset_pos[1])
-            if res < data_res and filter_repeated:
-                print(f'Changing resolution to {data_res} to eliminate repeated positions')
-                res = data_res
-                
-            self.n = int(np.linalg.norm(self.first_pos - self.last_pos) / res)
-        else:
-            self.n = n_steps
-        
-        xs = np.linspace(self.first_pos[0], self.last_pos[0], self.n).reshape((-1,1))
-        ys = np.linspace(self.first_pos[1], self.last_pos[1], self.n).reshape((-1,1))
-        zs = np.linspace(self.first_pos[2], self.last_pos[2], self.n).reshape((-1,1))
-        
-        interpolated_pos = np.hstack((xs,ys,zs))
-        idxs = np.array([np.argmin(np.linalg.norm(dataset_pos - pos, axis=1)) 
-                         for pos in interpolated_pos])
-        
-        if filter_repeated:
-            # soft: removes adjacent repeated only
-            idxs = np.concatenate(([idxs[0]], idxs[1:][(idxs[1:]-idxs[:-1]) != 0]))
-            
-            if filter_repeated == 'hard':
-                # hard: removes all repeated
-                idxs = np.unique(idxs)
-            
-            self.n = len(idxs)
-    
-        self.idxs = idxs
-        self.pos = dataset_pos[idxs]
-    
-    def _copy_data_from_dataset(self):
-        self.feature_names = ['LoS', 'pathloss', 'distance']
-        
-        self.LoS = self.dataset['user']['LoS'][self.idxs]
-        self.pathloss = self.dataset['user']['pathloss'][self.idxs]
-        self.distance = self.dataset['user']['distance'][self.idxs]
-        self.paths = self.dataset['user']['paths'][self.idxs]
-        self.channel = self.dataset['user']['channel'][self.idxs]
-        
-    def _extract_features(self):
-        # Main path features
-        self.path_features = ['DoD_phi', 'DoD_theta', 'DoA_phi', 'DoA_theta', 
-                              'ToA', 'phase', 'power']
-        self.feature_names += ['main_path_' + var for var in self.path_features]
-        for feat in self.path_features:
-            setattr(self, f'main_path_{feat}', 
-                    np.array([self.paths[i][feat][0] for i in range(self.n)]))#self.idxs]))
-        
-        # Other features
-        self.feature_names += ['pwr_ratio_main_path', 'total_power']
-        self.total_power = np.array([np.sum(self.paths[i]['power']) for i in range(self.n)])
-        self.pwr_ratio_main_path = np.array([self.main_path_power[i] / np.sum(self.paths[i]['power'])
-                                             if self.LoS[i] != -1 else np.nan for i in range(self.n)])
-
-    def get_feature_names(self):
-        return self.feature_names
-    
-# TODO: add more LinearPath functions
-# - To append paths use, for example: linpath3.append(linpath1, linpath2)
-# - To repeat back and forth: linpath3.append(linpath3.flip())
-# - Supposing the last position of linpath3 coincides with the first, it can be looped like:
-# linpath3.append(linpath3, linpath3, linpath3) or linpath3.repeat(3)
-
-
-
-def get_idxs_in_xy_box(data_pos, x_min, x_max, y_min, y_max):
-    """
-    Obtains the indices of <data_pos> that lie between the xy limits.
-
-    Parameters
-    ----------
-    data_pos : numpy.ndarray
-        Array with all positions. Dimensions: [n_positions, 2]
-    x_min : float
-        Minimum x limit. Only positions where x > x_min have their indices returned.
-    x_max : float
-        Maximum x limit. Only positions where x < x_max have their indices returned.
-    y_min : float
-        Minimum y limit. Only positions where y > y_min have their indices returned.
-    y_max : float
-        Maximum y limit. Only positions where y < y_max have their indices returned.
-
-    Returns
-    -------
-    numpy.ndarray
-        Indices of the positions in data_pos that are within the defined min-max box.
-
-    """
-
-    idxs_x = np.where((x_min < data_pos[:, 0]) & (data_pos[:, 0] < x_max))[0]
-    idxs_y = np.where((y_min < data_pos[:, 1]) & (data_pos[:, 1] < y_max))[0]
-    
-    return np.array(sorted(list(set(idxs_x).intersection(idxs_y))))
-
-
+# -*- coding: utf-8 -*-
+"""
+DeepMIMOv3 Python Implementation
+
+Description: Utilities
+
+Authors: Umut Demirhan, Ahmed Alkhateeb
+Date: 12/10/2021
+"""
+
+import time
+import DeepMIMOv3.consts as c
+from DeepMIMOv3.construct_deepmimo import ant_indices, array_response
+import numpy as np
+
+################################# Internal ####################################
+
+# Sleep between print and tqdm displays
+def safe_print(text, stop_dur=0.3):
+    print(text)
+    time.sleep(stop_dur)
+        
+# Determine active paths with the given configurations
+# (For OFDM, only the paths within DS are activated)
+class PathVerifier:
+    def __init__(self, params):
+        self.params = params
+        if self.params[c.PARAMSET_FDTD]: # IF OFDM
+            Ts = 1 / (params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_BW]*c.PARAMSET_OFDM_BW_MULT)
+            self.FFT_duration = params[c.PARAMSET_OFDM][c.PARAMSET_OFDM_SC_NUM] * Ts
+            self.max_ToA = 0
+            self.path_ratio_FFT = []
+    
+    def verify_path(self, ToA, power):
+        if self.params[c.PARAMSET_FDTD]: # OFDM CH
+            m_toa = np.max(ToA)
+            self.max_ToA = max(self.max_ToA, m_toa)
+            
+            if m_toa > self.FFT_duration:
+                violating_paths = ToA > self.FFT_duration
+                self.path_ratio_FFT.append( sum(power[violating_paths])/sum(power) )
+                        
+    def notify(self):
+        if self.params[c.PARAMSET_FDTD]: # IF OFDM
+            avg_ratio_FFT = 0
+            if len(self.path_ratio_FFT) != 0:
+                avg_ratio_FFT = np.mean(self.path_ratio_FFT)*100
+                
+            if self.max_ToA > self.FFT_duration and avg_ratio_FFT >= 1.:
+                safe_print('ToA of some paths of %i channels with an average total power of %.2f%% exceed the useful OFDM symbol duration and are clipped.' % (len(self.path_ratio_FFT), avg_ratio_FFT))
+            
+
+
+
+################################## For User ###################################
+
+def dbm2pow(val):
+    return 10**(val/10 - 3)
+
+def steering_vec(array, phi=0, theta=0, spacing=0.5):
+    """
+    Creates the array steering vector for uniform (linear and rectangular) arrays.
+
+    Parameters
+    ----------
+    array : tuple, list or numpy.ndarray
+        Number of [elements along the horizontal, elements along the vertical]
+    phi : float, optional    
+        Azimuth angle in degrees. 0 azimuth is normal to the array. 
+        Positive azimuth points beams to the right. The default is 0.
+    theta : float, optional
+        Elevation angle in degrees. 0 elevation is horizon (normal to the array). 
+        Positive elevation tilts the beam downards. The default is 0.
+    spacing : flaot, optional
+        Antenna spacing in wavelengths. The default is 0.5.
+
+    Returns
+    -------
+    numpy.ndarray
+        The normalized array response vector.
+
+    """
+    idxs = ant_indices(array)
+    resp = array_response(idxs, phi*np.pi/180, theta*np.pi/180 + np.pi/2, 2*np.pi*spacing)
+    return resp / np.linalg.norm(resp)
+
+# TODO: add info field to dataset (so data like number of users per row doesn't 
+#       need to be read from the webstie). This way, we can make the arguments
+#       of this function defaults based on the dataset
+
+def uniform_sampling(sampling_div, n_rows, users_per_row):
+    """
+    Returns indices of users at uniform steps/intervals.
+    
+    Parameters
+    ----------
+    steps : list
+        Step size along x and y dimensions. The list should have 2 elements only.
+        Examples:
+        [1,1] = indices of all users
+        [1,2] = same number of users across x, one every two users along y. Results: half the users.
+        [2,2] = takes one user every 2 users (step=2), along x and y. Results: 1/4 the total users
+    n_rows : int
+        Number of rows in the generated dataset. Necessary for indexing users.
+    users_per_row : int
+        Number of users per row in the generated dataset. Necessary for indexing users.
+        
+    Returns
+    -------
+    data : list
+        List of undersampled indices.
+    """
+    cols = np.arange(users_per_row, step=sampling_div[0])
+    rows = np.arange(n_rows, step=sampling_div[1])
+    uniform_idxs = np.array([j + i*users_per_row for i in rows for j in cols])
+    
+    return uniform_idxs
+
+
+def trim_by_idx(dataset, idxs):
+    """
+    Returns a DeepMIMO dataset with only the selected user indices.
+
+    Parameters
+    ----------
+    dataset : DeepMIMO dataset (dictionary)
+        A dataset as the output of DeepMIMO.generate_data()
+    idxs : list or array
+        List of selected indices.
+
+    Returns
+    -------
+    dataset_t : DeepMIMO dataset (dictionary)
+        Trimmed dataset.
+    """
+    
+    if len(idxs) == dataset[0]['user']['location'].shape[0]:
+        return dataset
+    
+    dataset_t = []
+    for bs_idx in range(len(dataset)):
+        dataset_t.append({})
+        for key in dataset[bs_idx].keys():
+            dataset_t[bs_idx]['location'] = dataset[bs_idx]['location']
+            dataset_t[bs_idx]['user'] = {}
+            for key in dataset[bs_idx]['user']:
+                dataset_t[bs_idx]['user'][key] = dataset[bs_idx]['user'][key][idxs]
+        
+    return dataset_t
+
+
+
+class LinearPath():
+    def __init__(self, deepmimo_dataset, first_pos, last_pos, res=1, n_steps=False, filter_repeated=True):
+        """
+        Creates a linear path of features. 
+
+        Parameters
+        ----------
+        deepmimo_dataset : DeepMIMO dataset
+            A dataset generated from DeepMIMO.generate_data(parameters).
+        first_pos : numpy.ndarray
+            [x, y, (z)] position of the start of the linear path.
+        last_pos : numpy.ndarray
+            [x, y, (z)] position of the end of the linear path.
+        res : float, optional
+            Resolution [in meters]. The same as providing n_steps. The default is 1.
+        n_steps : int, optional
+            Number of positions / samples between first and last position (including).
+            If False, either uses the resolution parameter <res>. The default is False.
+        filter_repeated : bool, optional
+            Whether to eliminated repeated positions. 
+            Repeated positions happen when a path is oversampled or the closest
+            dataste position repeats for a set of path positions. 
+            If True, the repeated positions are removed. The default is True.
+
+        Returns
+        -------
+        None.
+
+        """
+        
+        if len(first_pos) == 2: # if not given, assume z-coordinate = 0
+            first_pos = np.concatenate((first_pos,[0]))
+            last_pos = np.concatenate((last_pos,[0]))
+            
+        self.first_pos = first_pos
+        self.last_pos = last_pos
+        
+        self.dataset = deepmimo_dataset if type(deepmimo_dataset) != list else deepmimo_dataset[0]
+        self._set_idxs_pos_res_steps(res, n_steps, filter_repeated)
+        self._copy_data_from_dataset()
+        self._extract_features()
+        
+    def _set_idxs_pos_res_steps(self, res, n_steps, filter_repeated):
+        dataset_pos = self.dataset['user']['location']
+        if not n_steps:
+            data_res = np.linalg.norm(dataset_pos[0] - dataset_pos[1])
+            if res < data_res and filter_repeated:
+                print(f'Changing resolution to {data_res} to eliminate repeated positions')
+                res = data_res
+                
+            self.n = int(np.linalg.norm(self.first_pos - self.last_pos) / res)
+        else:
+            self.n = n_steps
+        
+        xs = np.linspace(self.first_pos[0], self.last_pos[0], self.n).reshape((-1,1))
+        ys = np.linspace(self.first_pos[1], self.last_pos[1], self.n).reshape((-1,1))
+        zs = np.linspace(self.first_pos[2], self.last_pos[2], self.n).reshape((-1,1))
+        
+        interpolated_pos = np.hstack((xs,ys,zs))
+        idxs = np.array([np.argmin(np.linalg.norm(dataset_pos - pos, axis=1)) 
+                         for pos in interpolated_pos])
+        
+        if filter_repeated:
+            # soft: removes adjacent repeated only
+            idxs = np.concatenate(([idxs[0]], idxs[1:][(idxs[1:]-idxs[:-1]) != 0]))
+            
+            if filter_repeated == 'hard':
+                # hard: removes all repeated
+                idxs = np.unique(idxs)
+            
+            self.n = len(idxs)
+    
+        self.idxs = idxs
+        self.pos = dataset_pos[idxs]
+    
+    def _copy_data_from_dataset(self):
+        self.feature_names = ['LoS', 'pathloss', 'distance']
+        
+        self.LoS = self.dataset['user']['LoS'][self.idxs]
+        self.pathloss = self.dataset['user']['pathloss'][self.idxs]
+        self.distance = self.dataset['user']['distance'][self.idxs]
+        self.paths = self.dataset['user']['paths'][self.idxs]
+        self.channel = self.dataset['user']['channel'][self.idxs]
+        
+    def _extract_features(self):
+        # Main path features
+        self.path_features = ['DoD_phi', 'DoD_theta', 'DoA_phi', 'DoA_theta', 
+                              'ToA', 'phase', 'power']
+        self.feature_names += ['main_path_' + var for var in self.path_features]
+        for feat in self.path_features:
+            setattr(self, f'main_path_{feat}', 
+                    np.array([self.paths[i][feat][0] for i in range(self.n)]))#self.idxs]))
+        
+        # Other features
+        self.feature_names += ['pwr_ratio_main_path', 'total_power']
+        self.total_power = np.array([np.sum(self.paths[i]['power']) for i in range(self.n)])
+        self.pwr_ratio_main_path = np.array([self.main_path_power[i] / np.sum(self.paths[i]['power'])
+                                             if self.LoS[i] != -1 else np.nan for i in range(self.n)])
+
+    def get_feature_names(self):
+        return self.feature_names
+    
+# TODO: add more LinearPath functions
+# - To append paths use, for example: linpath3.append(linpath1, linpath2)
+# - To repeat back and forth: linpath3.append(linpath3.flip())
+# - Supposing the last position of linpath3 coincides with the first, it can be looped like:
+# linpath3.append(linpath3, linpath3, linpath3) or linpath3.repeat(3)
+
+
+
+def get_idxs_in_xy_box(data_pos, x_min, x_max, y_min, y_max):
+    """
+    Obtains the indices of <data_pos> that lie between the xy limits.
+
+    Parameters
+    ----------
+    data_pos : numpy.ndarray
+        Array with all positions. Dimensions: [n_positions, 2]
+    x_min : float
+        Minimum x limit. Only positions where x > x_min have their indices returned.
+    x_max : float
+        Maximum x limit. Only positions where x < x_max have their indices returned.
+    y_min : float
+        Minimum y limit. Only positions where y > y_min have their indices returned.
+    y_max : float
+        Maximum y limit. Only positions where y < y_max have their indices returned.
+
+    Returns
+    -------
+    numpy.ndarray
+        Indices of the positions in data_pos that are within the defined min-max box.
+
+    """
+
+    idxs_x = np.where((x_min < data_pos[:, 0]) & (data_pos[:, 0] < x_max))[0]
+    idxs_y = np.where((y_min < data_pos[:, 1]) & (data_pos[:, 1] < y_max))[0]
+    
+    return np.array(sorted(list(set(idxs_x).intersection(idxs_y))))
+
+
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3/visualization.py` & `deepmimov3-0.2.5/src/DeepMIMOv3/visualization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-import matplotlib.pyplot as plt
-import numpy as np
-
-
-def plot_LoS_status(bs_location, user_locations, user_LoS, scat_size='auto'):
-    """
-    Scatters the users and one basestations and colors the users based on their
-    line-of-sight status.
-
-    Parameters
-    ----------
-    bs_location : numpy array
-        One dimensional array with the xy position of the basestation.
-    user_locations : numpy array
-        A matrix containing user locations across rows and xy positions across
-        columns. Expected shape: <n_users> by 2
-    user_LoS : numpy array
-        One dimensional array with the LoS status of each user. The length
-        should match the number of users in user_locations.
-    scat_size : float, optional
-        Size of the scatter points. The default is 'auto'.
-
-    Returns
-    -------
-    None.
-
-    """
-    LoS_map = {-1: ('r', 'No Path'), 0: ('b', 'NLoS'), 1: ('g', 'LoS')}
-    
-    # Calculate scatter size based on point density
-    if scat_size == 'auto':
-        n_points = user_locations.shape[0]
-        area = np.prod(np.max(user_locations, axis=0)[:2] - 
-                       np.min(user_locations, axis=0)[:2])
-        point_density = n_points / area
-        scat_size = 1 / (100 * point_density)
-    
-    for unique_LoS_status in LoS_map.keys():
-    # Plot different status one by one to assign legend labels
-        users_w_key = user_LoS==unique_LoS_status
-        plt.scatter(user_locations[users_w_key, 0], 
-                    user_locations[users_w_key, 1], 
-                    c=LoS_map[unique_LoS_status][0], 
-                    label=LoS_map[unique_LoS_status][1], s=scat_size)
-    plt.scatter(bs_location[0], bs_location[1], 
-                c='k', marker='x', label='Basestation')
-    plt.xlabel('x (m)')
-    plt.ylabel('y (m)')
-    lgd = plt.legend(framealpha=.9, loc='lower left')
-    lgd.legend_handles[0]._sizes = [20]
-    lgd.legend_handles[1]._sizes = [20]
-    lgd.legend_handles[2]._sizes = [20]
-    plt.xlim([user_locations[:, 0].min(), user_locations[:, 0].max()])
-    plt.ylim([user_locations[:, 1].min(), user_locations[:, 1].max()])
-
-
-def plot_coverage(rxs, cov_map, dpi=300, figsize=(6,4), cbar_title=None, title=False,
-                  scat_sz=.5, bs_pos=None, bs_ori=None, legend=False, lims=None,
-                  proj_3D=False, equal_aspect=False, tight=True, cmap='viridis'):
-    """
-    This function scatters the users' positions <rxs> and colors them with <cov_map>.
-
-    Parameters
-    ----------
-    rxs : numpy.ndarray
-        User position array. Dimensions: [n_users, 3].
-    cov_map : tuple, list or numpy.ndarray
-        Coverage map. Or a map of the feature based on which to color the user positions.
-        Dimension: n_users
-    dpi : int, optional
-        Resolution. The default is 300.
-    figsize : tuple, optional
-        Figure (horizontal size, vertical size) in inches. The default is (6,4).
-    cbar_title : string, optional
-        Title/text of the colorbar. The default is None.
-    title : string, optional
-        Title of the plot. No title if None, empty string or False. The default is False.
-    scat_sz : float, optional
-        Scatter marker size. The default is .5.
-    bs_pos : tuple, list or numpy.ndarray, optional
-        Transmitter (considered the Base station) position. If valid (not None),
-        it puts a 'x' marker in that [x,y (,z)] position. The default is None.
-    bs_ori : tuple, list or numpy.ndarray, optional
-        Transmitter (considered the Base station) orientation. If valid (not None),
-        it draws a line with this direction, starting at the BS position. 
-        Orientation/Rotation is around [x,y,z] following the right hand rule. 
-        [0,0,0] = Antenna pointing towards +x
-        [0,0,90] = Antenna pointing towards +y
-        [0,90,0] = Antenna pointing towards -z
-        Another way of interpreting: 
-            z-rotation is azimuth (where 0 is +x)
-            y-rotation is elevation/tilt (where 0 is the horizon)
-        The default is None.
-    legend : bool, optional
-        Whether to include a plot legend. The default is False.
-    lims : tuple, list or numpy.ndarray, optional
-        Coverage color limits. Helps setting the limits of the colormap and colorbar. 
-        The default is None.
-    proj_3D : bool, optional
-        Whether to make a 3D or 2D plot. True is 3D, False is 2D. The default is False.
-    equal_aspect : bool, optional
-        Whether to have axis with the same scale. Note: if not done with 
-        precaution, it can ruin a 3D visualization. The default is False.
-    tight : bool, optional
-        Whether to set the plot xy(z) limits automatically based on the values
-        so that the axis are maximally used and no data is omitted.
-        The default is True.
-    cmap : string, optional
-        Colormap string identifier for matplotlib. 
-        See available colormaps in: 
-        https://matplotlib.org/stable/users/explain/colors/colormaps.html
-        or by runnign: plt.colormaps.get_cmap('not a colormap')
-        The default is 'viridis'.
-
-    Returns
-    -------
-    fig : matplotlib figure
-        fig as in "fig, ax = plt.subplots()"
-        The motivation behind returning these elements is allowing editing and
-        saving, before displaying (plt.show() is not used).
-    ax : matplotlib axes
-        ax as in "fig, ax = plt.subplots()"
-    cbar : matplotlib colorbar
-        The colorbar associated with the coverage map. 
-
-    """
-    
-    plt_params = {'cmap': cmap}
-    if lims:
-        plt_params['vmin'], plt_params['vmax'] = lims[0], lims[1]
-    
-    n = 3 if proj_3D else 2 # n = coordinates to consider
-    
-    xyz = {s: rxs[:,i] for s,i in zip(['x', 'y', 'zs'], range(n))}
-    
-    fig, ax = plt.subplots(dpi=dpi, figsize=figsize,
-                           subplot_kw={'projection': '3d'} if proj_3D else {})
-    
-    im = plt.scatter(**xyz, c=cov_map, s=scat_sz, marker='s', **plt_params)
-
-    cbar = plt.colorbar(im, label='Received Power [dBm]' if not cbar_title else cbar_title)
-    
-    plt.xlabel('x (m)')
-    plt.ylabel('y (m)')
-    
-    # TX position
-    if bs_pos is not None:
-        ax.scatter(*bs_pos[:n], marker='P', c='r', label='TX')
-    
-    # TX orientation
-    if bs_ori is not None and bs_pos is not None:
-        r = 30 # ref size of pointing direction
-        tx_lookat = np.copy(bs_pos)
-        tx_lookat[:2] += r * np.array([np.cos(bs_ori[2]), np.sin(bs_ori[2])]) # azimuth
-        tx_lookat[2] -= r / 10 * np.sin(bs_ori[1]) # elevation
-        
-        line_components = [[bs_pos[i], tx_lookat[i]] for i in range(n)]
-        ax.plot(*line_components, c='k', alpha=.5, zorder=3)
-        
-    if title:
-        ax.set_title(title)
-    
-    if legend:
-        plt.legend(loc='upper center', ncols=10, framealpha=.5)
-    
-    if tight:
-        s = 1
-        mins, maxs = np.min(rxs, axis=0)-s, np.max(rxs, axis=0)+s
-        
-        plt.xlim([mins[0], maxs[0]])
-        plt.ylim([mins[1], maxs[1]])
-        if proj_3D:
-            zlims = [mins[2], maxs[2]] if bs_pos is None else [np.min([mins[2], bs_pos[2]]),
-                                                               np.max([mins[2], bs_pos[2]])]
-            ax.axes.set_zlim3d(zlims)
-    
-    if equal_aspect: # often disrups the plot if in 3D.
-        plt.axis('scaled')
-    
-    return fig, ax, cbar
+import matplotlib.pyplot as plt
+import numpy as np
+
+
+def plot_LoS_status(bs_location, user_locations, user_LoS, scat_size='auto'):
+    """
+    Scatters the users and one basestations and colors the users based on their
+    line-of-sight status.
+
+    Parameters
+    ----------
+    bs_location : numpy array
+        One dimensional array with the xy position of the basestation.
+    user_locations : numpy array
+        A matrix containing user locations across rows and xy positions across
+        columns. Expected shape: <n_users> by 2
+    user_LoS : numpy array
+        One dimensional array with the LoS status of each user. The length
+        should match the number of users in user_locations.
+    scat_size : float, optional
+        Size of the scatter points. The default is 'auto'.
+
+    Returns
+    -------
+    None.
+
+    """
+    LoS_map = {-1: ('r', 'No Path'), 0: ('b', 'NLoS'), 1: ('g', 'LoS')}
+    
+    # Calculate scatter size based on point density
+    if scat_size == 'auto':
+        n_points = user_locations.shape[0]
+        area = np.prod(np.max(user_locations, axis=0)[:2] - 
+                       np.min(user_locations, axis=0)[:2])
+        point_density = n_points / area
+        scat_size = 1 / (3 * point_density)
+    
+    for unique_LoS_status in LoS_map.keys():
+    # Plot different status one by one to assign legend labels
+        users_w_key = user_LoS==unique_LoS_status
+        plt.scatter(user_locations[users_w_key, 0], 
+                    user_locations[users_w_key, 1], 
+                    c=LoS_map[unique_LoS_status][0], 
+                    label=LoS_map[unique_LoS_status][1], s=scat_size)
+    plt.scatter(bs_location[0], bs_location[1], 
+                c='k', marker='x', label='Basestation')
+    plt.xlabel('x (m)')
+    plt.ylabel('y (m)')
+    lgd = plt.legend(framealpha=.9, loc='lower left')
+    lgd.legend_handles[0]._sizes = [20]
+    lgd.legend_handles[1]._sizes = [20]
+    lgd.legend_handles[2]._sizes = [20]
+    plt.xlim([user_locations[:, 0].min(), user_locations[:, 0].max()])
+    plt.ylim([user_locations[:, 1].min(), user_locations[:, 1].max()])
+
+
+def plot_coverage(rxs, cov_map, dpi=300, figsize=(6,4), cbar_title=None, title=False,
+                  scat_sz=.5, bs_pos=None, bs_ori=None, legend=False, lims=None,
+                  proj_3D=False, equal_aspect=False, tight=True, cmap='viridis'):
+    """
+    This function scatters the users' positions <rxs> and colors them with <cov_map>.
+
+    Parameters
+    ----------
+    rxs : numpy.ndarray
+        User position array. Dimensions: [n_users, 3].
+    cov_map : tuple, list or numpy.ndarray
+        Coverage map. Or a map of the feature based on which to color the user positions.
+        Dimension: n_users
+    dpi : int, optional
+        Resolution. The default is 300.
+    figsize : tuple, optional
+        Figure (horizontal size, vertical size) in inches. The default is (6,4).
+    cbar_title : string, optional
+        Title/text of the colorbar. The default is None.
+    title : string, optional
+        Title of the plot. No title if None, empty string or False. The default is False.
+    scat_sz : float, optional
+        Scatter marker size. The default is .5.
+    bs_pos : tuple, list or numpy.ndarray, optional
+        Transmitter (considered the Base station) position. If valid (not None),
+        it puts a 'x' marker in that [x,y (,z)] position. The default is None.
+    bs_ori : tuple, list or numpy.ndarray, optional
+        Transmitter (considered the Base station) orientation. If valid (not None),
+        it draws a line with this direction, starting at the BS position. 
+        Orientation/Rotation is around [x,y,z] following the right hand rule. 
+        [0,0,0] = Antenna pointing towards +x
+        [0,0,90] = Antenna pointing towards +y
+        [0,90,0] = Antenna pointing towards -z
+        Another way of interpreting: 
+            z-rotation is azimuth (where 0 is +x)
+            y-rotation is elevation/tilt (where 0 is the horizon)
+        The default is None.
+    legend : bool, optional
+        Whether to include a plot legend. The default is False.
+    lims : tuple, list or numpy.ndarray, optional
+        Coverage color limits. Helps setting the limits of the colormap and colorbar. 
+        The default is None.
+    proj_3D : bool, optional
+        Whether to make a 3D or 2D plot. True is 3D, False is 2D. The default is False.
+    equal_aspect : bool, optional
+        Whether to have axis with the same scale. Note: if not done with 
+        precaution, it can ruin a 3D visualization. The default is False.
+    tight : bool, optional
+        Whether to set the plot xy(z) limits automatically based on the values
+        so that the axis are maximally used and no data is omitted.
+        The default is True.
+    cmap : string, optional
+        Colormap string identifier for matplotlib. 
+        See available colormaps in: 
+        https://matplotlib.org/stable/users/explain/colors/colormaps.html
+        or by runnign: plt.colormaps.get_cmap('not a colormap')
+        The default is 'viridis'.
+
+    Returns
+    -------
+    fig : matplotlib figure
+        fig as in "fig, ax = plt.subplots()"
+        The motivation behind returning these elements is allowing editing and
+        saving, before displaying (plt.show() is not used).
+    ax : matplotlib axes
+        ax as in "fig, ax = plt.subplots()"
+    cbar : matplotlib colorbar
+        The colorbar associated with the coverage map. 
+
+    """
+    
+    plt_params = {'cmap': cmap}
+    if lims:
+        plt_params['vmin'], plt_params['vmax'] = lims[0], lims[1]
+    
+    n = 3 if proj_3D else 2 # n = coordinates to consider
+    
+    xyz = {s: rxs[:,i] for s,i in zip(['x', 'y', 'zs'], range(n))}
+    
+    fig, ax = plt.subplots(dpi=dpi, figsize=figsize,
+                           subplot_kw={'projection': '3d'} if proj_3D else {})
+    
+    im = plt.scatter(**xyz, c=cov_map, s=scat_sz, marker='s', **plt_params)
+
+    cbar = plt.colorbar(im, label='Received Power [dBm]' if not cbar_title else cbar_title)
+    
+    plt.xlabel('x (m)')
+    plt.ylabel('y (m)')
+    
+    # TX position
+    if bs_pos is not None:
+        ax.scatter(*bs_pos[:n], marker='P', c='r', label='TX')
+    
+    # TX orientation
+    if bs_ori is not None and bs_pos is not None:
+        r = 30 # ref size of pointing direction
+        tx_lookat = np.copy(bs_pos)
+        tx_lookat[:2] += r * np.array([np.cos(bs_ori[2]), np.sin(bs_ori[2])]) # azimuth
+        tx_lookat[2] -= r / 10 * np.sin(bs_ori[1]) # elevation
+        
+        line_components = [[bs_pos[i], tx_lookat[i]] for i in range(n)]
+        ax.plot(*line_components, c='k', alpha=.5, zorder=3)
+        
+    if title:
+        ax.set_title(title)
+    
+    if legend:
+        plt.legend(loc='upper center', ncols=10, framealpha=.5)
+    
+    if tight:
+        s = 1
+        mins, maxs = np.min(rxs, axis=0)-s, np.max(rxs, axis=0)+s
+        
+        plt.xlim([mins[0], maxs[0]])
+        plt.ylim([mins[1], maxs[1]])
+        if proj_3D:
+            zlims = [mins[2], maxs[2]] if bs_pos is None else [np.min([mins[2], bs_pos[2]]),
+                                                               np.max([mins[2], bs_pos[2]])]
+            ax.axes.set_zlim3d(zlims)
+    
+    if equal_aspect: # often disrups the plot if in 3D.
+        plt.axis('scaled')
+    
+    return fig, ax, cbar
```

### Comparing `deepmimov3-0.2.4/src/DeepMIMOv3.egg-info/SOURCES.txt` & `deepmimov3-0.2.5/src/DeepMIMOv3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

