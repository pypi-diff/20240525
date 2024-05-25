# Comparing `tmp/sforecast-0.4.4.tar.gz` & `tmp/sforecast-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sforecast-0.4.4.tar", max compression
+gzip compressed data, was "sforecast-0.5.8.tar", max compression
```

## Comparing `sforecast-0.4.4.tar` & `sforecast-0.5.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1076 2022-09-11 14:58:50.467840 sforecast-0.4.4/LICENSE
--rw-r--r--   0        0        0      633 2023-01-14 04:06:03.412588 sforecast-0.4.4/README.md
--rw-r--r--   0        0        0      872 2023-01-28 00:03:33.735287 sforecast-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      149 2023-01-13 21:32:18.872371 sforecast-0.4.4/src/sforecast/__init__.py
--rw-r--r--   0        0        0   130595 2023-01-27 23:58:54.184240 sforecast-0.4.4/src/sforecast/sforecast.py
--rw-r--r--   0        0        0     1670 2023-01-28 00:06:08.832723 sforecast-0.4.4/setup.py
--rw-r--r--   0        0        0     1550 2023-01-28 00:06:08.833081 sforecast-0.4.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1076 2022-09-11 14:58:50.467840 sforecast-0.5.8/LICENSE
+-rw-r--r--   0        0        0      680 2024-05-06 14:01:10.743254 sforecast-0.5.8/README.md
+-rw-r--r--   0        0        0      891 2024-05-25 13:14:36.811342 sforecast-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      183 2024-05-18 14:05:57.690530 sforecast-0.5.8/src/sforecast/__init__.py
+-rw-r--r--   0        0        0   130741 2024-05-23 12:51:45.100657 sforecast-0.5.8/src/sforecast/sforecast.py
+-rw-r--r--   0        0        0     1739 2024-05-25 13:26:06.571485 sforecast-0.5.8/setup.py
+-rw-r--r--   0        0        0     1581 2024-05-25 13:26:06.572286 sforecast-0.5.8/PKG-INFO
```

### Comparing `sforecast-0.4.4/LICENSE` & `sforecast-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sforecast-0.4.4/README.md` & `sforecast-0.5.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # sforecast
 
 A framework for running forecasting models within a sliding (expanding) window out-of-sample fit (train/test) and prediction (forecasts). The package includes support of classical forecasting models, SK Learn ML models, and TensorFlow deep learning models.
 
+- https://sforecast.readthedocs.io/en/latest/
+
 ## Installation
 
 ```bash
 $ pip install sforecast
 ```
 
 ## License
```

### Comparing `sforecast-0.4.4/src/sforecast/sforecast.py` & `sforecast-0.5.8/src/sforecast/sforecast.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,34 +220,32 @@
         assert self.Nlags >=0 ,f'Nlags = {self.Nlags} not allowed. Nlags must be >= 0'
         
     def fit(self,df):
         
         self.dfmemory = df.tail(self.Nmemory) if df.index.size > self.Nmemory else df.index.size
         return self
     
-    def transform(self, df=None, Nout=None, dfnewrows=None, debug=False):
+    def transform(self, df=pd.DataFrame(), Nout=None, dfnewrows=pd.DataFrame(), debug=False):
         # if df not spefified then transform dfmemory
         # add new row(s) and update dfmemory
-        """Create lagged variables from covariates.
+        """Create lagged covariates.
 
         Args:
-            df (DataFrame, optional): _description_. Defaults to None.
+            df (DataFrame, optional): dataframe containing covariats. Defaults to empty dataframe..
             Nout (int, optional): Number of output rows. Defaults to None.
             dfnewrows (DataFrame, optional): new row to append to the DataFrame. The DataFrame memory will be updated with the last Nlags+1 rows. Defaults to None.
             debug (bool, optional): _description_. Defaults to False.
 
         Returns:
             DataFrame with the addition of lagged variables
         """
         
-        if not isinstance(df,pd.DataFrame):
+        if len(df)==0:
             df = self.dfmemory
-            #print("covarlags.transform: dfmemory before new rows =")
-            #display(df.tail())
-            if isinstance(dfnewrows,pd.DataFrame):
+            if len(dfnewrows)>0:
                 df = pd.concat([df,dfnewrows])
                 self.dfmemory = df.tail(self.Nmemory)    
             
             if debug == True:    
                 print("  covarlags.transform: new row dfmemory.tail()")
                 display(df.tail(3))
         
@@ -521,15 +519,15 @@
             print("test_train_predict: i_initial_predt =", i_initial_pred)
             print("test_train_predict: i_last_fit =", i_last_fit)
             print("test_train_predict: i_loop_first =", i_loop_first)
             print("test_train_predict: i_loop_last =", i_loop_last)
             print("test_train_predict: N_loop_step = ",N_loop_step)
     
         # initialize additional varialbels 
-        make_lags = None  # default ot none ... None for cm models, not none for sk and tf models
+        make_lags = None  # default to none ... None for cm models, not none for sk and tf models
         make_derived_attributes = None # default to noe ...None for cm models, not none for sk and tf models
         scaler = None # # default to noe ...None for cm models, not none for sk and tf models
         
         y_pred_nda = None
         y_test_nda = None
         y_pred_idx = None
         
@@ -580,26 +578,29 @@
             dfy = dfXY[y]
             dfXY_train = dfXY.iloc[:i + Nclip] # add Nclip since adjusted for Nclip above
             dfY_train = dfy.iloc[:i + Nclip] # add Nclip since adjusted for Nclip above
 
             
             #### Covarlags
             if lags: #  need lags for cm if have derived_attributes
+
                 make_lags = covarlags(covars=covars,Nlags=Nlags)
                 if model_type == "tf":
                     if catvars != None:
                         dfXcats_train = dfXY_train[catvars] 
                         _dfXY_train = dfXY_train.drop(catvars, axis =1 )
                         dfXY_train=make_lags.fit_transform(_dfXY_train) #
                     else:
                         dfXY_train=make_lags.fit_transform(dfXY_train)
                         
                 else:
+                    
                     dfXY_train=make_lags.fit_transform(dfXY_train)
 
+
             # dfX_train ... after make lags 
             dfX_train = dfXY_train.drop(covars,axis=1)
             
             #### Derived Variables
             # dfXexen
             #   ouput of derived variables contains 
             #     endogenous derived variables 
@@ -968,35 +969,38 @@
                         if horizon_predict_method == "single_step" or k == 0:   # single_step any k or multi_step only when k == 0
                         
                             p_index = [dfxy.index[i+k]] if fit == True else [index_pred[i+k]]
                             
                             dfXY_pred = pd.DataFrame(data = {_cv:np.NaN for _cv in covars } , columns = covars, index = p_index)
                             
                             # update y with previous prediction in covarlags
+
                             if (fit == True and k > 0) or (predict == True and predict_cnt > 0): 
                                 # update the previous y in make_lags
+                                
                                 for _cv in covars:
                                     make_lags.set_last_y(_cv,y_pred_nda[_cv][predict_cnt-1], debug=debug)
                             # lags
-                            dfXY_pred = make_lags.transform(dfnewrows=dfXY_pred, Nout = 1, debug=debug)
+                            # def transform(self, df=None, Nout=None, dfnewrows=None, debug=False)
+                            dfXY_pred = make_lags.transform( pd.DataFrame(),dfnewrows=dfXY_pred, Nout = 1, debug=debug)
                             
                             
                             dfX_pred = dfXY_pred.drop(covars,axis=1)
-                            
-                                                            
+                                                          
                             # exogs
                             #dfXexen[exogvars] = dfxy.iloc[i+k:i+k+1][exogvars].values if exogvars != None else dfXexen
                             if fit == True:
                                 if exogvars != None: dfX_pred[exogvars] = dfxy.iloc[i+k:i+k+1][exogvars].values
                             elif predict == True:
                                 if exogvars != None: dfX_pred[exogvars] = pred_params["dfexogs"].iloc[i+k:i+k+1].values
                             
                             # derived attributes
                             if derived:
-                                dfX_pred = make_derived_attributes.transform(dfnewrows=dfX_pred,Nout=1 )
+                                
+                                dfX_pred = make_derived_attributes.transform(pd.DataFrame(),dfnewrows=dfX_pred,Nout=1 )
                              
                                 
                             # scale
                             dfX_pred = scaler.transform(dfX_pred)
                             X_pred = dfX_pred.values
 
                                     
@@ -1014,28 +1018,28 @@
                         #Lags
                         # update y with previous prediction in covarlags
                         if (fit == True and k > 0) or (predict == True and predict_cnt > 0): # 
                             # update the previous y in make_lags
                             for _cv in covars:
                                 make_lags.set_last_y(_cv,y_pred_nda[_cv][predict_cnt-1])  #
                                     
-                        dfXY_pred = make_lags.transform(dfnewrows=dfXY_pred, Nout = 1, debug=debug)
+                        dfXY_pred = make_lags.transform(pd.DataFrame(),dfnewrows=dfXY_pred, Nout = 1, debug=debug)
                         dfX_pred = dfXY_pred.drop(covars,axis=1) 
                         
                         # exogs
                         #dfXexen[exogvars] = dfxy.iloc[i+k:i+k+1][exogvars].values if exogvars != None else dfXexen
                         if fit == True:
                             if exogvars != None: dfX_pred[exogvars] = dfxy.iloc[i+k:i+k+1][exogvars].values
                         elif predict == True:
                             if exogvars != None: dfX_pred[exogvars] = pred_params["dfexogs"].iloc[i+k:i+k+1].values
                             
                         
                         # endogs ... derived 
                         if derived:
-                            dfX_pred = make_derived_attributes.transform(dfnewrows=dfX_pred,Nout=1 )
+                            dfX_pred = make_derived_attributes.transform(   pd.DataFrame(), dfnewrows=dfX_pred,Nout=1 )
                             
                         if debug == True:
                             exen_str = "w exenvars" if exenvars != None else ""
                             print(f'  test_train_predict: df_pred {exen_str}')
                             display(dfX_pred.tail(3))
 
                         # scale
@@ -1185,19 +1189,19 @@
                                 # only autoarima with derived variables will use this .. y_pred_nda[k-1] is a scaler
                                 
                             # exogs
                             if exogvars != None: 
                                 dfXexen_pred[exogvars] = dfxy.iloc[i+k:i+k+1][exogvars].values if fit == True else pred_params["dfexogs"].iloc[k:k+1].values 
 
                             # make_lags
-                            dfXexen_pred = make_lags.transform(dfnewrows=dfXexen_pred, Nout = 1, debug=debug)
+                            dfXexen_pred = make_lags.transform(pd.DataFrame(),dfnewrows=dfXexen_pred, Nout = 1, debug=debug)
                             dfXexen_pred = dfXexen_pred.drop(y,axis=1)
                             
                             # derived attributes
-                            dfXexen_pred = make_derived_attributes.transform(dfnewrows=dfXexen_pred,Nout=1 )
+                            dfXexen_pred = make_derived_attributes.transform(pd.DataFrame(),dfnewrows=dfXexen_pred,Nout=1 )
                             dfXexen_pred = dfXexen_pred[exenvars]
                             
                             if debug == True:
                                 print("  test_train_predict: cm fit predict dfXexen_test w derived =")
                                 display(dfXexen_pred)
                             
                             Xexen_pred = dfXexen_pred.values
```

### Comparing `sforecast-0.4.4/setup.py` & `sforecast-0.5.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['beautifulplots>=0.2.6',
  'pandas>=1.4.0',
  'pmdarima>=1.8.0',
- 'sklearn>=0.0',
+ 'scikit-learn>=1.4.2',
  'statsmodels>=0.13.2',
- 'tensorflow>=2.7.0']
+ 'tensorflow>=2.7.0',
+ 'xgboost>=2.0.3']
 
 setup_kwargs = {
     'name': 'sforecast',
-    'version': '0.4.4',
+    'version': '0.5.8',
     'description': 'A framework for running forecasting models within a sliding/expanding window out-of-sample forecast fit (train/test) and prediction (forecasts). The package includes support of classical forecasting models, SK Learn supervised learning ML models, and TensorFlow deep learning models.',
-    'long_description': '# sforecast\n\nA framework for running forecasting models within a sliding (expanding) window out-of-sample fit (train/test) and prediction (forecasts). The package includes support of classical forecasting models, SK Learn ML models, and TensorFlow deep learning models.\n\n## Installation\n\n```bash\n$ pip install sforecast\n```\n\n## License\n\n`sforecast` was created by Alberto Gutierrez. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`sforecast` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
+    'long_description': '# sforecast\n\nA framework for running forecasting models within a sliding (expanding) window out-of-sample fit (train/test) and prediction (forecasts). The package includes support of classical forecasting models, SK Learn ML models, and TensorFlow deep learning models.\n\n- https://sforecast.readthedocs.io/en/latest/\n\n## Installation\n\n```bash\n$ pip install sforecast\n```\n\n## License\n\n`sforecast` was created by Alberto Gutierrez. It is licensed under the terms of the MIT license.\n\n## Credits\n\n`sforecast` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Alberto Gutierrez',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.9',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `sforecast-0.4.4/PKG-INFO` & `sforecast-0.5.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: sforecast
-Version: 0.4.4
+Version: 0.5.8
 Summary: A framework for running forecasting models within a sliding/expanding window out-of-sample forecast fit (train/test) and prediction (forecasts). The package includes support of classical forecasting models, SK Learn supervised learning ML models, and TensorFlow deep learning models.
 License: MIT
 Author: Alberto Gutierrez
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulplots (>=0.2.6)
 Requires-Dist: pandas (>=1.4.0)
 Requires-Dist: pmdarima (>=1.8.0)
-Requires-Dist: sklearn (>=0.0)
+Requires-Dist: scikit-learn (>=1.4.2)
 Requires-Dist: statsmodels (>=0.13.2)
 Requires-Dist: tensorflow (>=2.7.0)
+Requires-Dist: xgboost (>=2.0.3)
 Description-Content-Type: text/markdown
 
 # sforecast
 
 A framework for running forecasting models within a sliding (expanding) window out-of-sample fit (train/test) and prediction (forecasts). The package includes support of classical forecasting models, SK Learn ML models, and TensorFlow deep learning models.
 
+- https://sforecast.readthedocs.io/en/latest/
+
 ## Installation
 
 ```bash
 $ pip install sforecast
 ```
 
 ## License
```

