# Comparing `tmp/pg_sync_roles-0.0.8.tar.gz` & `tmp/pg_sync_roles-0.0.9.tar.gz`

## Comparing `pg_sync_roles-0.0.8.tar` & `pg_sync_roles-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/pg_sync_roles.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/LICENSE
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/README.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.9/pg_sync_roles.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.9/README.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.9/PKG-INFO
```

### Comparing `pg_sync_roles-0.0.8/.gitignore` & `pg_sync_roles-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.8/LICENSE` & `pg_sync_roles-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.8/README.md` & `pg_sync_roles-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -79,24 +79,24 @@
         ),
     )
 ```
 
 
 ## Under the hood
 
-pg-sync-roles maintains a role per database perimission, a role per schema pemission, and and per table permission, and rather than roles being granted permissions directly on objects, membership is granted to these roles that indirectly grant permissions on objects. This means that from the object's point of view, only 1 role has any given permission. This works around the de-facto limit on the number of roles that can have permission to any object.
+pg-sync-roles maintains a role per database perimission, a role per schema pemission, and a role per table permission. Rather than roles being granted permissions directly on objects, membership is granted to these roles that indirectly grant permissions on objects. This means that from the object's point of view, only 1 role has any given permission. This works around the de-facto limit on the number of roles that can have permission to any object.
 
 The names of the roles maintained by pg-sync-roles begin with the prefix `_pgsr_`. Each name ends with a randomly generated unique identifier.
 
 
 ## Compatibility
 
 pg-sync-roles aims to be compatible with a wide range of Python and other dependencies:
 
 - Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
-- psycopg2 >= 2.9.2 and Psycopg 3 >= 3.1.4
+- psycopg2 >= 2.9.2 (tested on 3.9.2) and Psycopg 3 >= 3.1.4 (tested on 3.1.4)
 - SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
 - PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, and 16.0)
 
 Note that SQLAlchemy < 2 does not support Psycopg 3, and for SQLAlchemy < 2 `future=True` must be passed to its create_engine function.
 
 There are no plans to drop support for any of the above.
```

### Comparing `pg_sync_roles-0.0.8/pyproject.toml` & `pg_sync_roles-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-sync-roles"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Department for Business and Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_sync_roles-0.0.8/PKG-INFO` & `pg_sync_roles-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pg-sync-roles
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships
 Project-URL: Source, https://github.com/uktrade/pg-sync-roles
 Author-email: Department for Business and Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -107,24 +107,24 @@
         ),
     )
 ```
 
 
 ## Under the hood
 
-pg-sync-roles maintains a role per database perimission, a role per schema pemission, and and per table permission, and rather than roles being granted permissions directly on objects, membership is granted to these roles that indirectly grant permissions on objects. This means that from the object's point of view, only 1 role has any given permission. This works around the de-facto limit on the number of roles that can have permission to any object.
+pg-sync-roles maintains a role per database perimission, a role per schema pemission, and a role per table permission. Rather than roles being granted permissions directly on objects, membership is granted to these roles that indirectly grant permissions on objects. This means that from the object's point of view, only 1 role has any given permission. This works around the de-facto limit on the number of roles that can have permission to any object.
 
 The names of the roles maintained by pg-sync-roles begin with the prefix `_pgsr_`. Each name ends with a randomly generated unique identifier.
 
 
 ## Compatibility
 
 pg-sync-roles aims to be compatible with a wide range of Python and other dependencies:
 
 - Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
-- psycopg2 >= 2.9.2 and Psycopg 3 >= 3.1.4
+- psycopg2 >= 2.9.2 (tested on 3.9.2) and Psycopg 3 >= 3.1.4 (tested on 3.1.4)
 - SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
 - PostgreSQL >= 9.6 (tested on 9.6, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, and 16.0)
 
 Note that SQLAlchemy < 2 does not support Psycopg 3, and for SQLAlchemy < 2 `future=True` must be passed to its create_engine function.
 
 There are no plans to drop support for any of the above.
```

