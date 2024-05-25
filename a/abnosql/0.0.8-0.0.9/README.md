# Comparing `tmp/abnosql-0.0.8.tar.gz` & `tmp/abnosql-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abnosql-0.0.8.tar", last modified: Thu Aug 24 15:08:30 2023, max compression
+gzip compressed data, was "abnosql-0.0.9.tar", last modified: Thu Aug 31 12:15:09 2023, max compression
```

## Comparing `abnosql-0.0.8.tar` & `abnosql-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:30.622902 abnosql-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (999)     1084 2023-08-24 15:08:16.000000 abnosql-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)    19109 2023-08-24 15:08:30.622902 abnosql-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    17981 2023-08-24 15:08:16.000000 abnosql-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:30.618902 abnosql-0.0.8/abnosql/
--rw-r--r--   0 runner    (1001) docker     (999)      206 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     4128 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/cli.py
--rw-r--r--   0 runner    (1001) docker     (999)      289 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (999)     3060 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/kms.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:30.622902 abnosql-0.0.8/abnosql/mocks/
--rw-r--r--   0 runner    (1001) docker     (999)      250 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6576 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/mocks/mock_azure_kms.py
--rw-r--r--   0 runner    (1001) docker     (999)     5486 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/mocks/mock_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (999)     1761 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/mocks/mock_dynamodbx.py
--rw-r--r--   0 runner    (1001) docker     (999)     2586 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:30.622902 abnosql-0.0.8/abnosql/plugins/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:30.622902 abnosql-0.0.8/abnosql/plugins/kms/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/plugins/kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3238 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/plugins/kms/aws.py
--rw-r--r--   0 runner    (1001) docker     (999)     3899 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/plugins/kms/azure.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:30.622902 abnosql-0.0.8/abnosql/plugins/table/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/plugins/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    10951 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/plugins/table/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (999)    10201 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/plugins/table/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (999)     8889 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/plugins/table/memory.py
--rw-r--r--   0 runner    (1001) docker     (999)    16467 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/table.py
--rw-r--r--   0 runner    (1001) docker     (999)       74 2023-08-24 15:08:16.000000 abnosql-0.0.8/abnosql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 15:08:30.618902 abnosql-0.0.8/abnosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    19109 2023-08-24 15:08:30.000000 abnosql-0.0.8/abnosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      717 2023-08-24 15:08:30.000000 abnosql-0.0.8/abnosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 15:08:30.000000 abnosql-0.0.8/abnosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       44 2023-08-24 15:08:30.000000 abnosql-0.0.8/abnosql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      715 2023-08-24 15:08:30.000000 abnosql-0.0.8/abnosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-24 15:08:30.000000 abnosql-0.0.8/abnosql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      234 2023-08-24 15:08:30.622902 abnosql-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (999)     2818 2023-08-24 15:08:16.000000 abnosql-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:15:09.598323 abnosql-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (999)     1084 2023-08-31 12:14:50.000000 abnosql-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)    19465 2023-08-31 12:15:09.598323 abnosql-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)    18337 2023-08-31 12:14:50.000000 abnosql-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:15:09.594323 abnosql-0.0.9/abnosql/
+-rw-r--r--   0 runner    (1001) docker     (999)      206 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (999)     4128 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (999)      289 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3155 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/kms.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:15:09.598323 abnosql-0.0.9/abnosql/mocks/
+-rw-r--r--   0 runner    (1001) docker     (999)      250 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6576 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/mocks/mock_azure_kms.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5486 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/mocks/mock_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1761 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/mocks/mock_dynamodbx.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2604 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:15:09.598323 abnosql-0.0.9/abnosql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:15:09.598323 abnosql-0.0.9/abnosql/plugins/kms/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/plugins/kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3238 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/plugins/kms/aws.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3899 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/plugins/kms/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:15:09.598323 abnosql-0.0.9/abnosql/plugins/table/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/plugins/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10951 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/plugins/table/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10201 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/plugins/table/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8889 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/plugins/table/memory.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16563 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/table.py
+-rw-r--r--   0 runner    (1001) docker     (999)       74 2023-08-31 12:14:50.000000 abnosql-0.0.9/abnosql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-31 12:15:09.594323 abnosql-0.0.9/abnosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)    19465 2023-08-31 12:15:09.000000 abnosql-0.0.9/abnosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      717 2023-08-31 12:15:09.000000 abnosql-0.0.9/abnosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-31 12:15:09.000000 abnosql-0.0.9/abnosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       44 2023-08-31 12:15:09.000000 abnosql-0.0.9/abnosql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      715 2023-08-31 12:15:09.000000 abnosql-0.0.9/abnosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-31 12:15:09.000000 abnosql-0.0.9/abnosql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      234 2023-08-31 12:15:09.598323 abnosql-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (999)     2818 2023-08-31 12:14:50.000000 abnosql-0.0.9/setup.py
```

### Comparing `abnosql-0.0.8/LICENSE` & `abnosql-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/PKG-INFO` & `abnosql-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.8
+Version: 0.0.9
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
@@ -195,40 +195,42 @@
 
 NOTE: created* will only be added if `update` is not True in a `put_item()` operation
 
 If you prefer snake_case over CamelCase, you can set env var `ABNOSQL_CAMELCASE` = `FALSE`
 
 ## Change Feed / Stream Support
 
-**AWS DynamoDB** [Streams](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html) allow Lambda functions to be triggered upon create, update and delete table operations.  The event sent to the lambda (see [aws docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.Lambda.Tutorial2.html)) contains `eventName` and `eventSource`, where:
+**AWS DynamoDB** [Streams](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html) allow Lambda functions to be triggered upon create, update and delete table operations.  The event sent to the lambda (see [aws docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.Lambda.Tutorial2.html)) contains `eventName` and `eventSourceARN`, where:
 
-- `eventName` - name of event, eg `INSERT`, `UPDATE` or `DELETE`
-- `eventSource` - ARN of the table name
+- `eventName` - name of event, eg `INSERT`, `MODIFY` or `REMOVE` (see [here](https://docs.aws.amazon.com/amazondynamodb/latest/APIReference/API_streams_Record.html))
+- `eventSourceARN` - ARN of the table name
 
 This allows a single stream processor lambda to process events from multiple tables (eg for writing into ElasticSearch)
 
 Like DynamoDB, **Azure CosmosDB** supports [change feeds](https://learn.microsoft.com/en-us/azure/cosmos-db/change-feed), however the event sent to the function (currently) omits the event source (table name) and only delete event names are available if a [preview change feed mode](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html) is enabled, which needs explicit enablement for.
 
 Because both the eventName and eventSource are ideally needed (irrespective of preview mode or not), abnosql library automatically adds the `changeMetadata` to an item during create, update and delete, eg:
 
 ```
 item = {
     "hk": "1",
     "rk": "a",
     "changeMetadata": {
-        "eventType": "INSERT",
+        "eventName": "INSERT",
         "eventSource": "sometable"
     }
 }
 ```
 
-Because no DELETE event is sent at all without preview change feed mode above - abnosql must first update the item, and then delete it.  This is also needed for the eventSource / table name to be captured in the event, so unfortunately until Cosmos supports both attributes, update is needed before a delete
+Because no REMOVE event is sent at all without preview change feed mode above - abnosql must first update the item, and then delete it.  This is also needed for the eventSource / table name to be captured in the event, so unfortunately until Cosmos supports both attributes, update is needed before a delete
 
 This behaviour is enabled by default, however can be disabled by setting `ABNOSQL_COSMOS_CHANGE_META` env var to `FALSE` or `cosmos_change_meta=False` in table config.  `ABNOSQL_CAMELCASE` = `FALSE` env var can also be used to change attribute names used to snake_case if needed
 
+To write an Azure Function / AWS Lambda that is able to process both DynamoDB and Cosmos events, look for `changeMetadata` first and if present use that otherwise look for `eventName` and `eventSourceARN` in the event payload assuming its DynamoDB
+
 ## Client Side Encryption
 
 If configured in table config with `kms` attribute, abnosql will perform client side encryption using AWS KMS or Azure KeyVault
 
 Each attribute value defined in the config is encrypted with a 256-bit AES-GCM data key generated for each attribute value:
 
 - `aws` uses [AWS Encryption SDK for Python](https://docs.aws.amazon.com/encryption-sdk/latest/developer-guide/python.html)
```

### Comparing `abnosql-0.0.8/README.md` & `abnosql-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -159,40 +159,42 @@
 
 NOTE: created* will only be added if `update` is not True in a `put_item()` operation
 
 If you prefer snake_case over CamelCase, you can set env var `ABNOSQL_CAMELCASE` = `FALSE`
 
 ## Change Feed / Stream Support
 
-**AWS DynamoDB** [Streams](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html) allow Lambda functions to be triggered upon create, update and delete table operations.  The event sent to the lambda (see [aws docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.Lambda.Tutorial2.html)) contains `eventName` and `eventSource`, where:
+**AWS DynamoDB** [Streams](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html) allow Lambda functions to be triggered upon create, update and delete table operations.  The event sent to the lambda (see [aws docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.Lambda.Tutorial2.html)) contains `eventName` and `eventSourceARN`, where:
 
-- `eventName` - name of event, eg `INSERT`, `UPDATE` or `DELETE`
-- `eventSource` - ARN of the table name
+- `eventName` - name of event, eg `INSERT`, `MODIFY` or `REMOVE` (see [here](https://docs.aws.amazon.com/amazondynamodb/latest/APIReference/API_streams_Record.html))
+- `eventSourceARN` - ARN of the table name
 
 This allows a single stream processor lambda to process events from multiple tables (eg for writing into ElasticSearch)
 
 Like DynamoDB, **Azure CosmosDB** supports [change feeds](https://learn.microsoft.com/en-us/azure/cosmos-db/change-feed), however the event sent to the function (currently) omits the event source (table name) and only delete event names are available if a [preview change feed mode](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html) is enabled, which needs explicit enablement for.
 
 Because both the eventName and eventSource are ideally needed (irrespective of preview mode or not), abnosql library automatically adds the `changeMetadata` to an item during create, update and delete, eg:
 
 ```
 item = {
     "hk": "1",
     "rk": "a",
     "changeMetadata": {
-        "eventType": "INSERT",
+        "eventName": "INSERT",
         "eventSource": "sometable"
     }
 }
 ```
 
-Because no DELETE event is sent at all without preview change feed mode above - abnosql must first update the item, and then delete it.  This is also needed for the eventSource / table name to be captured in the event, so unfortunately until Cosmos supports both attributes, update is needed before a delete
+Because no REMOVE event is sent at all without preview change feed mode above - abnosql must first update the item, and then delete it.  This is also needed for the eventSource / table name to be captured in the event, so unfortunately until Cosmos supports both attributes, update is needed before a delete
 
 This behaviour is enabled by default, however can be disabled by setting `ABNOSQL_COSMOS_CHANGE_META` env var to `FALSE` or `cosmos_change_meta=False` in table config.  `ABNOSQL_CAMELCASE` = `FALSE` env var can also be used to change attribute names used to snake_case if needed
 
+To write an Azure Function / AWS Lambda that is able to process both DynamoDB and Cosmos events, look for `changeMetadata` first and if present use that otherwise look for `eventName` and `eventSourceARN` in the event payload assuming its DynamoDB
+
 ## Client Side Encryption
 
 If configured in table config with `kms` attribute, abnosql will perform client side encryption using AWS KMS or Azure KeyVault
 
 Each attribute value defined in the config is encrypted with a 256-bit AES-GCM data key generated for each attribute value:
 
 - `aws` uses [AWS Encryption SDK for Python](https://docs.aws.amazon.com/encryption-sdk/latest/developer-guide/python.html)
```

### Comparing `abnosql-0.0.8/abnosql/cli.py` & `abnosql-0.0.9/abnosql/cli.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/abnosql/kms.py` & `abnosql-0.0.9/abnosql/kms.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,14 +111,18 @@
 
     Returns:
         KmsBase object
 
     """
     if provider is None:
         provider = os.environ.get('ABNOSQL_KMS')
+
+    if provider is None:
+        raise ex.PluginException('kms plugin provider not defined')
+
     pm = plugin.get_pm('kms')
     module = pm.get_plugin(provider)
     if module is None:
         raise ex.PluginException(f'kms.{provider} plugin not found')
     if hasattr(module, 'MISSING_DEPS'):
         raise ex.PluginException(
             f'kms.{provider} plugin missing dependencies'
```

### Comparing `abnosql-0.0.8/abnosql/mocks/mock_azure_kms.py` & `abnosql-0.0.9/abnosql/mocks/mock_azure_kms.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/abnosql/mocks/mock_cosmos.py` & `abnosql-0.0.9/abnosql/mocks/mock_cosmos.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/abnosql/mocks/mock_dynamodbx.py` & `abnosql-0.0.9/abnosql/mocks/mock_dynamodbx.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/abnosql/plugin.py` & `abnosql-0.0.9/abnosql/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     _PMS = {}
 
 
 def get_pm(
     entity: str,
     prefix: t.Optional[str] = None,
     nocache: t.Optional[bool] = False
-) -> PM:
+) -> pluggy.PluginManager:
     """Generic pluggy loader for loading specs, hooks and plugins
 
     plugins/hooks etc loaded into {mypkg}.{entity} namespace
     default prefix = entity.title()
 
     Example structure:
```

### Comparing `abnosql-0.0.8/abnosql/plugins/kms/aws.py` & `abnosql-0.0.9/abnosql/plugins/kms/aws.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/abnosql/plugins/kms/azure.py` & `abnosql-0.0.9/abnosql/plugins/kms/azure.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/abnosql/plugins/table/cosmos.py` & `abnosql-0.0.9/abnosql/plugins/table/cosmos.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     ) -> t.Dict:
         if audit_user:
             item = add_audit(item, update or False, audit_user)
 
         # add change metadata if enabled
         if self.change_meta is True:
             item = add_change_meta(
-                item, self.name, 'UPDATE' if update is True else 'INSERT'
+                item, self.name, 'MODIFY' if update is True else 'INSERT'
             )
 
         _item = self.pm.hook.put_item_pre(table=self.name, item=item)
         if _item:
             item = _item[0]
         item = kms_encrypt_item(self.config, item)
         # do update
@@ -199,15 +199,15 @@
 
     @cosmos_ex_handler()
     def delete_item(self, **kwargs):
 
         # if change metadata enabled do update first then delete
         if self.change_meta is True:
             item = add_change_meta(
-                dict(**kwargs), self.name, 'DELETE'
+                dict(**kwargs), self.name, 'REMOVE'
             )
             self.put_item(item, update=False)
             # sleep defined number of milliseconds to allow time between
             # update then delete events if needed (if this is an issue)
             sleep_ms = int(os.environ.get(
                 'ABNOSQL_COSMOS_CHANGE_META_SLEEPMS', '0'
             ))
```

### Comparing `abnosql-0.0.8/abnosql/plugins/table/dynamodb.py` & `abnosql-0.0.9/abnosql/plugins/table/dynamodb.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/abnosql/plugins/table/memory.py` & `abnosql-0.0.9/abnosql/plugins/table/memory.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/abnosql/table.py` & `abnosql-0.0.9/abnosql/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,22 +510,22 @@
 def add_change_meta(item: t.Dict, event_source: str, event_name: str) -> t.Dict:
     """Add changeMetadata object to item containing eventName and eventSource
 
     Args:
 
         item: item dict
         event_source: str
-        event_name: str - INSERT, UPDATE or DELETE
+        event_name: str - INSERT, MODIFY or REMOVE
 
     Returns:
         item
 
     """
     event_name = event_name.upper()
-    if event_name not in ['INSERT', 'UPDATE', 'DELETE']:
+    if event_name not in ['INSERT', 'MODIFY', 'REMOVE']:
         return item
     camel_case = os.environ.get('ABNOSQL_CAMELCASE', 'TRUE') == 'TRUE'
     meta_attr = 'changeMetadata' if camel_case else 'change_metadata'
     source_attr = 'eventSource' if camel_case else 'event_source'
     name_attr = 'eventName' if camel_case else 'event_name'
     item.update({
         meta_attr: {
@@ -573,14 +573,17 @@
             'FUNCTIONS_WORKER_RUNTIME': 'cosmos'
         }
         for envvar, _database in defaults.items():
             if os.environ.get(envvar) is not None:
                 database = _database
                 break
 
+    if database is None:
+        raise ex.PluginException('table plugin database not defined')
+
     pm = plugin.get_pm('table')
     module = pm.get_plugin(database)
     if module is None:
         raise ex.PluginException(f'table.{database} plugin not found')
     if hasattr(module, 'MISSING_DEPS'):
         raise ex.PluginException(
             f'table.{database} plugin missing dependencies'
```

### Comparing `abnosql-0.0.8/abnosql.egg-info/PKG-INFO` & `abnosql-0.0.9/abnosql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.8
+Version: 0.0.9
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
@@ -195,40 +195,42 @@
 
 NOTE: created* will only be added if `update` is not True in a `put_item()` operation
 
 If you prefer snake_case over CamelCase, you can set env var `ABNOSQL_CAMELCASE` = `FALSE`
 
 ## Change Feed / Stream Support
 
-**AWS DynamoDB** [Streams](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html) allow Lambda functions to be triggered upon create, update and delete table operations.  The event sent to the lambda (see [aws docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.Lambda.Tutorial2.html)) contains `eventName` and `eventSource`, where:
+**AWS DynamoDB** [Streams](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html) allow Lambda functions to be triggered upon create, update and delete table operations.  The event sent to the lambda (see [aws docs](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.Lambda.Tutorial2.html)) contains `eventName` and `eventSourceARN`, where:
 
-- `eventName` - name of event, eg `INSERT`, `UPDATE` or `DELETE`
-- `eventSource` - ARN of the table name
+- `eventName` - name of event, eg `INSERT`, `MODIFY` or `REMOVE` (see [here](https://docs.aws.amazon.com/amazondynamodb/latest/APIReference/API_streams_Record.html))
+- `eventSourceARN` - ARN of the table name
 
 This allows a single stream processor lambda to process events from multiple tables (eg for writing into ElasticSearch)
 
 Like DynamoDB, **Azure CosmosDB** supports [change feeds](https://learn.microsoft.com/en-us/azure/cosmos-db/change-feed), however the event sent to the function (currently) omits the event source (table name) and only delete event names are available if a [preview change feed mode](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.html) is enabled, which needs explicit enablement for.
 
 Because both the eventName and eventSource are ideally needed (irrespective of preview mode or not), abnosql library automatically adds the `changeMetadata` to an item during create, update and delete, eg:
 
 ```
 item = {
     "hk": "1",
     "rk": "a",
     "changeMetadata": {
-        "eventType": "INSERT",
+        "eventName": "INSERT",
         "eventSource": "sometable"
     }
 }
 ```
 
-Because no DELETE event is sent at all without preview change feed mode above - abnosql must first update the item, and then delete it.  This is also needed for the eventSource / table name to be captured in the event, so unfortunately until Cosmos supports both attributes, update is needed before a delete
+Because no REMOVE event is sent at all without preview change feed mode above - abnosql must first update the item, and then delete it.  This is also needed for the eventSource / table name to be captured in the event, so unfortunately until Cosmos supports both attributes, update is needed before a delete
 
 This behaviour is enabled by default, however can be disabled by setting `ABNOSQL_COSMOS_CHANGE_META` env var to `FALSE` or `cosmos_change_meta=False` in table config.  `ABNOSQL_CAMELCASE` = `FALSE` env var can also be used to change attribute names used to snake_case if needed
 
+To write an Azure Function / AWS Lambda that is able to process both DynamoDB and Cosmos events, look for `changeMetadata` first and if present use that otherwise look for `eventName` and `eventSourceARN` in the event payload assuming its DynamoDB
+
 ## Client Side Encryption
 
 If configured in table config with `kms` attribute, abnosql will perform client side encryption using AWS KMS or Azure KeyVault
 
 Each attribute value defined in the config is encrypted with a 256-bit AES-GCM data key generated for each attribute value:
 
 - `aws` uses [AWS Encryption SDK for Python](https://docs.aws.amazon.com/encryption-sdk/latest/developer-guide/python.html)
```

### Comparing `abnosql-0.0.8/abnosql.egg-info/SOURCES.txt` & `abnosql-0.0.9/abnosql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/abnosql.egg-info/requires.txt` & `abnosql-0.0.9/abnosql.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.8/setup.py` & `abnosql-0.0.9/setup.py`

 * *Files identical despite different names*

