# Comparing `tmp/xlcompose-0.3.1.tar.gz` & `tmp/xlcompose-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlcompose-0.3.1.tar", last modified: Sat Dec  4 20:58:33 2021, max compression
+gzip compressed data, was "xlcompose-0.3.2.tar", last modified: Sat May 25 00:21:23 2024, max compression
```

## Comparing `xlcompose-0.3.1.tar` & `xlcompose-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-04 20:58:33.575005 xlcompose-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-12-04 20:58:25.000000 xlcompose-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-12-04 20:58:25.000000 xlcompose-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-12-04 20:58:33.571005 xlcompose-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3601 2021-12-04 20:58:25.000000 xlcompose-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-12-04 20:58:25.000000 xlcompose-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-04 20:58:33.575005 xlcompose-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-12-04 20:58:25.000000 xlcompose-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-04 20:58:33.571005 xlcompose-0.3.1/xlcompose/
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-12-04 20:58:25.000000 xlcompose-0.3.1/xlcompose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35370 2021-12-04 20:58:25.000000 xlcompose-0.3.1/xlcompose/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2021-12-04 20:58:25.000000 xlcompose-0.3.1/xlcompose/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2021-12-04 20:58:25.000000 xlcompose-0.3.1/xlcompose/styles.css
--rw-r--r--   0 runner    (1001) docker     (121)     4632 2021-12-04 20:58:25.000000 xlcompose-0.3.1/xlcompose/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-12-04 20:58:25.000000 xlcompose-0.3.1/xlcompose/test_xlc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-04 20:58:33.571005 xlcompose-0.3.1/xlcompose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      375 2021-12-04 20:58:33.000000 xlcompose-0.3.1/xlcompose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      349 2021-12-04 20:58:33.000000 xlcompose-0.3.1/xlcompose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-04 20:58:33.000000 xlcompose-0.3.1/xlcompose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-12-04 20:58:33.000000 xlcompose-0.3.1/xlcompose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-04 20:58:33.000000 xlcompose-0.3.1/xlcompose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:21:23.375458 xlcompose-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-25 00:21:09.000000 xlcompose-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-25 00:21:09.000000 xlcompose-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-25 00:21:23.375458 xlcompose-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-25 00:21:09.000000 xlcompose-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-25 00:21:09.000000 xlcompose-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 00:21:23.375458 xlcompose-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-25 00:21:09.000000 xlcompose-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:21:23.375458 xlcompose-0.3.2/xlcompose/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-25 00:21:09.000000 xlcompose-0.3.2/xlcompose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35414 2024-05-25 00:21:09.000000 xlcompose-0.3.2/xlcompose/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-25 00:21:09.000000 xlcompose-0.3.2/xlcompose/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-25 00:21:09.000000 xlcompose-0.3.2/xlcompose/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-25 00:21:09.000000 xlcompose-0.3.2/xlcompose/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-25 00:21:09.000000 xlcompose-0.3.2/xlcompose/test_xlc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 00:21:23.375458 xlcompose-0.3.2/xlcompose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-25 00:21:23.000000 xlcompose-0.3.2/xlcompose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-25 00:21:23.000000 xlcompose-0.3.2/xlcompose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 00:21:23.000000 xlcompose-0.3.2/xlcompose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-25 00:21:23.000000 xlcompose-0.3.2/xlcompose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 00:21:23.000000 xlcompose-0.3.2/xlcompose.egg-info/top_level.txt
```

### Comparing `xlcompose-0.3.1/LICENSE` & `xlcompose-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xlcompose-0.3.1/README.md` & `xlcompose-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `xlcompose-0.3.1/setup.py` & `xlcompose-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('requirements.txt', 'r') as f:
     dependencies = f.read().splitlines()
 
 descr = "A declarative API for composing spreadsheets from python"
 name = 'xlcompose'
 url = 'https://github.com/jbogaardt/xlcompose'
-version='0.3.1' # Put this in __init__.py
+version='0.3.2' # Put this in __init__.py
 
 data_path = ''
 setup(
     name=name,
     version=version,
     maintainer='John Bogaardt',
     maintainer_email='jbogaardt@gmail.com',
```

### Comparing `xlcompose-0.3.1/xlcompose/core.py` & `xlcompose-0.3.2/xlcompose/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             self.exhibits = Tabs(self.exhibits)
         if self.exhibits.__class__.__name__ != 'Tabs':
             self.exhibits = Tabs(Sheet('sheet1', self.exhibits))
         for sheet in self.exhibits:
             self._write(sheet.layout, sheet.name)
             sheet.layout.kwargs.update(sheet.kwargs)
             self._set_worksheet_properties(sheet.layout, sheet.name)
-        self.writer.save()
+        self.writer.close()
 
 
     def _write(self, exhibit, sheet, start_row=0, start_col=0):
         """
         Parameters
         ----------
         exhibit :
@@ -583,15 +583,15 @@
         '''
 
         if self.data.columns.name is not None:
             idx = self.data.index.to_frame().dtypes
             idx.index = [self.data.columns.name]
         else:
             idx = pd.Series(dtype='object')
-        cols = self.data.dtypes.append(idx)
+        cols = pd.concat((self.data.dtypes, idx), axis=0)
         self.formats = {
             k: self.base_formats.get(v, self.base_formats['object'])
             for k, v in dict(zip(cols.index, cols.values)).items()}
         if type(formats) is list:
             self.formats.update(dict(zip(self.data.columns, formats)))
         elif type(formats) is str:
             self.formats.update(dict(zip(
@@ -800,15 +800,16 @@
 
     @property
     def column_widths(self):
         if hasattr(self, '_column_widths'):
             return self._column_widths
         data = np.array(
             [item.column_widths for item in self.args
-             if item.__class__.__name__ not in ['Title']])
+             if item.__class__.__name__ not in ['Title']],
+             dtype='object')
         lens = np.array([len(i) for i in data])
         mask = np.arange(lens.max()) < lens[:,None]
         out = np.zeros(mask.shape, dtype=data.dtype)
         out[mask] = np.concatenate(data)
         return list(np.max(out, axis=0))
 
     @column_widths.setter
```

### Comparing `xlcompose-0.3.1/xlcompose/settings.yaml` & `xlcompose-0.3.2/xlcompose/settings.yaml`

 * *Files identical despite different names*

### Comparing `xlcompose-0.3.1/xlcompose/styles.css` & `xlcompose-0.3.2/xlcompose/styles.css`

 * *Files identical despite different names*

### Comparing `xlcompose-0.3.1/xlcompose/templates.py` & `xlcompose-0.3.2/xlcompose/templates.py`

 * *Files identical despite different names*

