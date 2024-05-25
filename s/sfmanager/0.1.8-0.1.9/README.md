# Comparing `tmp/sfmanager-0.1.8.tar.gz` & `tmp/sfmanager-0.1.9.tar.gz`

## Comparing `sfmanager-0.1.8.tar` & `sfmanager-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 sfmanager-0.1.8/update
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 sfmanager-0.1.8/version
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.8/sfmanager/__init__.py
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 sfmanager-0.1.8/sfmanager/app.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 sfmanager-0.1.8/sfmanager/utils.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.8/LICENSE
--rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 sfmanager-0.1.8/README.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 sfmanager-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 sfmanager-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 sfmanager-0.1.9/update
+-rwxr-xr-x   0        0        0        5 2020-02-02 00:00:00.000000 sfmanager-0.1.9/version
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.9/sfmanager/__init__.py
+-rwxr-xr-x   0        0        0     7736 2020-02-02 00:00:00.000000 sfmanager-0.1.9/sfmanager/app.py
+-rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 sfmanager-0.1.9/sfmanager/utils.py
+-rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.9/.gitignore
+-rwxr-xr-x   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.9/LICENSE
+-rwxr-xr-x   0        0        0     5560 2020-02-02 00:00:00.000000 sfmanager-0.1.9/README.md
+-rwxr-xr-x   0        0        0      750 2020-02-02 00:00:00.000000 sfmanager-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6209 2020-02-02 00:00:00.000000 sfmanager-0.1.9/PKG-INFO
```

### Comparing `sfmanager-0.1.8/sfmanager/app.py` & `sfmanager-0.1.9/sfmanager/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,17 +242,17 @@
 	# Funcs for general work with files
 
 	# Create line
 
 	def create(self, dst, use_wd=True):
 		if self.level >= 2:
 			if use_wd == True and "/" in self._dir:
-				f = open(f"{self._dir}{dst}")
+				f = open(f"{self._dir}{dst}", "w")
 			else:
-				f = open(f"{dst}", "a")
+				f = open(f"{dst}", "w")
 			f.close()
 		else:
 			print(f"Low access level! {self.level}, but need 2")
 
 	# Rename file(from self.filename to name)
 
 	def rename(self, dst, name, use_wd=True):
@@ -311,8 +311,8 @@
 
 	# Set work directory (cd)
 
 	def cd(self, _dir):
 		if "/" in _dir:
 			self._dir = _dir
 		else:
-			print("Error! It's not directory!")
+			print("Error! It's not directory!")
```

### Comparing `sfmanager-0.1.8/sfmanager/utils.py` & `sfmanager-0.1.9/sfmanager/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,31 +35,34 @@
 		print(f"Whats new in v{v}?")
 		print(updates.text[0:])
 	print("Homepage on github: https://github.com/GrandTheBest/sfmanager")
 	print("Issues page on github: https://github.com/GrandTheBest/sfmanager/issues")
 	print("Documentation: https://github.com/GrandTheBest/sfmanager/blob/main/README.md")
 
 @logger.catch
-def checkUpdates():
-	logger.info("Checking for updates")
+def checkUpdates(no_updates="U"):
+	if no_updates == "N"
+		whatIsIt()
+	else:
+		logger.info("Checking for updates")
+
+		installed_v = pkg_resources.get_distribution("sfmanager").version
+		v = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/version")
+		updates = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/update")
+
+		if v.status_code == 200:
+			value_v = v.text[0:5]
+
+			if str(installed_v) == str(value_v):
+				logger.success("No update required")
+				whatIsIt()
+			else:
+				logger.info("Downloading an update using pip")
+
+				subprocess.check_call([sys.executable, "-m", "pip", "install", "sfmanager==" + value_v])
+				logger.success("sfmanager updated, changes will take effect after restart")
+
+				if updates.status_code == 200:
+					print(f"Whats new in v{value_v}?")
+					print(updates.text[0:])
 
-	installed_v = pkg_resources.get_distribution("sfmanager").version
-	v = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/version")
-	updates = httpx.get("https://raw.githubusercontent.com/GrandTheBest/sfmanager/main/update")
-
-	if v.status_code == 200:
-		value_v = v.text[0:5]
-
-		if str(installed_v) == str(value_v):
-			logger.success("No update required")
-			whatIsIt()
-		else:
-			logger.info("Downloading an update using pip")
-
-			subprocess.check_call([sys.executable, "-m", "pip", "install", "sfmanager==" + value_v])
-			logger.success("sfmanager updated, changes will take effect after restart")
-
-			if updates.status_code == 200:
-				print(f"Whats new in v{value_v}?")
-				print(updates.text[0:])
-
-			os.chdir(os.path.join(pkg_resources.get_distribution("sfmanager").location, "sfmanager"))
+				os.chdir(os.path.join(pkg_resources.get_distribution("sfmanager").location, "sfmanager"))
```

### Comparing `sfmanager-0.1.8/.gitignore` & `sfmanager-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.8/LICENSE` & `sfmanager-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.8/README.md` & `sfmanager-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.8/pyproject.toml` & `sfmanager-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "sfmanager"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
 	{name="GrandTheBest", email="grandinfo-cm@gmail.com"},
 ]
 description = "This library is not that useful. Perhaps someday it will become great."
 readme = "README.md"
 requires-python = ">=3.10.0"
 dependencies = [
```

### Comparing `sfmanager-0.1.8/PKG-INFO` & `sfmanager-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sfmanager
-Version: 0.1.8
+Version: 0.1.9
 Summary: This library is not that useful. Perhaps someday it will become great.
 Project-URL: Homepage, https://github.com/GrandTheBest/sfmanager
 Project-URL: Issues, https://github.com/GrandTheBest/sfmanager/issues
 Author-email: GrandTheBest <grandinfo-cm@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

