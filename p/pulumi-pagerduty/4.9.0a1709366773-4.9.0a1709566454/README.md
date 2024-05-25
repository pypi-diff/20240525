# Comparing `tmp/pulumi_pagerduty-4.9.0a1709366773.tar.gz` & `tmp/pulumi_pagerduty-4.9.0a1709566454.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_pagerduty-4.9.0a1709366773.tar", last modified: Sat Mar  2 08:12:17 2024, max compression
+gzip compressed data, was "pulumi_pagerduty-4.9.0a1709566454.tar", last modified: Mon Mar  4 15:56:17 2024, max compression
```

## Comparing `pulumi_pagerduty-4.9.0a1709366773.tar` & `pulumi_pagerduty-4.9.0a1709566454.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 08:12:17.737364 pulumi_pagerduty-4.9.0a1709366773/
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-02 08:12:17.737364 pulumi_pagerduty-4.9.0a1709366773/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 08:12:17.733363 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/
--rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   332722 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/addon.py
--rw-r--r--   0 runner    (1001) docker     (127)    29736 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    12379 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_action_service_association.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_action_team_association.py
--rw-r--r--   0 runner    (1001) docker     (127)    21639 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_runner_team_association.py
--rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/business_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13703 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/business_service_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 08:12:17.733363 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/escalation_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14738 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration.py
--rw-r--r--   0 runner    (1001) docker     (127)    22396 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_global.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17341 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    32623 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17913 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_unrouted.py
--rw-r--r--   0 runner    (1001) docker     (127)    21924 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    31642 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/extension_service_now.py
--rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_automation_actions_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_automation_actions_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_business_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_escalation_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_event_orchestration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_event_orchestration_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_event_orchestrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_extension_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_incident_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_incident_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_priority.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_ruleset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_service_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_team_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_user_contact_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_vendor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/incident_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/incident_custom_field_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    13573 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/incident_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    19556 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/incident_workflow_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15820 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (127)   297031 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    37277 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/response_play.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/ruleset.py
--rw-r--r--   0 runner    (1001) docker     (127)    32019 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/ruleset_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23490 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    59033 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/service_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)    26813 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/service_event_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    46642 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/service_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    25945 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/slack_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/tag_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/team_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    35044 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/user_contact_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/user_notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    27122 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/webhook_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 08:12:17.737364 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-02 08:12:17.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-03-02 08:12:17.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 08:12:17.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-02 08:12:17.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-02 08:12:17.000000 pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-02 08:12:10.000000 pulumi_pagerduty-4.9.0a1709366773/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 08:12:17.737364 pulumi_pagerduty-4.9.0a1709366773/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:56:17.725324 pulumi_pagerduty-4.9.0a1709566454/
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-04 15:56:17.725324 pulumi_pagerduty-4.9.0a1709566454/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:56:17.725324 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (127)    10843 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   342174 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/addon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29736 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12379 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_action_service_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_action_team_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21639 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_runner_team_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19315 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/business_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13703 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/business_service_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:56:17.725324 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/escalation_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14738 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22396 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17341 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33737 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17913 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_unrouted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21924 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24565 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31642 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/extension_service_now.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_automation_actions_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_automation_actions_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_business_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_escalation_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_event_orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_event_orchestration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_event_orchestrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_extension_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_incident_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_incident_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11726 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8000 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_standards_resource_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_standards_resources_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_team_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_user_contact_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/incident_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/incident_custom_field_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13573 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/incident_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19556 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/incident_workflow_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15820 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)   317666 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    37277 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/response_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32019 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/ruleset_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23490 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59033 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/service_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26813 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/service_event_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46642 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/service_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25945 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/slack_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/tag_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/team_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35044 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/user_contact_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17613 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/user_notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27122 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/webhook_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 15:56:17.725324 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-04 15:56:17.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-03-04 15:56:17.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 15:56:17.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-04 15:56:17.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 15:56:17.000000 pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-04 15:56:10.000000 pulumi_pagerduty-4.9.0a1709566454/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 15:56:17.725324 pulumi_pagerduty-4.9.0a1709566454/setup.cfg
```

### Comparing `pulumi_pagerduty-4.9.0a1709366773/PKG-INFO` & `pulumi_pagerduty-4.9.0a1709566454/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_pagerduty
-Version: 4.9.0a1709366773
+Version: 4.9.0a1709566454
 Summary: A Pulumi package for creating and managing pagerduty cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-pagerduty
 Keywords: pulumi,pagerduty
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_pagerduty-4.9.0a1709366773/README.md` & `pulumi_pagerduty-4.9.0a1709566454/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/__init__.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 from .get_license import *
 from .get_licenses import *
 from .get_priority import *
 from .get_ruleset import *
 from .get_schedule import *
 from .get_service import *
 from .get_service_integration import *
+from .get_standards import *
+from .get_standards_resource_scores import *
+from .get_standards_resources_scores import *
 from .get_tag import *
 from .get_team import *
 from .get_team_members import *
 from .get_user import *
 from .get_user_contact_method import *
 from .get_users import *
 from .get_vendor import *
```

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/_inputs.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,24 @@
     'EscalationPolicyRuleTargetArgs',
     'EventOrchestrationGlobalCatchAllArgs',
     'EventOrchestrationGlobalCatchAllActionsArgs',
     'EventOrchestrationGlobalCatchAllActionsAutomationActionArgs',
     'EventOrchestrationGlobalCatchAllActionsAutomationActionHeaderArgs',
     'EventOrchestrationGlobalCatchAllActionsAutomationActionParameterArgs',
     'EventOrchestrationGlobalCatchAllActionsExtractionArgs',
+    'EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdateArgs',
     'EventOrchestrationGlobalCatchAllActionsVariableArgs',
     'EventOrchestrationGlobalSetArgs',
     'EventOrchestrationGlobalSetRuleArgs',
     'EventOrchestrationGlobalSetRuleActionsArgs',
     'EventOrchestrationGlobalSetRuleActionsAutomationActionArgs',
     'EventOrchestrationGlobalSetRuleActionsAutomationActionHeaderArgs',
     'EventOrchestrationGlobalSetRuleActionsAutomationActionParameterArgs',
     'EventOrchestrationGlobalSetRuleActionsExtractionArgs',
+    'EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdateArgs',
     'EventOrchestrationGlobalSetRuleActionsVariableArgs',
     'EventOrchestrationGlobalSetRuleConditionArgs',
     'EventOrchestrationIntegrationArgs',
     'EventOrchestrationIntegrationParameterArgs',
     'EventOrchestrationRouterCatchAllArgs',
     'EventOrchestrationRouterCatchAllActionsArgs',
     'EventOrchestrationRouterSetArgs',
@@ -40,23 +42,25 @@
     'EventOrchestrationRouterSetRuleConditionArgs',
     'EventOrchestrationServiceCatchAllArgs',
     'EventOrchestrationServiceCatchAllActionsArgs',
     'EventOrchestrationServiceCatchAllActionsAutomationActionArgs',
     'EventOrchestrationServiceCatchAllActionsAutomationActionHeaderArgs',
     'EventOrchestrationServiceCatchAllActionsAutomationActionParameterArgs',
     'EventOrchestrationServiceCatchAllActionsExtractionArgs',
+    'EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdateArgs',
     'EventOrchestrationServiceCatchAllActionsPagerdutyAutomationActionArgs',
     'EventOrchestrationServiceCatchAllActionsVariableArgs',
     'EventOrchestrationServiceSetArgs',
     'EventOrchestrationServiceSetRuleArgs',
     'EventOrchestrationServiceSetRuleActionsArgs',
     'EventOrchestrationServiceSetRuleActionsAutomationActionArgs',
     'EventOrchestrationServiceSetRuleActionsAutomationActionHeaderArgs',
     'EventOrchestrationServiceSetRuleActionsAutomationActionParameterArgs',
     'EventOrchestrationServiceSetRuleActionsExtractionArgs',
+    'EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdateArgs',
     'EventOrchestrationServiceSetRuleActionsPagerdutyAutomationActionArgs',
     'EventOrchestrationServiceSetRuleActionsVariableArgs',
     'EventOrchestrationServiceSetRuleConditionArgs',
     'EventOrchestrationUnroutedCatchAllArgs',
     'EventOrchestrationUnroutedCatchAllActionsArgs',
     'EventOrchestrationUnroutedCatchAllActionsExtractionArgs',
     'EventOrchestrationUnroutedCatchAllActionsVariableArgs',
@@ -381,26 +385,28 @@
 class EventOrchestrationGlobalCatchAllActionsArgs:
     def __init__(__self__, *,
                  annotate: Optional[pulumi.Input[str]] = None,
                  automation_action: Optional[pulumi.Input['EventOrchestrationGlobalCatchAllActionsAutomationActionArgs']] = None,
                  drop_event: Optional[pulumi.Input[bool]] = None,
                  event_action: Optional[pulumi.Input[str]] = None,
                  extractions: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalCatchAllActionsExtractionArgs']]]] = None,
+                 incident_custom_field_updates: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdateArgs']]]] = None,
                  priority: Optional[pulumi.Input[str]] = None,
                  route_to: Optional[pulumi.Input[str]] = None,
                  severity: Optional[pulumi.Input[str]] = None,
                  suppress: Optional[pulumi.Input[bool]] = None,
                  suspend: Optional[pulumi.Input[int]] = None,
                  variables: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalCatchAllActionsVariableArgs']]]] = None):
         """
         :param pulumi.Input[str] annotate: Add this text as a note on the resulting incident.
         :param pulumi.Input['EventOrchestrationGlobalCatchAllActionsAutomationActionArgs'] automation_action: Create a [Webhook](https://support.pagerduty.com/docs/event-orchestration#webhooks) associated with the resulting incident.
         :param pulumi.Input[bool] drop_event: When true, this event will be dropped. Dropped events will not trigger or resolve an alert or an incident. Dropped events will not be evaluated against router rules.
         :param pulumi.Input[str] event_action: sets whether the resulting alert status is trigger or resolve. Allowed values are: `trigger`, `resolve`
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalCatchAllActionsExtractionArgs']]] extractions: Replace any CEF field or Custom Details object field using custom variables.
+        :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdateArgs']]] incident_custom_field_updates: Assign a custom field to the resulting incident.
         :param pulumi.Input[str] priority: The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         :param pulumi.Input[str] route_to: The ID of a Set from this Global Orchestration whose rules you also want to use with events that match this rule.
         :param pulumi.Input[str] severity: sets Severity of the resulting alert. Allowed values are: `info`, `error`, `warning`, `critical`
         :param pulumi.Input[bool] suppress: Set whether the resulting alert is suppressed. Suppressed alerts will not trigger an incident.
         :param pulumi.Input[int] suspend: The number of seconds to suspend the resulting alert before triggering. This effectively pauses incident notifications. If a `resolve` event arrives before the alert triggers then PagerDuty won't create an incident for this alert.
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalCatchAllActionsVariableArgs']]] variables: Populate variables from event payloads and use those variables in other event actions.
         """
@@ -410,14 +416,16 @@
             pulumi.set(__self__, "automation_action", automation_action)
         if drop_event is not None:
             pulumi.set(__self__, "drop_event", drop_event)
         if event_action is not None:
             pulumi.set(__self__, "event_action", event_action)
         if extractions is not None:
             pulumi.set(__self__, "extractions", extractions)
+        if incident_custom_field_updates is not None:
+            pulumi.set(__self__, "incident_custom_field_updates", incident_custom_field_updates)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if route_to is not None:
             pulumi.set(__self__, "route_to", route_to)
         if severity is not None:
             pulumi.set(__self__, "severity", severity)
         if suppress is not None:
@@ -484,14 +492,26 @@
         return pulumi.get(self, "extractions")
 
     @extractions.setter
     def extractions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalCatchAllActionsExtractionArgs']]]]):
         pulumi.set(self, "extractions", value)
 
     @property
+    @pulumi.getter(name="incidentCustomFieldUpdates")
+    def incident_custom_field_updates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdateArgs']]]]:
+        """
+        Assign a custom field to the resulting incident.
+        """
+        return pulumi.get(self, "incident_custom_field_updates")
+
+    @incident_custom_field_updates.setter
+    def incident_custom_field_updates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdateArgs']]]]):
+        pulumi.set(self, "incident_custom_field_updates", value)
+
+    @property
     @pulumi.getter
     def priority(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         """
         return pulumi.get(self, "priority")
 
@@ -790,14 +810,51 @@
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template", value)
 
 
 @pulumi.input_type
+class EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdateArgs:
+    def __init__(__self__, *,
+                 id: pulumi.Input[str],
+                 value: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] id: The custom field id
+        :param pulumi.Input[str] value: The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> pulumi.Input[str]:
+        """
+        The custom field id
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        """
+        The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
 class EventOrchestrationGlobalCatchAllActionsVariableArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  path: pulumi.Input[str],
                  type: pulumi.Input[str],
                  value: pulumi.Input[str]):
         """
@@ -902,15 +959,15 @@
                  disabled: Optional[pulumi.Input[bool]] = None,
                  id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input['EventOrchestrationGlobalSetRuleActionsArgs'] actions: Actions that will be taken to change the resulting alert and incident, when an event matches this rule.
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleConditionArgs']]] conditions: Each of these conditions is evaluated to check if an event matches this rule. The rule is considered a match if any of these conditions match. If none are provided, the event will `always` match against the rule.
         :param pulumi.Input[bool] disabled: Indicates whether the rule is disabled and would therefore not be evaluated.
-        :param pulumi.Input[str] id: The ID of this set of rules. Rules in other sets can route events into this set using the rule's `route_to` property.
+        :param pulumi.Input[str] id: The custom field id
         :param pulumi.Input[str] label: A description of this rule's purpose.
         """
         pulumi.set(__self__, "actions", actions)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
         if disabled is not None:
             pulumi.set(__self__, "disabled", disabled)
@@ -955,15 +1012,15 @@
     def disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disabled", value)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of this set of rules. Rules in other sets can route events into this set using the rule's `route_to` property.
+        The custom field id
         """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "id", value)
 
@@ -984,26 +1041,28 @@
 class EventOrchestrationGlobalSetRuleActionsArgs:
     def __init__(__self__, *,
                  annotate: Optional[pulumi.Input[str]] = None,
                  automation_action: Optional[pulumi.Input['EventOrchestrationGlobalSetRuleActionsAutomationActionArgs']] = None,
                  drop_event: Optional[pulumi.Input[bool]] = None,
                  event_action: Optional[pulumi.Input[str]] = None,
                  extractions: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleActionsExtractionArgs']]]] = None,
+                 incident_custom_field_updates: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdateArgs']]]] = None,
                  priority: Optional[pulumi.Input[str]] = None,
                  route_to: Optional[pulumi.Input[str]] = None,
                  severity: Optional[pulumi.Input[str]] = None,
                  suppress: Optional[pulumi.Input[bool]] = None,
                  suspend: Optional[pulumi.Input[int]] = None,
                  variables: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleActionsVariableArgs']]]] = None):
         """
         :param pulumi.Input[str] annotate: Add this text as a note on the resulting incident.
         :param pulumi.Input['EventOrchestrationGlobalSetRuleActionsAutomationActionArgs'] automation_action: Create a [Webhook](https://support.pagerduty.com/docs/event-orchestration#webhooks) associated with the resulting incident.
         :param pulumi.Input[bool] drop_event: When true, this event will be dropped. Dropped events will not trigger or resolve an alert or an incident. Dropped events will not be evaluated against router rules.
         :param pulumi.Input[str] event_action: sets whether the resulting alert status is trigger or resolve. Allowed values are: `trigger`, `resolve`
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleActionsExtractionArgs']]] extractions: Replace any CEF field or Custom Details object field using custom variables.
+        :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdateArgs']]] incident_custom_field_updates: Assign a custom field to the resulting incident.
         :param pulumi.Input[str] priority: The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         :param pulumi.Input[str] route_to: The ID of a Set from this Global Orchestration whose rules you also want to use with events that match this rule.
         :param pulumi.Input[str] severity: sets Severity of the resulting alert. Allowed values are: `info`, `error`, `warning`, `critical`
         :param pulumi.Input[bool] suppress: Set whether the resulting alert is suppressed. Suppressed alerts will not trigger an incident.
         :param pulumi.Input[int] suspend: The number of seconds to suspend the resulting alert before triggering. This effectively pauses incident notifications. If a `resolve` event arrives before the alert triggers then PagerDuty won't create an incident for this alert.
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleActionsVariableArgs']]] variables: Populate variables from event payloads and use those variables in other event actions.
         """
@@ -1013,14 +1072,16 @@
             pulumi.set(__self__, "automation_action", automation_action)
         if drop_event is not None:
             pulumi.set(__self__, "drop_event", drop_event)
         if event_action is not None:
             pulumi.set(__self__, "event_action", event_action)
         if extractions is not None:
             pulumi.set(__self__, "extractions", extractions)
+        if incident_custom_field_updates is not None:
+            pulumi.set(__self__, "incident_custom_field_updates", incident_custom_field_updates)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if route_to is not None:
             pulumi.set(__self__, "route_to", route_to)
         if severity is not None:
             pulumi.set(__self__, "severity", severity)
         if suppress is not None:
@@ -1087,14 +1148,26 @@
         return pulumi.get(self, "extractions")
 
     @extractions.setter
     def extractions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleActionsExtractionArgs']]]]):
         pulumi.set(self, "extractions", value)
 
     @property
+    @pulumi.getter(name="incidentCustomFieldUpdates")
+    def incident_custom_field_updates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdateArgs']]]]:
+        """
+        Assign a custom field to the resulting incident.
+        """
+        return pulumi.get(self, "incident_custom_field_updates")
+
+    @incident_custom_field_updates.setter
+    def incident_custom_field_updates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdateArgs']]]]):
+        pulumi.set(self, "incident_custom_field_updates", value)
+
+    @property
     @pulumi.getter
     def priority(self) -> Optional[pulumi.Input[str]]:
         """
         The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         """
         return pulumi.get(self, "priority")
 
@@ -1393,14 +1466,51 @@
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template", value)
 
 
 @pulumi.input_type
+class EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdateArgs:
+    def __init__(__self__, *,
+                 id: pulumi.Input[str],
+                 value: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] id: The custom field id
+        :param pulumi.Input[str] value: The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> pulumi.Input[str]:
+        """
+        The custom field id
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        """
+        The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
 class EventOrchestrationGlobalSetRuleActionsVariableArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  path: pulumi.Input[str],
                  type: pulumi.Input[str],
                  value: pulumi.Input[str]):
         """
@@ -1804,26 +1914,28 @@
 @pulumi.input_type
 class EventOrchestrationServiceCatchAllActionsArgs:
     def __init__(__self__, *,
                  annotate: Optional[pulumi.Input[str]] = None,
                  automation_action: Optional[pulumi.Input['EventOrchestrationServiceCatchAllActionsAutomationActionArgs']] = None,
                  event_action: Optional[pulumi.Input[str]] = None,
                  extractions: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceCatchAllActionsExtractionArgs']]]] = None,
+                 incident_custom_field_updates: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdateArgs']]]] = None,
                  pagerduty_automation_action: Optional[pulumi.Input['EventOrchestrationServiceCatchAllActionsPagerdutyAutomationActionArgs']] = None,
                  priority: Optional[pulumi.Input[str]] = None,
                  route_to: Optional[pulumi.Input[str]] = None,
                  severity: Optional[pulumi.Input[str]] = None,
                  suppress: Optional[pulumi.Input[bool]] = None,
                  suspend: Optional[pulumi.Input[int]] = None,
                  variables: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceCatchAllActionsVariableArgs']]]] = None):
         """
         :param pulumi.Input[str] annotate: Add this text as a note on the resulting incident.
         :param pulumi.Input['EventOrchestrationServiceCatchAllActionsAutomationActionArgs'] automation_action: Create a [Webhook](https://support.pagerduty.com/docs/event-orchestration#webhooks) associated with the resulting incident.
         :param pulumi.Input[str] event_action: sets whether the resulting alert status is trigger or resolve. Allowed values are: `trigger`, `resolve`
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceCatchAllActionsExtractionArgs']]] extractions: Replace any CEF field or Custom Details object field using custom variables.
+        :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdateArgs']]] incident_custom_field_updates: Assign a custom field to the resulting incident.
         :param pulumi.Input['EventOrchestrationServiceCatchAllActionsPagerdutyAutomationActionArgs'] pagerduty_automation_action: Configure a [Process Automation](https://support.pagerduty.com/docs/event-orchestration#process-automation) associated with the resulting incident.
         :param pulumi.Input[str] priority: The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         :param pulumi.Input[str] route_to: The ID of a Set from this Service Orchestration whose rules you also want to use with events that match this rule.
         :param pulumi.Input[str] severity: sets Severity of the resulting alert. Allowed values are: `info`, `error`, `warning`, `critical`
         :param pulumi.Input[bool] suppress: Set whether the resulting alert is suppressed. Suppressed alerts will not trigger an incident.
         :param pulumi.Input[int] suspend: The number of seconds to suspend the resulting alert before triggering. This effectively pauses incident notifications. If a `resolve` event arrives before the alert triggers then PagerDuty won't create an incident for this alert.
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceCatchAllActionsVariableArgs']]] variables: Populate variables from event payloads and use those variables in other event actions.
@@ -1832,14 +1944,16 @@
             pulumi.set(__self__, "annotate", annotate)
         if automation_action is not None:
             pulumi.set(__self__, "automation_action", automation_action)
         if event_action is not None:
             pulumi.set(__self__, "event_action", event_action)
         if extractions is not None:
             pulumi.set(__self__, "extractions", extractions)
+        if incident_custom_field_updates is not None:
+            pulumi.set(__self__, "incident_custom_field_updates", incident_custom_field_updates)
         if pagerduty_automation_action is not None:
             pulumi.set(__self__, "pagerduty_automation_action", pagerduty_automation_action)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if route_to is not None:
             pulumi.set(__self__, "route_to", route_to)
         if severity is not None:
@@ -1896,14 +2010,26 @@
         return pulumi.get(self, "extractions")
 
     @extractions.setter
     def extractions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceCatchAllActionsExtractionArgs']]]]):
         pulumi.set(self, "extractions", value)
 
     @property
+    @pulumi.getter(name="incidentCustomFieldUpdates")
+    def incident_custom_field_updates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdateArgs']]]]:
+        """
+        Assign a custom field to the resulting incident.
+        """
+        return pulumi.get(self, "incident_custom_field_updates")
+
+    @incident_custom_field_updates.setter
+    def incident_custom_field_updates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdateArgs']]]]):
+        pulumi.set(self, "incident_custom_field_updates", value)
+
+    @property
     @pulumi.getter(name="pagerdutyAutomationAction")
     def pagerduty_automation_action(self) -> Optional[pulumi.Input['EventOrchestrationServiceCatchAllActionsPagerdutyAutomationActionArgs']]:
         """
         Configure a [Process Automation](https://support.pagerduty.com/docs/event-orchestration#process-automation) associated with the resulting incident.
         """
         return pulumi.get(self, "pagerduty_automation_action")
 
@@ -2214,14 +2340,51 @@
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template", value)
 
 
 @pulumi.input_type
+class EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdateArgs:
+    def __init__(__self__, *,
+                 id: pulumi.Input[str],
+                 value: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] id: The custom field id
+        :param pulumi.Input[str] value: The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> pulumi.Input[str]:
+        """
+        The custom field id
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        """
+        The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
 class EventOrchestrationServiceCatchAllActionsPagerdutyAutomationActionArgs:
     def __init__(__self__, *,
                  action_id: pulumi.Input[str]):
         """
         :param pulumi.Input[str] action_id: Id of the Process Automation action to be triggered.
         """
         pulumi.set(__self__, "action_id", action_id)
@@ -2348,15 +2511,15 @@
                  disabled: Optional[pulumi.Input[bool]] = None,
                  id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input['EventOrchestrationServiceSetRuleActionsArgs'] actions: Actions that will be taken to change the resulting alert and incident, when an event matches this rule.
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleConditionArgs']]] conditions: Each of these conditions is evaluated to check if an event matches this rule. The rule is considered a match if any of these conditions match. If none are provided, the event will `always` match against the rule.
         :param pulumi.Input[bool] disabled: Indicates whether the rule is disabled and would therefore not be evaluated.
-        :param pulumi.Input[str] id: The ID of this set of rules. Rules in other sets can route events into this set using the rule's `route_to` property.
+        :param pulumi.Input[str] id: The custom field id
         :param pulumi.Input[str] label: A description of this rule's purpose.
         """
         pulumi.set(__self__, "actions", actions)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
         if disabled is not None:
             pulumi.set(__self__, "disabled", disabled)
@@ -2401,15 +2564,15 @@
     def disabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disabled", value)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of this set of rules. Rules in other sets can route events into this set using the rule's `route_to` property.
+        The custom field id
         """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "id", value)
 
@@ -2429,26 +2592,28 @@
 @pulumi.input_type
 class EventOrchestrationServiceSetRuleActionsArgs:
     def __init__(__self__, *,
                  annotate: Optional[pulumi.Input[str]] = None,
                  automation_action: Optional[pulumi.Input['EventOrchestrationServiceSetRuleActionsAutomationActionArgs']] = None,
                  event_action: Optional[pulumi.Input[str]] = None,
                  extractions: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleActionsExtractionArgs']]]] = None,
+                 incident_custom_field_updates: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdateArgs']]]] = None,
                  pagerduty_automation_action: Optional[pulumi.Input['EventOrchestrationServiceSetRuleActionsPagerdutyAutomationActionArgs']] = None,
                  priority: Optional[pulumi.Input[str]] = None,
                  route_to: Optional[pulumi.Input[str]] = None,
                  severity: Optional[pulumi.Input[str]] = None,
                  suppress: Optional[pulumi.Input[bool]] = None,
                  suspend: Optional[pulumi.Input[int]] = None,
                  variables: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleActionsVariableArgs']]]] = None):
         """
         :param pulumi.Input[str] annotate: Add this text as a note on the resulting incident.
         :param pulumi.Input['EventOrchestrationServiceSetRuleActionsAutomationActionArgs'] automation_action: Create a [Webhook](https://support.pagerduty.com/docs/event-orchestration#webhooks) associated with the resulting incident.
         :param pulumi.Input[str] event_action: sets whether the resulting alert status is trigger or resolve. Allowed values are: `trigger`, `resolve`
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleActionsExtractionArgs']]] extractions: Replace any CEF field or Custom Details object field using custom variables.
+        :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdateArgs']]] incident_custom_field_updates: Assign a custom field to the resulting incident.
         :param pulumi.Input['EventOrchestrationServiceSetRuleActionsPagerdutyAutomationActionArgs'] pagerduty_automation_action: Configure a [Process Automation](https://support.pagerduty.com/docs/event-orchestration#process-automation) associated with the resulting incident.
         :param pulumi.Input[str] priority: The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         :param pulumi.Input[str] route_to: The ID of a Set from this Service Orchestration whose rules you also want to use with events that match this rule.
         :param pulumi.Input[str] severity: sets Severity of the resulting alert. Allowed values are: `info`, `error`, `warning`, `critical`
         :param pulumi.Input[bool] suppress: Set whether the resulting alert is suppressed. Suppressed alerts will not trigger an incident.
         :param pulumi.Input[int] suspend: The number of seconds to suspend the resulting alert before triggering. This effectively pauses incident notifications. If a `resolve` event arrives before the alert triggers then PagerDuty won't create an incident for this alert.
         :param pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleActionsVariableArgs']]] variables: Populate variables from event payloads and use those variables in other event actions.
@@ -2457,14 +2622,16 @@
             pulumi.set(__self__, "annotate", annotate)
         if automation_action is not None:
             pulumi.set(__self__, "automation_action", automation_action)
         if event_action is not None:
             pulumi.set(__self__, "event_action", event_action)
         if extractions is not None:
             pulumi.set(__self__, "extractions", extractions)
+        if incident_custom_field_updates is not None:
+            pulumi.set(__self__, "incident_custom_field_updates", incident_custom_field_updates)
         if pagerduty_automation_action is not None:
             pulumi.set(__self__, "pagerduty_automation_action", pagerduty_automation_action)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if route_to is not None:
             pulumi.set(__self__, "route_to", route_to)
         if severity is not None:
@@ -2521,14 +2688,26 @@
         return pulumi.get(self, "extractions")
 
     @extractions.setter
     def extractions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleActionsExtractionArgs']]]]):
         pulumi.set(self, "extractions", value)
 
     @property
+    @pulumi.getter(name="incidentCustomFieldUpdates")
+    def incident_custom_field_updates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdateArgs']]]]:
+        """
+        Assign a custom field to the resulting incident.
+        """
+        return pulumi.get(self, "incident_custom_field_updates")
+
+    @incident_custom_field_updates.setter
+    def incident_custom_field_updates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdateArgs']]]]):
+        pulumi.set(self, "incident_custom_field_updates", value)
+
+    @property
     @pulumi.getter(name="pagerdutyAutomationAction")
     def pagerduty_automation_action(self) -> Optional[pulumi.Input['EventOrchestrationServiceSetRuleActionsPagerdutyAutomationActionArgs']]:
         """
         Configure a [Process Automation](https://support.pagerduty.com/docs/event-orchestration#process-automation) associated with the resulting incident.
         """
         return pulumi.get(self, "pagerduty_automation_action")
 
@@ -2839,14 +3018,51 @@
 
     @template.setter
     def template(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "template", value)
 
 
 @pulumi.input_type
+class EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdateArgs:
+    def __init__(__self__, *,
+                 id: pulumi.Input[str],
+                 value: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] id: The custom field id
+        :param pulumi.Input[str] value: The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> pulumi.Input[str]:
+        """
+        The custom field id
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[str]:
+        """
+        The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[str]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
 class EventOrchestrationServiceSetRuleActionsPagerdutyAutomationActionArgs:
     def __init__(__self__, *,
                  action_id: pulumi.Input[str]):
         """
         :param pulumi.Input[str] action_id: Id of the Process Automation action to be triggered.
         """
         pulumi.set(__self__, "action_id", action_id)
```

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/_utilities.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/addon.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/addon.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_action.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_action_service_association.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_action_service_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_action_team_association.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_action_team_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_runner.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/automation_actions_runner_team_association.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/automation_actions_runner_team_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/business_service.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/business_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
         if point_of_contact is not None:
             pulumi.set(__self__, "point_of_contact", point_of_contact)
         if team is not None:
             pulumi.set(__self__, "team", team)
         if type is not None:
-            warnings.warn("""This will change to a computed resource in the next major release.""", DeprecationWarning)
-            pulumi.log.warn("""type is deprecated: This will change to a computed resource in the next major release.""")
+            warnings.warn("""This will become a computed attribute in the next major release.""", DeprecationWarning)
+            pulumi.log.warn("""type is deprecated: This will become a computed attribute in the next major release.""")
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "description")
@@ -89,16 +89,16 @@
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         **Deprecated** (Optional) Default (and only supported) value is `business_service`.
         """
-        warnings.warn("""This will change to a computed resource in the next major release.""", DeprecationWarning)
-        pulumi.log.warn("""type is deprecated: This will change to a computed resource in the next major release.""")
+        warnings.warn("""This will become a computed attribute in the next major release.""", DeprecationWarning)
+        pulumi.log.warn("""type is deprecated: This will become a computed attribute in the next major release.""")
 
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -137,16 +137,16 @@
         if self is not None:
             pulumi.set(__self__, "self", self)
         if summary is not None:
             pulumi.set(__self__, "summary", summary)
         if team is not None:
             pulumi.set(__self__, "team", team)
         if type is not None:
-            warnings.warn("""This will change to a computed resource in the next major release.""", DeprecationWarning)
-            pulumi.log.warn("""type is deprecated: This will change to a computed resource in the next major release.""")
+            warnings.warn("""This will become a computed attribute in the next major release.""", DeprecationWarning)
+            pulumi.log.warn("""type is deprecated: This will become a computed attribute in the next major release.""")
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "description")
@@ -229,16 +229,16 @@
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         **Deprecated** (Optional) Default (and only supported) value is `business_service`.
         """
-        warnings.warn("""This will change to a computed resource in the next major release.""", DeprecationWarning)
-        pulumi.log.warn("""type is deprecated: This will change to a computed resource in the next major release.""")
+        warnings.warn("""This will become a computed attribute in the next major release.""", DeprecationWarning)
+        pulumi.log.warn("""type is deprecated: This will become a computed attribute in the next major release.""")
 
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
@@ -450,16 +450,16 @@
         """
         ID of the team that owns the business service.
         """
         return pulumi.get(self, "team")
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Output[Optional[str]]:
+    def type(self) -> pulumi.Output[str]:
         """
         **Deprecated** (Optional) Default (and only supported) value is `business_service`.
         """
-        warnings.warn("""This will change to a computed resource in the next major release.""", DeprecationWarning)
-        pulumi.log.warn("""type is deprecated: This will change to a computed resource in the next major release.""")
+        warnings.warn("""This will become a computed attribute in the next major release.""", DeprecationWarning)
+        pulumi.log.warn("""type is deprecated: This will become a computed attribute in the next major release.""")
 
         return pulumi.get(self, "type")
```

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/business_service_subscriber.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/business_service_subscriber.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/config/__init__.pyi` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/config/outputs.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/config/vars.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/escalation_policy.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/escalation_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_global.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_global.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_integration.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_router.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_router.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_service.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,31 +180,36 @@
         The `catch_all` actions will be applied if an Event reaches the end of any set without matching any rules in that set. In this example the `catch_all` doesn't have any `actions` so it'll leave events as-is.
 
         ```python
         import pulumi
         import pulumi_pagerduty as pagerduty
 
         engineering = pagerduty.Team("engineering")
-        example_user = pagerduty.User("exampleUser",
-            email="125.greenholt.earline@graham.name",
-            teams=[engineering.id])
-        foo = pagerduty.EscalationPolicy("foo",
+        example_user = pagerduty.User("exampleUser", email="125.greenholt.earline@graham.name")
+        foo = pagerduty.TeamMembership("foo",
+            user_id=example_user.id,
+            team_id=engineering.id,
+            role="manager")
+        example_escalation_policy = pagerduty.EscalationPolicy("exampleEscalationPolicy",
             num_loops=2,
             rules=[pagerduty.EscalationPolicyRuleArgs(
                 escalation_delay_in_minutes=10,
                 targets=[pagerduty.EscalationPolicyRuleTargetArgs(
-                    type="user",
+                    type="user_reference",
                     id=example_user.id,
                 )],
             )])
         example_service = pagerduty.Service("exampleService",
             auto_resolve_timeout="14400",
             acknowledgement_timeout="600",
-            escalation_policy=pagerduty_escalation_policy["example"]["id"],
+            escalation_policy=example_escalation_policy.id,
             alert_creation="create_alerts_and_incidents")
+        cs_impact = pagerduty.IncidentCustomField("csImpact",
+            data_type="string",
+            field_type="single_value")
         p1 = pagerduty.get_priority(name="P1")
         www = pagerduty.EventOrchestrationService("www",
             service=example_service.id,
             enable_event_orchestration_for_service=True,
             sets=[
                 pagerduty.EventOrchestrationServiceSetArgs(
                     id="start",
@@ -239,14 +244,18 @@
                             label="All critical alerts should be treated as P1 incident",
                             conditions=[pagerduty.EventOrchestrationServiceSetRuleConditionArgs(
                                 expression="event.severity matches 'critical'",
                             )],
                             actions=pagerduty.EventOrchestrationServiceSetRuleActionsArgs(
                                 annotate="Please use our P1 runbook: https://docs.test/p1-runbook",
                                 priority=p1.id,
+                                incident_custom_field_updates=[pagerduty.EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdateArgs(
+                                    id=cs_impact.id,
+                                    value="High Impact",
+                                )],
                             ),
                         ),
                         pagerduty.EventOrchestrationServiceSetRuleArgs(
                             label="If there's something wrong on the canary let the team know about it in our deployments Slack channel",
                             conditions=[pagerduty.EventOrchestrationServiceSetRuleConditionArgs(
                                 expression="event.custom_details.hostname matches part 'canary'",
                             )],
@@ -326,31 +335,36 @@
         The `catch_all` actions will be applied if an Event reaches the end of any set without matching any rules in that set. In this example the `catch_all` doesn't have any `actions` so it'll leave events as-is.
 
         ```python
         import pulumi
         import pulumi_pagerduty as pagerduty
 
         engineering = pagerduty.Team("engineering")
-        example_user = pagerduty.User("exampleUser",
-            email="125.greenholt.earline@graham.name",
-            teams=[engineering.id])
-        foo = pagerduty.EscalationPolicy("foo",
+        example_user = pagerduty.User("exampleUser", email="125.greenholt.earline@graham.name")
+        foo = pagerduty.TeamMembership("foo",
+            user_id=example_user.id,
+            team_id=engineering.id,
+            role="manager")
+        example_escalation_policy = pagerduty.EscalationPolicy("exampleEscalationPolicy",
             num_loops=2,
             rules=[pagerduty.EscalationPolicyRuleArgs(
                 escalation_delay_in_minutes=10,
                 targets=[pagerduty.EscalationPolicyRuleTargetArgs(
-                    type="user",
+                    type="user_reference",
                     id=example_user.id,
                 )],
             )])
         example_service = pagerduty.Service("exampleService",
             auto_resolve_timeout="14400",
             acknowledgement_timeout="600",
-            escalation_policy=pagerduty_escalation_policy["example"]["id"],
+            escalation_policy=example_escalation_policy.id,
             alert_creation="create_alerts_and_incidents")
+        cs_impact = pagerduty.IncidentCustomField("csImpact",
+            data_type="string",
+            field_type="single_value")
         p1 = pagerduty.get_priority(name="P1")
         www = pagerduty.EventOrchestrationService("www",
             service=example_service.id,
             enable_event_orchestration_for_service=True,
             sets=[
                 pagerduty.EventOrchestrationServiceSetArgs(
                     id="start",
@@ -385,14 +399,18 @@
                             label="All critical alerts should be treated as P1 incident",
                             conditions=[pagerduty.EventOrchestrationServiceSetRuleConditionArgs(
                                 expression="event.severity matches 'critical'",
                             )],
                             actions=pagerduty.EventOrchestrationServiceSetRuleActionsArgs(
                                 annotate="Please use our P1 runbook: https://docs.test/p1-runbook",
                                 priority=p1.id,
+                                incident_custom_field_updates=[pagerduty.EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdateArgs(
+                                    id=cs_impact.id,
+                                    value="High Impact",
+                                )],
                             ),
                         ),
                         pagerduty.EventOrchestrationServiceSetRuleArgs(
                             label="If there's something wrong on the canary let the team know about it in our deployments Slack channel",
                             conditions=[pagerduty.EventOrchestrationServiceSetRuleConditionArgs(
                                 expression="event.custom_details.hostname matches part 'canary'",
                             )],
```

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_orchestration_unrouted.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_orchestration_unrouted.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/event_rule.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/event_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/extension.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/extension.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/extension_service_now.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/extension_service_now.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_automation_actions_action.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_automation_actions_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_automation_actions_runner.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_automation_actions_runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_business_service.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_business_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_escalation_policy.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_escalation_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_event_orchestration.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_event_orchestration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_event_orchestration_integration.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_event_orchestration_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_event_orchestrations.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_event_orchestrations.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_extension_schema.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_extension_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_incident_custom_field.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_incident_custom_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_incident_workflow.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_incident_workflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_license.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_license.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_licenses.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_licenses.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_priority.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_priority.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_ruleset.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_schedule.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_service.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_service_integration.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_tag.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_team.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_team_members.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_team_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_user.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_user_contact_method.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_user_contact_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_users.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/get_vendor.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/get_vendor.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/incident_custom_field.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/incident_custom_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/incident_custom_field_option.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/incident_custom_field_option.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/incident_workflow.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/incident_workflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/incident_workflow_trigger.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/incident_workflow_trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/maintenance_window.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/outputs.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,24 @@
     'EscalationPolicyRuleTarget',
     'EventOrchestrationGlobalCatchAll',
     'EventOrchestrationGlobalCatchAllActions',
     'EventOrchestrationGlobalCatchAllActionsAutomationAction',
     'EventOrchestrationGlobalCatchAllActionsAutomationActionHeader',
     'EventOrchestrationGlobalCatchAllActionsAutomationActionParameter',
     'EventOrchestrationGlobalCatchAllActionsExtraction',
+    'EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdate',
     'EventOrchestrationGlobalCatchAllActionsVariable',
     'EventOrchestrationGlobalSet',
     'EventOrchestrationGlobalSetRule',
     'EventOrchestrationGlobalSetRuleActions',
     'EventOrchestrationGlobalSetRuleActionsAutomationAction',
     'EventOrchestrationGlobalSetRuleActionsAutomationActionHeader',
     'EventOrchestrationGlobalSetRuleActionsAutomationActionParameter',
     'EventOrchestrationGlobalSetRuleActionsExtraction',
+    'EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdate',
     'EventOrchestrationGlobalSetRuleActionsVariable',
     'EventOrchestrationGlobalSetRuleCondition',
     'EventOrchestrationIntegration',
     'EventOrchestrationIntegrationParameter',
     'EventOrchestrationRouterCatchAll',
     'EventOrchestrationRouterCatchAllActions',
     'EventOrchestrationRouterSet',
@@ -41,23 +43,25 @@
     'EventOrchestrationRouterSetRuleCondition',
     'EventOrchestrationServiceCatchAll',
     'EventOrchestrationServiceCatchAllActions',
     'EventOrchestrationServiceCatchAllActionsAutomationAction',
     'EventOrchestrationServiceCatchAllActionsAutomationActionHeader',
     'EventOrchestrationServiceCatchAllActionsAutomationActionParameter',
     'EventOrchestrationServiceCatchAllActionsExtraction',
+    'EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdate',
     'EventOrchestrationServiceCatchAllActionsPagerdutyAutomationAction',
     'EventOrchestrationServiceCatchAllActionsVariable',
     'EventOrchestrationServiceSet',
     'EventOrchestrationServiceSetRule',
     'EventOrchestrationServiceSetRuleActions',
     'EventOrchestrationServiceSetRuleActionsAutomationAction',
     'EventOrchestrationServiceSetRuleActionsAutomationActionHeader',
     'EventOrchestrationServiceSetRuleActionsAutomationActionParameter',
     'EventOrchestrationServiceSetRuleActionsExtraction',
+    'EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdate',
     'EventOrchestrationServiceSetRuleActionsPagerdutyAutomationAction',
     'EventOrchestrationServiceSetRuleActionsVariable',
     'EventOrchestrationServiceSetRuleCondition',
     'EventOrchestrationUnroutedCatchAll',
     'EventOrchestrationUnroutedCatchAllActions',
     'EventOrchestrationUnroutedCatchAllActionsExtraction',
     'EventOrchestrationUnroutedCatchAllActionsVariable',
@@ -142,14 +146,22 @@
     'GetEventOrchestrationIntegrationDetailParameterResult',
     'GetEventOrchestrationIntegrationParameterResult',
     'GetEventOrchestrationsEventOrchestrationResult',
     'GetEventOrchestrationsEventOrchestrationIntegrationResult',
     'GetEventOrchestrationsEventOrchestrationIntegrationParameterResult',
     'GetLicensesLicenseResult',
     'GetServiceTeamResult',
+    'GetStandardsResourceScoresScoreResult',
+    'GetStandardsResourceScoresStandardResult',
+    'GetStandardsResourcesScoresResourceResult',
+    'GetStandardsResourcesScoresResourceScoreResult',
+    'GetStandardsResourcesScoresResourceStandardResult',
+    'GetStandardsStandardResult',
+    'GetStandardsStandardExclusionResult',
+    'GetStandardsStandardInclusionResult',
     'GetTeamMembersMemberResult',
     'GetUsersUserResult',
 ]
 
 @pulumi.output_type
 class AutomationActionsActionActionDataReference(dict):
     @staticmethod
@@ -382,14 +394,16 @@
         suggest = None
         if key == "automationAction":
             suggest = "automation_action"
         elif key == "dropEvent":
             suggest = "drop_event"
         elif key == "eventAction":
             suggest = "event_action"
+        elif key == "incidentCustomFieldUpdates":
+            suggest = "incident_custom_field_updates"
         elif key == "routeTo":
             suggest = "route_to"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in EventOrchestrationGlobalCatchAllActions. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
@@ -402,26 +416,28 @@
 
     def __init__(__self__, *,
                  annotate: Optional[str] = None,
                  automation_action: Optional['outputs.EventOrchestrationGlobalCatchAllActionsAutomationAction'] = None,
                  drop_event: Optional[bool] = None,
                  event_action: Optional[str] = None,
                  extractions: Optional[Sequence['outputs.EventOrchestrationGlobalCatchAllActionsExtraction']] = None,
+                 incident_custom_field_updates: Optional[Sequence['outputs.EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdate']] = None,
                  priority: Optional[str] = None,
                  route_to: Optional[str] = None,
                  severity: Optional[str] = None,
                  suppress: Optional[bool] = None,
                  suspend: Optional[int] = None,
                  variables: Optional[Sequence['outputs.EventOrchestrationGlobalCatchAllActionsVariable']] = None):
         """
         :param str annotate: Add this text as a note on the resulting incident.
         :param 'EventOrchestrationGlobalCatchAllActionsAutomationActionArgs' automation_action: Create a [Webhook](https://support.pagerduty.com/docs/event-orchestration#webhooks) associated with the resulting incident.
         :param bool drop_event: When true, this event will be dropped. Dropped events will not trigger or resolve an alert or an incident. Dropped events will not be evaluated against router rules.
         :param str event_action: sets whether the resulting alert status is trigger or resolve. Allowed values are: `trigger`, `resolve`
         :param Sequence['EventOrchestrationGlobalCatchAllActionsExtractionArgs'] extractions: Replace any CEF field or Custom Details object field using custom variables.
+        :param Sequence['EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdateArgs'] incident_custom_field_updates: Assign a custom field to the resulting incident.
         :param str priority: The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         :param str route_to: The ID of a Set from this Global Orchestration whose rules you also want to use with events that match this rule.
         :param str severity: sets Severity of the resulting alert. Allowed values are: `info`, `error`, `warning`, `critical`
         :param bool suppress: Set whether the resulting alert is suppressed. Suppressed alerts will not trigger an incident.
         :param int suspend: The number of seconds to suspend the resulting alert before triggering. This effectively pauses incident notifications. If a `resolve` event arrives before the alert triggers then PagerDuty won't create an incident for this alert.
         :param Sequence['EventOrchestrationGlobalCatchAllActionsVariableArgs'] variables: Populate variables from event payloads and use those variables in other event actions.
         """
@@ -431,14 +447,16 @@
             pulumi.set(__self__, "automation_action", automation_action)
         if drop_event is not None:
             pulumi.set(__self__, "drop_event", drop_event)
         if event_action is not None:
             pulumi.set(__self__, "event_action", event_action)
         if extractions is not None:
             pulumi.set(__self__, "extractions", extractions)
+        if incident_custom_field_updates is not None:
+            pulumi.set(__self__, "incident_custom_field_updates", incident_custom_field_updates)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if route_to is not None:
             pulumi.set(__self__, "route_to", route_to)
         if severity is not None:
             pulumi.set(__self__, "severity", severity)
         if suppress is not None:
@@ -485,14 +503,22 @@
     def extractions(self) -> Optional[Sequence['outputs.EventOrchestrationGlobalCatchAllActionsExtraction']]:
         """
         Replace any CEF field or Custom Details object field using custom variables.
         """
         return pulumi.get(self, "extractions")
 
     @property
+    @pulumi.getter(name="incidentCustomFieldUpdates")
+    def incident_custom_field_updates(self) -> Optional[Sequence['outputs.EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdate']]:
+        """
+        Assign a custom field to the resulting incident.
+        """
+        return pulumi.get(self, "incident_custom_field_updates")
+
+    @property
     @pulumi.getter
     def priority(self) -> Optional[str]:
         """
         The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         """
         return pulumi.get(self, "priority")
 
@@ -732,14 +758,43 @@
         * Use variables named `ip` and `subnet` with a template like: `{{variables.ip}}/{{variables.subnet}}`
         * Combine the event severity & summary with template like: `{{event.severity}}:{{event.summary}}`
         """
         return pulumi.get(self, "template")
 
 
 @pulumi.output_type
+class EventOrchestrationGlobalCatchAllActionsIncidentCustomFieldUpdate(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 value: str):
+        """
+        :param str id: The custom field id
+        :param str value: The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The custom field id
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def value(self) -> str:
+        """
+        The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
 class EventOrchestrationGlobalCatchAllActionsVariable(dict):
     def __init__(__self__, *,
                  name: str,
                  path: str,
                  type: str,
                  value: str):
         """
@@ -820,15 +875,15 @@
                  disabled: Optional[bool] = None,
                  id: Optional[str] = None,
                  label: Optional[str] = None):
         """
         :param 'EventOrchestrationGlobalSetRuleActionsArgs' actions: Actions that will be taken to change the resulting alert and incident, when an event matches this rule.
         :param Sequence['EventOrchestrationGlobalSetRuleConditionArgs'] conditions: Each of these conditions is evaluated to check if an event matches this rule. The rule is considered a match if any of these conditions match. If none are provided, the event will `always` match against the rule.
         :param bool disabled: Indicates whether the rule is disabled and would therefore not be evaluated.
-        :param str id: The ID of this set of rules. Rules in other sets can route events into this set using the rule's `route_to` property.
+        :param str id: The custom field id
         :param str label: A description of this rule's purpose.
         """
         pulumi.set(__self__, "actions", actions)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
         if disabled is not None:
             pulumi.set(__self__, "disabled", disabled)
@@ -861,15 +916,15 @@
         """
         return pulumi.get(self, "disabled")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
-        The ID of this set of rules. Rules in other sets can route events into this set using the rule's `route_to` property.
+        The custom field id
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def label(self) -> Optional[str]:
         """
@@ -885,14 +940,16 @@
         suggest = None
         if key == "automationAction":
             suggest = "automation_action"
         elif key == "dropEvent":
             suggest = "drop_event"
         elif key == "eventAction":
             suggest = "event_action"
+        elif key == "incidentCustomFieldUpdates":
+            suggest = "incident_custom_field_updates"
         elif key == "routeTo":
             suggest = "route_to"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in EventOrchestrationGlobalSetRuleActions. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
@@ -905,26 +962,28 @@
 
     def __init__(__self__, *,
                  annotate: Optional[str] = None,
                  automation_action: Optional['outputs.EventOrchestrationGlobalSetRuleActionsAutomationAction'] = None,
                  drop_event: Optional[bool] = None,
                  event_action: Optional[str] = None,
                  extractions: Optional[Sequence['outputs.EventOrchestrationGlobalSetRuleActionsExtraction']] = None,
+                 incident_custom_field_updates: Optional[Sequence['outputs.EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdate']] = None,
                  priority: Optional[str] = None,
                  route_to: Optional[str] = None,
                  severity: Optional[str] = None,
                  suppress: Optional[bool] = None,
                  suspend: Optional[int] = None,
                  variables: Optional[Sequence['outputs.EventOrchestrationGlobalSetRuleActionsVariable']] = None):
         """
         :param str annotate: Add this text as a note on the resulting incident.
         :param 'EventOrchestrationGlobalSetRuleActionsAutomationActionArgs' automation_action: Create a [Webhook](https://support.pagerduty.com/docs/event-orchestration#webhooks) associated with the resulting incident.
         :param bool drop_event: When true, this event will be dropped. Dropped events will not trigger or resolve an alert or an incident. Dropped events will not be evaluated against router rules.
         :param str event_action: sets whether the resulting alert status is trigger or resolve. Allowed values are: `trigger`, `resolve`
         :param Sequence['EventOrchestrationGlobalSetRuleActionsExtractionArgs'] extractions: Replace any CEF field or Custom Details object field using custom variables.
+        :param Sequence['EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdateArgs'] incident_custom_field_updates: Assign a custom field to the resulting incident.
         :param str priority: The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         :param str route_to: The ID of a Set from this Global Orchestration whose rules you also want to use with events that match this rule.
         :param str severity: sets Severity of the resulting alert. Allowed values are: `info`, `error`, `warning`, `critical`
         :param bool suppress: Set whether the resulting alert is suppressed. Suppressed alerts will not trigger an incident.
         :param int suspend: The number of seconds to suspend the resulting alert before triggering. This effectively pauses incident notifications. If a `resolve` event arrives before the alert triggers then PagerDuty won't create an incident for this alert.
         :param Sequence['EventOrchestrationGlobalSetRuleActionsVariableArgs'] variables: Populate variables from event payloads and use those variables in other event actions.
         """
@@ -934,14 +993,16 @@
             pulumi.set(__self__, "automation_action", automation_action)
         if drop_event is not None:
             pulumi.set(__self__, "drop_event", drop_event)
         if event_action is not None:
             pulumi.set(__self__, "event_action", event_action)
         if extractions is not None:
             pulumi.set(__self__, "extractions", extractions)
+        if incident_custom_field_updates is not None:
+            pulumi.set(__self__, "incident_custom_field_updates", incident_custom_field_updates)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if route_to is not None:
             pulumi.set(__self__, "route_to", route_to)
         if severity is not None:
             pulumi.set(__self__, "severity", severity)
         if suppress is not None:
@@ -988,14 +1049,22 @@
     def extractions(self) -> Optional[Sequence['outputs.EventOrchestrationGlobalSetRuleActionsExtraction']]:
         """
         Replace any CEF field or Custom Details object field using custom variables.
         """
         return pulumi.get(self, "extractions")
 
     @property
+    @pulumi.getter(name="incidentCustomFieldUpdates")
+    def incident_custom_field_updates(self) -> Optional[Sequence['outputs.EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdate']]:
+        """
+        Assign a custom field to the resulting incident.
+        """
+        return pulumi.get(self, "incident_custom_field_updates")
+
+    @property
     @pulumi.getter
     def priority(self) -> Optional[str]:
         """
         The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         """
         return pulumi.get(self, "priority")
 
@@ -1235,14 +1304,43 @@
         * Use variables named `ip` and `subnet` with a template like: `{{variables.ip}}/{{variables.subnet}}`
         * Combine the event severity & summary with template like: `{{event.severity}}:{{event.summary}}`
         """
         return pulumi.get(self, "template")
 
 
 @pulumi.output_type
+class EventOrchestrationGlobalSetRuleActionsIncidentCustomFieldUpdate(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 value: str):
+        """
+        :param str id: The custom field id
+        :param str value: The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The custom field id
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def value(self) -> str:
+        """
+        The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
 class EventOrchestrationGlobalSetRuleActionsVariable(dict):
     def __init__(__self__, *,
                  name: str,
                  path: str,
                  type: str,
                  value: str):
         """
@@ -1611,14 +1709,16 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "automationAction":
             suggest = "automation_action"
         elif key == "eventAction":
             suggest = "event_action"
+        elif key == "incidentCustomFieldUpdates":
+            suggest = "incident_custom_field_updates"
         elif key == "pagerdutyAutomationAction":
             suggest = "pagerduty_automation_action"
         elif key == "routeTo":
             suggest = "route_to"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in EventOrchestrationServiceCatchAllActions. Access the value via the '{suggest}' property getter instead.")
@@ -1632,26 +1732,28 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  annotate: Optional[str] = None,
                  automation_action: Optional['outputs.EventOrchestrationServiceCatchAllActionsAutomationAction'] = None,
                  event_action: Optional[str] = None,
                  extractions: Optional[Sequence['outputs.EventOrchestrationServiceCatchAllActionsExtraction']] = None,
+                 incident_custom_field_updates: Optional[Sequence['outputs.EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdate']] = None,
                  pagerduty_automation_action: Optional['outputs.EventOrchestrationServiceCatchAllActionsPagerdutyAutomationAction'] = None,
                  priority: Optional[str] = None,
                  route_to: Optional[str] = None,
                  severity: Optional[str] = None,
                  suppress: Optional[bool] = None,
                  suspend: Optional[int] = None,
                  variables: Optional[Sequence['outputs.EventOrchestrationServiceCatchAllActionsVariable']] = None):
         """
         :param str annotate: Add this text as a note on the resulting incident.
         :param 'EventOrchestrationServiceCatchAllActionsAutomationActionArgs' automation_action: Create a [Webhook](https://support.pagerduty.com/docs/event-orchestration#webhooks) associated with the resulting incident.
         :param str event_action: sets whether the resulting alert status is trigger or resolve. Allowed values are: `trigger`, `resolve`
         :param Sequence['EventOrchestrationServiceCatchAllActionsExtractionArgs'] extractions: Replace any CEF field or Custom Details object field using custom variables.
+        :param Sequence['EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdateArgs'] incident_custom_field_updates: Assign a custom field to the resulting incident.
         :param 'EventOrchestrationServiceCatchAllActionsPagerdutyAutomationActionArgs' pagerduty_automation_action: Configure a [Process Automation](https://support.pagerduty.com/docs/event-orchestration#process-automation) associated with the resulting incident.
         :param str priority: The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         :param str route_to: The ID of a Set from this Service Orchestration whose rules you also want to use with events that match this rule.
         :param str severity: sets Severity of the resulting alert. Allowed values are: `info`, `error`, `warning`, `critical`
         :param bool suppress: Set whether the resulting alert is suppressed. Suppressed alerts will not trigger an incident.
         :param int suspend: The number of seconds to suspend the resulting alert before triggering. This effectively pauses incident notifications. If a `resolve` event arrives before the alert triggers then PagerDuty won't create an incident for this alert.
         :param Sequence['EventOrchestrationServiceCatchAllActionsVariableArgs'] variables: Populate variables from event payloads and use those variables in other event actions.
@@ -1660,14 +1762,16 @@
             pulumi.set(__self__, "annotate", annotate)
         if automation_action is not None:
             pulumi.set(__self__, "automation_action", automation_action)
         if event_action is not None:
             pulumi.set(__self__, "event_action", event_action)
         if extractions is not None:
             pulumi.set(__self__, "extractions", extractions)
+        if incident_custom_field_updates is not None:
+            pulumi.set(__self__, "incident_custom_field_updates", incident_custom_field_updates)
         if pagerduty_automation_action is not None:
             pulumi.set(__self__, "pagerduty_automation_action", pagerduty_automation_action)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if route_to is not None:
             pulumi.set(__self__, "route_to", route_to)
         if severity is not None:
@@ -1708,14 +1812,22 @@
     def extractions(self) -> Optional[Sequence['outputs.EventOrchestrationServiceCatchAllActionsExtraction']]:
         """
         Replace any CEF field or Custom Details object field using custom variables.
         """
         return pulumi.get(self, "extractions")
 
     @property
+    @pulumi.getter(name="incidentCustomFieldUpdates")
+    def incident_custom_field_updates(self) -> Optional[Sequence['outputs.EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdate']]:
+        """
+        Assign a custom field to the resulting incident.
+        """
+        return pulumi.get(self, "incident_custom_field_updates")
+
+    @property
     @pulumi.getter(name="pagerdutyAutomationAction")
     def pagerduty_automation_action(self) -> Optional['outputs.EventOrchestrationServiceCatchAllActionsPagerdutyAutomationAction']:
         """
         Configure a [Process Automation](https://support.pagerduty.com/docs/event-orchestration#process-automation) associated with the resulting incident.
         """
         return pulumi.get(self, "pagerduty_automation_action")
 
@@ -1963,14 +2075,43 @@
         * Use variables named `ip` and `subnet` with a template like: `{{variables.ip}}/{{variables.subnet}}`
         * Combine the event severity & summary with template like: `{{event.severity}}:{{event.summary}}`
         """
         return pulumi.get(self, "template")
 
 
 @pulumi.output_type
+class EventOrchestrationServiceCatchAllActionsIncidentCustomFieldUpdate(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 value: str):
+        """
+        :param str id: The custom field id
+        :param str value: The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The custom field id
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def value(self) -> str:
+        """
+        The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
 class EventOrchestrationServiceCatchAllActionsPagerdutyAutomationAction(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "actionId":
             suggest = "action_id"
 
@@ -2086,15 +2227,15 @@
                  disabled: Optional[bool] = None,
                  id: Optional[str] = None,
                  label: Optional[str] = None):
         """
         :param 'EventOrchestrationServiceSetRuleActionsArgs' actions: Actions that will be taken to change the resulting alert and incident, when an event matches this rule.
         :param Sequence['EventOrchestrationServiceSetRuleConditionArgs'] conditions: Each of these conditions is evaluated to check if an event matches this rule. The rule is considered a match if any of these conditions match. If none are provided, the event will `always` match against the rule.
         :param bool disabled: Indicates whether the rule is disabled and would therefore not be evaluated.
-        :param str id: The ID of this set of rules. Rules in other sets can route events into this set using the rule's `route_to` property.
+        :param str id: The custom field id
         :param str label: A description of this rule's purpose.
         """
         pulumi.set(__self__, "actions", actions)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
         if disabled is not None:
             pulumi.set(__self__, "disabled", disabled)
@@ -2127,15 +2268,15 @@
         """
         return pulumi.get(self, "disabled")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
-        The ID of this set of rules. Rules in other sets can route events into this set using the rule's `route_to` property.
+        The custom field id
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def label(self) -> Optional[str]:
         """
@@ -2149,14 +2290,16 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "automationAction":
             suggest = "automation_action"
         elif key == "eventAction":
             suggest = "event_action"
+        elif key == "incidentCustomFieldUpdates":
+            suggest = "incident_custom_field_updates"
         elif key == "pagerdutyAutomationAction":
             suggest = "pagerduty_automation_action"
         elif key == "routeTo":
             suggest = "route_to"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in EventOrchestrationServiceSetRuleActions. Access the value via the '{suggest}' property getter instead.")
@@ -2170,26 +2313,28 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  annotate: Optional[str] = None,
                  automation_action: Optional['outputs.EventOrchestrationServiceSetRuleActionsAutomationAction'] = None,
                  event_action: Optional[str] = None,
                  extractions: Optional[Sequence['outputs.EventOrchestrationServiceSetRuleActionsExtraction']] = None,
+                 incident_custom_field_updates: Optional[Sequence['outputs.EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdate']] = None,
                  pagerduty_automation_action: Optional['outputs.EventOrchestrationServiceSetRuleActionsPagerdutyAutomationAction'] = None,
                  priority: Optional[str] = None,
                  route_to: Optional[str] = None,
                  severity: Optional[str] = None,
                  suppress: Optional[bool] = None,
                  suspend: Optional[int] = None,
                  variables: Optional[Sequence['outputs.EventOrchestrationServiceSetRuleActionsVariable']] = None):
         """
         :param str annotate: Add this text as a note on the resulting incident.
         :param 'EventOrchestrationServiceSetRuleActionsAutomationActionArgs' automation_action: Create a [Webhook](https://support.pagerduty.com/docs/event-orchestration#webhooks) associated with the resulting incident.
         :param str event_action: sets whether the resulting alert status is trigger or resolve. Allowed values are: `trigger`, `resolve`
         :param Sequence['EventOrchestrationServiceSetRuleActionsExtractionArgs'] extractions: Replace any CEF field or Custom Details object field using custom variables.
+        :param Sequence['EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdateArgs'] incident_custom_field_updates: Assign a custom field to the resulting incident.
         :param 'EventOrchestrationServiceSetRuleActionsPagerdutyAutomationActionArgs' pagerduty_automation_action: Configure a [Process Automation](https://support.pagerduty.com/docs/event-orchestration#process-automation) associated with the resulting incident.
         :param str priority: The ID of the priority you want to set on resulting incident. Consider using the `get_priority` data source.
         :param str route_to: The ID of a Set from this Service Orchestration whose rules you also want to use with events that match this rule.
         :param str severity: sets Severity of the resulting alert. Allowed values are: `info`, `error`, `warning`, `critical`
         :param bool suppress: Set whether the resulting alert is suppressed. Suppressed alerts will not trigger an incident.
         :param int suspend: The number of seconds to suspend the resulting alert before triggering. This effectively pauses incident notifications. If a `resolve` event arrives before the alert triggers then PagerDuty won't create an incident for this alert.
         :param Sequence['EventOrchestrationServiceSetRuleActionsVariableArgs'] variables: Populate variables from event payloads and use those variables in other event actions.
@@ -2198,14 +2343,16 @@
             pulumi.set(__self__, "annotate", annotate)
         if automation_action is not None:
             pulumi.set(__self__, "automation_action", automation_action)
         if event_action is not None:
             pulumi.set(__self__, "event_action", event_action)
         if extractions is not None:
             pulumi.set(__self__, "extractions", extractions)
+        if incident_custom_field_updates is not None:
+            pulumi.set(__self__, "incident_custom_field_updates", incident_custom_field_updates)
         if pagerduty_automation_action is not None:
             pulumi.set(__self__, "pagerduty_automation_action", pagerduty_automation_action)
         if priority is not None:
             pulumi.set(__self__, "priority", priority)
         if route_to is not None:
             pulumi.set(__self__, "route_to", route_to)
         if severity is not None:
@@ -2246,14 +2393,22 @@
     def extractions(self) -> Optional[Sequence['outputs.EventOrchestrationServiceSetRuleActionsExtraction']]:
         """
         Replace any CEF field or Custom Details object field using custom variables.
         """
         return pulumi.get(self, "extractions")
 
     @property
+    @pulumi.getter(name="incidentCustomFieldUpdates")
+    def incident_custom_field_updates(self) -> Optional[Sequence['outputs.EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdate']]:
+        """
+        Assign a custom field to the resulting incident.
+        """
+        return pulumi.get(self, "incident_custom_field_updates")
+
+    @property
     @pulumi.getter(name="pagerdutyAutomationAction")
     def pagerduty_automation_action(self) -> Optional['outputs.EventOrchestrationServiceSetRuleActionsPagerdutyAutomationAction']:
         """
         Configure a [Process Automation](https://support.pagerduty.com/docs/event-orchestration#process-automation) associated with the resulting incident.
         """
         return pulumi.get(self, "pagerduty_automation_action")
 
@@ -2501,14 +2656,43 @@
         * Use variables named `ip` and `subnet` with a template like: `{{variables.ip}}/{{variables.subnet}}`
         * Combine the event severity & summary with template like: `{{event.severity}}:{{event.summary}}`
         """
         return pulumi.get(self, "template")
 
 
 @pulumi.output_type
+class EventOrchestrationServiceSetRuleActionsIncidentCustomFieldUpdate(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 value: str):
+        """
+        :param str id: The custom field id
+        :param str value: The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The custom field id
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def value(self) -> str:
+        """
+        The Regex expression to match against. Must use valid [RE2 regular expression](https://github.com/google/re2/wiki/Syntax) syntax.
+        """
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
 class EventOrchestrationServiceSetRuleActionsPagerdutyAutomationAction(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "actionId":
             suggest = "action_id"
 
@@ -6964,14 +7148,422 @@
         """
         The service name to use to find a service in the PagerDuty API.
         """
         return pulumi.get(self, "name")
 
 
 @pulumi.output_type
+class GetStandardsResourceScoresScoreResult(dict):
+    def __init__(__self__, *,
+                 passing: int,
+                 total: int):
+        """
+        :param int passing: Number of standards this resource successfully complies to.
+        :param int total: Number of standards associated to this resource.
+        """
+        pulumi.set(__self__, "passing", passing)
+        pulumi.set(__self__, "total", total)
+
+    @property
+    @pulumi.getter
+    def passing(self) -> int:
+        """
+        Number of standards this resource successfully complies to.
+        """
+        return pulumi.get(self, "passing")
+
+    @property
+    @pulumi.getter
+    def total(self) -> int:
+        """
+        Number of standards associated to this resource.
+        """
+        return pulumi.get(self, "total")
+
+
+@pulumi.output_type
+class GetStandardsResourceScoresStandardResult(dict):
+    def __init__(__self__, *,
+                 active: bool,
+                 description: str,
+                 id: str,
+                 name: str,
+                 pass_: bool,
+                 type: str):
+        """
+        :param bool active: Indicates whether the standard is currently active and applicable to the resource.
+        :param str description: Provides a textual description of the standard.
+        :param str id: Identifier of said resource.
+        :param str name: The human-readable name of the standard.
+        :param bool pass_: Indicates whether the resource complies to this standard.
+        :param str type: The type of the standard.
+        """
+        pulumi.set(__self__, "active", active)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "pass_", pass_)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def active(self) -> bool:
+        """
+        Indicates whether the standard is currently active and applicable to the resource.
+        """
+        return pulumi.get(self, "active")
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        Provides a textual description of the standard.
+        """
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        Identifier of said resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The human-readable name of the standard.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="pass")
+    def pass_(self) -> bool:
+        """
+        Indicates whether the resource complies to this standard.
+        """
+        return pulumi.get(self, "pass_")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        The type of the standard.
+        """
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
+class GetStandardsResourcesScoresResourceResult(dict):
+    def __init__(__self__, *,
+                 resource_id: str,
+                 resource_type: str,
+                 score: 'outputs.GetStandardsResourcesScoresResourceScoreResult',
+                 standards: Sequence['outputs.GetStandardsResourcesScoresResourceStandardResult']):
+        """
+        :param str resource_id: Unique Identifier.
+        :param str resource_type: Type of the object the standards are associated to. Allowed values are `technical_services`.
+        :param 'GetStandardsResourcesScoresResourceScoreArgs' score: Summary of the scores for standards associated with this resource.
+        :param Sequence['GetStandardsResourcesScoresResourceStandardArgs'] standards: The list of standards evaluated against.
+        """
+        pulumi.set(__self__, "resource_id", resource_id)
+        pulumi.set(__self__, "resource_type", resource_type)
+        pulumi.set(__self__, "score", score)
+        pulumi.set(__self__, "standards", standards)
+
+    @property
+    @pulumi.getter(name="resourceId")
+    def resource_id(self) -> str:
+        """
+        Unique Identifier.
+        """
+        return pulumi.get(self, "resource_id")
+
+    @property
+    @pulumi.getter(name="resourceType")
+    def resource_type(self) -> str:
+        """
+        Type of the object the standards are associated to. Allowed values are `technical_services`.
+        """
+        return pulumi.get(self, "resource_type")
+
+    @property
+    @pulumi.getter
+    def score(self) -> 'outputs.GetStandardsResourcesScoresResourceScoreResult':
+        """
+        Summary of the scores for standards associated with this resource.
+        """
+        return pulumi.get(self, "score")
+
+    @property
+    @pulumi.getter
+    def standards(self) -> Sequence['outputs.GetStandardsResourcesScoresResourceStandardResult']:
+        """
+        The list of standards evaluated against.
+        """
+        return pulumi.get(self, "standards")
+
+
+@pulumi.output_type
+class GetStandardsResourcesScoresResourceScoreResult(dict):
+    def __init__(__self__, *,
+                 passing: int,
+                 total: int):
+        """
+        :param int passing: Number of standards this resource successfully complies to.
+        :param int total: Number of standards associated to this resource.
+        """
+        pulumi.set(__self__, "passing", passing)
+        pulumi.set(__self__, "total", total)
+
+    @property
+    @pulumi.getter
+    def passing(self) -> int:
+        """
+        Number of standards this resource successfully complies to.
+        """
+        return pulumi.get(self, "passing")
+
+    @property
+    @pulumi.getter
+    def total(self) -> int:
+        """
+        Number of standards associated to this resource.
+        """
+        return pulumi.get(self, "total")
+
+
+@pulumi.output_type
+class GetStandardsResourcesScoresResourceStandardResult(dict):
+    def __init__(__self__, *,
+                 active: bool,
+                 description: str,
+                 id: str,
+                 name: str,
+                 pass_: bool,
+                 type: str):
+        """
+        :param bool active: Indicates whether the standard is currently active and applicable to the resource.
+        :param str description: Provides a textual description of the standard.
+        :param str id: A unique identifier for the standard.
+        :param str name: The human-readable name of the standard.
+        :param bool pass_: Indicates whether the resource complies to this standard.
+        :param str type: The type of the standard.
+        """
+        pulumi.set(__self__, "active", active)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "pass_", pass_)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def active(self) -> bool:
+        """
+        Indicates whether the standard is currently active and applicable to the resource.
+        """
+        return pulumi.get(self, "active")
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        Provides a textual description of the standard.
+        """
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        A unique identifier for the standard.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The human-readable name of the standard.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="pass")
+    def pass_(self) -> bool:
+        """
+        Indicates whether the resource complies to this standard.
+        """
+        return pulumi.get(self, "pass_")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        The type of the standard.
+        """
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
+class GetStandardsStandardResult(dict):
+    def __init__(__self__, *,
+                 active: bool,
+                 description: str,
+                 exclusions: Sequence['outputs.GetStandardsStandardExclusionResult'],
+                 id: str,
+                 inclusions: Sequence['outputs.GetStandardsStandardInclusionResult'],
+                 name: str,
+                 resource_type: str,
+                 type: str):
+        """
+        :param bool active: Indicates whether the standard is currently active and applicable to the resource.
+        :param str description: Provides a textual description of the standard.
+        :param Sequence['GetStandardsStandardExclusionArgs'] exclusions: A list of exceptions for the application of this standard.
+        :param str id: The unique identifier for the resource being included.
+        :param Sequence['GetStandardsStandardInclusionArgs'] inclusions: A list of explict instances this standard applies to.
+        :param str name: The human-readable name of the standard.
+        :param str resource_type: Filter by `resource_type` the received standards. Allowed values are `technical_service`.
+        :param str type: Specifies the type of resource this inclusion applies to.
+        """
+        pulumi.set(__self__, "active", active)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "exclusions", exclusions)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "inclusions", inclusions)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "resource_type", resource_type)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def active(self) -> bool:
+        """
+        Indicates whether the standard is currently active and applicable to the resource.
+        """
+        return pulumi.get(self, "active")
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        Provides a textual description of the standard.
+        """
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def exclusions(self) -> Sequence['outputs.GetStandardsStandardExclusionResult']:
+        """
+        A list of exceptions for the application of this standard.
+        """
+        return pulumi.get(self, "exclusions")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The unique identifier for the resource being included.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def inclusions(self) -> Sequence['outputs.GetStandardsStandardInclusionResult']:
+        """
+        A list of explict instances this standard applies to.
+        """
+        return pulumi.get(self, "inclusions")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The human-readable name of the standard.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="resourceType")
+    def resource_type(self) -> str:
+        """
+        Filter by `resource_type` the received standards. Allowed values are `technical_service`.
+        """
+        return pulumi.get(self, "resource_type")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        Specifies the type of resource this inclusion applies to.
+        """
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
+class GetStandardsStandardExclusionResult(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 type: str):
+        """
+        :param str id: The unique identifier for the resource being included.
+        :param str type: Specifies the type of resource this inclusion applies to.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The unique identifier for the resource being included.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        Specifies the type of resource this inclusion applies to.
+        """
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
+class GetStandardsStandardInclusionResult(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 type: str):
+        """
+        :param str id: The unique identifier for the resource being included.
+        :param str type: Specifies the type of resource this inclusion applies to.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "type", type)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        """
+        The unique identifier for the resource being included.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        """
+        Specifies the type of resource this inclusion applies to.
+        """
+        return pulumi.get(self, "type")
+
+
+@pulumi.output_type
 class GetTeamMembersMemberResult(dict):
     def __init__(__self__, *,
                  id: str,
                  role: str,
                  summary: str,
                  type: str):
         """
```

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/provider.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/response_play.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/response_play.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/ruleset.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/ruleset_rule.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/ruleset_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/schedule.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/service.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/service_dependency.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/service_dependency.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/service_event_rule.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/service_event_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/service_integration.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/service_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/slack_connection.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/slack_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/tag.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/tag_assignment.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/tag_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/team.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/team_membership.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/team_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/user.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/user_contact_method.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/user_contact_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/user_notification_rule.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/user_notification_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty/webhook_subscription.py` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty/webhook_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty.egg-info/PKG-INFO` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_pagerduty
-Version: 4.9.0a1709366773
+Version: 4.9.0a1709566454
 Summary: A Pulumi package for creating and managing pagerduty cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-pagerduty
 Keywords: pulumi,pagerduty
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pulumi_pagerduty.egg-info/SOURCES.txt` & `pulumi_pagerduty-4.9.0a1709566454/pulumi_pagerduty.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 pulumi_pagerduty/get_license.py
 pulumi_pagerduty/get_licenses.py
 pulumi_pagerduty/get_priority.py
 pulumi_pagerduty/get_ruleset.py
 pulumi_pagerduty/get_schedule.py
 pulumi_pagerduty/get_service.py
 pulumi_pagerduty/get_service_integration.py
+pulumi_pagerduty/get_standards.py
+pulumi_pagerduty/get_standards_resource_scores.py
+pulumi_pagerduty/get_standards_resources_scores.py
 pulumi_pagerduty/get_tag.py
 pulumi_pagerduty/get_team.py
 pulumi_pagerduty/get_team_members.py
 pulumi_pagerduty/get_user.py
 pulumi_pagerduty/get_user_contact_method.py
 pulumi_pagerduty/get_users.py
 pulumi_pagerduty/get_vendor.py
```

### Comparing `pulumi_pagerduty-4.9.0a1709366773/pyproject.toml` & `pulumi_pagerduty-4.9.0a1709566454/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_pagerduty"
   description = "A Pulumi package for creating and managing pagerduty cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "pagerduty"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.9.0a1709366773"
+  version = "4.9.0a1709566454"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-pagerduty"
 
 [build-system]
```

