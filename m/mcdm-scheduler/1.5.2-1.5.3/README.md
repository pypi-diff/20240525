# Comparing `tmp/mcdm_scheduler-1.5.2.tar.gz` & `tmp/mcdm_scheduler-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mcdm_scheduler-1.5.2.tar", last modified: Fri May 24 01:05:20 2024, max compression
+gzip compressed data, was "dist\mcdm_scheduler-1.5.3.tar", last modified: Sat May 25 20:38:44 2024, max compression
```

## Comparing `mcdm_scheduler-1.5.2.tar` & `mcdm_scheduler-1.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 01:05:20.000000 mcdm_scheduler-1.5.2/
--rw-rw-rw-   0        0        0      668 2024-05-22 01:01:37.000000 mcdm_scheduler-1.5.2/LICENSE
--rw-rw-rw-   0        0        0     1879 2024-05-24 01:05:20.000000 mcdm_scheduler-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1528 2024-05-24 01:03:06.000000 mcdm_scheduler-1.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 01:05:20.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 01:05:20.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/algorithm/
--rw-rw-rw-   0        0        0       19 2024-05-23 23:46:34.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/algorithm/__init__.py
--rw-rw-rw-   0        0        0    15381 2024-05-24 00:17:46.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/algorithm/src.py
-drwxrwxrwx   0        0        0        0 2024-05-24 01:05:20.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/util/
--rw-rw-rw-   0        0        0       87 2024-05-23 23:47:52.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/util/__init__.py
--rw-rw-rw-   0        0        0     2924 2024-05-24 00:42:10.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/util/fuzzy_ppf_ahp.py
--rw-rw-rw-   0        0        0     7629 2024-05-24 00:31:01.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/util/ga.py
--rw-rw-rw-   0        0        0     2460 2024-05-21 23:05:20.000000 mcdm_scheduler-1.5.2/mcdm_scheduler/util/ht2fs.py
-drwxrwxrwx   0        0        0        0 2024-05-24 01:05:20.000000 mcdm_scheduler-1.5.2/mcdm_scheduler.egg-info/
--rw-rw-rw-   0        0        0     1879 2024-05-24 01:05:19.000000 mcdm_scheduler-1.5.2/mcdm_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-05-24 01:05:20.000000 mcdm_scheduler-1.5.2/mcdm_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 01:05:19.000000 mcdm_scheduler-1.5.2/mcdm_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-24 01:05:19.000000 mcdm_scheduler-1.5.2/mcdm_scheduler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-24 01:05:19.000000 mcdm_scheduler-1.5.2/mcdm_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 01:05:20.000000 mcdm_scheduler-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      644 2024-05-23 23:49:09.000000 mcdm_scheduler-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/
+-rw-rw-rw-   0        0        0      668 2024-05-22 01:01:37.000000 mcdm_scheduler-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0     1877 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1526 2024-05-24 01:19:05.000000 mcdm_scheduler-1.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/algorithm/
+-rw-rw-rw-   0        0        0       19 2024-05-23 23:46:34.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/algorithm/__init__.py
+-rw-rw-rw-   0        0        0    16760 2024-05-25 20:36:23.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/algorithm/src.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/
+-rw-rw-rw-   0        0        0       87 2024-05-23 23:47:52.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/__init__.py
+-rw-rw-rw-   0        0        0     2924 2024-05-24 00:42:10.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/fuzzy_ppf_ahp.py
+-rw-rw-rw-   0        0        0     7629 2024-05-24 00:31:01.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/ga.py
+-rw-rw-rw-   0        0        0     2460 2024-05-21 23:05:20.000000 mcdm_scheduler-1.5.3/mcdm_scheduler/util/ht2fs.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/
+-rw-rw-rw-   0        0        0     1877 2024-05-25 20:38:42.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2024-05-25 20:38:43.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 20:38:42.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-25 20:38:42.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-25 20:38:42.000000 mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 20:38:44.000000 mcdm_scheduler-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      644 2024-05-25 20:37:32.000000 mcdm_scheduler-1.5.3/setup.py
```

### Comparing `mcdm_scheduler-1.5.2/LICENSE` & `mcdm_scheduler-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.2/PKG-INFO` & `mcdm_scheduler-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdm_scheduler
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Library Incorporating a MCDM tools for Scheduling Problems
 Home-page: https://github.com/Valdecy/mcdm_scheduler
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,9 +22,9 @@
 - Genetic Algorithm Optimization: Applies a Genetic Algorithm (GA) to optimize scheduling tasks, leveraging its ability to handle complex and variable conditions to find near-optimal solutions efficiently.
 - Custom Values: Offers the flexibility for users to input their custom weights for objectives, including selecting one or more objectives, jobs, and even defining a specific job sequence. This customization ensures that the scheduling solution is precisely aligned with the user's specific needs and preferences.
 
 ## Usage
 
 2. Try it in **Colab**:
 
-- Example ( [ Colab Demo ](https://colab.research.google.com/drive/10px7FHlGmcXwshZFzkS7JubpJYwj7J-f?usp=sharing)) ) 
+- Example ( [ Colab Demo ](https://colab.research.google.com/drive/10px7FHlGmcXwshZFzkS7JubpJYwj7J-f?usp=sharing))
```

### Comparing `mcdm_scheduler-1.5.2/README.md` & `mcdm_scheduler-1.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,9 +11,9 @@
 - Genetic Algorithm Optimization: Applies a Genetic Algorithm (GA) to optimize scheduling tasks, leveraging its ability to handle complex and variable conditions to find near-optimal solutions efficiently.
 - Custom Values: Offers the flexibility for users to input their custom weights for objectives, including selecting one or more objectives, jobs, and even defining a specific job sequence. This customization ensures that the scheduling solution is precisely aligned with the user's specific needs and preferences.
 
 ## Usage
 
 2. Try it in **Colab**:
 
-- Example ( [ Colab Demo ](https://colab.research.google.com/drive/10px7FHlGmcXwshZFzkS7JubpJYwj7J-f?usp=sharing)) ) 
+- Example ( [ Colab Demo ](https://colab.research.google.com/drive/10px7FHlGmcXwshZFzkS7JubpJYwj7J-f?usp=sharing))
```

### Comparing `mcdm_scheduler-1.5.2/mcdm_scheduler/algorithm/src.py` & `mcdm_scheduler-1.5.3/mcdm_scheduler/algorithm/src.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from mcdm_scheduler.util.ga            import genetic_algorithm
 from mcdm_scheduler.util.ht2fs         import ht2fs_weight_calculation
 
 ############################################################################
 
 # MCDM Scheduler Class
 class load_mcdm_scheduler():
-    def __init__(self, sequences = [], due_dates = [], setup_time_matrix = [], setup_waste_matrix = [], comparison_matrix = [], crisp_inputs = [], uncertainty_ranges = [], criteria_importance = [], population_size = 5, elite = 1, mutation_rate = 0.1, generations = 100, custom_job_weights = [], custom_objective_weights = [], custom_job_sequence = [], brute_force = False): 
+    def __init__(self, sequences = [], due_dates = [], setup_time_matrix = [], setup_waste_matrix = [], comparison_matrix = [], crisp_inputs = [], uncertainty_ranges = [], criteria_importance = [], population_size = 5, elite = 1, mutation_rate = 0.1, generations = 100, custom_job_weights = [], custom_objective_weights = [], custom_job_sequence = [], brute_force = False, parallel = False): 
       self.job_weights                    = custom_job_weights         # Job Weights: Opitional
       self.objectives_weights             = custom_objective_weights   # Objectives Weights (Makespan, Max WeightedTardiness, Total Waste, Total Setup Time): Opitional
       self.custom_job_sequence            = custom_job_sequence
       self.sequences                      = sequences                  # Job Shop Scheduling Input: Mandatory
       self.due_dates                      = due_dates                  # Job Shop Scheduling Input: Only Relevant if Due Date    is a measure
       self.setup_time_matrix              = setup_time_matrix          # Job Shop Scheduling Input: Only Relevant if Setup Time  is a measure
       self.setup_waste_matrix             = setup_waste_matrix         # Job Shop Scheduling Input: Only Relevant if Setup Waste is a measure
@@ -38,14 +38,15 @@
       self.uncertainty_ranges             = uncertainty_ranges         # HT2FS               Input: Only Relevant if custom_job_weights        = []
       self.criteria_importance            = criteria_importance        # HT2FS               Input: Only Relevant if custom_job_weights        = []
       self.population_size                = population_size            # GA
       self.elite                          = int(elite)                 # GA
       self.mutation_rate                  = mutation_rate              # GA
       self.generations                    = generations                # GA
       self.brute_force                    = brute_force
+      self.parallel                       = parallel
       self.machine_sequences, self.matrix = self.sequence_inputs()
       self.num_jobs                       = len(self.sequences)
       self.num_machines                   = self.matrix.shape[1]
     
     ###############################################################################
     
     # Plot
@@ -92,15 +93,14 @@
         ax.set_xticklabels(np.arange(0, total_length + 1, 1))  
         ax.set_yticks(np.arange(0, self.num_machines, 1))
         ax.set_yticklabels([])
         for i in range(0, self.num_machines):
             ax.text(-0.5, self.num_machines - i - 0.5, f'Machine {i}', va = 'center', ha = 'right', fontsize = 10)
         ax.set_xlabel('Time')
         ax.set_title('Gantt Chart')
-        #ax.grid(True)
         ax.grid(True, linestyle = '--', alpha = 0.7)
         plt.show()
     
     ###############################################################################
     
     # Objectives
     def calculate_makespan(self, schedule_matrix):
@@ -160,86 +160,110 @@
     
     # Schedule
     def schedule_jobs(self, permutation):
         total_length      = np.sum(self.matrix)
         schedule          = [['' for _ in range(0, total_length)] for _ in range(0, self.num_machines)]
         machine_end_times = [0] * self.num_machines
         job_end_times     = [0] * self.num_jobs
-        for job_id in permutation:
-            operations = self.machine_sequences[job_id]
-            for op_index, machine in enumerate(operations):
-                time_required = self.matrix[job_id, machine]
-                start_time    = job_end_times[job_id]
-                while any(schedule[machine][start_time:start_time + time_required]):
-                    start_time = start_time + 1
-                end_time = start_time + time_required
-                for t in range(start_time, end_time):
-                    schedule[machine][t] = f"j{job_id}"
-                job_end_times[job_id]      = end_time
-                machine_end_times[machine] = end_time
+        if (self.parallel == False):
+            for job_id in permutation:
+                operations = self.machine_sequences[job_id]
+                for op_index, machine in enumerate(operations):
+                    time_required = self.matrix[job_id, machine]
+                    start_time    = job_end_times[job_id]
+                    while any(schedule[machine][start_time:start_time + time_required]):
+                        start_time = start_time + 1
+                    end_time = start_time + time_required
+                    for t in range(start_time, end_time):
+                        schedule[machine][t] = f"j{job_id}"
+                    job_end_times[job_id]      = end_time
+                    machine_end_times[machine] = end_time
+        else:        
+            for job_id in permutation:
+                earliest_start_time = float('inf')
+                best_machine = None
+                
+                for machine, time_required in self.sequences[job_id]:
+                    start_time = machine_end_times[machine]
+                    while any(schedule[machine][start_time:start_time + time_required]):
+                        start_time = start_time + 1
+                    if (start_time < earliest_start_time):
+                        earliest_start_time = start_time
+                        best_machine = machine
+                time_required = self.matrix[job_id, best_machine]
+                end_time = earliest_start_time + time_required
+                for t in range(earliest_start_time, end_time):
+                    schedule[best_machine][t] = f"j{job_id}"
+                machine_end_times[best_machine] = end_time
+                job_end_times[job_id] = end_time
         max_time = max(len(row) for row in schedule)
         for col in range(max_time - 1, -1, -1):
-            if all(row[col] == '' for row in schedule):
+            if (all(row[col] == '' for row in schedule)):
                 for row in schedule:
                     row.pop()
             else:
                 break
         return np.array(schedule)
     
     def brute_force_search(self):
-        job_ids                        = list(range(len(self.sequences)))
-        best_sequence                  = None
-        minimal_objective_value        = float('inf')
+        job_ids                 = list(range(len(self.sequences)))
+        best_sequence           = None
+        minimal_objective_value = float('inf')
         for permutation in itertools.permutations(job_ids):
-            schedule_matrix        = self.schedule_jobs(permutation)
-            makespan               = self.calculate_makespan(schedule_matrix)
-            max_weighted_tardiness = self.calculate_max_weighted_tardiness(schedule_matrix)
-            total_waste            = self.calculate_total_waste(permutation)
-            total_setup_time       = self.calculate_total_setup_time(permutation)
-            objective_value        = (
-                                        self.objectives_weights[0] * makespan +
-                                        self.objectives_weights[1] * max_weighted_tardiness +
-                                        self.objectives_weights[2] * total_waste +
-                                        self.objectives_weights[3] * total_setup_time
-                                      ) / 1.0
-            print(permutation, makespan, max_weighted_tardiness, total_waste, total_setup_time, objective_value )
+            schedule_matrix = self.schedule_jobs(permutation)
+            objective_value = 0.0 / 1.0
+            if (self.objectives_weights[0] != 0):
+                makespan               = self.calculate_makespan(schedule_matrix)
+                objective_value        = objective_value + self.objectives_weights[0] * makespan
+            if (self.objectives_weights[1] != 0):
+                max_weighted_tardiness = self.calculate_max_weighted_tardiness(schedule_matrix)
+                objective_value        = objective_value + self.objectives_weights[1] * max_weighted_tardiness
+            if (self.objectives_weights[2] != 0):
+                total_waste            = self.calculate_total_waste(permutation)
+                objective_value        = objective_value + self.objectives_weights[2] * total_waste
+            if (self.objectives_weights[3] != 0):
+                total_setup_time       = self.calculate_total_setup_time(permutation)
+                objective_value        = objective_value + self.objectives_weights[3] * total_setup_time
             if (objective_value < minimal_objective_value):
                 minimal_objective_value = objective_value
                 best_sequence           = permutation
         self.best_sequence = best_sequence
         return best_sequence, minimal_objective_value
     
     def target_function(self, permutation): 
-        schedule_matrix           = self.schedule_jobs(permutation)
-        makespan                  = self.calculate_makespan(schedule_matrix)
-        max_weighted_tardiness    = self.calculate_max_weighted_tardiness(schedule_matrix)
-        total_waste               = self.calculate_total_waste(permutation)
-        total_setup_time          = self.calculate_total_setup_time(permutation)
-        objective_value           = (
-                                      self.objectives_weights[0] * makespan +
-                                      self.objectives_weights[1] * max_weighted_tardiness +
-                                      self.objectives_weights[2] * total_waste +
-                                      self.objectives_weights[3] * total_setup_time
-                                    ) / 1.0
+        schedule_matrix = self.schedule_jobs(permutation)
+        objective_value = 0.0 / 1.0
+        if (self.objectives_weights[0] != 0):
+            makespan               = self.calculate_makespan(schedule_matrix)
+            objective_value        = objective_value + self.objectives_weights[0] * makespan
+        if (self.objectives_weights[1] != 0):
+            max_weighted_tardiness = self.calculate_max_weighted_tardiness(schedule_matrix)
+            objective_value        = objective_value + self.objectives_weights[1] * max_weighted_tardiness
+        if (self.objectives_weights[2] != 0):
+            total_waste            = self.calculate_total_waste(permutation)
+            objective_value        = objective_value + self.objectives_weights[2] * total_waste
+        if (self.objectives_weights[3] != 0):
+            total_setup_time       = self.calculate_total_setup_time(permutation)
+            objective_value        = objective_value + self.objectives_weights[3] * total_setup_time
         return objective_value
     
     def run_mcdm_scheduler(self):
         if (len(self.objectives_weights) == 0):
             weights = [[] for item in self.comparison_matrix]
             rc      = [[] for item in self.comparison_matrix]
             g_mean  = []
             i       = 0
             for item in self.comparison_matrix:
                 weights[i], rc[i] = ppf_ahp_method(item)
                 if (len(g_mean) == 0):
                     g_mean = weights[i]
                 else:
                     g_mean = [g_mean[j]*weights[i][j] for j in range(0, len(weights[i]))]
-                i                 = i + 1
-            g_mean                  = [g_mean[j]**(1/len(weights)) for j in range(0, len(g_mean))]   
+                i = i + 1
+            g_mean = [g_mean[j]**(1/len(weights)) for j in range(0, len(g_mean))]   
             self.objectives_weights = g_mean
         if (len(self.job_weights) == 0):
             for k in range(0, len(self.crisp_inputs)):
                 job_weights = ht2fs_weight_calculation(self.crisp_inputs[k], self.uncertainty_ranges[k], self.criteria_importance[k])
                 if (len(self.job_weights) == 0):
                     self.job_weights = job_weights
                 else:
```

### Comparing `mcdm_scheduler-1.5.2/mcdm_scheduler/util/fuzzy_ppf_ahp.py` & `mcdm_scheduler-1.5.3/mcdm_scheduler/util/fuzzy_ppf_ahp.py`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.2/mcdm_scheduler/util/ga.py` & `mcdm_scheduler-1.5.3/mcdm_scheduler/util/ga.py`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.2/mcdm_scheduler/util/ht2fs.py` & `mcdm_scheduler-1.5.3/mcdm_scheduler/util/ht2fs.py`

 * *Files identical despite different names*

### Comparing `mcdm_scheduler-1.5.2/mcdm_scheduler.egg-info/PKG-INFO` & `mcdm_scheduler-1.5.3/mcdm_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcdm-scheduler
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Library Incorporating a MCDM tools for Scheduling Problems
 Home-page: https://github.com/Valdecy/mcdm_scheduler
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,9 +22,9 @@
 - Genetic Algorithm Optimization: Applies a Genetic Algorithm (GA) to optimize scheduling tasks, leveraging its ability to handle complex and variable conditions to find near-optimal solutions efficiently.
 - Custom Values: Offers the flexibility for users to input their custom weights for objectives, including selecting one or more objectives, jobs, and even defining a specific job sequence. This customization ensures that the scheduling solution is precisely aligned with the user's specific needs and preferences.
 
 ## Usage
 
 2. Try it in **Colab**:
 
-- Example ( [ Colab Demo ](https://colab.research.google.com/drive/10px7FHlGmcXwshZFzkS7JubpJYwj7J-f?usp=sharing)) ) 
+- Example ( [ Colab Demo ](https://colab.research.google.com/drive/10px7FHlGmcXwshZFzkS7JubpJYwj7J-f?usp=sharing))
```

### Comparing `mcdm_scheduler-1.5.2/setup.py` & `mcdm_scheduler-1.5.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='mcdm_scheduler',
-    version='1.5.2',
+    version='1.5.3',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/mcdm_scheduler',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

