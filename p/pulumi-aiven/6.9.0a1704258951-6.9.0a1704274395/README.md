# Comparing `tmp/pulumi_aiven-6.9.0a1704258951.tar.gz` & `tmp/pulumi_aiven-6.9.0a1704274395.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aiven-6.9.0a1704258951.tar", last modified: Wed Jan  3 05:19:54 2024, max compression
+gzip compressed data, was "pulumi_aiven-6.9.0a1704274395.tar", last modified: Wed Jan  3 09:36:59 2024, max compression
```

## Comparing `pulumi_aiven-6.9.0a1704258951.tar` & `pulumi_aiven-6.9.0a1704274395.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:19:54.945131 pulumi_aiven-6.9.0a1704258951/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-01-03 05:19:54.945131 pulumi_aiven-6.9.0a1704258951/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:19:54.941131 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/
--rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   800515 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    18336 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    36913 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account_team.py
--rw-r--r--   0 runner    (1001) docker     (127)    17174 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15297 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    18483 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    18159 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/azure_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    33976 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    77687 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/cassandra.py
--rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    77872 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    17227 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    26764 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:19:54.945131 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    26197 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    77215 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/flink.py
--rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/flink_application.py
--rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/flink_application_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/gcp_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    16110 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/gcp_privatelink_connection_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)    15247 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account_team_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account_team_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_aws_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_aws_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_azure_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_azure_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_billing_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22935 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_cassanda.py
--rw-r--r--   0 runner    (1001) docker     (127)    22604 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_cassandra.py
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_cassandra_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22681 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_clickhouse_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_clickhouse_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_flink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_flink_application.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_flink_application_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_gcp_privatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_gcp_vpc_peering_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    22462 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_grafana.py
--rw-r--r--   0 runner    (1001) docker     (127)    22540 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_influx_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    22839 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    23112 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22786 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22291 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_m3_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13941 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    22368 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_my_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_open_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_opensearch_security_plugin_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_organization_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_organization_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_pg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_pg_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_pg_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_project_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22335 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_service_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    18127 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_transit_gateway_vpc_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    80219 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/grafana.py
--rw-r--r--   0 runner    (1001) docker     (127)    77408 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/influx_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/influxdb_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    19380 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/influxdb_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    82490 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    81682 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    24756 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    82294 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_mirror_maker.py
--rw-r--r--   0 runner    (1001) docker     (127)    23081 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_schema_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    24119 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    81082 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/m3_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)    79856 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/m3_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    40445 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/mirror_maker_replication_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    80493 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/my_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/mysql_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/mysql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    78329 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/open_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    18471 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/open_search_acl_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22685 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/open_search_acl_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/opensearch_security_plugin_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10803 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/organization_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/organization_user_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/organizational_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)  1125235 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    75652 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/pg.py
--rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/pg_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/pg_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    45996 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/project_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13331 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/project_vpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    79989 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)    30212 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    53125 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    59286 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/service_integration_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/static_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven/transit_gateway_vpc_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 05:19:54.945131 pulumi_aiven-6.9.0a1704258951/pulumi_aiven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-01-03 05:19:54.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-01-03 05:19:54.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 05:19:54.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-03 05:19:54.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-03 05:19:54.000000 pulumi_aiven-6.9.0a1704258951/pulumi_aiven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-03 05:19:41.000000 pulumi_aiven-6.9.0a1704258951/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 05:19:54.945131 pulumi_aiven-6.9.0a1704258951/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 09:36:59.734400 pulumi_aiven-6.9.0a1704274395/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-01-03 09:36:59.734400 pulumi_aiven-6.9.0a1704274395/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 09:36:59.730400 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/
+-rw-r--r--   0 runner    (1001) docker     (127)    16645 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   800515 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18336 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36913 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17174 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15297 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18483 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18159 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/azure_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33976 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77687 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77872 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17227 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26764 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16426 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 09:36:59.734400 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26197 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77215 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/flink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17471 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22264 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/flink_application_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/gcp_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16110 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/gcp_privatelink_connection_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15247 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account_team_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_aws_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_aws_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_azure_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_azure_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22935 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_cassanda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22604 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_cassandra_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22681 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_clickhouse_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_clickhouse_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9261 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_flink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_flink_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_flink_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_gcp_privatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_gcp_vpc_peering_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22462 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_grafana.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22540 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22839 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23112 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22786 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22291 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13941 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22368 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_open_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_opensearch_security_plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_organization_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_project_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22335 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_service_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18127 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_transit_gateway_vpc_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80219 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77408 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/influx_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/influxdb_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19380 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/influxdb_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82490 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81682 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24756 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82294 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_mirror_maker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23081 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_schema_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19053 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24119 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81082 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/m3_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79856 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/m3_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40445 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/mirror_maker_replication_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80493 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/my_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/mysql_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/mysql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78329 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/open_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18471 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/open_search_acl_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22685 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/open_search_acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/opensearch_security_plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10803 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/organization_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/organization_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/organizational_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1125235 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75652 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/pg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22840 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/pg_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/pg_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45996 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/project_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13331 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/project_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    79989 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30212 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53125 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59286 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/service_integration_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven/transit_gateway_vpc_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 09:36:59.734400 pulumi_aiven-6.9.0a1704274395/pulumi_aiven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-01-03 09:36:59.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-01-03 09:36:59.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 09:36:59.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-03 09:36:59.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-03 09:36:59.000000 pulumi_aiven-6.9.0a1704274395/pulumi_aiven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-03 09:36:48.000000 pulumi_aiven-6.9.0a1704274395/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 09:36:59.734400 pulumi_aiven-6.9.0a1704274395/setup.cfg
```

### Comparing `pulumi_aiven-6.9.0a1704258951/PKG-INFO` & `pulumi_aiven-6.9.0a1704274395/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.9.0a1704258951
+Version: 6.9.0a1704274395
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi,aiven
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_aiven-6.9.0a1704258951/README.md` & `pulumi_aiven-6.9.0a1704274395/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/__init__.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/_inputs.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/_utilities.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account_authentication.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account_team.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account_team_member.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/account_team_project.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/aws_privatelink.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/aws_vpc_peering_connection.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/azure_privatelink.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/azure_privatelink_connection_approval.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/azure_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/azure_vpc_peering_connection.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/billing_group.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/cassandra.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/cassandra_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse_database.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse_grant.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse_role.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/clickhouse_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/config/vars.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/connection_pool.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/flink.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/flink_application.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/flink_application_deployment.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/flink_application_deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/flink_application_version.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/gcp_privatelink.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/gcp_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/gcp_privatelink_connection_approval.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/gcp_privatelink_connection_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/gcp_vpc_peering_connection.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account_authentication.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account_team.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account_team_member.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account_team_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_account_team_project.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_account_team_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_aws_privatelink.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_aws_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_aws_vpc_peering_connection.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_aws_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_azure_privatelink.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_azure_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_azure_vpc_peering_connection.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_azure_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_billing_group.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_billing_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_cassanda.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_cassanda.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_cassandra.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_cassandra.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_cassandra_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_cassandra_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_clickhouse.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_clickhouse.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_clickhouse_database.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_clickhouse_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_clickhouse_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_clickhouse_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_connection_pool.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_flink.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_flink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_flink_application.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_flink_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_flink_application_version.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_flink_application_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_gcp_privatelink.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_gcp_privatelink.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_gcp_vpc_peering_connection.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_gcp_vpc_peering_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_grafana.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_influx_db.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_influxdb_database.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_influxdb_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_acl.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_connect.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_connector.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_mirror_maker.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_schema.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_schema_configuration.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_schema_registry_acl.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_topic.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_kafka_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_m3_aggregator.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_m3_db.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_m3db_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_mirror_maker_replication_flow.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_my_sql.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_mysql_database.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_mysql_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_open_search.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_open_search_acl_config.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_open_search_acl_rule.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_opensearch_security_plugin_config.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_opensearch_security_plugin_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_opensearch_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_organization.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_organization_user_group.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_organization_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_organizational_unit.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_pg.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_pg_database.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_pg_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_project.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_project_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_project_vpc.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_redis.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_redis_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_service_component.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_service_component.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_service_integration.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_service_integration_endpoint.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/get_transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/get_transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/grafana.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/grafana.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/influx_db.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/influx_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/influxdb_database.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/influxdb_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/influxdb_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_acl.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_connect.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_connect.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_connector.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_mirror_maker.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_mirror_maker.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_schema.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_schema_configuration.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_schema_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_schema_registry_acl.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_topic.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/kafka_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/kafka_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/m3_aggregator.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/m3_aggregator.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/m3_db.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/m3_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/m3db_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/mirror_maker_replication_flow.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/mirror_maker_replication_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/my_sql.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/my_sql.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/mysql_database.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/mysql_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/mysql_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/mysql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/open_search.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/open_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/open_search_acl_config.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/open_search_acl_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/open_search_acl_rule.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/open_search_acl_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/opensearch_security_plugin_config.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/opensearch_security_plugin_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/opensearch_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/organization.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/organization_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/organization_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -52,40 +52,53 @@
 @pulumi.input_type
 class _OrganizationUserState:
     def __init__(__self__, *,
                  accepted: Optional[pulumi.Input[bool]] = None,
                  create_time: Optional[pulumi.Input[str]] = None,
                  invited_by: Optional[pulumi.Input[str]] = None,
                  organization_id: Optional[pulumi.Input[str]] = None,
-                 user_email: Optional[pulumi.Input[str]] = None):
+                 user_email: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering OrganizationUser resources.
         :param pulumi.Input[bool] accepted: This is a boolean flag that determines whether an invitation was accepted or not by the user. `false` value means that the invitation was sent to the user but not yet accepted. `true` means that the user accepted the invitation and now a member of an organization.
         :param pulumi.Input[str] create_time: Time of creation
         :param pulumi.Input[str] invited_by: The email address of the user who sent an invitation to the user.
         :param pulumi.Input[str] organization_id: The unique organization ID. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] user_email: This is a user email address that first will be invited, and after accepting an invitation, they become a member of the organization. Should be lowercase. This property cannot be changed, doing so forces recreation of the resource.
+        :param pulumi.Input[str] user_id: The unique organization user ID
         """
         if accepted is not None:
+            warnings.warn("""This field is deprecated and will be removed in the next major release. """, DeprecationWarning)
+            pulumi.log.warn("""accepted is deprecated: This field is deprecated and will be removed in the next major release. """)
+        if accepted is not None:
             pulumi.set(__self__, "accepted", accepted)
         if create_time is not None:
             pulumi.set(__self__, "create_time", create_time)
         if invited_by is not None:
+            warnings.warn("""This field is deprecated and will be removed in the next major release. """, DeprecationWarning)
+            pulumi.log.warn("""invited_by is deprecated: This field is deprecated and will be removed in the next major release. """)
+        if invited_by is not None:
             pulumi.set(__self__, "invited_by", invited_by)
         if organization_id is not None:
             pulumi.set(__self__, "organization_id", organization_id)
         if user_email is not None:
             pulumi.set(__self__, "user_email", user_email)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
 
     @property
     @pulumi.getter
     def accepted(self) -> Optional[pulumi.Input[bool]]:
         """
         This is a boolean flag that determines whether an invitation was accepted or not by the user. `false` value means that the invitation was sent to the user but not yet accepted. `true` means that the user accepted the invitation and now a member of an organization.
         """
+        warnings.warn("""This field is deprecated and will be removed in the next major release. """, DeprecationWarning)
+        pulumi.log.warn("""accepted is deprecated: This field is deprecated and will be removed in the next major release. """)
+
         return pulumi.get(self, "accepted")
 
     @accepted.setter
     def accepted(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "accepted", value)
 
     @property
@@ -102,14 +115,17 @@
 
     @property
     @pulumi.getter(name="invitedBy")
     def invited_by(self) -> Optional[pulumi.Input[str]]:
         """
         The email address of the user who sent an invitation to the user.
         """
+        warnings.warn("""This field is deprecated and will be removed in the next major release. """, DeprecationWarning)
+        pulumi.log.warn("""invited_by is deprecated: This field is deprecated and will be removed in the next major release. """)
+
         return pulumi.get(self, "invited_by")
 
     @invited_by.setter
     def invited_by(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "invited_by", value)
 
     @property
@@ -132,14 +148,26 @@
         """
         return pulumi.get(self, "user_email")
 
     @user_email.setter
     def user_email(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_email", value)
 
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The unique organization user ID
+        """
+        return pulumi.get(self, "user_id")
+
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_id", value)
+
 
 class OrganizationUser(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  organization_id: Optional[pulumi.Input[str]] = None,
@@ -205,59 +233,66 @@
             __props__.__dict__["organization_id"] = organization_id
             if user_email is None and not opts.urn:
                 raise TypeError("Missing required property 'user_email'")
             __props__.__dict__["user_email"] = user_email
             __props__.__dict__["accepted"] = None
             __props__.__dict__["create_time"] = None
             __props__.__dict__["invited_by"] = None
+            __props__.__dict__["user_id"] = None
         super(OrganizationUser, __self__).__init__(
             'aiven:index/organizationUser:OrganizationUser',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             accepted: Optional[pulumi.Input[bool]] = None,
             create_time: Optional[pulumi.Input[str]] = None,
             invited_by: Optional[pulumi.Input[str]] = None,
             organization_id: Optional[pulumi.Input[str]] = None,
-            user_email: Optional[pulumi.Input[str]] = None) -> 'OrganizationUser':
+            user_email: Optional[pulumi.Input[str]] = None,
+            user_id: Optional[pulumi.Input[str]] = None) -> 'OrganizationUser':
         """
         Get an existing OrganizationUser resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] accepted: This is a boolean flag that determines whether an invitation was accepted or not by the user. `false` value means that the invitation was sent to the user but not yet accepted. `true` means that the user accepted the invitation and now a member of an organization.
         :param pulumi.Input[str] create_time: Time of creation
         :param pulumi.Input[str] invited_by: The email address of the user who sent an invitation to the user.
         :param pulumi.Input[str] organization_id: The unique organization ID. This property cannot be changed, doing so forces recreation of the resource.
         :param pulumi.Input[str] user_email: This is a user email address that first will be invited, and after accepting an invitation, they become a member of the organization. Should be lowercase. This property cannot be changed, doing so forces recreation of the resource.
+        :param pulumi.Input[str] user_id: The unique organization user ID
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _OrganizationUserState.__new__(_OrganizationUserState)
 
         __props__.__dict__["accepted"] = accepted
         __props__.__dict__["create_time"] = create_time
         __props__.__dict__["invited_by"] = invited_by
         __props__.__dict__["organization_id"] = organization_id
         __props__.__dict__["user_email"] = user_email
+        __props__.__dict__["user_id"] = user_id
         return OrganizationUser(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def accepted(self) -> pulumi.Output[bool]:
         """
         This is a boolean flag that determines whether an invitation was accepted or not by the user. `false` value means that the invitation was sent to the user but not yet accepted. `true` means that the user accepted the invitation and now a member of an organization.
         """
+        warnings.warn("""This field is deprecated and will be removed in the next major release. """, DeprecationWarning)
+        pulumi.log.warn("""accepted is deprecated: This field is deprecated and will be removed in the next major release. """)
+
         return pulumi.get(self, "accepted")
 
     @property
     @pulumi.getter(name="createTime")
     def create_time(self) -> pulumi.Output[str]:
         """
         Time of creation
@@ -266,14 +301,17 @@
 
     @property
     @pulumi.getter(name="invitedBy")
     def invited_by(self) -> pulumi.Output[str]:
         """
         The email address of the user who sent an invitation to the user.
         """
+        warnings.warn("""This field is deprecated and will be removed in the next major release. """, DeprecationWarning)
+        pulumi.log.warn("""invited_by is deprecated: This field is deprecated and will be removed in the next major release. """)
+
         return pulumi.get(self, "invited_by")
 
     @property
     @pulumi.getter(name="organizationId")
     def organization_id(self) -> pulumi.Output[str]:
         """
         The unique organization ID. This property cannot be changed, doing so forces recreation of the resource.
@@ -284,7 +322,15 @@
     @pulumi.getter(name="userEmail")
     def user_email(self) -> pulumi.Output[str]:
         """
         This is a user email address that first will be invited, and after accepting an invitation, they become a member of the organization. Should be lowercase. This property cannot be changed, doing so forces recreation of the resource.
         """
         return pulumi.get(self, "user_email")
 
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Output[str]:
+        """
+        The unique organization user ID
+        """
+        return pulumi.get(self, "user_id")
+
```

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/organization_user_group.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/organization_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/organizational_unit.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/organizational_unit.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/outputs.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/pg.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/pg.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/pg_database.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/pg_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/pg_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/pg_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/project.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/project_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/project_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/project_vpc.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/project_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/provider.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/redis.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/redis.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/redis_user.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/service_integration.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/service_integration_endpoint.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/service_integration_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/static_ip.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/static_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven/transit_gateway_vpc_attachment.py` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven/transit_gateway_vpc_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven.egg-info/PKG-INFO` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aiven
-Version: 6.9.0a1704258951
+Version: 6.9.0a1704274395
 Summary: A Pulumi package for creating and managing Aiven cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-aiven
 Keywords: pulumi,aiven
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_aiven-6.9.0a1704258951/pulumi_aiven.egg-info/SOURCES.txt` & `pulumi_aiven-6.9.0a1704274395/pulumi_aiven.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_aiven-6.9.0a1704258951/pyproject.toml` & `pulumi_aiven-6.9.0a1704274395/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_aiven"
   description = "A Pulumi package for creating and managing Aiven cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "aiven"]
   readme = "README.md"
   requires-python = ">=3.7"
-  version = "6.9.0a1704258951"
+  version = "6.9.0a1704274395"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-aiven"
 
 [build-system]
```

