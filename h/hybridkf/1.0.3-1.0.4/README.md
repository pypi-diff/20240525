# Comparing `tmp/hybridkf-1.0.3.tar.gz` & `tmp/hybridkf-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybridkf-1.0.3.tar", last modified: Fri May 24 21:26:14 2024, max compression
+gzip compressed data, was "hybridkf-1.0.4.tar", last modified: Fri May 24 22:07:42 2024, max compression
```

## Comparing `hybridkf-1.0.3.tar` & `hybridkf-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:26:14.868379 hybridkf-1.0.3/
--rw-r--r--   0 aleckain   (501) staff       (20)     5775 2024-05-24 21:26:14.868057 hybridkf-1.0.3/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)     5192 2024-05-24 17:56:29.000000 hybridkf-1.0.3/README.md
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:26:14.866530 hybridkf-1.0.3/hybridkf/
--rw-r--r--   0 aleckain   (501) staff       (20)       36 2024-05-24 21:05:14.000000 hybridkf-1.0.3/hybridkf/__init__.py
--rw-r--r--   0 aleckain   (501) staff       (20)     9537 2024-05-24 21:25:24.000000 hybridkf-1.0.3/hybridkf/main.py
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:26:14.867751 hybridkf-1.0.3/hybridkf.egg-info/
--rw-r--r--   0 aleckain   (501) staff       (20)     5775 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)      215 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/SOURCES.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/dependency_links.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/requires.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        9 2024-05-24 21:26:14.000000 hybridkf-1.0.3/hybridkf.egg-info/top_level.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 21:26:14.868424 hybridkf-1.0.3/setup.cfg
--rw-r--r--   0 aleckain   (501) staff       (20)      783 2024-05-24 21:26:06.000000 hybridkf-1.0.3/setup.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:07:42.012895 hybridkf-1.0.4/
+-rw-r--r--   0 aleckain   (501) staff       (20)     6289 2024-05-24 22:07:42.012682 hybridkf-1.0.4/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)     5707 2024-05-24 22:06:38.000000 hybridkf-1.0.4/README.md
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:07:42.011435 hybridkf-1.0.4/hybridkf/
+-rw-r--r--   0 aleckain   (501) staff       (20)       36 2024-05-24 21:05:14.000000 hybridkf-1.0.4/hybridkf/__init__.py
+-rw-r--r--   0 aleckain   (501) staff       (20)     9537 2024-05-24 21:25:24.000000 hybridkf-1.0.4/hybridkf/main.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 22:07:42.012443 hybridkf-1.0.4/hybridkf.egg-info/
+-rw-r--r--   0 aleckain   (501) staff       (20)     6289 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)      215 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/SOURCES.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/dependency_links.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/requires.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        9 2024-05-24 22:07:41.000000 hybridkf-1.0.4/hybridkf.egg-info/top_level.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 22:07:42.012930 hybridkf-1.0.4/setup.cfg
+-rw-r--r--   0 aleckain   (501) staff       (20)      783 2024-05-24 22:07:38.000000 hybridkf-1.0.4/setup.py
```

### Comparing `hybridkf-1.0.3/PKG-INFO` & `hybridkf-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.3
+Version: 1.0.4
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -67,41 +67,47 @@
                                                                                         [0, 0, 0, 5, 0, 0], 
                                                                                         [0, 0, 0, 0, 13, 0], 
                                                                                         [0, 0, 0, 0, 0, 13]]), 
 B=0, linear_timesteps=True, timestep_var=0.1, linear_motion_x_factor=2, linear_motion_y_factor=5, 
 nonlinear_motion_x_factor=6, nonlinear_motion_y_factor=6, seed=42)
 ```
 #### Parameters
-dt: Time step for state prediction.
-noise_std: Noise standard deviation for observation Gaussian distributions.
-noise_covariance_factor: Factor to scale the noise covariance matrix.
-n: Number of observations/objects to generate.
-max_x: Maximum x coordinate for state estimation.
-max_y: Maximum y coordinate for state estimation.
-motion_type: Type of motion model ('linear' or 'nonlinear').
-verbose: Verbosity mode (True or False) - view all true, noisy, and estimated measurements for all observations at each time step.
-state_transition_factor: Factor to scale the state transition matrix.
-process_noise_covariance_factor: Factor to scale the process noise covariance matrix.
-u: Control input.
-P_init: Initial uncertainty weights matrix.
-B: Input control matrix.
-linear_timesteps: Flag indicating whether time steps are linear (True) or nonlinear (False).
-timestep_var: Variance of time steps.
-linear_motion_x_factor: Factor to scale linear motion in the x direction.
-linear_motion_y_factor: Factor to scale linear motion in the y direction.
-nonlinear_motion_x_factor: Factor to scale nonlinear motion in the x direction.
-nonlinear_motion_y_factor: Factor to scale nonlinear motion in the y direction.
-seed: Random seed for reproducibility.
+- dt: Time step for state prediction.
+- noise_std: Noise standard deviation for observation Gaussian distributions.
+- noise_covariance_factor: Factor to scale the noise covariance matrix.
+- n: Number of observations/objects to generate.
+- max_x: Maximum x coordinate for state estimation.
+- max_y: Maximum y coordinate for state estimation.
+- motion_type: Type of motion model ('linear' or 'nonlinear').
+- verbose: Verbosity mode (True or False) - view all true, noisy, and estimated measurements for all observations at each time step.
+- state_transition_factor: Factor to scale the state transition matrix.
+- process_noise_covariance_factor: Factor to scale the process noise covariance matrix.
+- u: Control input.
+- P_init: Initial uncertainty weights matrix.
+- B: Input control matrix.
+- linear_timesteps: Flag indicating whether time steps are linear (True) or nonlinear (False).
+- timestep_var: Variance of time steps.
+- linear_motion_x_factor: Factor to scale linear motion in the x direction.
+- linear_motion_y_factor: Factor to scale linear motion in the y direction.
+- nonlinear_motion_x_factor: Factor to scale nonlinear motion in the x direction.
+- nonlinear_motion_y_factor: Factor to scale nonlinear motion in the y direction.
+- seed: Random seed for reproducibility.
 
 #### Methods
-generate_true_positions: Generates random true positions for objects.
-generate_noisy_observations: Simulates noisy observations based on true positions.
-predict: Predicts the state of an object based on the current state and input.
-measurement_update: Updates the state estimate based on noisy observations.
-execute_hybrid_kf: Executes the Hybrid Kalman Filter algorithm for the specified number of time steps.
+- generate_true_positions: Generates random true positions for objects, outputs a dictionary with simulated objects where the keys are ids and values are pairs of coordinates.
+- generate_noisy_observations: Simulates noisy observations based on generated true positions.
+- predict: Predicts the state of an object based on the current state and input.
+- measurement_update: Updates the state estimate based on noisy observations.
+- execute_hybrid_kf: Executes the Hybrid Kalman Filter algorithm for the specified number of time steps.
+
+## Output Examples
+### Linear state evolution (linear motion), nonlinear timesteps
+![image](https://github.com/akain0/hybridkf/assets/48894841/4ca9cbb7-01dd-45e6-83a8-5e967fe175d1)
+### Nonlinear state evolution (nonlinear motion), nonlinear timesteps
+![image](https://github.com/akain0/hybridkf/assets/48894841/b45c34c0-055e-4897-84ac-01c7d930bd02)
 
 ## Contributing
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on GitHub.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `hybridkf-1.0.3/README.md` & `hybridkf-1.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -52,44 +52,50 @@
                                                                                         [0, 0, 0, 5, 0, 0], 
                                                                                         [0, 0, 0, 0, 13, 0], 
                                                                                         [0, 0, 0, 0, 0, 13]]), 
 B=0, linear_timesteps=True, timestep_var=0.1, linear_motion_x_factor=2, linear_motion_y_factor=5, 
 nonlinear_motion_x_factor=6, nonlinear_motion_y_factor=6, seed=42)
 ```
 #### Parameters
-dt: Time step for state prediction.
-noise_std: Noise standard deviation for observation Gaussian distributions.
-noise_covariance_factor: Factor to scale the noise covariance matrix.
-n: Number of observations/objects to generate.
-max_x: Maximum x coordinate for state estimation.
-max_y: Maximum y coordinate for state estimation.
-motion_type: Type of motion model ('linear' or 'nonlinear').
-verbose: Verbosity mode (True or False) - view all true, noisy, and estimated measurements for all observations at each time step.
-state_transition_factor: Factor to scale the state transition matrix.
-process_noise_covariance_factor: Factor to scale the process noise covariance matrix.
-u: Control input.
-P_init: Initial uncertainty weights matrix.
-B: Input control matrix.
-linear_timesteps: Flag indicating whether time steps are linear (True) or nonlinear (False).
-timestep_var: Variance of time steps.
-linear_motion_x_factor: Factor to scale linear motion in the x direction.
-linear_motion_y_factor: Factor to scale linear motion in the y direction.
-nonlinear_motion_x_factor: Factor to scale nonlinear motion in the x direction.
-nonlinear_motion_y_factor: Factor to scale nonlinear motion in the y direction.
-seed: Random seed for reproducibility.
+- dt: Time step for state prediction.
+- noise_std: Noise standard deviation for observation Gaussian distributions.
+- noise_covariance_factor: Factor to scale the noise covariance matrix.
+- n: Number of observations/objects to generate.
+- max_x: Maximum x coordinate for state estimation.
+- max_y: Maximum y coordinate for state estimation.
+- motion_type: Type of motion model ('linear' or 'nonlinear').
+- verbose: Verbosity mode (True or False) - view all true, noisy, and estimated measurements for all observations at each time step.
+- state_transition_factor: Factor to scale the state transition matrix.
+- process_noise_covariance_factor: Factor to scale the process noise covariance matrix.
+- u: Control input.
+- P_init: Initial uncertainty weights matrix.
+- B: Input control matrix.
+- linear_timesteps: Flag indicating whether time steps are linear (True) or nonlinear (False).
+- timestep_var: Variance of time steps.
+- linear_motion_x_factor: Factor to scale linear motion in the x direction.
+- linear_motion_y_factor: Factor to scale linear motion in the y direction.
+- nonlinear_motion_x_factor: Factor to scale nonlinear motion in the x direction.
+- nonlinear_motion_y_factor: Factor to scale nonlinear motion in the y direction.
+- seed: Random seed for reproducibility.
 
 #### Methods
-generate_true_positions: Generates random true positions for objects.
-generate_noisy_observations: Simulates noisy observations based on true positions.
-predict: Predicts the state of an object based on the current state and input.
-measurement_update: Updates the state estimate based on noisy observations.
-execute_hybrid_kf: Executes the Hybrid Kalman Filter algorithm for the specified number of time steps.
+- generate_true_positions: Generates random true positions for objects, outputs a dictionary with simulated objects where the keys are ids and values are pairs of coordinates.
+- generate_noisy_observations: Simulates noisy observations based on generated true positions.
+- predict: Predicts the state of an object based on the current state and input.
+- measurement_update: Updates the state estimate based on noisy observations.
+- execute_hybrid_kf: Executes the Hybrid Kalman Filter algorithm for the specified number of time steps.
+
+## Output Examples
+### Linear state evolution (linear motion), nonlinear timesteps
+![image](https://github.com/akain0/hybridkf/assets/48894841/4ca9cbb7-01dd-45e6-83a8-5e967fe175d1)
+### Nonlinear state evolution (nonlinear motion), nonlinear timesteps
+![image](https://github.com/akain0/hybridkf/assets/48894841/b45c34c0-055e-4897-84ac-01c7d930bd02)
 
 ## Contributing
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on GitHub.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## References
 Wikipedia contributors. "Kalman filter." Wikipedia, The Free Encyclopedia. Wikipedia, The Free Encyclopedia, 5 May. 2024. Link
-Wikipedia contributors. "Hybrid Kalman filter." Wikipedia, The Free Encyclopedia. Wikipedia, The Free Encyclopedia, 28 Dec. 2023. Link
+Wikipedia contributors. "Hybrid Kalman filter." Wikipedia, The Free Encyclopedia. Wikipedia, The Free Encyclopedia, 28 Dec. 2023. Link
```

### Comparing `hybridkf-1.0.3/hybridkf/main.py` & `hybridkf-1.0.4/hybridkf/main.py`

 * *Files identical despite different names*

### Comparing `hybridkf-1.0.3/hybridkf.egg-info/PKG-INFO` & `hybridkf-1.0.4/hybridkf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.3
+Version: 1.0.4
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -67,41 +67,47 @@
                                                                                         [0, 0, 0, 5, 0, 0], 
                                                                                         [0, 0, 0, 0, 13, 0], 
                                                                                         [0, 0, 0, 0, 0, 13]]), 
 B=0, linear_timesteps=True, timestep_var=0.1, linear_motion_x_factor=2, linear_motion_y_factor=5, 
 nonlinear_motion_x_factor=6, nonlinear_motion_y_factor=6, seed=42)
 ```
 #### Parameters
-dt: Time step for state prediction.
-noise_std: Noise standard deviation for observation Gaussian distributions.
-noise_covariance_factor: Factor to scale the noise covariance matrix.
-n: Number of observations/objects to generate.
-max_x: Maximum x coordinate for state estimation.
-max_y: Maximum y coordinate for state estimation.
-motion_type: Type of motion model ('linear' or 'nonlinear').
-verbose: Verbosity mode (True or False) - view all true, noisy, and estimated measurements for all observations at each time step.
-state_transition_factor: Factor to scale the state transition matrix.
-process_noise_covariance_factor: Factor to scale the process noise covariance matrix.
-u: Control input.
-P_init: Initial uncertainty weights matrix.
-B: Input control matrix.
-linear_timesteps: Flag indicating whether time steps are linear (True) or nonlinear (False).
-timestep_var: Variance of time steps.
-linear_motion_x_factor: Factor to scale linear motion in the x direction.
-linear_motion_y_factor: Factor to scale linear motion in the y direction.
-nonlinear_motion_x_factor: Factor to scale nonlinear motion in the x direction.
-nonlinear_motion_y_factor: Factor to scale nonlinear motion in the y direction.
-seed: Random seed for reproducibility.
+- dt: Time step for state prediction.
+- noise_std: Noise standard deviation for observation Gaussian distributions.
+- noise_covariance_factor: Factor to scale the noise covariance matrix.
+- n: Number of observations/objects to generate.
+- max_x: Maximum x coordinate for state estimation.
+- max_y: Maximum y coordinate for state estimation.
+- motion_type: Type of motion model ('linear' or 'nonlinear').
+- verbose: Verbosity mode (True or False) - view all true, noisy, and estimated measurements for all observations at each time step.
+- state_transition_factor: Factor to scale the state transition matrix.
+- process_noise_covariance_factor: Factor to scale the process noise covariance matrix.
+- u: Control input.
+- P_init: Initial uncertainty weights matrix.
+- B: Input control matrix.
+- linear_timesteps: Flag indicating whether time steps are linear (True) or nonlinear (False).
+- timestep_var: Variance of time steps.
+- linear_motion_x_factor: Factor to scale linear motion in the x direction.
+- linear_motion_y_factor: Factor to scale linear motion in the y direction.
+- nonlinear_motion_x_factor: Factor to scale nonlinear motion in the x direction.
+- nonlinear_motion_y_factor: Factor to scale nonlinear motion in the y direction.
+- seed: Random seed for reproducibility.
 
 #### Methods
-generate_true_positions: Generates random true positions for objects.
-generate_noisy_observations: Simulates noisy observations based on true positions.
-predict: Predicts the state of an object based on the current state and input.
-measurement_update: Updates the state estimate based on noisy observations.
-execute_hybrid_kf: Executes the Hybrid Kalman Filter algorithm for the specified number of time steps.
+- generate_true_positions: Generates random true positions for objects, outputs a dictionary with simulated objects where the keys are ids and values are pairs of coordinates.
+- generate_noisy_observations: Simulates noisy observations based on generated true positions.
+- predict: Predicts the state of an object based on the current state and input.
+- measurement_update: Updates the state estimate based on noisy observations.
+- execute_hybrid_kf: Executes the Hybrid Kalman Filter algorithm for the specified number of time steps.
+
+## Output Examples
+### Linear state evolution (linear motion), nonlinear timesteps
+![image](https://github.com/akain0/hybridkf/assets/48894841/4ca9cbb7-01dd-45e6-83a8-5e967fe175d1)
+### Nonlinear state evolution (nonlinear motion), nonlinear timesteps
+![image](https://github.com/akain0/hybridkf/assets/48894841/b45c34c0-055e-4897-84ac-01c7d930bd02)
 
 ## Contributing
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on GitHub.
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `hybridkf-1.0.3/setup.py` & `hybridkf-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hybridkf',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     description='''An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.'''
     ,
     author='akain0',
     install_requires=[
         'numpy',
         'scipy',
```

