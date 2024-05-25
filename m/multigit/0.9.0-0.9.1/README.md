# Comparing `tmp/multigit-0.9.0.tar.gz` & `tmp/multigit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jmnav/REPOS/python-multigit/src/dist/tmpcptshjym/multigit-0.9.0.tar", last modified: Tue Sep 14 10:12:22 2021, max compression
+gzip compressed data, was "/home/jmnav/REPOS/python-multigit/src/dist/tmpa636zt8k/multigit-0.9.1.tar", last modified: Thu Sep 16 07:33:10 2021, max compression
```

## Comparing `multigit-0.9.0.tar` & `multigit-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jmnav     (1000) jmnav     (1000)        0 2021-09-14 10:12:22.000000 multigit-0.9.0/
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)    35149 2021-08-03 13:17:14.000000 multigit-0.9.0/LICENSE
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)       54 2021-08-11 14:27:27.000000 multigit-0.9.0/MANIFEST.in
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)     1297 2021-09-14 10:12:22.000000 multigit-0.9.0/PKG-INFO
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)      581 2021-08-11 14:27:27.000000 multigit-0.9.0/README.md
-drwxr-xr-x   0 jmnav     (1000) jmnav     (1000)        0 2021-09-14 10:12:22.000000 multigit-0.9.0/multigit/
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)     1916 2021-09-14 10:11:22.000000 multigit-0.9.0/multigit/__init__.py
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)       81 2021-08-05 15:34:59.000000 multigit-0.9.0/multigit/__main__.py
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)    12378 2021-09-14 10:11:22.000000 multigit-0.9.0/multigit/subrepos.py
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)      894 2021-08-11 14:27:27.000000 multigit-0.9.0/multigit/subrepos_schema.yaml
-drwxr-xr-x   0 jmnav     (1000) jmnav     (1000)        0 2021-09-14 10:12:22.000000 multigit-0.9.0/multigit.egg-info/
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)     1297 2021-09-14 10:12:22.000000 multigit-0.9.0/multigit.egg-info/PKG-INFO
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)      341 2021-09-14 10:12:22.000000 multigit-0.9.0/multigit.egg-info/SOURCES.txt
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)        1 2021-09-14 10:12:22.000000 multigit-0.9.0/multigit.egg-info/dependency_links.txt
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)       44 2021-09-14 10:12:22.000000 multigit-0.9.0/multigit.egg-info/entry_points.txt
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)       64 2021-09-14 10:12:22.000000 multigit-0.9.0/multigit.egg-info/requires.txt
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)        9 2021-09-14 10:12:22.000000 multigit-0.9.0/multigit.egg-info/top_level.txt
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)       90 2021-08-05 15:34:59.000000 multigit-0.9.0/pyproject.toml
--rw-r--r--   0 jmnav     (1000) jmnav     (1000)      942 2021-09-14 10:12:22.000000 multigit-0.9.0/setup.cfg
+drwxr-xr-x   0 jmnav     (1000) jmnav     (1000)        0 2021-09-16 07:33:10.000000 multigit-0.9.1/
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)    35149 2021-08-03 13:17:14.000000 multigit-0.9.1/LICENSE
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)       54 2021-08-11 14:27:27.000000 multigit-0.9.1/MANIFEST.in
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)     1297 2021-09-16 07:33:10.000000 multigit-0.9.1/PKG-INFO
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)      581 2021-08-11 14:27:27.000000 multigit-0.9.1/README.md
+drwxr-xr-x   0 jmnav     (1000) jmnav     (1000)        0 2021-09-16 07:33:10.000000 multigit-0.9.1/multigit/
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)     1916 2021-09-16 07:32:04.000000 multigit-0.9.1/multigit/__init__.py
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)       81 2021-08-05 15:34:59.000000 multigit-0.9.1/multigit/__main__.py
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)    13099 2021-09-16 07:30:48.000000 multigit-0.9.1/multigit/subrepos.py
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)      894 2021-08-11 14:27:27.000000 multigit-0.9.1/multigit/subrepos_schema.yaml
+drwxr-xr-x   0 jmnav     (1000) jmnav     (1000)        0 2021-09-16 07:33:10.000000 multigit-0.9.1/multigit.egg-info/
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)     1297 2021-09-16 07:33:10.000000 multigit-0.9.1/multigit.egg-info/PKG-INFO
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)      341 2021-09-16 07:33:10.000000 multigit-0.9.1/multigit.egg-info/SOURCES.txt
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)        1 2021-09-16 07:33:10.000000 multigit-0.9.1/multigit.egg-info/dependency_links.txt
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)       44 2021-09-16 07:33:10.000000 multigit-0.9.1/multigit.egg-info/entry_points.txt
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)       64 2021-09-16 07:33:10.000000 multigit-0.9.1/multigit.egg-info/requires.txt
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)        9 2021-09-16 07:33:10.000000 multigit-0.9.1/multigit.egg-info/top_level.txt
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)       90 2021-08-05 15:34:59.000000 multigit-0.9.1/pyproject.toml
+-rw-r--r--   0 jmnav     (1000) jmnav     (1000)      942 2021-09-16 07:33:10.000000 multigit-0.9.1/setup.cfg
```

### Comparing `multigit-0.9.0/LICENSE` & `multigit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multigit-0.9.0/PKG-INFO` & `multigit-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multigit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Manages git repos within git repos.
 Home-page: https://github.com/jmnavarrol/python-multigit
 Author: Jesús M. Navarro
 Author-email: "Jesús M. Navarro" <jesusmnavarrolopez@gmail.com>
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jmnavarrol/python-multigit/issues
 Platform: UNKNOWN
```

### Comparing `multigit-0.9.0/README.md` & `multigit-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `multigit-0.9.0/multigit/__init__.py` & `multigit-0.9.1/multigit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 :package: multigit |release|
 :author: `Jesús M. Navarro <mailto:jesusmnavarrolopez@gmail.com>`_
 :license: `GNU General Public License v3.0 <https://github.com/jmnavarrol/python-multigit/blob/main/LICENSE>`_
 :source: https://github.com/jmnavarrol/python-multigit
 """
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 # Import stuff
 import os, sys
 import argparse
 
 # "local" imports
 from .subrepos import Subrepos, SUBREPOS_FILE
```

### Comparing `multigit-0.9.0/multigit/subrepos.py` & `multigit-0.9.1/multigit/subrepos.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,23 +176,27 @@
 				sys.exit(errno.EINVAL)
 		else:
 			subrepo_list = None
 			
 		return subrepo_list
 		
 		
+	# TODO: Refactor this method, most possibly "breaking it" into steps:
+	# 1. clone
+	# 2. fetch (if no previous error)
+	# 3. update (if no previous error and gitref mismatch)
 	def __process_subrepo(self, subrepo, report_only=True):
 		'''
 		Operates the requested subrepo.
 		
 		:param dict subrepo:  a dictionary in the form returned by __load_subrepos_file()
 		:param bool report_only: when True, only reviews subrepo's current status.  When False, tries to honor the requested values of *subrepo*.
 		:return dict: an "enhanced" subrepo dict reporting its status.  It will add the following keys:
 		
-			* **subrepo['status']:** one of *'NOT_CLONED'*, *'CLONED'*, *'UPDATED'*, *'PENDING_UPDATE'*, *'DIRTY'* or *'UP_TO_DATE'*.
+			* **subrepo['status']:** one of *'ERROR'*, *'NOT_CLONED'*, *'CLONED'*, *'UPDATED'*, *'PENDING_UPDATE'*, *'DIRTY'* or *'UP_TO_DATE'*.
 		'''
 		
 		# find or clone given subrepo
 		try:
 			repo = Repo(subrepo['path'])
 		except git_exception.NoSuchPathError as e:
 			# repo not yet cloned
@@ -229,67 +233,83 @@
 			# desired_gitref: what's requested? a tag, a branch, a commit...
 			# desired_commit: the "topmost" commit on the desired_gitref
 			# since I "converted" the desired_gitref into a commit,
 			# I can just compare sandbox' current commit with the desired one to know if there're pending updates
 			
 			local_commit = repo.commit().hexsha
 			# grab details about remote updates (if any)
-			repo.remotes.origin.fetch()
+			try:
+				repo.remotes.origin.fetch()
+			except git_exception.GitCommandError as e:
+				if (
+					e.status == 128
+					and 'Could not read from remote repository' in e.stderr
+				):
+					subrepo['status'] = 'ERROR'
+					subrepo['extra_info'] = e.stderr.replace('stderr: ','').strip('\n').strip()
+				else:
+					print(Style.BRIGHT + Fore.RED + "ERROR:", end=' ')
+					print(Style.BRIGHT + e.stderr.strip('\n'))
+					sys.exit(errno.EBADE)
 		
 			# Find the "new" topmost commit
-			if subrepo['gitref_type']:
-				gitref_type = subrepo['gitref_type']
-				
-				desired_gitref = subrepo[gitref_type]
-				
-				if gitref_type == 'branch':
-					remote_ref = str('origin/' + subrepo[gitref_type])
+			if (
+				not 'status' in subrepo
+				or subrepo['status'] != 'ERROR'
+			):
+				if subrepo['gitref_type']:
+					gitref_type = subrepo['gitref_type']
+					
+					desired_gitref = subrepo[gitref_type]
+					
+					if gitref_type == 'branch':
+						remote_ref = str('origin/' + subrepo[gitref_type])
+					else:
+						remote_ref = str(subrepo[gitref_type])
+					
+					try:
+						desired_commit = str(repo.commit(remote_ref))
+					except git_exception.BadName as e:
+						print(Style.BRIGHT + Fore.RED + "ERROR:", end=' ')
+						print("Repo " + Style.BRIGHT + "'" + subrepo['repo'] + "'")
+						print("\tCloned at: " + Style.BRIGHT + "'" + subrepo['path'] + "'")
+						print("\tNo such " + gitref_type + ": " + Style.BRIGHT + "'" + subrepo[gitref_type] + "'", end=': ')
+						print(e)
+						sys.exit(errno.ENOENT)
 				else:
-					remote_ref = str(subrepo[gitref_type])
-				
-				try:
-					desired_commit = str(repo.commit(remote_ref))
-				except git_exception.BadName as e:
-					print(Style.BRIGHT + Fore.RED + "ERROR:", end=' ')
-					print("Repo " + Style.BRIGHT + "'" + subrepo['repo'] + "'")
-					print("\tCloned at: " + Style.BRIGHT + "'" + subrepo['path'] + "'")
-					print("\tNo such " + gitref_type + ": " + Style.BRIGHT + "'" + subrepo[gitref_type] + "'", end=': ')
-					print(e)
-					sys.exit(errno.ENOENT)
-			else:
-				desired_commit = repo.remotes.origin.refs.HEAD.commit.hexsha
-				desired_gitref = repo.git.symbolic_ref('refs/remotes/origin/HEAD').replace('refs/remotes/origin/','')
-				
-			# The sandbox update itself
-			if local_commit != desired_commit:
-				subrepo['from'] = local_commit
-				subrepo['to'] = desired_commit
-				
-				if not repo.is_dirty():
-					if not report_only:
-						try:
-							repo.git.checkout(desired_gitref)
-						except git_exception.GitCommandError as e:
-							print(Style.BRIGHT + Fore.RED + "ERROR:", end=' ')
-							print(Style.BRIGHT + "'" + subrepo['repo'] + "'")
-							print("\tat " + Style.BRIGHT + "'" + subrepo['path'] + "'")
-							print(Style.BRIGHT + "\t" + e.stderr.strip())
-							sys.exit(errno.EBADE)
-							
-						if not repo.head.is_detached:
-							repo.git.pull()
-							
-						subrepo['status'] = 'UPDATED'
+					desired_commit = repo.remotes.origin.refs.HEAD.commit.hexsha
+					desired_gitref = repo.git.symbolic_ref('refs/remotes/origin/HEAD').replace('refs/remotes/origin/','')
+					
+				# The sandbox update itself
+				if local_commit != desired_commit:
+					subrepo['from'] = local_commit
+					subrepo['to'] = desired_commit
+					
+					if not repo.is_dirty():
+						if not report_only:
+							try:
+								repo.git.checkout(desired_gitref)
+							except git_exception.GitCommandError as e:
+								print(Style.BRIGHT + Fore.RED + "ERROR:", end=' ')
+								print(Style.BRIGHT + "'" + subrepo['repo'] + "'")
+								print("\tat " + Style.BRIGHT + "'" + subrepo['path'] + "'")
+								print(Style.BRIGHT + "\t" + e.stderr.strip())
+								sys.exit(errno.EBADE)
+								
+							if not repo.head.is_detached:
+								repo.git.pull()
+								
+							subrepo['status'] = 'UPDATED'
+						else:
+							subrepo['status'] = 'PENDING_UPDATE'
 					else:
-						subrepo['status'] = 'PENDING_UPDATE'
+						subrepo['status'] = 'DIRTY'
 				else:
-					subrepo['status'] = 'DIRTY'
-			else:
-				subrepo['status'] = 'UP_TO_DATE'
-				
+					subrepo['status'] = 'UP_TO_DATE'
+					
 		return subrepo
 		
 		
 	def __print_subrepo_status(self, subrepo):
 		'''prints a report on the repo info provided as param.
 		
 		:param dict subrepo: a dictionary in the enhanced form returned by __process_subrepo()
```

### Comparing `multigit-0.9.0/multigit/subrepos_schema.yaml` & `multigit-0.9.1/multigit/subrepos_schema.yaml`

 * *Files identical despite different names*

### Comparing `multigit-0.9.0/multigit.egg-info/PKG-INFO` & `multigit-0.9.1/multigit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multigit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Manages git repos within git repos.
 Home-page: https://github.com/jmnavarrol/python-multigit
 Author: Jesús M. Navarro
 Author-email: "Jesús M. Navarro" <jesusmnavarrolopez@gmail.com>
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jmnavarrol/python-multigit/issues
 Platform: UNKNOWN
```

### Comparing `multigit-0.9.0/setup.cfg` & `multigit-0.9.1/setup.cfg`

 * *Files identical despite different names*

