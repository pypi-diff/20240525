# Comparing `tmp/pypomes_ldap-0.1.4.tar.gz` & `tmp/pypomes_ldap-0.1.5.tar.gz`

## Comparing `pypomes_ldap-0.1.4.tar` & `pypomes_ldap-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0  1418839 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/python_ldap-3.4.0-cp310-cp310-win_amd64.whl
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/src/pypomes_ldap/__init__.py
--rw-r--r--   0        0        0    18391 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/src/pypomes_ldap/ldap_pomes.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0  1418839 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.5/python_ldap-3.4.0-cp310-cp310-win_amd64.whl
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.5/src/pypomes_ldap/__init__.py
+-rw-r--r--   0        0        0    18239 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.5/src/pypomes_ldap/ldap_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.5/README.md
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pypomes_ldap-0.1.5/PKG-INFO
```

### Comparing `pypomes_ldap-0.1.4/python_ldap-3.4.0-cp310-cp310-win_amd64.whl` & `pypomes_ldap-0.1.5/python_ldap-3.4.0-cp310-cp310-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pypomes_ldap-0.1.4/src/pypomes_ldap/__init__.py` & `pypomes_ldap-0.1.5/src/pypomes_ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_ldap-0.1.4/src/pypomes_ldap/ldap_pomes.py` & `pypomes_ldap-0.1.5/src/pypomes_ldap/ldap_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import ldap
 import sys
-import tempfile
 from ldap import LDAPError, modlist
 from ldap.ldapobject import LDAPObject
 from pathlib import Path
 from typing import Final, TextIO
-from pypomes_core import APP_PREFIX, env_get_str, env_get_int, env_get_path, exc_format
+from pypomes_core import (
+    APP_PREFIX, TEMP_FOLDER,
+    env_get_str, env_get_int, env_get_path, exc_format
+)
 
 _val: str = env_get_str(f"{APP_PREFIX}_LDAP_BASE_DN")
 LDAP_BASE_DN: Final[str] = None if _val is None else _val.replace(":", "=")
 _val = env_get_str(f"{APP_PREFIX}_LDAP_BIND_DN")
 LDAP_BIND_DN:  Final[str] = None if _val is None else _val.replace(":", "=")
 LDAP_BIND_PWD:  Final[str] = env_get_str(f"{APP_PREFIX}_LDAP_BIND_PWD")
 LDAP_SERVER_URI:  Final[str] = env_get_str(f"{APP_PREFIX}_LDAP_SERVER_URI")
 LDAP_TIMEOUT:  Final[int] = env_get_int(f"{APP_PREFIX}_LDAP_TIMEOUT", 30)
 LDAP_TRACE_FILEPATH:  Final[Path] = env_get_path(f"{APP_PREFIX}_LDAP_TRACE_FILEPATH",
-                                                 Path(tempfile.gettempdir()) / f"{APP_PREFIX}_ldap.log")
+                                                 TEMP_FOLDER / f"{APP_PREFIX}_ldap.log")
 LDAP_TRACE_LEVEL:  Final[int] = env_get_int(f"{APP_PREFIX}_LDAP_TRACE_LEVEL", 0)
 
 
 def ldap_init(errors: list[str], server_uri: str = LDAP_SERVER_URI,
               trace_filepath: Path = LDAP_TRACE_FILEPATH, trace_level: int = LDAP_TRACE_LEVEL) -> LDAPObject:
     """
     Initialize and return the LDAP client object.
-    
+
     :param errors: incidental error messages
     :param server_uri: URI to access the LDAP server
     :param trace_filepath: path for the trace log file
     :param trace_level: level for the trace log
     :return: the LDAP client object
     """
     # initialize the return variable
@@ -61,15 +63,15 @@
     return result
 
 
 def ldap_bind(errors: list[str], ldap_client: LDAPObject,
               bind_dn: str = LDAP_BIND_DN, bind_pwd: str = LDAP_BIND_PWD) -> bool:
     """
     Bind the given LDAP client object *conn* with the LDAP server, using the *DN* credentials *bind_dn*.
-    
+
     :param errors: incidental error messages
     :param ldap_client: the LDAP client object
     :param bind_dn: DN credentials for the bind operation
     :param bind_pwd: password for the bind operation
     :return: True if the bind operation ewas successful, False otherwise
     """
     # initialize the return variable
@@ -85,15 +87,15 @@
 
     return result
 
 
 def ldap_unbind(errors: list[str], ldap_client: LDAPObject) -> None:
     """
     Unbind the given LDAP client object *conn* with the LDAP server.
-    
+
     :param errors: incidental error messages
     :param ldap_client: the LDAP client object
     """
     try:
         ldap_client.unbind_s()
         # is the log device 'stdout' ou 'stderr' ?
         # noinspection PyProtectedMember
@@ -104,30 +106,30 @@
     except Exception as e:
         errors.append(f"Error unbinding with the LDAP server: {__ldap_except_msg(e)}")
 
 
 def ldap_add_entry(errors: list[str], entry_dn: str, attrs: dict) -> None:
     """
     Add an entry to the LDAP store.
-    
+
     :param errors: incidental error messages
     :param entry_dn: the entry DN
     :param attrs: the entry attributes
     """
     # obtain the LDAP client object
     ldap_client: LDAPObject = ldap_init(errors)
 
     bound: bool = False
     # was the LDAP client object obtained ?
-    if ldap_client is not None:
+    if ldap_client:
         # yes, bind it with the LDAP server
         bound = ldap_bind(errors, ldap_client)
 
     # were there errors ?
-    if len(errors) == 0:
+    if not errors:
         # no, proceed
         ldiff: list[tuple[any, any]] = modlist.addModlist(attrs)
         try:
             ldap_client.add_s(dn=entry_dn,
                               modlist=ldiff)
         except Exception as e:
             errors.append(f"Error on the LDAP add entry operation: {__ldap_except_msg(e)}")
@@ -136,30 +138,30 @@
     if bound:
         ldap_unbind(errors, ldap_client)
 
 
 def ldap_modify_entry(errors: list[str], entry_dn: str, mod_entry: list[tuple[int, str, any]]) -> None:
     """
     Add an entry to the LDAP store.
-    
+
     :param errors: incidental error messages
     :param entry_dn: the entry DN
     :param mod_entry: the list of modified entry attributes
     """
     # obtain the LDAP client object
     conn: LDAPObject = ldap_init(errors)
 
     bound: bool = False
     # was the LDAP client object obtained ?
-    if conn is not None:
+    if conn:
         # yes, bind it with the LDAP server
         bound = ldap_bind(errors, conn)
 
     # were there errors ?
-    if len(errors) == 0:
+    if not errors:
         # no, proceed
         try:
             conn.modify_s(dn=entry_dn,
                           modlist=mod_entry)
         except Exception as e:
             errors.append(f"Error on the LDAP modify entry operation: {__ldap_except_msg(e)}")
 
@@ -167,114 +169,115 @@
     if bound:
         ldap_unbind(errors, conn)
 
 
 def ldap_delete_entry(errors: list[str], entry_dn: str) -> None:
     """
     Remove an entry to the LDAP store.
-    
+
     :param errors: incidental error messages
     :param entry_dn: the entry DN
     """
     # obtain the LDAP client object
     conn: LDAPObject = ldap_init(errors)
 
     bound: bool = False
     # was the LDAP client object obtained ?
-    if conn is not None:
+    if conn:
         # yes, bind it with the LDAP server
         bound = ldap_bind(errors, conn)
 
     # were there errors ?
-    if len(errors) == 0:
+    if not errors:
         # no, proceed
         try:
             conn.delete_s(dn=entry_dn)
         except Exception as e:
             errors.append(f"Error on the LDAP delete entry operation: {__ldap_except_msg(e)}")
 
     # unbind the LDAP client, if applicable
     if bound:
         ldap_unbind(errors, conn)
 
 
 def ldap_modify_user(errors: list[str], user_id: str, attrs: list[tuple[str, bytes | None]]) -> None:
     """
     Modify a user entry at the LDAP store.
-    
+
     :param errors: incidental error messages
     :param user_id: id of the user
     :param attrs: the list of modified attributes
     """
     # invoke the search operation
     search_data: list[tuple[str, dict]] = ldap_search(errors, f"cn=users,{LDAP_BASE_DN}",
                                                       [attr[0] for attr in attrs],
                                                       ldap.SCOPE_ONELEVEL, f"cn={user_id}")
 
     # did the search operation returned data ?
-    if search_data is None or len(search_data) == 0:
+    if not search_data:  # search_data is None or len(search_data) == 0
         # no, report the error
         errors.append(f"Error on the LDAP modify user operation: User '{user_id}' not found")
 
     # were there errors ?
-    if len(errors) == 0:
+    if not errors:
         # no, proceed
         entry_dn: str = search_data[0][0]
 
         # build the modification list
         mod_entries: list[tuple[int, str, bytes | None]] = []
         for attr_name, new_value in attrs:
             entry_list: list[bytes] = search_data[0][1].get(attr_name)
-            if new_value is not None:
+            if new_value:
                 curr_value: bytes = None if entry_list is None else entry_list[0]
                 # assert whether the old and new values are equal
                 if new_value != curr_value:
                     # define the modification mode
                     if curr_value is None:
                         mode: int = ldap.MOD_ADD
                     else:
                         mode: int = ldap.MOD_REPLACE
                     mod_entries.append((mode, attr_name, new_value))
-            elif entry_list is not None:
+            elif entry_list:
                 mod_entries.append((ldap.MOD_DELETE, attr_name, None))
 
         # are there attributes to be modified ?
         if len(mod_entries) > 0:
             # yes, modify them
             ldap_modify_entry(errors, entry_dn, mod_entries)
 
 
 def ldap_change_pwd(errors: list[str], user_dn: str, new_pwd: str, curr_pwd: str | None = None) -> str:
     """
     Modify a user password at the LDAP store.
-    
+
     :param errors: incidental error messages
     :param user_dn: the user's DN credentials
     :param new_pwd: the new password
     :param curr_pwd: optional current password
     """
     # initialize the return variable
     result: str | None = None
 
     # obtain the LDAP client object
     ldap_client: LDAPObject = ldap_init(errors)
 
     bound: bool = False
     # bind the LDAP client with the LDAP server, if obtained
-    if ldap_client is not None:
+    if ldap_client:
         # was the password provided ?
-        if curr_pwd is None:
-            # no, perform the standard bind
-            bound = ldap_bind(errors, ldap_client)
-        else:
+        if curr_pwd:
             # yes, perform the bind with the DN provided
             bound = ldap_bind(errors, ldap_client, user_dn, curr_pwd)
+        else:
+            # no, perform the standard bind
+            bound = ldap_bind(errors, ldap_client)
 
     # were there errors ?
-    if len(errors) == 0:
+    if not errors:
+        # no, proceed
         try:
             # is the connection safe ?
             if __is_secure(ldap_client):
                 # yes, use the directive 'passwd_s'
                 resp: tuple[None, bytes] = ldap_client.passwd_s(user=user_dn,
                                                                 oldpw=curr_pwd,
                                                                 newpw=new_pwd,
@@ -312,20 +315,20 @@
     result:  list[tuple[str, dict]] | None = None
 
     # obtain the LDAP client object
     conn: LDAPObject = ldap_init(errors)
 
     bound: bool = False
     # was the LDAP client object obtained ?
-    if conn is not None:
+    if conn:
         # yes, bind it with the LDAP server
         bound = ldap_bind(errors, conn)
 
     # were there errors ?
-    if len(errors) == 0:
+    if not errors:
         # no, proceed (if 'attrs_only' is specified, the values for the attributes are not returned)
         attr_vals: int = 1 if attrs_only else 0
         try:
             # perform the search operation
             result = conn.search_s(base=base_dn,
                                    scope=scope or ldap.SCOPE_BASE,
                                    filterstr=filter_str or "(objectClass=*)",
@@ -380,15 +383,15 @@
     :param value: value to add to the target attribute
     :return: the target attribute's value
     """
     # obtain the target attribute's current value
     curr_value: bytes = ldap_get_value(errors, entry_dn, attr)
 
     # were there errors ?
-    if len(errors) == 0:
+    if not errors:
         # no, determine the modification mode
         mode: int | None = None
         if curr_value is None:
             if value is not None:
                 mode = ldap.MOD_ADD
         elif value is None:
             mode = ldap.MOD_DELETE
@@ -422,49 +425,49 @@
         # yes, proceed
         user_data: dict = search_data[0][1]
         result = user_data.get(attr)
 
     return result
 
 
-def ldap_get_values(errors: list[str], entry_dn: str, attrs: list[str]) -> tuple[bytes]:
+def ldap_get_values(errors: list[str], entry_dn: str, attrs: list[str]) -> tuple[bytes,...]:
     """
     Retrieve and return the values of attributes *attrs* in the LDAP store.
 
     :param errors: incidental error messages
     :param entry_dn: the DN of the target entry
     :param attrs: the list of target attributes
     :return: the values for the target attributes
     """
     # initialize the return variable
-    result: tuple[bytes] | None = None
+    result: tuple[bytes,...] | None = None
 
     # perform the search operation
-    search_data: tuple[list[bytes | None] | None] = ldap_get_values_lists(errors, entry_dn, attrs)
+    search_data: tuple = ldap_get_values_lists(errors, entry_dn, attrs)
 
     # did the search operation return data ?
     if isinstance(search_data, tuple):
         # yes, proceed
         search_items: list[bytes] = [item if item is None else item[0] for item in search_data]
         result = tuple(search_items)
 
     return result
 
 
-def ldap_get_values_lists(errors: list[str], entry_dn: str, attrs: list[str]) -> tuple[list[bytes]]:
+def ldap_get_values_lists(errors: list[str], entry_dn: str, attrs: list[str]) -> tuple[list[bytes],...]:
     """
     Retrieve and return the lists of values of attributes *attrs* in the LDAP store.
 
     :param errors: incidental error messages
     :param entry_dn: the DN of the target entry
     :param attrs: the list of target attributes
     :return: the target attributes' lists of values
     """
     # initialize the return variable
-    result: tuple[list[bytes]] | None = None
+    result: tuple[list[bytes],...] | None = None
 
     # perform the search operation
     search_data: list[tuple[str, dict]] = ldap_search(errors, entry_dn, attrs)
 
     # did the search operation return data ?
     if isinstance(search_data, list) and len(search_data) > 0:
         # yes, proceed
@@ -486,13 +489,13 @@
 
     if isinstance(exc, LDAPError):
         err_data: any = exc.args[0]
         # type(exc) -> <class '<nome-da-classe'>
         cls: str = f"{type(exc)}"[8:-2]
         result: str = f"'Type: {cls}; Code: {err_data.get('result')}; Msg: {err_data.get('desc')}'"
         info: str = err_data.get("info")
-        if info is not None:
+        if info:
             result = f"{result[:-1]}; Info: {info}'"
     else:
         result: str = exc_format(exc, sys.exc_info())
 
     return result
```

### Comparing `pypomes_ldap-0.1.4/LICENSE` & `pypomes_ldap-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_ldap-0.1.4/pyproject.toml` & `pypomes_ldap-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = [
-    "hatchling"
+    "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_ldap"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (LDAP module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "pip>=23.1.2",
-    "pypomes_core>=0.2.3",
+    "pypomes_core>=1.0.7",
     "python-ldap>=3.4.0",
     "setuptools>=68.0.0",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-LDAP"
```

### Comparing `pypomes_ldap-0.1.4/PKG-INFO` & `pypomes_ldap-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pypomes_ldap
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of Python pomes, pennyeach (LDAP module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-LDAP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-LDAP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=23.1.2
-Requires-Dist: pypomes-core>=0.2.3
+Requires-Dist: pypomes-core>=1.0.7
 Requires-Dist: python-ldap>=3.4.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
```

