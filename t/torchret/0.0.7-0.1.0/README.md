# Comparing `tmp/torchret-0.0.7.tar.gz` & `tmp/torchret-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchret-0.0.7.tar", last modified: Tue May 14 19:10:39 2024, max compression
+gzip compressed data, was "torchret-0.1.0.tar", last modified: Sat May 25 18:23:13 2024, max compression
```

## Comparing `torchret-0.0.7.tar` & `torchret-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 19:10:39.170760 torchret-0.0.7/
--rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 19:10:39.170601 torchret-0.0.7/PKG-INFO
--rw-r--r--   0 parth      (501) staff       (20)       38 2024-05-14 19:10:39.170829 torchret-0.0.7/setup.cfg
--rw-r--r--   0 parth      (501) staff       (20)      564 2024-05-14 19:09:26.000000 torchret-0.0.7/setup.py
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 19:10:39.169395 torchret-0.0.7/torchret/
--rw-r--r--   0 parth      (501) staff       (20)       25 2024-05-14 03:58:19.000000 torchret-0.0.7/torchret/__init__.py
--rw-r--r--   0 parth      (501) staff       (20)    13531 2024-05-14 19:09:10.000000 torchret-0.0.7/torchret/model.py
--rw-r--r--   0 parth      (501) staff       (20)      921 2024-05-14 01:12:58.000000 torchret-0.0.7/torchret/utils.py
-drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-14 19:10:39.170350 torchret-0.0.7/torchret.egg-info/
--rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-14 19:10:39.000000 torchret-0.0.7/torchret.egg-info/PKG-INFO
--rw-r--r--   0 parth      (501) staff       (20)      224 2024-05-14 19:10:39.000000 torchret-0.0.7/torchret.egg-info/SOURCES.txt
--rw-r--r--   0 parth      (501) staff       (20)        1 2024-05-14 19:10:39.000000 torchret-0.0.7/torchret.egg-info/dependency_links.txt
--rw-r--r--   0 parth      (501) staff       (20)       13 2024-05-14 19:10:39.000000 torchret-0.0.7/torchret.egg-info/requires.txt
--rw-r--r--   0 parth      (501) staff       (20)        9 2024-05-14 19:10:39.000000 torchret-0.0.7/torchret.egg-info/top_level.txt
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-25 18:23:13.468757 torchret-0.1.0/
+-rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-25 18:23:13.468598 torchret-0.1.0/PKG-INFO
+-rw-r--r--   0 parth      (501) staff       (20)       38 2024-05-25 18:23:13.468841 torchret-0.1.0/setup.cfg
+-rw-r--r--   0 parth      (501) staff       (20)      564 2024-05-25 18:23:10.000000 torchret-0.1.0/setup.py
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-25 18:23:13.467352 torchret-0.1.0/torchret/
+-rw-r--r--   0 parth      (501) staff       (20)       25 2024-05-14 03:58:19.000000 torchret-0.1.0/torchret/__init__.py
+-rw-r--r--   0 parth      (501) staff       (20)    15290 2024-05-25 18:22:26.000000 torchret-0.1.0/torchret/model.py
+-rw-r--r--   0 parth      (501) staff       (20)      921 2024-05-14 01:12:58.000000 torchret-0.1.0/torchret/utils.py
+drwxr-xr-x   0 parth      (501) staff       (20)        0 2024-05-25 18:23:13.468345 torchret-0.1.0/torchret.egg-info/
+-rw-r--r--   0 parth      (501) staff       (20)      244 2024-05-25 18:23:13.000000 torchret-0.1.0/torchret.egg-info/PKG-INFO
+-rw-r--r--   0 parth      (501) staff       (20)      224 2024-05-25 18:23:13.000000 torchret-0.1.0/torchret.egg-info/SOURCES.txt
+-rw-r--r--   0 parth      (501) staff       (20)        1 2024-05-25 18:23:13.000000 torchret-0.1.0/torchret.egg-info/dependency_links.txt
+-rw-r--r--   0 parth      (501) staff       (20)       13 2024-05-25 18:23:13.000000 torchret-0.1.0/torchret.egg-info/requires.txt
+-rw-r--r--   0 parth      (501) staff       (20)        9 2024-05-25 18:23:13.000000 torchret-0.1.0/torchret.egg-info/top_level.txt
```

### Comparing `torchret-0.0.7/setup.py` & `torchret-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = f.read().splitlines()
 
 
 setup(
     name="torchret",
     description="",
     long_description="",
-    version = '0.0.7',
+    version = '0.1.0',
     long_description_content_type="text/markdown",
     author="Parth Dhameliya",
     url="https://github.com/parthdhameliya7",
     license="Apache License 2.0",
     packages=find_packages(),
     include_package_data=True,
     platforms=["linux", "unix"],
```

### Comparing `torchret-0.0.7/torchret/model.py` & `torchret-0.1.0/torchret/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -131,48 +131,68 @@
         # Apply mixup or cutmix augmentation
         if random.uniform(0, 1) > self.mixup:
             data = self.get_mixup(data)
         elif random.uniform(0, 1) > self.cutmix:
             data = self.get_cutmix(data)
 
         # Apply train step with fp16 precision training 
-        if self.fp16 is not None:
+        if self.fp16 is True:
             self.optimizer.zero_grad()
             _, loss, metrics = self.model_fn(data)
             self.scaler.scale(loss).backward()
             self.scaler.step(self.optimizer)
             self.scaler.update()
 
         # Apply train step with Sharpness-Aware Minimization 
-        elif self.sam_training is not None:
+        elif self.sam_training is True:
             _, loss1, metrics = self.model_fn(data)
             loss1.backward()
             self.optimizer.first_step(zero_grad = True)
 
             _, loss2, metrics = self.model_fn(data)
             loss2.backward()
             self.optimizer.second_step(zero_grad = True)
 
         else:
             self.optimizer.zero_grad()
             _, loss, metrics = self.model_fn(data)
             loss.backward()
             self.optimizer.step()
 
-        if self.scheduler is not None:
+        if self.scheduler is True:
             if self.step_scheduler_after == 'batch':
                 self.scheduler.step()
                 
         return loss, metrics
     
     def valid_one_step(self, data):
+        """
+        Perform one step of validation.
+
+        Args:
+            data (dict): Dictionary containing input data tensors.
+
+        Returns:
+            loss: Loss tensor.
+            metrics: Dictionary containing additional metrics.
+        """
         _, loss, metrics = self.model_fn(data)
         return loss, metrics
 
     def train_one_epoch(self, dataloader):
+        """
+        Perform one epoch of training.
+
+        Args:
+            dataloader (torch.nn.Module): batches of data.
+
+        Returns:
+            loss: Loss Average.
+            monitor: Dictionary containing additional metrics with averages.
+        """
         self.train()
         losses = AverageMeter()
         tracker = tqdm(dataloader, total = len(dataloader))
         for batch_id, data in enumerate(tracker):
             loss, metrics = self.train_one_step(data)
             losses.update(loss.item(), dataloader.batch_size)
             if batch_id == 0:
@@ -180,29 +200,39 @@
             monitor = {}
             for m_m in metrics_meter:
                 metrics_meter[m_m].update(metrics[m_m].item(), dataloader.batch_size)
                 monitor[m_m] = metrics_meter[m_m].avg
             tracker.set_postfix(epoch = self.current_epoch, loss='%.6f' %float(losses.avg), stage="train", current_lr = self.optimizer.param_groups[0]['lr'], **monitor)
             self.current_train_step += 1
 
-        if self.swa_training is not None:
+        if self.swa_training is True:
             if self.current_epoch + 1 >= self.swa_start:
                 self.swa_model.update_parameters(self)
             else:
-                if self.scheduler is not None:
+                if self.scheduler is True:
                     if self.step_scheduler_after == 'epoch':
                         self.scheduler.step()
         else:
-            if self.scheduler is not None:
+            if self.scheduler is True:
                 if self.step_scheduler_after == 'epoch':
                     self.scheduler.step()
         tracker.close()
         return losses.avg, monitor
     
     def valid_one_epoch(self, dataloader):
+        """
+        Perform one epoch of validation.
+
+        Args:
+            dataloader (torch.nn.Module): batches of data.
+
+        Returns:
+            loss: Loss Average.
+            monitor: Dictionary containing additional metrics with averages.
+        """
         self.eval()
         losses = AverageMeter()
         tracker = tqdm(dataloader, total = len(dataloader))
         with torch.no_grad():
             for batch_id, data in enumerate(tracker):
                 loss, metrics = self.valid_one_step(data)
                 losses.update(loss.item(), dataloader.batch_size)
@@ -214,22 +244,49 @@
                     monitor[m_m] = metrics_meter[m_m].avg
                 tracker.set_postfix(epoch = self.current_epoch, loss='%.6f' %float(losses.avg), stage="eval", **monitor)
                 self.current_valid_step += 1
             tracker.close()
             return losses.avg, monitor
         
     def predict_one_step(self, data):
+        """
+        Predict one step of test.
+
+        Args:
+            data (dict): Dictionary containing input data tensors.
+
+        Returns:
+            output: output tensor
+        """
         output, _, _ = self.model_fn(data)
         return output
         
     def process_output(self, output):
+        """
+        Move output to cpu and convert into numpy 
+
+        Args:
+            output (Torch.Tensor): A tensor containing output of the model
+        Returns:
+            output: output tensor
+        """
         output = output.cpu().detach().numpy()
         return output
         
     def predict(self, dataset, batch_size = 16, collate_fn = None):
+        """
+        Move output to cpu and convert into numpy 
+
+        Args:
+            data (Torch Dataset): Torch Dataset
+            batch_size (int) : 16
+            collate function 
+        Returns:
+            output: output tensor
+        """
         if next(self.parameters()).device != self.device:
             self.to(self.device)
 
         if self.num_workers is None:
             n_jobs = 0
 
         data_loader = torch.utils.data.DataLoader(
@@ -246,14 +303,23 @@
                 out = self.predict_one_step(data)
                 out = self.process_output(out)
                 yield out 
                 tracker.set_postfix(stage = 'test')
         tracker.close()
         
     def save(self, model_path, weights_only = False):
+        """
+        Move output to cpu and convert into numpy 
+
+        Args:
+            model_path (str): model filepath
+            weights_only (bool) : to save only weights
+        Returns:
+            output: output tensor
+        """
         model_state_dict = self.state_dict()
         if weights_only:
             torch.save(model_state_dict, model_path)
             return 
         if self.optimizer is not None:
             opt_state_dict = self.optimizer.state_dict()
         else:
@@ -297,32 +363,35 @@
             train_dataset,
             valid_dataset = None,
             device = 'cuda',
             epochs = 10,
             train_bs = 64,
             valid_bs = 64,
     ):
+        self.device = device
 
         if self.trainloader is None:
             self.trainloader = torch.utils.data.DataLoader(
                 train_dataset,
                 train_bs,
                 shuffle = True
             )
-        
-        if self.validloader is None:
+        if valid_dataset is not None: 
             self.validloader = torch.utils.data.DataLoader(
                 valid_dataset,
                 valid_bs,
                 shuffle = True
             )
+        else:
+            self.validloader = None
+            
         if next(self.parameters()).device != self.device:
             self.to(self.device)
         
-        if self.fp16:
+        if self.fp16 is True:
             self.scaler = torch.cuda.amp.GradScaler()
 
         self.optimizer, self.scheduler = self.fetch_optimizer()
         self.current_epoch += 1
         self.best_loss = 1000
         self.best_score = 0.0
 
@@ -337,15 +406,15 @@
                 if self.save_best_model == 'on_eval_loss':
                     if self.valid_loss < self.best_loss:
                         if self.model_path is not None:
                             self.save(f'{self.model_path}', self.weights_only)
                         print(f'Model was saved based {self.save_best_model} with {self.valid_loss} loss')
                         self.best_loss = self.valid_loss
                 elif self.save_best_model == 'on_eval_metric':
-                    if self.save_on_metric in self.train_metrics:
+                    if self.save_on_metric in self.valid_metrics:
                         if self.valid_metrics[self.save_on_metric] > self.best_score:
                             self.save(f'{self.model_path}', self.weights_only)
                             print(f'Model was saved based {self.save_best_model} with {self.valid_metrics[self.save_on_metric]} {self.save_on_metric}')
                             self.best_score = self.valid_metrics[self.save_on_metric]
             if self.save_model_at_every_epoch is True:
                 self.save(self.model_path, self.weights_only)
```

### Comparing `torchret-0.0.7/torchret/utils.py` & `torchret-0.1.0/torchret/utils.py`

 * *Files identical despite different names*

