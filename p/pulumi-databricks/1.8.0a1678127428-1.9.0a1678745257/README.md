# Comparing `tmp/pulumi_databricks-1.8.0a1678127428.tar.gz` & `tmp/pulumi_databricks-1.9.0a1678745257.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_databricks-1.8.0a1678127428.tar", last modified: Mon Mar  6 18:37:27 2023, max compression
+gzip compressed data, was "pulumi_databricks-1.9.0a1678745257.tar", last modified: Mon Mar 13 22:12:15 2023, max compression
```

## Comparing `pulumi_databricks-1.8.0a1678127428.tar` & `pulumi_databricks-1.9.0a1678745257.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:37:27.097766 pulumi_databricks-1.8.0a1678127428/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-06 18:37:27.093766 pulumi_databricks-1.8.0a1678127428/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:37:27.093766 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   708087 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    24296 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)   112616 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/cluster_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:37:27.093766 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/dbfs_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    29011 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/entitlements.py
--rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/external_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_aws_assume_role_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_aws_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_aws_cross_account_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_cluster_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_current_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_dbfs_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_dbfs_file_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_mws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_mws_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    16699 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_notebook_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10591 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_service_principal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_service_principals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_share.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_shares.py
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_spark_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20000 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_sql_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_sql_warehouses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_zones.py
--rw-r--r--   0 runner    (1001) docker     (123)    14969 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/git_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/global_init_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/grants.py
--rw-r--r--   0 runner    (1001) docker     (123)    27330 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/group_instance_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/group_member.py
--rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/group_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    49655 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    30030 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/instance_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/ip_access_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    69219 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    35465 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/metastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/metastore_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19924 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/metastore_data_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/metastore_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mlflow_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mlflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mlflow_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    33920 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_customer_managed_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    46685 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_log_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    29433 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_permission_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    30905 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_private_access_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_storage_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22414 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_vpc_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    57683 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    18935 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/obo_token.py
--rw-r--r--   0 runner    (1001) docker     (123)   601498 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/permission_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    46014 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    24578 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22476 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/secret_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/secret_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    46205 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/service_principal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/service_principal_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/service_principal_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/share.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    49029 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    26154 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_global_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    19238 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/storage_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    42458 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/user_instance_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks/workspace_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:37:27.093766 pulumi_databricks-1.8.0a1678127428/pulumi_databricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-06 18:37:27.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-03-06 18:37:27.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 18:37:27.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 18:37:27.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-06 18:37:27.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-06 18:37:27.000000 pulumi_databricks-1.8.0a1678127428/pulumi_databricks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 18:37:27.097766 pulumi_databricks-1.8.0a1678127428/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-06 18:37:26.000000 pulumi_databricks-1.8.0a1678127428/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:12:15.786188 pulumi_databricks-1.9.0a1678745257/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-13 22:12:15.786188 pulumi_databricks-1.9.0a1678745257/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:12:15.782188 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15163 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   722584 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24296 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112616 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/cluster_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:12:15.786188 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/dbfs_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29011 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/entitlements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/external_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_aws_assume_role_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_aws_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_aws_cross_account_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_cluster_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_current_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_dbfs_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_dbfs_file_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_mws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_mws_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_notebook_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10591 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_service_principals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_shares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_spark_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20000 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_sql_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_sql_warehouses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/git_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15231 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/global_init_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27330 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/group_instance_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10675 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/group_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/group_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49655 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30030 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/instance_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/ip_access_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69219 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35465 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/metastore_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22416 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/metastore_data_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/metastore_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20408 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mlflow_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19314 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mlflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mlflow_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/model_serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19053 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33920 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_customer_managed_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46685 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_log_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29433 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_permission_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30905 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_private_access_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17030 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_storage_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22414 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_vpc_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57683 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18935 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/obo_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)   615196 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/permission_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43950 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46014 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24578 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22476 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/secret_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/secret_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46205 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/service_principal_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/service_principal_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/share.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49029 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26154 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_global_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24402 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19238 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26621 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/storage_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42458 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/user_instance_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks/workspace_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:12:15.786188 pulumi_databricks-1.9.0a1678745257/pulumi_databricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/pulumi_databricks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 22:12:15.786188 pulumi_databricks-1.9.0a1678745257/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-13 22:12:15.000000 pulumi_databricks-1.9.0a1678745257/setup.py
```

### Comparing `pulumi_databricks-1.8.0a1678127428/PKG-INFO` & `pulumi_databricks-1.9.0a1678745257/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_databricks
-Version: 1.8.0a1678127428
+Version: 1.9.0a1678745257
 Summary: A Pulumi package for creating and managing databricks cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-databricks
 Keywords: pulumi databricks category/infrastructure
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_databricks-1.8.0a1678127428/README.md` & `pulumi_databricks-1.9.0a1678745257/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/__init__.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 from .metastore import *
 from .metastore_assignment import *
 from .metastore_data_access import *
 from .metastore_provider import *
 from .mlflow_experiment import *
 from .mlflow_model import *
 from .mlflow_webhook import *
+from .model_serving import *
 from .mount import *
 from .mws_credentials import *
 from .mws_customer_managed_keys import *
 from .mws_log_delivery import *
 from .mws_networks import *
 from .mws_permission_assignment import *
 from .mws_private_access_settings import *
@@ -322,14 +323,22 @@
   "fqn": "pulumi_databricks",
   "classes": {
    "databricks:index/mlflowWebhook:MlflowWebhook": "MlflowWebhook"
   }
  },
  {
   "pkg": "databricks",
+  "mod": "index/modelServing",
+  "fqn": "pulumi_databricks",
+  "classes": {
+   "databricks:index/modelServing:ModelServing": "ModelServing"
+  }
+ },
+ {
+  "pkg": "databricks",
   "mod": "index/mount",
   "fqn": "pulumi_databricks",
   "classes": {
    "databricks:index/mount:Mount": "Mount"
   }
  },
  {
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/_inputs.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,18 +145,23 @@
     'JobWebhookNotificationsOnSuccessArgs',
     'LibraryCranArgs',
     'LibraryMavenArgs',
     'LibraryPypiArgs',
     'MetastoreDataAccessAwsIamRoleArgs',
     'MetastoreDataAccessAzureManagedIdentityArgs',
     'MetastoreDataAccessAzureServicePrincipalArgs',
+    'MetastoreDataAccessDatabricksGcpServiceAccountArgs',
     'MetastoreDataAccessGcpServiceAccountKeyArgs',
     'MlflowModelTagArgs',
     'MlflowWebhookHttpUrlSpecArgs',
     'MlflowWebhookJobSpecArgs',
+    'ModelServingConfigArgs',
+    'ModelServingConfigServedModelArgs',
+    'ModelServingConfigTrafficConfigArgs',
+    'ModelServingConfigTrafficConfigRouteArgs',
     'MountAbfsArgs',
     'MountAdlArgs',
     'MountGsArgs',
     'MountS3Args',
     'MountWasbArgs',
     'MwsCustomerManagedKeysAwsKeyInfoArgs',
     'MwsCustomerManagedKeysGcpKeyInfoArgs',
@@ -222,14 +227,15 @@
     'SqlQueryScheduleDailyArgs',
     'SqlQueryScheduleWeeklyArgs',
     'SqlWidgetParameterArgs',
     'SqlWidgetPositionArgs',
     'StorageCredentialAwsIamRoleArgs',
     'StorageCredentialAzureManagedIdentityArgs',
     'StorageCredentialAzureServicePrincipalArgs',
+    'StorageCredentialDatabricksGcpServiceAccountArgs',
     'StorageCredentialGcpServiceAccountKeyArgs',
     'TableColumnArgs',
     'GetClusterClusterInfoArgs',
     'GetClusterClusterInfoAutoscaleArgs',
     'GetClusterClusterInfoAwsAttributesArgs',
     'GetClusterClusterInfoAzureAttributesArgs',
     'GetClusterClusterInfoClusterLogConfArgs',
@@ -240,15 +246,18 @@
     'GetClusterClusterInfoDockerImageBasicAuthArgs',
     'GetClusterClusterInfoDriverArgs',
     'GetClusterClusterInfoDriverNodeAwsAttributesArgs',
     'GetClusterClusterInfoExecutorArgs',
     'GetClusterClusterInfoExecutorNodeAwsAttributesArgs',
     'GetClusterClusterInfoGcpAttributesArgs',
     'GetClusterClusterInfoInitScriptArgs',
+    'GetClusterClusterInfoInitScriptAbfssArgs',
     'GetClusterClusterInfoInitScriptDbfsArgs',
+    'GetClusterClusterInfoInitScriptFileArgs',
+    'GetClusterClusterInfoInitScriptGcsArgs',
     'GetClusterClusterInfoInitScriptS3Args',
     'GetClusterClusterInfoTerminationReasonArgs',
     'GetInstancePoolPoolInfoArgs',
     'GetInstancePoolPoolInfoAwsAttributesArgs',
     'GetInstancePoolPoolInfoAzureAttributesArgs',
     'GetInstancePoolPoolInfoDiskSpecArgs',
     'GetInstancePoolPoolInfoDiskSpecDiskTypeArgs',
@@ -7248,26 +7257,55 @@
 
     @directory_id.setter
     def directory_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "directory_id", value)
 
 
 @pulumi.input_type
+class MetastoreDataAccessDatabricksGcpServiceAccountArgs:
+    def __init__(__self__, *,
+                 email: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] email: The email of the GCP service account created, to be granted access to relevant buckets.
+        """
+        if email is not None:
+            pulumi.set(__self__, "email", email)
+
+    @property
+    @pulumi.getter
+    def email(self) -> Optional[pulumi.Input[str]]:
+        """
+        The email of the GCP service account created, to be granted access to relevant buckets.
+        """
+        return pulumi.get(self, "email")
+
+    @email.setter
+    def email(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "email", value)
+
+
+@pulumi.input_type
 class MetastoreDataAccessGcpServiceAccountKeyArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
                  private_key: pulumi.Input[str],
                  private_key_id: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] email: The email of the GCP service account created, to be granted access to relevant buckets.
+        """
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "private_key", private_key)
         pulumi.set(__self__, "private_key_id", private_key_id)
 
     @property
     @pulumi.getter
     def email(self) -> pulumi.Input[str]:
+        """
+        The email of the GCP service account created, to be granted access to relevant buckets.
+        """
         return pulumi.get(self, "email")
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
@@ -7436,14 +7474,196 @@
 
     @workspace_url.setter
     def workspace_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "workspace_url", value)
 
 
 @pulumi.input_type
+class ModelServingConfigArgs:
+    def __init__(__self__, *,
+                 served_models: pulumi.Input[Sequence[pulumi.Input['ModelServingConfigServedModelArgs']]],
+                 traffic_config: Optional[pulumi.Input['ModelServingConfigTrafficConfigArgs']] = None):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input['ModelServingConfigServedModelArgs']]] served_models: Each block represents a served model for the endpoint to serve. A model serving endpoint can have up to 10 served models.
+        :param pulumi.Input['ModelServingConfigTrafficConfigArgs'] traffic_config: A single block represents the traffic split configuration amongst the served models.
+        """
+        pulumi.set(__self__, "served_models", served_models)
+        if traffic_config is not None:
+            pulumi.set(__self__, "traffic_config", traffic_config)
+
+    @property
+    @pulumi.getter(name="servedModels")
+    def served_models(self) -> pulumi.Input[Sequence[pulumi.Input['ModelServingConfigServedModelArgs']]]:
+        """
+        Each block represents a served model for the endpoint to serve. A model serving endpoint can have up to 10 served models.
+        """
+        return pulumi.get(self, "served_models")
+
+    @served_models.setter
+    def served_models(self, value: pulumi.Input[Sequence[pulumi.Input['ModelServingConfigServedModelArgs']]]):
+        pulumi.set(self, "served_models", value)
+
+    @property
+    @pulumi.getter(name="trafficConfig")
+    def traffic_config(self) -> Optional[pulumi.Input['ModelServingConfigTrafficConfigArgs']]:
+        """
+        A single block represents the traffic split configuration amongst the served models.
+        """
+        return pulumi.get(self, "traffic_config")
+
+    @traffic_config.setter
+    def traffic_config(self, value: Optional[pulumi.Input['ModelServingConfigTrafficConfigArgs']]):
+        pulumi.set(self, "traffic_config", value)
+
+
+@pulumi.input_type
+class ModelServingConfigServedModelArgs:
+    def __init__(__self__, *,
+                 model_name: pulumi.Input[str],
+                 model_version: pulumi.Input[str],
+                 workload_size: pulumi.Input[str],
+                 name: Optional[pulumi.Input[str]] = None,
+                 scale_to_zero_enabled: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[str] model_name: The name of the model in Databricks Model Registry to be served.
+        :param pulumi.Input[str] model_version: The version of the model in Databricks Model Registry to be served.
+        :param pulumi.Input[str] workload_size: The workload size of the served model. The workload size corresponds to a range of provisioned concurrency that the compute will autoscale between. A single unit of provisioned concurrency can process one request at a time. Valid workload sizes are "Small" (4 - 4 provisioned concurrency), "Medium" (8 - 16 provisioned concurrency), and "Large" (16 - 64 provisioned concurrency).
+        :param pulumi.Input[str] name: The name of a served model. It must be unique across an endpoint. If not specified, this field will default to `modelname-modelversion`. A served model name can consist of alphanumeric characters, dashes, and underscores.
+        :param pulumi.Input[bool] scale_to_zero_enabled: Whether the compute resources for the served model should scale down to zero. If scale-to-zero is enabled, the lower bound of the provisioned concurrency for each workload size will be 0. The default value is `true`.
+        """
+        pulumi.set(__self__, "model_name", model_name)
+        pulumi.set(__self__, "model_version", model_version)
+        pulumi.set(__self__, "workload_size", workload_size)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if scale_to_zero_enabled is not None:
+            pulumi.set(__self__, "scale_to_zero_enabled", scale_to_zero_enabled)
+
+    @property
+    @pulumi.getter(name="modelName")
+    def model_name(self) -> pulumi.Input[str]:
+        """
+        The name of the model in Databricks Model Registry to be served.
+        """
+        return pulumi.get(self, "model_name")
+
+    @model_name.setter
+    def model_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "model_name", value)
+
+    @property
+    @pulumi.getter(name="modelVersion")
+    def model_version(self) -> pulumi.Input[str]:
+        """
+        The version of the model in Databricks Model Registry to be served.
+        """
+        return pulumi.get(self, "model_version")
+
+    @model_version.setter
+    def model_version(self, value: pulumi.Input[str]):
+        pulumi.set(self, "model_version", value)
+
+    @property
+    @pulumi.getter(name="workloadSize")
+    def workload_size(self) -> pulumi.Input[str]:
+        """
+        The workload size of the served model. The workload size corresponds to a range of provisioned concurrency that the compute will autoscale between. A single unit of provisioned concurrency can process one request at a time. Valid workload sizes are "Small" (4 - 4 provisioned concurrency), "Medium" (8 - 16 provisioned concurrency), and "Large" (16 - 64 provisioned concurrency).
+        """
+        return pulumi.get(self, "workload_size")
+
+    @workload_size.setter
+    def workload_size(self, value: pulumi.Input[str]):
+        pulumi.set(self, "workload_size", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The name of a served model. It must be unique across an endpoint. If not specified, this field will default to `modelname-modelversion`. A served model name can consist of alphanumeric characters, dashes, and underscores.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="scaleToZeroEnabled")
+    def scale_to_zero_enabled(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether the compute resources for the served model should scale down to zero. If scale-to-zero is enabled, the lower bound of the provisioned concurrency for each workload size will be 0. The default value is `true`.
+        """
+        return pulumi.get(self, "scale_to_zero_enabled")
+
+    @scale_to_zero_enabled.setter
+    def scale_to_zero_enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "scale_to_zero_enabled", value)
+
+
+@pulumi.input_type
+class ModelServingConfigTrafficConfigArgs:
+    def __init__(__self__, *,
+                 routes: Optional[pulumi.Input[Sequence[pulumi.Input['ModelServingConfigTrafficConfigRouteArgs']]]] = None):
+        """
+        :param pulumi.Input[Sequence[pulumi.Input['ModelServingConfigTrafficConfigRouteArgs']]] routes: Each block represents a route that defines traffic to each served model. Each `served_models` block needs to have a corresponding `routes` block
+        """
+        if routes is not None:
+            pulumi.set(__self__, "routes", routes)
+
+    @property
+    @pulumi.getter
+    def routes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ModelServingConfigTrafficConfigRouteArgs']]]]:
+        """
+        Each block represents a route that defines traffic to each served model. Each `served_models` block needs to have a corresponding `routes` block
+        """
+        return pulumi.get(self, "routes")
+
+    @routes.setter
+    def routes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ModelServingConfigTrafficConfigRouteArgs']]]]):
+        pulumi.set(self, "routes", value)
+
+
+@pulumi.input_type
+class ModelServingConfigTrafficConfigRouteArgs:
+    def __init__(__self__, *,
+                 served_model_name: pulumi.Input[str],
+                 traffic_percentage: pulumi.Input[int]):
+        """
+        :param pulumi.Input[str] served_model_name: The name of the served model this route configures traffic for. This needs to match the name of a `served_models` block
+        :param pulumi.Input[int] traffic_percentage: The percentage of endpoint traffic to send to this route. It must be an integer between 0 and 100 inclusive.
+        """
+        pulumi.set(__self__, "served_model_name", served_model_name)
+        pulumi.set(__self__, "traffic_percentage", traffic_percentage)
+
+    @property
+    @pulumi.getter(name="servedModelName")
+    def served_model_name(self) -> pulumi.Input[str]:
+        """
+        The name of the served model this route configures traffic for. This needs to match the name of a `served_models` block
+        """
+        return pulumi.get(self, "served_model_name")
+
+    @served_model_name.setter
+    def served_model_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "served_model_name", value)
+
+    @property
+    @pulumi.getter(name="trafficPercentage")
+    def traffic_percentage(self) -> pulumi.Input[int]:
+        """
+        The percentage of endpoint traffic to send to this route. It must be an integer between 0 and 100 inclusive.
+        """
+        return pulumi.get(self, "traffic_percentage")
+
+    @traffic_percentage.setter
+    def traffic_percentage(self, value: pulumi.Input[int]):
+        pulumi.set(self, "traffic_percentage", value)
+
+
+@pulumi.input_type
 class MountAbfsArgs:
     def __init__(__self__, *,
                  client_id: pulumi.Input[str],
                  client_secret_key: pulumi.Input[str],
                  client_secret_scope: pulumi.Input[str],
                  initialize_file_system: pulumi.Input[bool],
                  container_name: Optional[pulumi.Input[str]] = None,
@@ -10768,26 +10988,55 @@
 
     @directory_id.setter
     def directory_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "directory_id", value)
 
 
 @pulumi.input_type
+class StorageCredentialDatabricksGcpServiceAccountArgs:
+    def __init__(__self__, *,
+                 email: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] email: The email of the GCP service account created, to be granted access to relevant buckets.
+        """
+        if email is not None:
+            pulumi.set(__self__, "email", email)
+
+    @property
+    @pulumi.getter
+    def email(self) -> Optional[pulumi.Input[str]]:
+        """
+        The email of the GCP service account created, to be granted access to relevant buckets.
+        """
+        return pulumi.get(self, "email")
+
+    @email.setter
+    def email(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "email", value)
+
+
+@pulumi.input_type
 class StorageCredentialGcpServiceAccountKeyArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
                  private_key: pulumi.Input[str],
                  private_key_id: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] email: The email of the GCP service account created, to be granted access to relevant buckets.
+        """
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "private_key", private_key)
         pulumi.set(__self__, "private_key_id", private_key_id)
 
     @property
     @pulumi.getter
     def email(self) -> pulumi.Input[str]:
+        """
+        The email of the GCP service account created, to be granted access to relevant buckets.
+        """
         return pulumi.get(self, "email")
 
     @email.setter
     def email(self, value: pulumi.Input[str]):
         pulumi.set(self, "email", value)
 
     @property
@@ -12197,41 +12446,94 @@
     def zone_id(self, value: Optional[str]):
         pulumi.set(self, "zone_id", value)
 
 
 @pulumi.input_type
 class GetClusterClusterInfoInitScriptArgs:
     def __init__(__self__, *,
+                 abfss: Optional['GetClusterClusterInfoInitScriptAbfssArgs'] = None,
                  dbfs: Optional['GetClusterClusterInfoInitScriptDbfsArgs'] = None,
+                 file: Optional['GetClusterClusterInfoInitScriptFileArgs'] = None,
+                 gcs: Optional['GetClusterClusterInfoInitScriptGcsArgs'] = None,
                  s3: Optional['GetClusterClusterInfoInitScriptS3Args'] = None):
+        if abfss is not None:
+            pulumi.set(__self__, "abfss", abfss)
         if dbfs is not None:
             pulumi.set(__self__, "dbfs", dbfs)
+        if file is not None:
+            pulumi.set(__self__, "file", file)
+        if gcs is not None:
+            pulumi.set(__self__, "gcs", gcs)
         if s3 is not None:
             pulumi.set(__self__, "s3", s3)
 
     @property
     @pulumi.getter
+    def abfss(self) -> Optional['GetClusterClusterInfoInitScriptAbfssArgs']:
+        return pulumi.get(self, "abfss")
+
+    @abfss.setter
+    def abfss(self, value: Optional['GetClusterClusterInfoInitScriptAbfssArgs']):
+        pulumi.set(self, "abfss", value)
+
+    @property
+    @pulumi.getter
     def dbfs(self) -> Optional['GetClusterClusterInfoInitScriptDbfsArgs']:
         return pulumi.get(self, "dbfs")
 
     @dbfs.setter
     def dbfs(self, value: Optional['GetClusterClusterInfoInitScriptDbfsArgs']):
         pulumi.set(self, "dbfs", value)
 
     @property
     @pulumi.getter
+    def file(self) -> Optional['GetClusterClusterInfoInitScriptFileArgs']:
+        return pulumi.get(self, "file")
+
+    @file.setter
+    def file(self, value: Optional['GetClusterClusterInfoInitScriptFileArgs']):
+        pulumi.set(self, "file", value)
+
+    @property
+    @pulumi.getter
+    def gcs(self) -> Optional['GetClusterClusterInfoInitScriptGcsArgs']:
+        return pulumi.get(self, "gcs")
+
+    @gcs.setter
+    def gcs(self, value: Optional['GetClusterClusterInfoInitScriptGcsArgs']):
+        pulumi.set(self, "gcs", value)
+
+    @property
+    @pulumi.getter
     def s3(self) -> Optional['GetClusterClusterInfoInitScriptS3Args']:
         return pulumi.get(self, "s3")
 
     @s3.setter
     def s3(self, value: Optional['GetClusterClusterInfoInitScriptS3Args']):
         pulumi.set(self, "s3", value)
 
 
 @pulumi.input_type
+class GetClusterClusterInfoInitScriptAbfssArgs:
+    def __init__(__self__, *,
+                 destination: Optional[str] = None):
+        if destination is not None:
+            pulumi.set(__self__, "destination", destination)
+
+    @property
+    @pulumi.getter
+    def destination(self) -> Optional[str]:
+        return pulumi.get(self, "destination")
+
+    @destination.setter
+    def destination(self, value: Optional[str]):
+        pulumi.set(self, "destination", value)
+
+
+@pulumi.input_type
 class GetClusterClusterInfoInitScriptDbfsArgs:
     def __init__(__self__, *,
                  destination: str):
         pulumi.set(__self__, "destination", destination)
 
     @property
     @pulumi.getter
@@ -12240,14 +12542,48 @@
 
     @destination.setter
     def destination(self, value: str):
         pulumi.set(self, "destination", value)
 
 
 @pulumi.input_type
+class GetClusterClusterInfoInitScriptFileArgs:
+    def __init__(__self__, *,
+                 destination: Optional[str] = None):
+        if destination is not None:
+            pulumi.set(__self__, "destination", destination)
+
+    @property
+    @pulumi.getter
+    def destination(self) -> Optional[str]:
+        return pulumi.get(self, "destination")
+
+    @destination.setter
+    def destination(self, value: Optional[str]):
+        pulumi.set(self, "destination", value)
+
+
+@pulumi.input_type
+class GetClusterClusterInfoInitScriptGcsArgs:
+    def __init__(__self__, *,
+                 destination: Optional[str] = None):
+        if destination is not None:
+            pulumi.set(__self__, "destination", destination)
+
+    @property
+    @pulumi.getter
+    def destination(self) -> Optional[str]:
+        return pulumi.get(self, "destination")
+
+    @destination.setter
+    def destination(self, value: Optional[str]):
+        pulumi.set(self, "destination", value)
+
+
+@pulumi.input_type
 class GetClusterClusterInfoInitScriptS3Args:
     def __init__(__self__, *,
                  destination: str,
                  canned_acl: Optional[str] = None,
                  enable_encryption: Optional[bool] = None,
                  encryption_type: Optional[str] = None,
                  endpoint: Optional[str] = None,
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/_utilities.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/catalog.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/cluster.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/cluster_policy.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/cluster_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/config/vars.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/dbfs_file.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/dbfs_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/directory.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/entitlements.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/entitlements.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/external_location.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/external_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  metastore_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner: Optional[pulumi.Input[str]] = None,
                  skip_validation: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a ExternalLocation resource.
         :param pulumi.Input[str] credential_name: Name of the StorageCredential to use with this External Location.
-        :param pulumi.Input[str] url: Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure).
+        :param pulumi.Input[str] url: Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure), `gs://[bucket-host]/[bucket-dir]` (GCP).
         :param pulumi.Input[str] comment: User-supplied free-form text.
         :param pulumi.Input[str] name: Name of External Location, which must be unique within the databricks_metastore. Change forces creation of a new resource.
         :param pulumi.Input[str] owner: Username/groupname/sp application_id of the external Location owner.
         :param pulumi.Input[bool] skip_validation: Suppress validation errors if any & force save the external location
         """
         pulumi.set(__self__, "credential_name", credential_name)
         pulumi.set(__self__, "url", url)
@@ -55,15 +55,15 @@
     def credential_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "credential_name", value)
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Input[str]:
         """
-        Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure).
+        Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure), `gs://[bucket-host]/[bucket-dir]` (GCP).
         """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
@@ -138,15 +138,15 @@
         """
         Input properties used for looking up and filtering ExternalLocation resources.
         :param pulumi.Input[str] comment: User-supplied free-form text.
         :param pulumi.Input[str] credential_name: Name of the StorageCredential to use with this External Location.
         :param pulumi.Input[str] name: Name of External Location, which must be unique within the databricks_metastore. Change forces creation of a new resource.
         :param pulumi.Input[str] owner: Username/groupname/sp application_id of the external Location owner.
         :param pulumi.Input[bool] skip_validation: Suppress validation errors if any & force save the external location
-        :param pulumi.Input[str] url: Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure).
+        :param pulumi.Input[str] url: Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure), `gs://[bucket-host]/[bucket-dir]` (GCP).
         """
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
         if credential_name is not None:
             pulumi.set(__self__, "credential_name", credential_name)
         if metastore_id is not None:
             pulumi.set(__self__, "metastore_id", metastore_id)
@@ -228,15 +228,15 @@
     def skip_validation(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "skip_validation", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
         """
-        Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure).
+        Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure), `gs://[bucket-host]/[bucket-dir]` (GCP).
         """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
@@ -271,15 +271,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] comment: User-supplied free-form text.
         :param pulumi.Input[str] credential_name: Name of the StorageCredential to use with this External Location.
         :param pulumi.Input[str] name: Name of External Location, which must be unique within the databricks_metastore. Change forces creation of a new resource.
         :param pulumi.Input[str] owner: Username/groupname/sp application_id of the external Location owner.
         :param pulumi.Input[bool] skip_validation: Suppress validation errors if any & force save the external location
-        :param pulumi.Input[str] url: Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure).
+        :param pulumi.Input[str] url: Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure), `gs://[bucket-host]/[bucket-dir]` (GCP).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ExternalLocationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -364,15 +364,15 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] comment: User-supplied free-form text.
         :param pulumi.Input[str] credential_name: Name of the StorageCredential to use with this External Location.
         :param pulumi.Input[str] name: Name of External Location, which must be unique within the databricks_metastore. Change forces creation of a new resource.
         :param pulumi.Input[str] owner: Username/groupname/sp application_id of the external Location owner.
         :param pulumi.Input[bool] skip_validation: Suppress validation errors if any & force save the external location
-        :param pulumi.Input[str] url: Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure).
+        :param pulumi.Input[str] url: Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure), `gs://[bucket-host]/[bucket-dir]` (GCP).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ExternalLocationState.__new__(_ExternalLocationState)
 
         __props__.__dict__["comment"] = comment
         __props__.__dict__["credential_name"] = credential_name
@@ -428,11 +428,11 @@
         """
         return pulumi.get(self, "skip_validation")
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Output[str]:
         """
-        Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure).
+        Path URL in cloud storage, of the form: `s3://[bucket-host]/[bucket-dir]` (AWS), `abfss://[user]@[host]/[path]` (Azure), `gs://[bucket-host]/[bucket-dir]` (GCP).
         """
         return pulumi.get(self, "url")
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_aws_assume_role_policy.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_aws_assume_role_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_aws_bucket_policy.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_aws_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_aws_cross_account_policy.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_aws_cross_account_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_catalogs.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_catalogs.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_cluster.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_cluster_policy.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_cluster_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_clusters.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_current_user.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_current_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_dbfs_file.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_dbfs_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_dbfs_file_paths.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_dbfs_file_paths.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_directory.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_group.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_instance_pool.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_instance_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_job.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_jobs.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_jobs.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_mws_credentials.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_mws_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_mws_workspaces.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_mws_workspaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_node_type.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_node_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 
 @pulumi.output_type
 class GetNodeTypeResult:
     """
     A collection of values returned by getNodeType.
     """
-    def __init__(__self__, category=None, fleet=None, gb_per_core=None, graviton=None, id=None, is_io_cache_enabled=None, local_disk=None, local_disk_min_size=None, min_cores=None, min_gpus=None, min_memory_gb=None, photon_driver_capable=None, photon_worker_capable=None, support_port_forwarding=None, vcpu=None):
+    def __init__(__self__, category=None, fleet=None, gb_per_core=None, graviton=None, id=None, is_io_cache_enabled=None, local_disk=None, local_disk_min_size=None, min_cores=None, min_gpus=None, min_memory_gb=None, photon_driver_capable=None, photon_worker_capable=None, support_port_forwarding=None):
         if category and not isinstance(category, str):
             raise TypeError("Expected argument 'category' to be a str")
         pulumi.set(__self__, "category", category)
         if fleet and not isinstance(fleet, bool):
             raise TypeError("Expected argument 'fleet' to be a bool")
         pulumi.set(__self__, "fleet", fleet)
         if gb_per_core and not isinstance(gb_per_core, int):
@@ -60,17 +60,14 @@
         pulumi.set(__self__, "photon_driver_capable", photon_driver_capable)
         if photon_worker_capable and not isinstance(photon_worker_capable, bool):
             raise TypeError("Expected argument 'photon_worker_capable' to be a bool")
         pulumi.set(__self__, "photon_worker_capable", photon_worker_capable)
         if support_port_forwarding and not isinstance(support_port_forwarding, bool):
             raise TypeError("Expected argument 'support_port_forwarding' to be a bool")
         pulumi.set(__self__, "support_port_forwarding", support_port_forwarding)
-        if vcpu and not isinstance(vcpu, bool):
-            raise TypeError("Expected argument 'vcpu' to be a bool")
-        pulumi.set(__self__, "vcpu", vcpu)
 
     @property
     @pulumi.getter
     def category(self) -> Optional[str]:
         return pulumi.get(self, "category")
 
     @property
@@ -88,15 +85,15 @@
     def graviton(self) -> Optional[bool]:
         return pulumi.get(self, "graviton")
 
     @property
     @pulumi.getter
     def id(self) -> str:
         """
-        The provider-assigned unique ID for this managed resource.
+        node type, that can be used for databricks_job, databricks_cluster, or databricks_instance_pool.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter(name="isIoCacheEnabled")
     def is_io_cache_enabled(self) -> Optional[bool]:
         return pulumi.get(self, "is_io_cache_enabled")
@@ -137,19 +134,14 @@
         return pulumi.get(self, "photon_worker_capable")
 
     @property
     @pulumi.getter(name="supportPortForwarding")
     def support_port_forwarding(self) -> Optional[bool]:
         return pulumi.get(self, "support_port_forwarding")
 
-    @property
-    @pulumi.getter
-    def vcpu(self) -> Optional[bool]:
-        return pulumi.get(self, "vcpu")
-
 
 class AwaitableGetNodeTypeResult(GetNodeTypeResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetNodeTypeResult(
@@ -162,32 +154,31 @@
             local_disk=self.local_disk,
             local_disk_min_size=self.local_disk_min_size,
             min_cores=self.min_cores,
             min_gpus=self.min_gpus,
             min_memory_gb=self.min_memory_gb,
             photon_driver_capable=self.photon_driver_capable,
             photon_worker_capable=self.photon_worker_capable,
-            support_port_forwarding=self.support_port_forwarding,
-            vcpu=self.vcpu)
+            support_port_forwarding=self.support_port_forwarding)
 
 
 def get_node_type(category: Optional[str] = None,
                   fleet: Optional[bool] = None,
                   gb_per_core: Optional[int] = None,
                   graviton: Optional[bool] = None,
+                  id: Optional[str] = None,
                   is_io_cache_enabled: Optional[bool] = None,
                   local_disk: Optional[bool] = None,
                   local_disk_min_size: Optional[int] = None,
                   min_cores: Optional[int] = None,
                   min_gpus: Optional[int] = None,
                   min_memory_gb: Optional[int] = None,
                   photon_driver_capable: Optional[bool] = None,
                   photon_worker_capable: Optional[bool] = None,
                   support_port_forwarding: Optional[bool] = None,
-                  vcpu: Optional[bool] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNodeTypeResult:
     """
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_databricks as databricks
@@ -225,14 +216,15 @@
            * `Compute Optimized` (all clouds)
            * `Memory Optimized` (all clouds)
            * `Memory Optimized (Remote HDD)` (Azure)
            * `Storage Optimized` (AWS, Azure)
            * `GPU Accelerated` (AWS, Azure)
     :param int gb_per_core: Number of gigabytes per core available on instance. Conflicts with `min_memory_gb`. Defaults to *0*.
     :param bool graviton: if we should limit the search only to nodes with AWS Graviton CPUs. Default to *false*.
+    :param str id: node type, that can be used for databricks_job, databricks_cluster, or databricks_instance_pool.
     :param bool is_io_cache_enabled: . Pick only nodes that have IO Cache. Defaults to *false*.
     :param bool local_disk: Pick only nodes with local storage. Defaults to *false*.
     :param int local_disk_min_size: Pick only nodes that have size local storage greater or equal to given value. Defaults to *0*.
     :param int min_cores: Minimum number of CPU cores available on instance. Defaults to *0*.
     :param int min_gpus: Minimum number of GPU's attached to instance. Defaults to *0*.
     :param int min_memory_gb: Minimum amount of memory per node in gigabytes. Defaults to *0*.
     :param bool photon_driver_capable: Pick only nodes that can run Photon driver. Defaults to *false*.
@@ -240,24 +232,24 @@
     :param bool support_port_forwarding: Pick only nodes that support port forwarding. Defaults to *false*.
     """
     __args__ = dict()
     __args__['category'] = category
     __args__['fleet'] = fleet
     __args__['gbPerCore'] = gb_per_core
     __args__['graviton'] = graviton
+    __args__['id'] = id
     __args__['isIoCacheEnabled'] = is_io_cache_enabled
     __args__['localDisk'] = local_disk
     __args__['localDiskMinSize'] = local_disk_min_size
     __args__['minCores'] = min_cores
     __args__['minGpus'] = min_gpus
     __args__['minMemoryGb'] = min_memory_gb
     __args__['photonDriverCapable'] = photon_driver_capable
     __args__['photonWorkerCapable'] = photon_worker_capable
     __args__['supportPortForwarding'] = support_port_forwarding
-    __args__['vcpu'] = vcpu
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('databricks:index/getNodeType:getNodeType', __args__, opts=opts, typ=GetNodeTypeResult).value
 
     return AwaitableGetNodeTypeResult(
         category=__ret__.category,
         fleet=__ret__.fleet,
         gb_per_core=__ret__.gb_per_core,
@@ -267,33 +259,32 @@
         local_disk=__ret__.local_disk,
         local_disk_min_size=__ret__.local_disk_min_size,
         min_cores=__ret__.min_cores,
         min_gpus=__ret__.min_gpus,
         min_memory_gb=__ret__.min_memory_gb,
         photon_driver_capable=__ret__.photon_driver_capable,
         photon_worker_capable=__ret__.photon_worker_capable,
-        support_port_forwarding=__ret__.support_port_forwarding,
-        vcpu=__ret__.vcpu)
+        support_port_forwarding=__ret__.support_port_forwarding)
 
 
 @_utilities.lift_output_func(get_node_type)
 def get_node_type_output(category: Optional[pulumi.Input[Optional[str]]] = None,
                          fleet: Optional[pulumi.Input[Optional[bool]]] = None,
                          gb_per_core: Optional[pulumi.Input[Optional[int]]] = None,
                          graviton: Optional[pulumi.Input[Optional[bool]]] = None,
+                         id: Optional[pulumi.Input[Optional[str]]] = None,
                          is_io_cache_enabled: Optional[pulumi.Input[Optional[bool]]] = None,
                          local_disk: Optional[pulumi.Input[Optional[bool]]] = None,
                          local_disk_min_size: Optional[pulumi.Input[Optional[int]]] = None,
                          min_cores: Optional[pulumi.Input[Optional[int]]] = None,
                          min_gpus: Optional[pulumi.Input[Optional[int]]] = None,
                          min_memory_gb: Optional[pulumi.Input[Optional[int]]] = None,
                          photon_driver_capable: Optional[pulumi.Input[Optional[bool]]] = None,
                          photon_worker_capable: Optional[pulumi.Input[Optional[bool]]] = None,
                          support_port_forwarding: Optional[pulumi.Input[Optional[bool]]] = None,
-                         vcpu: Optional[pulumi.Input[Optional[bool]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodeTypeResult]:
     """
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_databricks as databricks
@@ -331,14 +322,15 @@
            * `Compute Optimized` (all clouds)
            * `Memory Optimized` (all clouds)
            * `Memory Optimized (Remote HDD)` (Azure)
            * `Storage Optimized` (AWS, Azure)
            * `GPU Accelerated` (AWS, Azure)
     :param int gb_per_core: Number of gigabytes per core available on instance. Conflicts with `min_memory_gb`. Defaults to *0*.
     :param bool graviton: if we should limit the search only to nodes with AWS Graviton CPUs. Default to *false*.
+    :param str id: node type, that can be used for databricks_job, databricks_cluster, or databricks_instance_pool.
     :param bool is_io_cache_enabled: . Pick only nodes that have IO Cache. Defaults to *false*.
     :param bool local_disk: Pick only nodes with local storage. Defaults to *false*.
     :param int local_disk_min_size: Pick only nodes that have size local storage greater or equal to given value. Defaults to *0*.
     :param int min_cores: Minimum number of CPU cores available on instance. Defaults to *0*.
     :param int min_gpus: Minimum number of GPU's attached to instance. Defaults to *0*.
     :param int min_memory_gb: Minimum amount of memory per node in gigabytes. Defaults to *0*.
     :param bool photon_driver_capable: Pick only nodes that can run Photon driver. Defaults to *false*.
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_notebook.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_notebook.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_notebook_paths.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_notebook_paths.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_schemas.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_schemas.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_service_principal.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_service_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_service_principals.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_service_principals.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_share.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_share.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_shares.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_shares.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_spark_version.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_spark_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_sql_warehouse.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_sql_warehouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_sql_warehouses.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_sql_warehouses.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_tables.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_user.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_views.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/get_zones.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/get_zones.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/git_credential.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/git_credential.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,74 +11,76 @@
 
 __all__ = ['GitCredentialArgs', 'GitCredential']
 
 @pulumi.input_type
 class GitCredentialArgs:
     def __init__(__self__, *,
                  git_provider: pulumi.Input[str],
-                 git_username: pulumi.Input[str],
-                 personal_access_token: pulumi.Input[str],
-                 force: Optional[pulumi.Input[bool]] = None):
+                 force: Optional[pulumi.Input[bool]] = None,
+                 git_username: Optional[pulumi.Input[str]] = None,
+                 personal_access_token: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a GitCredential resource.
         :param pulumi.Input[str] git_provider: case insensitive name of the Git provider.  Following values are supported right now (could be a subject for a change, consult [Git Credentials API documentation](https://docs.databricks.com/dev-tools/api/latest/gitcredentials.html)): `gitHub`, `gitHubEnterprise`, `bitbucketCloud`, `bitbucketServer`, `azureDevOpsServices`, `gitLab`, `gitLabEnterpriseEdition`, `awsCodeCommit`.
-        :param pulumi.Input[str] git_username: user name at Git provider.
         :param pulumi.Input[bool] force: specify if settings need to be enforced - right now, Databricks allows only single Git credential, so if it's already configured, the apply operation will fail.
+        :param pulumi.Input[str] git_username: user name at Git provider.
         """
         pulumi.set(__self__, "git_provider", git_provider)
-        pulumi.set(__self__, "git_username", git_username)
-        pulumi.set(__self__, "personal_access_token", personal_access_token)
         if force is not None:
             pulumi.set(__self__, "force", force)
+        if git_username is not None:
+            pulumi.set(__self__, "git_username", git_username)
+        if personal_access_token is not None:
+            pulumi.set(__self__, "personal_access_token", personal_access_token)
 
     @property
     @pulumi.getter(name="gitProvider")
     def git_provider(self) -> pulumi.Input[str]:
         """
         case insensitive name of the Git provider.  Following values are supported right now (could be a subject for a change, consult [Git Credentials API documentation](https://docs.databricks.com/dev-tools/api/latest/gitcredentials.html)): `gitHub`, `gitHubEnterprise`, `bitbucketCloud`, `bitbucketServer`, `azureDevOpsServices`, `gitLab`, `gitLabEnterpriseEdition`, `awsCodeCommit`.
         """
         return pulumi.get(self, "git_provider")
 
     @git_provider.setter
     def git_provider(self, value: pulumi.Input[str]):
         pulumi.set(self, "git_provider", value)
 
     @property
+    @pulumi.getter
+    def force(self) -> Optional[pulumi.Input[bool]]:
+        """
+        specify if settings need to be enforced - right now, Databricks allows only single Git credential, so if it's already configured, the apply operation will fail.
+        """
+        return pulumi.get(self, "force")
+
+    @force.setter
+    def force(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "force", value)
+
+    @property
     @pulumi.getter(name="gitUsername")
-    def git_username(self) -> pulumi.Input[str]:
+    def git_username(self) -> Optional[pulumi.Input[str]]:
         """
         user name at Git provider.
         """
         return pulumi.get(self, "git_username")
 
     @git_username.setter
-    def git_username(self, value: pulumi.Input[str]):
+    def git_username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "git_username", value)
 
     @property
     @pulumi.getter(name="personalAccessToken")
-    def personal_access_token(self) -> pulumi.Input[str]:
+    def personal_access_token(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "personal_access_token")
 
     @personal_access_token.setter
-    def personal_access_token(self, value: pulumi.Input[str]):
+    def personal_access_token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "personal_access_token", value)
 
-    @property
-    @pulumi.getter
-    def force(self) -> Optional[pulumi.Input[bool]]:
-        """
-        specify if settings need to be enforced - right now, Databricks allows only single Git credential, so if it's already configured, the apply operation will fail.
-        """
-        return pulumi.get(self, "force")
-
-    @force.setter
-    def force(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "force", value)
-
 
 @pulumi.input_type
 class _GitCredentialState:
     def __init__(__self__, *,
                  force: Optional[pulumi.Input[bool]] = None,
                  git_provider: Optional[pulumi.Input[str]] = None,
                  git_username: Optional[pulumi.Input[str]] = None,
@@ -212,22 +214,16 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = GitCredentialArgs.__new__(GitCredentialArgs)
 
             __props__.__dict__["force"] = force
             if git_provider is None and not opts.urn:
                 raise TypeError("Missing required property 'git_provider'")
             __props__.__dict__["git_provider"] = git_provider
-            if git_username is None and not opts.urn:
-                raise TypeError("Missing required property 'git_username'")
             __props__.__dict__["git_username"] = git_username
-            if personal_access_token is None and not opts.urn:
-                raise TypeError("Missing required property 'personal_access_token'")
-            __props__.__dict__["personal_access_token"] = None if personal_access_token is None else pulumi.Output.secret(personal_access_token)
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["personalAccessToken"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+            __props__.__dict__["personal_access_token"] = personal_access_token
         super(GitCredential, __self__).__init__(
             'databricks:index/gitCredential:GitCredential',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
@@ -273,18 +269,18 @@
         """
         case insensitive name of the Git provider.  Following values are supported right now (could be a subject for a change, consult [Git Credentials API documentation](https://docs.databricks.com/dev-tools/api/latest/gitcredentials.html)): `gitHub`, `gitHubEnterprise`, `bitbucketCloud`, `bitbucketServer`, `azureDevOpsServices`, `gitLab`, `gitLabEnterpriseEdition`, `awsCodeCommit`.
         """
         return pulumi.get(self, "git_provider")
 
     @property
     @pulumi.getter(name="gitUsername")
-    def git_username(self) -> pulumi.Output[str]:
+    def git_username(self) -> pulumi.Output[Optional[str]]:
         """
         user name at Git provider.
         """
         return pulumi.get(self, "git_username")
 
     @property
     @pulumi.getter(name="personalAccessToken")
-    def personal_access_token(self) -> pulumi.Output[str]:
+    def personal_access_token(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "personal_access_token")
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/global_init_script.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/global_init_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/grants.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/grants.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/group.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/group_instance_profile.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/group_instance_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/group_member.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/group_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/group_role.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/group_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/instance_pool.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/instance_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/instance_profile.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/instance_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/ip_access_list.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/ip_access_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/job.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/library.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/library.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/metastore.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/metastore.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/metastore_assignment.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/metastore_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/metastore_data_access.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/metastore_data_access.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 class MetastoreDataAccessArgs:
     def __init__(__self__, *,
                  metastore_id: pulumi.Input[str],
                  aws_iam_role: Optional[pulumi.Input['MetastoreDataAccessAwsIamRoleArgs']] = None,
                  azure_managed_identity: Optional[pulumi.Input['MetastoreDataAccessAzureManagedIdentityArgs']] = None,
                  azure_service_principal: Optional[pulumi.Input['MetastoreDataAccessAzureServicePrincipalArgs']] = None,
                  configuration_type: Optional[pulumi.Input[str]] = None,
+                 databricks_gcp_service_account: Optional[pulumi.Input['MetastoreDataAccessDatabricksGcpServiceAccountArgs']] = None,
                  gcp_service_account_key: Optional[pulumi.Input['MetastoreDataAccessGcpServiceAccountKeyArgs']] = None,
                  is_default: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a MetastoreDataAccess resource.
         :param pulumi.Input[str] metastore_id: Unique identifier of the parent Metastore
         :param pulumi.Input[str] name: Name of Data Access Configuration, which must be unique within the databricks_metastore. Change forces creation of a new resource.
@@ -34,14 +35,16 @@
             pulumi.set(__self__, "aws_iam_role", aws_iam_role)
         if azure_managed_identity is not None:
             pulumi.set(__self__, "azure_managed_identity", azure_managed_identity)
         if azure_service_principal is not None:
             pulumi.set(__self__, "azure_service_principal", azure_service_principal)
         if configuration_type is not None:
             pulumi.set(__self__, "configuration_type", configuration_type)
+        if databricks_gcp_service_account is not None:
+            pulumi.set(__self__, "databricks_gcp_service_account", databricks_gcp_service_account)
         if gcp_service_account_key is not None:
             pulumi.set(__self__, "gcp_service_account_key", gcp_service_account_key)
         if is_default is not None:
             pulumi.set(__self__, "is_default", is_default)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
@@ -90,14 +93,23 @@
         return pulumi.get(self, "configuration_type")
 
     @configuration_type.setter
     def configuration_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration_type", value)
 
     @property
+    @pulumi.getter(name="databricksGcpServiceAccount")
+    def databricks_gcp_service_account(self) -> Optional[pulumi.Input['MetastoreDataAccessDatabricksGcpServiceAccountArgs']]:
+        return pulumi.get(self, "databricks_gcp_service_account")
+
+    @databricks_gcp_service_account.setter
+    def databricks_gcp_service_account(self, value: Optional[pulumi.Input['MetastoreDataAccessDatabricksGcpServiceAccountArgs']]):
+        pulumi.set(self, "databricks_gcp_service_account", value)
+
+    @property
     @pulumi.getter(name="gcpServiceAccountKey")
     def gcp_service_account_key(self) -> Optional[pulumi.Input['MetastoreDataAccessGcpServiceAccountKeyArgs']]:
         return pulumi.get(self, "gcp_service_account_key")
 
     @gcp_service_account_key.setter
     def gcp_service_account_key(self, value: Optional[pulumi.Input['MetastoreDataAccessGcpServiceAccountKeyArgs']]):
         pulumi.set(self, "gcp_service_account_key", value)
@@ -127,14 +139,15 @@
 @pulumi.input_type
 class _MetastoreDataAccessState:
     def __init__(__self__, *,
                  aws_iam_role: Optional[pulumi.Input['MetastoreDataAccessAwsIamRoleArgs']] = None,
                  azure_managed_identity: Optional[pulumi.Input['MetastoreDataAccessAzureManagedIdentityArgs']] = None,
                  azure_service_principal: Optional[pulumi.Input['MetastoreDataAccessAzureServicePrincipalArgs']] = None,
                  configuration_type: Optional[pulumi.Input[str]] = None,
+                 databricks_gcp_service_account: Optional[pulumi.Input['MetastoreDataAccessDatabricksGcpServiceAccountArgs']] = None,
                  gcp_service_account_key: Optional[pulumi.Input['MetastoreDataAccessGcpServiceAccountKeyArgs']] = None,
                  is_default: Optional[pulumi.Input[bool]] = None,
                  metastore_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering MetastoreDataAccess resources.
         :param pulumi.Input[str] metastore_id: Unique identifier of the parent Metastore
@@ -144,14 +157,16 @@
             pulumi.set(__self__, "aws_iam_role", aws_iam_role)
         if azure_managed_identity is not None:
             pulumi.set(__self__, "azure_managed_identity", azure_managed_identity)
         if azure_service_principal is not None:
             pulumi.set(__self__, "azure_service_principal", azure_service_principal)
         if configuration_type is not None:
             pulumi.set(__self__, "configuration_type", configuration_type)
+        if databricks_gcp_service_account is not None:
+            pulumi.set(__self__, "databricks_gcp_service_account", databricks_gcp_service_account)
         if gcp_service_account_key is not None:
             pulumi.set(__self__, "gcp_service_account_key", gcp_service_account_key)
         if is_default is not None:
             pulumi.set(__self__, "is_default", is_default)
         if metastore_id is not None:
             pulumi.set(__self__, "metastore_id", metastore_id)
         if name is not None:
@@ -190,14 +205,23 @@
         return pulumi.get(self, "configuration_type")
 
     @configuration_type.setter
     def configuration_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration_type", value)
 
     @property
+    @pulumi.getter(name="databricksGcpServiceAccount")
+    def databricks_gcp_service_account(self) -> Optional[pulumi.Input['MetastoreDataAccessDatabricksGcpServiceAccountArgs']]:
+        return pulumi.get(self, "databricks_gcp_service_account")
+
+    @databricks_gcp_service_account.setter
+    def databricks_gcp_service_account(self, value: Optional[pulumi.Input['MetastoreDataAccessDatabricksGcpServiceAccountArgs']]):
+        pulumi.set(self, "databricks_gcp_service_account", value)
+
+    @property
     @pulumi.getter(name="gcpServiceAccountKey")
     def gcp_service_account_key(self) -> Optional[pulumi.Input['MetastoreDataAccessGcpServiceAccountKeyArgs']]:
         return pulumi.get(self, "gcp_service_account_key")
 
     @gcp_service_account_key.setter
     def gcp_service_account_key(self, value: Optional[pulumi.Input['MetastoreDataAccessGcpServiceAccountKeyArgs']]):
         pulumi.set(self, "gcp_service_account_key", value)
@@ -241,14 +265,15 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aws_iam_role: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessAwsIamRoleArgs']]] = None,
                  azure_managed_identity: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessAzureManagedIdentityArgs']]] = None,
                  azure_service_principal: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessAzureServicePrincipalArgs']]] = None,
                  configuration_type: Optional[pulumi.Input[str]] = None,
+                 databricks_gcp_service_account: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessDatabricksGcpServiceAccountArgs']]] = None,
                  gcp_service_account_key: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessGcpServiceAccountKeyArgs']]] = None,
                  is_default: Optional[pulumi.Input[bool]] = None,
                  metastore_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Each Metastore requires an IAM role that will be assumed by Unity Catalog to access data. `MetastoreDataAccess` defines this
@@ -290,14 +315,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aws_iam_role: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessAwsIamRoleArgs']]] = None,
                  azure_managed_identity: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessAzureManagedIdentityArgs']]] = None,
                  azure_service_principal: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessAzureServicePrincipalArgs']]] = None,
                  configuration_type: Optional[pulumi.Input[str]] = None,
+                 databricks_gcp_service_account: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessDatabricksGcpServiceAccountArgs']]] = None,
                  gcp_service_account_key: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessGcpServiceAccountKeyArgs']]] = None,
                  is_default: Optional[pulumi.Input[bool]] = None,
                  metastore_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
@@ -307,14 +333,15 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = MetastoreDataAccessArgs.__new__(MetastoreDataAccessArgs)
 
             __props__.__dict__["aws_iam_role"] = aws_iam_role
             __props__.__dict__["azure_managed_identity"] = azure_managed_identity
             __props__.__dict__["azure_service_principal"] = azure_service_principal
             __props__.__dict__["configuration_type"] = configuration_type
+            __props__.__dict__["databricks_gcp_service_account"] = databricks_gcp_service_account
             __props__.__dict__["gcp_service_account_key"] = gcp_service_account_key
             __props__.__dict__["is_default"] = is_default
             if metastore_id is None and not opts.urn:
                 raise TypeError("Missing required property 'metastore_id'")
             __props__.__dict__["metastore_id"] = metastore_id
             __props__.__dict__["name"] = name
         super(MetastoreDataAccess, __self__).__init__(
@@ -327,14 +354,15 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             aws_iam_role: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessAwsIamRoleArgs']]] = None,
             azure_managed_identity: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessAzureManagedIdentityArgs']]] = None,
             azure_service_principal: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessAzureServicePrincipalArgs']]] = None,
             configuration_type: Optional[pulumi.Input[str]] = None,
+            databricks_gcp_service_account: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessDatabricksGcpServiceAccountArgs']]] = None,
             gcp_service_account_key: Optional[pulumi.Input[pulumi.InputType['MetastoreDataAccessGcpServiceAccountKeyArgs']]] = None,
             is_default: Optional[pulumi.Input[bool]] = None,
             metastore_id: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None) -> 'MetastoreDataAccess':
         """
         Get an existing MetastoreDataAccess resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
@@ -349,14 +377,15 @@
 
         __props__ = _MetastoreDataAccessState.__new__(_MetastoreDataAccessState)
 
         __props__.__dict__["aws_iam_role"] = aws_iam_role
         __props__.__dict__["azure_managed_identity"] = azure_managed_identity
         __props__.__dict__["azure_service_principal"] = azure_service_principal
         __props__.__dict__["configuration_type"] = configuration_type
+        __props__.__dict__["databricks_gcp_service_account"] = databricks_gcp_service_account
         __props__.__dict__["gcp_service_account_key"] = gcp_service_account_key
         __props__.__dict__["is_default"] = is_default
         __props__.__dict__["metastore_id"] = metastore_id
         __props__.__dict__["name"] = name
         return MetastoreDataAccess(resource_name, opts=opts, __props__=__props__)
 
     @property
@@ -376,14 +405,19 @@
 
     @property
     @pulumi.getter(name="configurationType")
     def configuration_type(self) -> pulumi.Output[str]:
         return pulumi.get(self, "configuration_type")
 
     @property
+    @pulumi.getter(name="databricksGcpServiceAccount")
+    def databricks_gcp_service_account(self) -> pulumi.Output[Optional['outputs.MetastoreDataAccessDatabricksGcpServiceAccount']]:
+        return pulumi.get(self, "databricks_gcp_service_account")
+
+    @property
     @pulumi.getter(name="gcpServiceAccountKey")
     def gcp_service_account_key(self) -> pulumi.Output[Optional['outputs.MetastoreDataAccessGcpServiceAccountKey']]:
         return pulumi.get(self, "gcp_service_account_key")
 
     @property
     @pulumi.getter(name="isDefault")
     def is_default(self) -> pulumi.Output[Optional[bool]]:
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/metastore_provider.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/metastore_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mlflow_experiment.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mlflow_experiment.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mlflow_model.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mlflow_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,16 @@
         * Permissions can control which groups or individual users can *Read*, *Edit*, *Manage Staging Versions*, *Manage Production Versions*, and *Manage* individual models.
 
         ## Related Resources
 
         The following resources are often used in the same context:
 
         * End to end workspace management guide.
-        * Directory to manage directories in [Databricks Workpace](https://docs.databricks.com/workspace/workspace-objects.html).
+        * ModelServing to serve this model on a Databricks serving endpoint.
+        * Directory to manage directories in [Databricks Workspace](https://docs.databricks.com/workspace/workspace-objects.html).
         * MlflowExperiment to manage [MLflow experiments](https://docs.databricks.com/data/data-sources/mlflow-experiment.html) in Databricks.
         * Notebook to manage [Databricks Notebooks](https://docs.databricks.com/notebooks/index.html).
         * Notebook data to export a notebook from Databricks Workspace.
         * Repo to manage [Databricks Repos](https://docs.databricks.com/repos.html).
 
         ## Import
 
@@ -318,15 +319,16 @@
         * Permissions can control which groups or individual users can *Read*, *Edit*, *Manage Staging Versions*, *Manage Production Versions*, and *Manage* individual models.
 
         ## Related Resources
 
         The following resources are often used in the same context:
 
         * End to end workspace management guide.
-        * Directory to manage directories in [Databricks Workpace](https://docs.databricks.com/workspace/workspace-objects.html).
+        * ModelServing to serve this model on a Databricks serving endpoint.
+        * Directory to manage directories in [Databricks Workspace](https://docs.databricks.com/workspace/workspace-objects.html).
         * MlflowExperiment to manage [MLflow experiments](https://docs.databricks.com/data/data-sources/mlflow-experiment.html) in Databricks.
         * Notebook to manage [Databricks Notebooks](https://docs.databricks.com/notebooks/index.html).
         * Notebook data to export a notebook from Databricks Workspace.
         * Repo to manage [Databricks Repos](https://docs.databricks.com/repos.html).
 
         ## Import
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mlflow_webhook.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mlflow_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mount.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mount.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_credentials.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_customer_managed_keys.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_customer_managed_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_log_delivery.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_log_delivery.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_networks.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_permission_assignment.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_permission_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_private_access_settings.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_private_access_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_storage_configurations.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_storage_configurations.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_vpc_endpoint.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/mws_workspaces.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/mws_workspaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/notebook.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/notebook.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/obo_token.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/obo_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/outputs.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,18 +146,23 @@
     'JobWebhookNotificationsOnSuccess',
     'LibraryCran',
     'LibraryMaven',
     'LibraryPypi',
     'MetastoreDataAccessAwsIamRole',
     'MetastoreDataAccessAzureManagedIdentity',
     'MetastoreDataAccessAzureServicePrincipal',
+    'MetastoreDataAccessDatabricksGcpServiceAccount',
     'MetastoreDataAccessGcpServiceAccountKey',
     'MlflowModelTag',
     'MlflowWebhookHttpUrlSpec',
     'MlflowWebhookJobSpec',
+    'ModelServingConfig',
+    'ModelServingConfigServedModel',
+    'ModelServingConfigTrafficConfig',
+    'ModelServingConfigTrafficConfigRoute',
     'MountAbfs',
     'MountAdl',
     'MountGs',
     'MountS3',
     'MountWasb',
     'MwsCustomerManagedKeysAwsKeyInfo',
     'MwsCustomerManagedKeysGcpKeyInfo',
@@ -223,14 +228,15 @@
     'SqlQueryScheduleDaily',
     'SqlQueryScheduleWeekly',
     'SqlWidgetParameter',
     'SqlWidgetPosition',
     'StorageCredentialAwsIamRole',
     'StorageCredentialAzureManagedIdentity',
     'StorageCredentialAzureServicePrincipal',
+    'StorageCredentialDatabricksGcpServiceAccount',
     'StorageCredentialGcpServiceAccountKey',
     'TableColumn',
     'GetClusterClusterInfoResult',
     'GetClusterClusterInfoAutoscaleResult',
     'GetClusterClusterInfoAwsAttributesResult',
     'GetClusterClusterInfoAzureAttributesResult',
     'GetClusterClusterInfoClusterLogConfResult',
@@ -241,15 +247,18 @@
     'GetClusterClusterInfoDockerImageBasicAuthResult',
     'GetClusterClusterInfoDriverResult',
     'GetClusterClusterInfoDriverNodeAwsAttributesResult',
     'GetClusterClusterInfoExecutorResult',
     'GetClusterClusterInfoExecutorNodeAwsAttributesResult',
     'GetClusterClusterInfoGcpAttributesResult',
     'GetClusterClusterInfoInitScriptResult',
+    'GetClusterClusterInfoInitScriptAbfssResult',
     'GetClusterClusterInfoInitScriptDbfsResult',
+    'GetClusterClusterInfoInitScriptFileResult',
+    'GetClusterClusterInfoInitScriptGcsResult',
     'GetClusterClusterInfoInitScriptS3Result',
     'GetClusterClusterInfoTerminationReasonResult',
     'GetDbfsFilePathsPathListResult',
     'GetInstancePoolPoolInfoResult',
     'GetInstancePoolPoolInfoAwsAttributesResult',
     'GetInstancePoolPoolInfoAzureAttributesResult',
     'GetInstancePoolPoolInfoDiskSpecResult',
@@ -7029,14 +7038,33 @@
         """
         The directory ID corresponding to the Azure Active Directory (AAD) tenant of the application
         """
         return pulumi.get(self, "directory_id")
 
 
 @pulumi.output_type
+class MetastoreDataAccessDatabricksGcpServiceAccount(dict):
+    def __init__(__self__, *,
+                 email: Optional[str] = None):
+        """
+        :param str email: The email of the GCP service account created, to be granted access to relevant buckets.
+        """
+        if email is not None:
+            pulumi.set(__self__, "email", email)
+
+    @property
+    @pulumi.getter
+    def email(self) -> Optional[str]:
+        """
+        The email of the GCP service account created, to be granted access to relevant buckets.
+        """
+        return pulumi.get(self, "email")
+
+
+@pulumi.output_type
 class MetastoreDataAccessGcpServiceAccountKey(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "privateKey":
             suggest = "private_key"
         elif key == "privateKeyId":
@@ -7053,21 +7081,27 @@
         MetastoreDataAccessGcpServiceAccountKey.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  email: str,
                  private_key: str,
                  private_key_id: str):
+        """
+        :param str email: The email of the GCP service account created, to be granted access to relevant buckets.
+        """
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "private_key", private_key)
         pulumi.set(__self__, "private_key_id", private_key_id)
 
     @property
     @pulumi.getter
     def email(self) -> str:
+        """
+        The email of the GCP service account created, to be granted access to relevant buckets.
+        """
         return pulumi.get(self, "email")
 
     @property
     @pulumi.getter(name="privateKey")
     def private_key(self) -> str:
         return pulumi.get(self, "private_key")
 
@@ -7226,14 +7260,217 @@
         """
         URL of the workspace containing the job that this webhook runs. If not specified, the job’s workspace URL is assumed to be the same as the workspace where the webhook is created.
         """
         return pulumi.get(self, "workspace_url")
 
 
 @pulumi.output_type
+class ModelServingConfig(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "servedModels":
+            suggest = "served_models"
+        elif key == "trafficConfig":
+            suggest = "traffic_config"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ModelServingConfig. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ModelServingConfig.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ModelServingConfig.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 served_models: Sequence['outputs.ModelServingConfigServedModel'],
+                 traffic_config: Optional['outputs.ModelServingConfigTrafficConfig'] = None):
+        """
+        :param Sequence['ModelServingConfigServedModelArgs'] served_models: Each block represents a served model for the endpoint to serve. A model serving endpoint can have up to 10 served models.
+        :param 'ModelServingConfigTrafficConfigArgs' traffic_config: A single block represents the traffic split configuration amongst the served models.
+        """
+        pulumi.set(__self__, "served_models", served_models)
+        if traffic_config is not None:
+            pulumi.set(__self__, "traffic_config", traffic_config)
+
+    @property
+    @pulumi.getter(name="servedModels")
+    def served_models(self) -> Sequence['outputs.ModelServingConfigServedModel']:
+        """
+        Each block represents a served model for the endpoint to serve. A model serving endpoint can have up to 10 served models.
+        """
+        return pulumi.get(self, "served_models")
+
+    @property
+    @pulumi.getter(name="trafficConfig")
+    def traffic_config(self) -> Optional['outputs.ModelServingConfigTrafficConfig']:
+        """
+        A single block represents the traffic split configuration amongst the served models.
+        """
+        return pulumi.get(self, "traffic_config")
+
+
+@pulumi.output_type
+class ModelServingConfigServedModel(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "modelName":
+            suggest = "model_name"
+        elif key == "modelVersion":
+            suggest = "model_version"
+        elif key == "workloadSize":
+            suggest = "workload_size"
+        elif key == "scaleToZeroEnabled":
+            suggest = "scale_to_zero_enabled"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ModelServingConfigServedModel. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ModelServingConfigServedModel.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ModelServingConfigServedModel.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 model_name: str,
+                 model_version: str,
+                 workload_size: str,
+                 name: Optional[str] = None,
+                 scale_to_zero_enabled: Optional[bool] = None):
+        """
+        :param str model_name: The name of the model in Databricks Model Registry to be served.
+        :param str model_version: The version of the model in Databricks Model Registry to be served.
+        :param str workload_size: The workload size of the served model. The workload size corresponds to a range of provisioned concurrency that the compute will autoscale between. A single unit of provisioned concurrency can process one request at a time. Valid workload sizes are "Small" (4 - 4 provisioned concurrency), "Medium" (8 - 16 provisioned concurrency), and "Large" (16 - 64 provisioned concurrency).
+        :param str name: The name of a served model. It must be unique across an endpoint. If not specified, this field will default to `modelname-modelversion`. A served model name can consist of alphanumeric characters, dashes, and underscores.
+        :param bool scale_to_zero_enabled: Whether the compute resources for the served model should scale down to zero. If scale-to-zero is enabled, the lower bound of the provisioned concurrency for each workload size will be 0. The default value is `true`.
+        """
+        pulumi.set(__self__, "model_name", model_name)
+        pulumi.set(__self__, "model_version", model_version)
+        pulumi.set(__self__, "workload_size", workload_size)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if scale_to_zero_enabled is not None:
+            pulumi.set(__self__, "scale_to_zero_enabled", scale_to_zero_enabled)
+
+    @property
+    @pulumi.getter(name="modelName")
+    def model_name(self) -> str:
+        """
+        The name of the model in Databricks Model Registry to be served.
+        """
+        return pulumi.get(self, "model_name")
+
+    @property
+    @pulumi.getter(name="modelVersion")
+    def model_version(self) -> str:
+        """
+        The version of the model in Databricks Model Registry to be served.
+        """
+        return pulumi.get(self, "model_version")
+
+    @property
+    @pulumi.getter(name="workloadSize")
+    def workload_size(self) -> str:
+        """
+        The workload size of the served model. The workload size corresponds to a range of provisioned concurrency that the compute will autoscale between. A single unit of provisioned concurrency can process one request at a time. Valid workload sizes are "Small" (4 - 4 provisioned concurrency), "Medium" (8 - 16 provisioned concurrency), and "Large" (16 - 64 provisioned concurrency).
+        """
+        return pulumi.get(self, "workload_size")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        The name of a served model. It must be unique across an endpoint. If not specified, this field will default to `modelname-modelversion`. A served model name can consist of alphanumeric characters, dashes, and underscores.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="scaleToZeroEnabled")
+    def scale_to_zero_enabled(self) -> Optional[bool]:
+        """
+        Whether the compute resources for the served model should scale down to zero. If scale-to-zero is enabled, the lower bound of the provisioned concurrency for each workload size will be 0. The default value is `true`.
+        """
+        return pulumi.get(self, "scale_to_zero_enabled")
+
+
+@pulumi.output_type
+class ModelServingConfigTrafficConfig(dict):
+    def __init__(__self__, *,
+                 routes: Optional[Sequence['outputs.ModelServingConfigTrafficConfigRoute']] = None):
+        """
+        :param Sequence['ModelServingConfigTrafficConfigRouteArgs'] routes: Each block represents a route that defines traffic to each served model. Each `served_models` block needs to have a corresponding `routes` block
+        """
+        if routes is not None:
+            pulumi.set(__self__, "routes", routes)
+
+    @property
+    @pulumi.getter
+    def routes(self) -> Optional[Sequence['outputs.ModelServingConfigTrafficConfigRoute']]:
+        """
+        Each block represents a route that defines traffic to each served model. Each `served_models` block needs to have a corresponding `routes` block
+        """
+        return pulumi.get(self, "routes")
+
+
+@pulumi.output_type
+class ModelServingConfigTrafficConfigRoute(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "servedModelName":
+            suggest = "served_model_name"
+        elif key == "trafficPercentage":
+            suggest = "traffic_percentage"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ModelServingConfigTrafficConfigRoute. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ModelServingConfigTrafficConfigRoute.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ModelServingConfigTrafficConfigRoute.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 served_model_name: str,
+                 traffic_percentage: int):
+        """
+        :param str served_model_name: The name of the served model this route configures traffic for. This needs to match the name of a `served_models` block
+        :param int traffic_percentage: The percentage of endpoint traffic to send to this route. It must be an integer between 0 and 100 inclusive.
+        """
+        pulumi.set(__self__, "served_model_name", served_model_name)
+        pulumi.set(__self__, "traffic_percentage", traffic_percentage)
+
+    @property
+    @pulumi.getter(name="servedModelName")
+    def served_model_name(self) -> str:
+        """
+        The name of the served model this route configures traffic for. This needs to match the name of a `served_models` block
+        """
+        return pulumi.get(self, "served_model_name")
+
+    @property
+    @pulumi.getter(name="trafficPercentage")
+    def traffic_percentage(self) -> int:
+        """
+        The percentage of endpoint traffic to send to this route. It must be an integer between 0 and 100 inclusive.
+        """
+        return pulumi.get(self, "traffic_percentage")
+
+
+@pulumi.output_type
 class MountAbfs(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "clientId":
             suggest = "client_id"
         elif key == "clientSecretKey":
@@ -10447,14 +10684,33 @@
         """
         The directory ID corresponding to the Azure Active Directory (AAD) tenant of the application
         """
         return pulumi.get(self, "directory_id")
 
 
 @pulumi.output_type
+class StorageCredentialDatabricksGcpServiceAccount(dict):
+    def __init__(__self__, *,
+                 email: Optional[str] = None):
+        """
+        :param str email: The email of the GCP service account created, to be granted access to relevant buckets.
+        """
+        if email is not None:
+            pulumi.set(__self__, "email", email)
+
+    @property
+    @pulumi.getter
+    def email(self) -> Optional[str]:
+        """
+        The email of the GCP service account created, to be granted access to relevant buckets.
+        """
+        return pulumi.get(self, "email")
+
+
+@pulumi.output_type
 class StorageCredentialGcpServiceAccountKey(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "privateKey":
             suggest = "private_key"
         elif key == "privateKeyId":
@@ -10471,21 +10727,27 @@
         StorageCredentialGcpServiceAccountKey.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  email: str,
                  private_key: str,
                  private_key_id: str):
+        """
+        :param str email: The email of the GCP service account created, to be granted access to relevant buckets.
+        """
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "private_key", private_key)
         pulumi.set(__self__, "private_key_id", private_key_id)
 
     @property
     @pulumi.getter
     def email(self) -> str:
+        """
+        The email of the GCP service account created, to be granted access to relevant buckets.
+        """
         return pulumi.get(self, "email")
 
     @property
     @pulumi.getter(name="privateKey")
     def private_key(self) -> str:
         return pulumi.get(self, "private_key")
 
@@ -11496,45 +11758,108 @@
     def zone_id(self) -> Optional[str]:
         return pulumi.get(self, "zone_id")
 
 
 @pulumi.output_type
 class GetClusterClusterInfoInitScriptResult(dict):
     def __init__(__self__, *,
+                 abfss: Optional['outputs.GetClusterClusterInfoInitScriptAbfssResult'] = None,
                  dbfs: Optional['outputs.GetClusterClusterInfoInitScriptDbfsResult'] = None,
+                 file: Optional['outputs.GetClusterClusterInfoInitScriptFileResult'] = None,
+                 gcs: Optional['outputs.GetClusterClusterInfoInitScriptGcsResult'] = None,
                  s3: Optional['outputs.GetClusterClusterInfoInitScriptS3Result'] = None):
+        if abfss is not None:
+            pulumi.set(__self__, "abfss", abfss)
         if dbfs is not None:
             pulumi.set(__self__, "dbfs", dbfs)
+        if file is not None:
+            pulumi.set(__self__, "file", file)
+        if gcs is not None:
+            pulumi.set(__self__, "gcs", gcs)
         if s3 is not None:
             pulumi.set(__self__, "s3", s3)
 
     @property
     @pulumi.getter
+    def abfss(self) -> Optional['outputs.GetClusterClusterInfoInitScriptAbfssResult']:
+        return pulumi.get(self, "abfss")
+
+    @property
+    @pulumi.getter
     def dbfs(self) -> Optional['outputs.GetClusterClusterInfoInitScriptDbfsResult']:
         return pulumi.get(self, "dbfs")
 
     @property
     @pulumi.getter
+    def file(self) -> Optional['outputs.GetClusterClusterInfoInitScriptFileResult']:
+        return pulumi.get(self, "file")
+
+    @property
+    @pulumi.getter
+    def gcs(self) -> Optional['outputs.GetClusterClusterInfoInitScriptGcsResult']:
+        return pulumi.get(self, "gcs")
+
+    @property
+    @pulumi.getter
     def s3(self) -> Optional['outputs.GetClusterClusterInfoInitScriptS3Result']:
         return pulumi.get(self, "s3")
 
 
 @pulumi.output_type
+class GetClusterClusterInfoInitScriptAbfssResult(dict):
+    def __init__(__self__, *,
+                 destination: Optional[str] = None):
+        if destination is not None:
+            pulumi.set(__self__, "destination", destination)
+
+    @property
+    @pulumi.getter
+    def destination(self) -> Optional[str]:
+        return pulumi.get(self, "destination")
+
+
+@pulumi.output_type
 class GetClusterClusterInfoInitScriptDbfsResult(dict):
     def __init__(__self__, *,
                  destination: str):
         pulumi.set(__self__, "destination", destination)
 
     @property
     @pulumi.getter
     def destination(self) -> str:
         return pulumi.get(self, "destination")
 
 
 @pulumi.output_type
+class GetClusterClusterInfoInitScriptFileResult(dict):
+    def __init__(__self__, *,
+                 destination: Optional[str] = None):
+        if destination is not None:
+            pulumi.set(__self__, "destination", destination)
+
+    @property
+    @pulumi.getter
+    def destination(self) -> Optional[str]:
+        return pulumi.get(self, "destination")
+
+
+@pulumi.output_type
+class GetClusterClusterInfoInitScriptGcsResult(dict):
+    def __init__(__self__, *,
+                 destination: Optional[str] = None):
+        if destination is not None:
+            pulumi.set(__self__, "destination", destination)
+
+    @property
+    @pulumi.getter
+    def destination(self) -> Optional[str]:
+        return pulumi.get(self, "destination")
+
+
+@pulumi.output_type
 class GetClusterClusterInfoInitScriptS3Result(dict):
     def __init__(__self__, *,
                  destination: str,
                  canned_acl: Optional[str] = None,
                  enable_encryption: Optional[bool] = None,
                  encryption_type: Optional[str] = None,
                  endpoint: Optional[str] = None,
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/permission_assignment.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/permission_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/permissions.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/pipeline.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/provider.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/recipient.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/recipient.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/repo.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/repo.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/schema.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/secret.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/secret_acl.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/secret_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/secret_scope.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/secret_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/service_principal.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/service_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/service_principal_role.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/service_principal_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/service_principal_secret.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/service_principal_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/share.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/share.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_dashboard.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_endpoint.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_global_config.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_global_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_permissions.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_query.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,17 @@
         if parameters is not None:
             pulumi.set(__self__, "parameters", parameters)
         if parent is not None:
             pulumi.set(__self__, "parent", parent)
         if run_as_role is not None:
             pulumi.set(__self__, "run_as_role", run_as_role)
         if schedule is not None:
+            warnings.warn("""Operations on `databricks_sql_query` schedules are deprecated. Please use `databricks_job` resource to schedule a `sql_task`.""", DeprecationWarning)
+            pulumi.log.warn("""schedule is deprecated: Operations on `databricks_sql_query` schedules are deprecated. Please use `databricks_job` resource to schedule a `sql_task`.""")
+        if schedule is not None:
             pulumi.set(__self__, "schedule", schedule)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="dataSourceId")
     def data_source_id(self) -> pulumi.Input[str]:
@@ -153,14 +156,17 @@
         if parent is not None:
             pulumi.set(__self__, "parent", parent)
         if query is not None:
             pulumi.set(__self__, "query", query)
         if run_as_role is not None:
             pulumi.set(__self__, "run_as_role", run_as_role)
         if schedule is not None:
+            warnings.warn("""Operations on `databricks_sql_query` schedules are deprecated. Please use `databricks_job` resource to schedule a `sql_task`.""", DeprecationWarning)
+            pulumi.log.warn("""schedule is deprecated: Operations on `databricks_sql_query` schedules are deprecated. Please use `databricks_job` resource to schedule a `sql_task`.""")
+        if schedule is not None:
             pulumi.set(__self__, "schedule", schedule)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="dataSourceId")
     def data_source_id(self) -> Optional[pulumi.Input[str]]:
@@ -325,14 +331,17 @@
             __props__.__dict__["name"] = name
             __props__.__dict__["parameters"] = parameters
             __props__.__dict__["parent"] = parent
             if query is None and not opts.urn:
                 raise TypeError("Missing required property 'query'")
             __props__.__dict__["query"] = query
             __props__.__dict__["run_as_role"] = run_as_role
+            if schedule is not None and not opts.urn:
+                warnings.warn("""Operations on `databricks_sql_query` schedules are deprecated. Please use `databricks_job` resource to schedule a `sql_task`.""", DeprecationWarning)
+                pulumi.log.warn("""schedule is deprecated: Operations on `databricks_sql_query` schedules are deprecated. Please use `databricks_job` resource to schedule a `sql_task`.""")
             __props__.__dict__["schedule"] = schedule
             __props__.__dict__["tags"] = tags
         super(SqlQuery, __self__).__init__(
             'databricks:index/sqlQuery:SqlQuery',
             resource_name,
             __props__,
             opts)
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_visualization.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_visualization.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/sql_widget.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/sql_widget.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/storage_credential.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/storage_credential.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @pulumi.input_type
 class StorageCredentialArgs:
     def __init__(__self__, *,
                  aws_iam_role: Optional[pulumi.Input['StorageCredentialAwsIamRoleArgs']] = None,
                  azure_managed_identity: Optional[pulumi.Input['StorageCredentialAzureManagedIdentityArgs']] = None,
                  azure_service_principal: Optional[pulumi.Input['StorageCredentialAzureServicePrincipalArgs']] = None,
                  comment: Optional[pulumi.Input[str]] = None,
+                 databricks_gcp_service_account: Optional[pulumi.Input['StorageCredentialDatabricksGcpServiceAccountArgs']] = None,
                  gcp_service_account_key: Optional[pulumi.Input['StorageCredentialGcpServiceAccountKeyArgs']] = None,
                  metastore_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a StorageCredential resource.
         :param pulumi.Input[str] name: Name of Storage Credentials, which must be unique within the databricks_metastore. Change forces creation of a new resource.
@@ -33,14 +34,16 @@
             pulumi.set(__self__, "aws_iam_role", aws_iam_role)
         if azure_managed_identity is not None:
             pulumi.set(__self__, "azure_managed_identity", azure_managed_identity)
         if azure_service_principal is not None:
             pulumi.set(__self__, "azure_service_principal", azure_service_principal)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
+        if databricks_gcp_service_account is not None:
+            pulumi.set(__self__, "databricks_gcp_service_account", databricks_gcp_service_account)
         if gcp_service_account_key is not None:
             pulumi.set(__self__, "gcp_service_account_key", gcp_service_account_key)
         if metastore_id is not None:
             pulumi.set(__self__, "metastore_id", metastore_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if owner is not None:
@@ -79,14 +82,23 @@
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
     @property
+    @pulumi.getter(name="databricksGcpServiceAccount")
+    def databricks_gcp_service_account(self) -> Optional[pulumi.Input['StorageCredentialDatabricksGcpServiceAccountArgs']]:
+        return pulumi.get(self, "databricks_gcp_service_account")
+
+    @databricks_gcp_service_account.setter
+    def databricks_gcp_service_account(self, value: Optional[pulumi.Input['StorageCredentialDatabricksGcpServiceAccountArgs']]):
+        pulumi.set(self, "databricks_gcp_service_account", value)
+
+    @property
     @pulumi.getter(name="gcpServiceAccountKey")
     def gcp_service_account_key(self) -> Optional[pulumi.Input['StorageCredentialGcpServiceAccountKeyArgs']]:
         return pulumi.get(self, "gcp_service_account_key")
 
     @gcp_service_account_key.setter
     def gcp_service_account_key(self, value: Optional[pulumi.Input['StorageCredentialGcpServiceAccountKeyArgs']]):
         pulumi.set(self, "gcp_service_account_key", value)
@@ -128,14 +140,15 @@
 @pulumi.input_type
 class _StorageCredentialState:
     def __init__(__self__, *,
                  aws_iam_role: Optional[pulumi.Input['StorageCredentialAwsIamRoleArgs']] = None,
                  azure_managed_identity: Optional[pulumi.Input['StorageCredentialAzureManagedIdentityArgs']] = None,
                  azure_service_principal: Optional[pulumi.Input['StorageCredentialAzureServicePrincipalArgs']] = None,
                  comment: Optional[pulumi.Input[str]] = None,
+                 databricks_gcp_service_account: Optional[pulumi.Input['StorageCredentialDatabricksGcpServiceAccountArgs']] = None,
                  gcp_service_account_key: Optional[pulumi.Input['StorageCredentialGcpServiceAccountKeyArgs']] = None,
                  metastore_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering StorageCredential resources.
         :param pulumi.Input[str] name: Name of Storage Credentials, which must be unique within the databricks_metastore. Change forces creation of a new resource.
@@ -145,14 +158,16 @@
             pulumi.set(__self__, "aws_iam_role", aws_iam_role)
         if azure_managed_identity is not None:
             pulumi.set(__self__, "azure_managed_identity", azure_managed_identity)
         if azure_service_principal is not None:
             pulumi.set(__self__, "azure_service_principal", azure_service_principal)
         if comment is not None:
             pulumi.set(__self__, "comment", comment)
+        if databricks_gcp_service_account is not None:
+            pulumi.set(__self__, "databricks_gcp_service_account", databricks_gcp_service_account)
         if gcp_service_account_key is not None:
             pulumi.set(__self__, "gcp_service_account_key", gcp_service_account_key)
         if metastore_id is not None:
             pulumi.set(__self__, "metastore_id", metastore_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if owner is not None:
@@ -191,14 +206,23 @@
         return pulumi.get(self, "comment")
 
     @comment.setter
     def comment(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "comment", value)
 
     @property
+    @pulumi.getter(name="databricksGcpServiceAccount")
+    def databricks_gcp_service_account(self) -> Optional[pulumi.Input['StorageCredentialDatabricksGcpServiceAccountArgs']]:
+        return pulumi.get(self, "databricks_gcp_service_account")
+
+    @databricks_gcp_service_account.setter
+    def databricks_gcp_service_account(self, value: Optional[pulumi.Input['StorageCredentialDatabricksGcpServiceAccountArgs']]):
+        pulumi.set(self, "databricks_gcp_service_account", value)
+
+    @property
     @pulumi.getter(name="gcpServiceAccountKey")
     def gcp_service_account_key(self) -> Optional[pulumi.Input['StorageCredentialGcpServiceAccountKeyArgs']]:
         return pulumi.get(self, "gcp_service_account_key")
 
     @gcp_service_account_key.setter
     def gcp_service_account_key(self, value: Optional[pulumi.Input['StorageCredentialGcpServiceAccountKeyArgs']]):
         pulumi.set(self, "gcp_service_account_key", value)
@@ -242,14 +266,15 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aws_iam_role: Optional[pulumi.Input[pulumi.InputType['StorageCredentialAwsIamRoleArgs']]] = None,
                  azure_managed_identity: Optional[pulumi.Input[pulumi.InputType['StorageCredentialAzureManagedIdentityArgs']]] = None,
                  azure_service_principal: Optional[pulumi.Input[pulumi.InputType['StorageCredentialAzureServicePrincipalArgs']]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
+                 databricks_gcp_service_account: Optional[pulumi.Input[pulumi.InputType['StorageCredentialDatabricksGcpServiceAccountArgs']]] = None,
                  gcp_service_account_key: Optional[pulumi.Input[pulumi.InputType['StorageCredentialGcpServiceAccountKeyArgs']]] = None,
                  metastore_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         To work with external tables, Unity Catalog introduces two new objects to access and work with external cloud storage:
@@ -278,40 +303,44 @@
             )])
         ```
 
         For Azure
 
         ```python
         import pulumi
-        import pulumi_azure as azure
         import pulumi_databricks as databricks
 
-        this = azure.core.get_resource_group(name="example-rg")
-        example = azure.databricks.AccessConnector("example",
-            resource_group_name=azurerm_resource_group["this"]["name"],
-            location=azurerm_resource_group["this"]["location"],
-            identity=azure.databricks.AccessConnectorIdentityArgs(
-                type="SystemAssigned",
-            ),
-            tags={
-                "Environment": "Production",
-            })
         external_mi = databricks.StorageCredential("externalMi",
             azure_managed_identity=databricks.StorageCredentialAzureManagedIdentityArgs(
-                access_connector_id=example.id,
+                access_connector_id=azurerm_databricks_access_connector["example"]["id"],
             ),
             comment="Managed identity credential managed by TF")
         external_creds = databricks.Grants("externalCreds",
             storage_credential=databricks_storage_credential["external"]["id"],
             grants=[databricks.GrantsGrantArgs(
                 principal="Data Engineers",
                 privileges=["CREATE_TABLE"],
             )])
         ```
 
+        For GCP
+
+        ```python
+        import pulumi
+        import pulumi_databricks as databricks
+
+        external = databricks.StorageCredential("external", databricks_gcp_service_account=databricks.StorageCredentialDatabricksGcpServiceAccountArgs())
+        external_creds = databricks.Grants("externalCreds",
+            storage_credential=external.id,
+            grants=[databricks.GrantsGrantArgs(
+                principal="Data Engineers",
+                privileges=["CREATE_TABLE"],
+            )])
+        ```
+
         ## Import
 
         This resource can be imported by namebash
 
         ```sh
          $ pulumi import databricks:index/storageCredential:StorageCredential this <name>
         ```
@@ -354,40 +383,44 @@
             )])
         ```
 
         For Azure
 
         ```python
         import pulumi
-        import pulumi_azure as azure
         import pulumi_databricks as databricks
 
-        this = azure.core.get_resource_group(name="example-rg")
-        example = azure.databricks.AccessConnector("example",
-            resource_group_name=azurerm_resource_group["this"]["name"],
-            location=azurerm_resource_group["this"]["location"],
-            identity=azure.databricks.AccessConnectorIdentityArgs(
-                type="SystemAssigned",
-            ),
-            tags={
-                "Environment": "Production",
-            })
         external_mi = databricks.StorageCredential("externalMi",
             azure_managed_identity=databricks.StorageCredentialAzureManagedIdentityArgs(
-                access_connector_id=example.id,
+                access_connector_id=azurerm_databricks_access_connector["example"]["id"],
             ),
             comment="Managed identity credential managed by TF")
         external_creds = databricks.Grants("externalCreds",
             storage_credential=databricks_storage_credential["external"]["id"],
             grants=[databricks.GrantsGrantArgs(
                 principal="Data Engineers",
                 privileges=["CREATE_TABLE"],
             )])
         ```
 
+        For GCP
+
+        ```python
+        import pulumi
+        import pulumi_databricks as databricks
+
+        external = databricks.StorageCredential("external", databricks_gcp_service_account=databricks.StorageCredentialDatabricksGcpServiceAccountArgs())
+        external_creds = databricks.Grants("externalCreds",
+            storage_credential=external.id,
+            grants=[databricks.GrantsGrantArgs(
+                principal="Data Engineers",
+                privileges=["CREATE_TABLE"],
+            )])
+        ```
+
         ## Import
 
         This resource can be imported by namebash
 
         ```sh
          $ pulumi import databricks:index/storageCredential:StorageCredential this <name>
         ```
@@ -407,14 +440,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aws_iam_role: Optional[pulumi.Input[pulumi.InputType['StorageCredentialAwsIamRoleArgs']]] = None,
                  azure_managed_identity: Optional[pulumi.Input[pulumi.InputType['StorageCredentialAzureManagedIdentityArgs']]] = None,
                  azure_service_principal: Optional[pulumi.Input[pulumi.InputType['StorageCredentialAzureServicePrincipalArgs']]] = None,
                  comment: Optional[pulumi.Input[str]] = None,
+                 databricks_gcp_service_account: Optional[pulumi.Input[pulumi.InputType['StorageCredentialDatabricksGcpServiceAccountArgs']]] = None,
                  gcp_service_account_key: Optional[pulumi.Input[pulumi.InputType['StorageCredentialGcpServiceAccountKeyArgs']]] = None,
                  metastore_id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  owner: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
@@ -424,14 +458,15 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = StorageCredentialArgs.__new__(StorageCredentialArgs)
 
             __props__.__dict__["aws_iam_role"] = aws_iam_role
             __props__.__dict__["azure_managed_identity"] = azure_managed_identity
             __props__.__dict__["azure_service_principal"] = azure_service_principal
             __props__.__dict__["comment"] = comment
+            __props__.__dict__["databricks_gcp_service_account"] = databricks_gcp_service_account
             __props__.__dict__["gcp_service_account_key"] = gcp_service_account_key
             __props__.__dict__["metastore_id"] = metastore_id
             __props__.__dict__["name"] = name
             __props__.__dict__["owner"] = owner
         super(StorageCredential, __self__).__init__(
             'databricks:index/storageCredential:StorageCredential',
             resource_name,
@@ -442,14 +477,15 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             aws_iam_role: Optional[pulumi.Input[pulumi.InputType['StorageCredentialAwsIamRoleArgs']]] = None,
             azure_managed_identity: Optional[pulumi.Input[pulumi.InputType['StorageCredentialAzureManagedIdentityArgs']]] = None,
             azure_service_principal: Optional[pulumi.Input[pulumi.InputType['StorageCredentialAzureServicePrincipalArgs']]] = None,
             comment: Optional[pulumi.Input[str]] = None,
+            databricks_gcp_service_account: Optional[pulumi.Input[pulumi.InputType['StorageCredentialDatabricksGcpServiceAccountArgs']]] = None,
             gcp_service_account_key: Optional[pulumi.Input[pulumi.InputType['StorageCredentialGcpServiceAccountKeyArgs']]] = None,
             metastore_id: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             owner: Optional[pulumi.Input[str]] = None) -> 'StorageCredential':
         """
         Get an existing StorageCredential resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
@@ -464,14 +500,15 @@
 
         __props__ = _StorageCredentialState.__new__(_StorageCredentialState)
 
         __props__.__dict__["aws_iam_role"] = aws_iam_role
         __props__.__dict__["azure_managed_identity"] = azure_managed_identity
         __props__.__dict__["azure_service_principal"] = azure_service_principal
         __props__.__dict__["comment"] = comment
+        __props__.__dict__["databricks_gcp_service_account"] = databricks_gcp_service_account
         __props__.__dict__["gcp_service_account_key"] = gcp_service_account_key
         __props__.__dict__["metastore_id"] = metastore_id
         __props__.__dict__["name"] = name
         __props__.__dict__["owner"] = owner
         return StorageCredential(resource_name, opts=opts, __props__=__props__)
 
     @property
@@ -491,14 +528,19 @@
 
     @property
     @pulumi.getter
     def comment(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "comment")
 
     @property
+    @pulumi.getter(name="databricksGcpServiceAccount")
+    def databricks_gcp_service_account(self) -> pulumi.Output['outputs.StorageCredentialDatabricksGcpServiceAccount']:
+        return pulumi.get(self, "databricks_gcp_service_account")
+
+    @property
     @pulumi.getter(name="gcpServiceAccountKey")
     def gcp_service_account_key(self) -> pulumi.Output[Optional['outputs.StorageCredentialGcpServiceAccountKey']]:
         return pulumi.get(self, "gcp_service_account_key")
 
     @property
     @pulumi.getter(name="metastoreId")
     def metastore_id(self) -> pulumi.Output[str]:
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/table.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/table.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/token.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/user.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/user_instance_profile.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/user_instance_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/user_role.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/user_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks/workspace_conf.py` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks/workspace_conf.py`

 * *Files identical despite different names*

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks.egg-info/PKG-INFO` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-databricks
-Version: 1.8.0a1678127428
+Version: 1.9.0a1678745257
 Summary: A Pulumi package for creating and managing databricks cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-databricks
 Keywords: pulumi databricks category/infrastructure
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_databricks-1.8.0a1678127428/pulumi_databricks.egg-info/SOURCES.txt` & `pulumi_databricks-1.9.0a1678745257/pulumi_databricks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 pulumi_databricks/metastore.py
 pulumi_databricks/metastore_assignment.py
 pulumi_databricks/metastore_data_access.py
 pulumi_databricks/metastore_provider.py
 pulumi_databricks/mlflow_experiment.py
 pulumi_databricks/mlflow_model.py
 pulumi_databricks/mlflow_webhook.py
+pulumi_databricks/model_serving.py
 pulumi_databricks/mount.py
 pulumi_databricks/mws_credentials.py
 pulumi_databricks/mws_customer_managed_keys.py
 pulumi_databricks/mws_log_delivery.py
 pulumi_databricks/mws_networks.py
 pulumi_databricks/mws_permission_assignment.py
 pulumi_databricks/mws_private_access_settings.py
```

### Comparing `pulumi_databricks-1.8.0a1678127428/setup.py` & `pulumi_databricks-1.9.0a1678745257/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.8.0a1678127428"
-PLUGIN_VERSION = "1.8.0-alpha.1678127428+5d921b2b"
+VERSION = "1.9.0a1678745257"
+PLUGIN_VERSION = "1.9.0-alpha.1678745257+e731a7fd"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'databricks', PLUGIN_VERSION])
         except OSError as error:
```

