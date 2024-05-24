# Comparing `tmp/django_appointment-3.5.2.tar.gz` & `tmp/django_appointment-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_appointment-3.5.2.tar", last modified: Tue May 21 12:26:01 2024, max compression
+gzip compressed data, was "django_appointment-3.6.0.tar", last modified: Fri May 24 23:09:53 2024, max compression
```

## Comparing `django_appointment-3.5.2.tar` & `django_appointment-3.6.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.048050 django_appointment-3.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-21 12:25:49.000000 django_appointment-3.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-21 12:25:49.000000 django_appointment-3.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-21 12:26:01.048050 django_appointment-3.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-05-21 12:25:49.000000 django_appointment-3.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.028050 django_appointment-3.5.2/appointment/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/email_sender/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/email_sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/email_sender/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/logger_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/messages_.py
--rw-r--r--   0 runner    (1001) docker     (127)    33603 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.024050 django_appointment-3.5.2/appointment/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/css/app_admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/admin.css
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/btn.css
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/days_off.css
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/display_appointment.css
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/service.css
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/staff_member.css
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/user_profile.css
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/working_hours.css
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/appointments-user-details.css
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/appointments.css
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/appt-common.css
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/thank_you.css
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/verification_code.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)   119329 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/img/email_hd_bg.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/js/app_admin/
--rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/app_admin/staff_index.js
--rw-r--r--   0 runner    (1001) docker     (127)    15140 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/appointments.js
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/js-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/js/modal/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/modal/error_modal.js
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/modal/show_modal.js
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.024050 django_appointment-3.5.2/appointment/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.036050 django_appointment-3.5.2/appointment/templates/administration/
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/display_appointment.html
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/email_change_verification_code.html
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_day_off.html
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_service.html
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_staff_member.html
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_staff_personal_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_working_hours.html
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/service_list.html
--rw-r--r--   0 runner    (1001) docker     (127)    16047 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/staff_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/staff_list.html
--rw-r--r--   0 runner    (1001) docker     (127)    15954 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/user_profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.036050 django_appointment-3.5.2/appointment/templates/appointment/
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/appointment_client_information.html
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/appointments.html
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/default_thank_you.html
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/enter_verification_code.html
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/rescheduling_thank_you.html
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/set_password.html
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/thank_you.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.036050 django_appointment-3.5.2/appointment/templates/base_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/base_templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.036050 django_appointment-3.5.2/appointment/templates/email_sender/
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/email_sender/admin_new_appointment_email.html
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/email_sender/reminder_email.html
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/email_sender/reschedule_email.html
--rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/email_sender/thank_you_email.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/templates/error_pages/
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/error_pages/304_already_submitted.html
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/error_pages/403_forbidden.html
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/error_pages/403_forbidden_rescheduling.html
--rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/error_pages/404_not_found.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/templates/modal/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/modal/confirm_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/modal/error_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/modal/event_details_modal.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/tests/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/base/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/mixins/base_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.044050 django_appointment-3.5.2/appointment/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_appointment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_appointment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_appointment_reschedule_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_day_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_email_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_password_reset_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_payment_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_staff_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_working_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)    41704 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    56544 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.044050 django_appointment-3.5.2/appointment/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    51195 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_email_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_json_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_staff_member_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_view_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.048050 django_appointment-3.5.2/appointment/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    26916 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/email_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/json_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/view_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27957 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    24134 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/views_admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.048050 django_appointment-3.5.2/django_appointment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-21 12:26:00.000000 django_appointment-3.5.2/django_appointment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-21 12:26:01.000000 django_appointment-3.5.2/django_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:26:00.000000 django_appointment-3.5.2/django_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 12:26:00.000000 django_appointment-3.5.2/django_appointment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 12:26:00.000000 django_appointment-3.5.2/django_appointment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-21 12:25:49.000000 django_appointment-3.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-21 12:25:49.000000 django_appointment-3.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-21 12:26:01.048050 django_appointment-3.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-21 12:25:49.000000 django_appointment-3.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.326605 django_appointment-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-24 23:09:45.000000 django_appointment-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-24 23:09:45.000000 django_appointment-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16231 2024-05-24 23:09:53.326605 django_appointment-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14633 2024-05-24 23:09:45.000000 django_appointment-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.306605 django_appointment-3.6.0/appointment/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.306605 django_appointment-3.6.0/appointment/email_sender/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/email_sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/email_sender/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/logger_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/messages_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33603 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.302605 django_appointment-3.6.0/appointment/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.306605 django_appointment-3.6.0/appointment/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.310605 django_appointment-3.6.0/appointment/static/css/app_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/app_admin/admin.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/app_admin/btn.css
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/app_admin/days_off.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/app_admin/display_appointment.css
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/app_admin/service.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/app_admin/staff_member.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/app_admin/user_profile.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/app_admin/working_hours.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/appointments-user-details.css
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/appointments.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/appt-common.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/thank_you.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/css/verification_code.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.310605 django_appointment-3.6.0/appointment/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   119329 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/img/email_hd_bg.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.310605 django_appointment-3.6.0/appointment/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.310605 django_appointment-3.6.0/appointment/static/js/app_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/js/app_admin/staff_index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15140 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/js/appointments.js
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/js/js-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.310605 django_appointment-3.6.0/appointment/static/js/modal/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/js/modal/error_modal.js
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/static/js/modal/show_modal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.302605 django_appointment-3.6.0/appointment/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.314605 django_appointment-3.6.0/appointment/templates/administration/
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/display_appointment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/email_change_verification_code.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/manage_day_off.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/manage_service.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/manage_staff_member.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/manage_staff_personal_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/manage_working_hours.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/service_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16047 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/staff_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/staff_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15954 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/administration/user_profile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.314605 django_appointment-3.6.0/appointment/templates/appointment/
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/appointment/appointment_client_information.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/appointment/appointments.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/appointment/default_thank_you.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/appointment/enter_verification_code.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/appointment/rescheduling_thank_you.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/appointment/set_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/appointment/thank_you.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.314605 django_appointment-3.6.0/appointment/templates/base_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/base_templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.314605 django_appointment-3.6.0/appointment/templates/email_sender/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/email_sender/admin_new_appointment_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/email_sender/reminder_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/email_sender/reschedule_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/email_sender/thank_you_email.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.314605 django_appointment-3.6.0/appointment/templates/error_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/error_pages/304_already_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/error_pages/403_forbidden.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/error_pages/403_forbidden_rescheduling.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/error_pages/404_not_found.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.318605 django_appointment-3.6.0/appointment/templates/modal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/modal/confirm_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/modal/error_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/templates/modal/event_details_modal.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.318605 django_appointment-3.6.0/appointment/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.318605 django_appointment-3.6.0/appointment/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/base/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.318605 django_appointment-3.6.0/appointment/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/mixins/base_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.318605 django_appointment-3.6.0/appointment/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_appointment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_appointment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_appointment_reschedule_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_day_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_email_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_password_reset_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_payment_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_staff_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/models/test_working_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41704 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56614 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.322605 django_appointment-3.6.0/appointment/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/test_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51195 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/test_db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/test_email_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/test_json_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/test_staff_member_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/tests/utils/test_view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.322605 django_appointment-3.6.0/appointment/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26978 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/email_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/json_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/utils/view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27957 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24134 2024-05-24 23:09:45.000000 django_appointment-3.6.0/appointment/views_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:09:53.322605 django_appointment-3.6.0/django_appointment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16231 2024-05-24 23:09:53.000000 django_appointment-3.6.0/django_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-24 23:09:53.000000 django_appointment-3.6.0/django_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:09:53.000000 django_appointment-3.6.0/django_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 23:09:53.000000 django_appointment-3.6.0/django_appointment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 23:09:53.000000 django_appointment-3.6.0/django_appointment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-24 23:09:45.000000 django_appointment-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-24 23:09:45.000000 django_appointment-3.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-24 23:09:53.326605 django_appointment-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-24 23:09:45.000000 django_appointment-3.6.0/setup.py
```

### Comparing `django_appointment-3.5.2/LICENSE` & `django_appointment-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/MANIFEST.in` & `django_appointment-3.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/PKG-INFO` & `django_appointment-3.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 3.5.2
+Version: 3.6.0
 Summary: Managing appointment scheduling with customizable slots, staff features, and conflict handling.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: django-appt@adamspierredavid.com
 License: Apache License 2.0
 Project-URL: Author's Website, https://adamspierredavid.com/
 Project-URL: Package's demo Website, https://django-appt.adamspierredavid.com/
@@ -164,29 +164,30 @@
    It will be used in the footer of the emails sent to clients upon scheduling an appointment:
 
    ```html
    <p>® 2023 {{ APPOINTMENT_WEBSITE_NAME }}. All Rights Reserved.</p>
    ```
 
    To be able to send email reminders after adding `django_q` to your `INSTALLED_APPS`, you must add this variable
-   `Q_CLUSTER` in your Django's `settings.py`. If done, and users check the box to receive reminders, you and them
+   `Q_CLUSTER` in your Django's `settings.py`. If done, and users check the box to receive reminders, you and they
    will receive an email reminder 24 hours before the appointment.
 
-   Here's a configuration example, that you can use without modification (if you don't want to do much research):
+   Here's a configuration example that you can use without modification (if you don't want to do much research):
 
    ```python
    Q_CLUSTER = {
       'name': 'DjangORM',
       'workers': 4,
       'timeout': 90,
       'retry': 120,
       'queue_limit': 50,
       'bulk': 10,
       'orm': 'default',
    }
+   USE_DJANGO_Q_FOR_EMAILS = True  # 🆕 Use Django Q for sending ALL email.
    ```
 
 5. Next would be to create the migrations and run them by doing `python manage.py makemigrations appointment` and right
    after, run `python manage.py migrate` to create the appointment models.
 
 6. Start the Django Q cluster with `python manage.py qcluster`.
 
@@ -194,14 +195,52 @@
    configurations, and handle appointment conflicts (the Admin app must be enabled).
 8. You must create at least one service before using the application on the admin page. If your service is free, input 0
    as the price. If your service is paid, input the price in the price field. You may also provide a description for
    your service.
 9. Visit http://127.0.0.1:8000/appointment/request/<service_id>/ to view the available time slots and schedule an
    appointment.
 
+## Template Configuration 📝
+
+If you're using a base.html template, you must include the following block in your template:
+
+```
+{% block customCSS %}
+{% endblock %}
+
+{% block title %}
+{% endblock %}
+
+{% block description %}
+{% endblock %}
+
+{% block body %}
+{% endblock %}
+
+{% block customJS %}
+{% endblock %}
+```
+
+At least the block for css, body and js are required; otherwise the application will not work properly. 
+Jquery is also required to be included in the template.
+
+The title and description are optional but recommended for SEO purposes.
+
+See an example of a base.html template [here](https://github.com/adamspd/django-appointment/blob/main/appointment/templates/base_templates/base.html).
+
+
+## Customization 🔧
+
+1. In your Django project's `settings.py`, you can override the default values for the appointment scheduler.
+   More information regarding available configurations can be found in
+   the [documentation](https://github.com/adamspd/django-appointment/tree/main/docs/README.md#configuration).
+2. Modify these values as needed for your application, and the app will adapt to the new settings.
+3. For further customization, you can extend the provided models, views, and templates or create your own.
+
+
 ## Docker Support 🐳
 
 Django-Appointment now supports Docker, making it easier to set up, develop, and test.
 
 ### Getting Started with Docker for Development or Local Testing
 
 Using Django-Appointment with Docker is primarily intended for **development purposes** or **local testing**.
@@ -226,16 +265,18 @@
    ```
 
 2. **Prepare an .env File**: Create an `.env` file in the root directory of your project with your configuration
    settings.
    You should include your email host user and password for Django's email functionality (if you want it to work):
 
    ```plaintext
-   EMAIL_HOST_USER=your_email@gmail.com
+   EMAIL_HOST_USER=your_email@example.com
    EMAIL_HOST_PASSWORD=your_password
+   ADMIN_NAME='Example Name'
+   ADMIN_EMAIL=django-appt@example.com
    ```
 
    > **Note:** The `.env` file is used to store sensitive information and should not be committed to version control.
 
 3. **Build and Run the Docker Containers**: Run the following command to build and run the Docker containers:
 
    ```bash
@@ -288,22 +329,15 @@
    docker-compose down
    # docker compose down
    ```
 
    > **Note:** I used the default database settings for the Docker container.
    > If you want to use a different database, you can modify the Dockerfile and docker-compose.yml files to use your
    > preferred database.
-
-## Customization 🔧
-
-1. In your Django project's `settings.py`, you can override the default values for the appointment scheduler. More
-   information regarding available configurations can be found in
-   the [documentation](https://github.com/adamspd/django-appointment/tree/main/docs/README.md#configuration).
-2. Modify these values as needed for your application, and the app will adapt to the new settings.
-3. For further customization, you can extend the provided models, views, and templates or create your own.
+   
 
 ## Compatibility Matrix 📊
 
 A compatibility matrix is available to help you determine which versions of Django and Python are compatible with the
 package.
 The matrix is updated regularly to reflect the latest compatibility test results. For more information, please
 refer to
```

### Comparing `django_appointment-3.5.2/README.md` & `django_appointment-3.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -128,29 +128,30 @@
    It will be used in the footer of the emails sent to clients upon scheduling an appointment:
 
    ```html
    <p>® 2023 {{ APPOINTMENT_WEBSITE_NAME }}. All Rights Reserved.</p>
    ```
 
    To be able to send email reminders after adding `django_q` to your `INSTALLED_APPS`, you must add this variable
-   `Q_CLUSTER` in your Django's `settings.py`. If done, and users check the box to receive reminders, you and them
+   `Q_CLUSTER` in your Django's `settings.py`. If done, and users check the box to receive reminders, you and they
    will receive an email reminder 24 hours before the appointment.
 
-   Here's a configuration example, that you can use without modification (if you don't want to do much research):
+   Here's a configuration example that you can use without modification (if you don't want to do much research):
 
    ```python
    Q_CLUSTER = {
       'name': 'DjangORM',
       'workers': 4,
       'timeout': 90,
       'retry': 120,
       'queue_limit': 50,
       'bulk': 10,
       'orm': 'default',
    }
+   USE_DJANGO_Q_FOR_EMAILS = True  # 🆕 Use Django Q for sending ALL email.
    ```
 
 5. Next would be to create the migrations and run them by doing `python manage.py makemigrations appointment` and right
    after, run `python manage.py migrate` to create the appointment models.
 
 6. Start the Django Q cluster with `python manage.py qcluster`.
 
@@ -158,14 +159,52 @@
    configurations, and handle appointment conflicts (the Admin app must be enabled).
 8. You must create at least one service before using the application on the admin page. If your service is free, input 0
    as the price. If your service is paid, input the price in the price field. You may also provide a description for
    your service.
 9. Visit http://127.0.0.1:8000/appointment/request/<service_id>/ to view the available time slots and schedule an
    appointment.
 
+## Template Configuration 📝
+
+If you're using a base.html template, you must include the following block in your template:
+
+```
+{% block customCSS %}
+{% endblock %}
+
+{% block title %}
+{% endblock %}
+
+{% block description %}
+{% endblock %}
+
+{% block body %}
+{% endblock %}
+
+{% block customJS %}
+{% endblock %}
+```
+
+At least the block for css, body and js are required; otherwise the application will not work properly. 
+Jquery is also required to be included in the template.
+
+The title and description are optional but recommended for SEO purposes.
+
+See an example of a base.html template [here](https://github.com/adamspd/django-appointment/blob/main/appointment/templates/base_templates/base.html).
+
+
+## Customization 🔧
+
+1. In your Django project's `settings.py`, you can override the default values for the appointment scheduler.
+   More information regarding available configurations can be found in
+   the [documentation](https://github.com/adamspd/django-appointment/tree/main/docs/README.md#configuration).
+2. Modify these values as needed for your application, and the app will adapt to the new settings.
+3. For further customization, you can extend the provided models, views, and templates or create your own.
+
+
 ## Docker Support 🐳
 
 Django-Appointment now supports Docker, making it easier to set up, develop, and test.
 
 ### Getting Started with Docker for Development or Local Testing
 
 Using Django-Appointment with Docker is primarily intended for **development purposes** or **local testing**.
@@ -190,16 +229,18 @@
    ```
 
 2. **Prepare an .env File**: Create an `.env` file in the root directory of your project with your configuration
    settings.
    You should include your email host user and password for Django's email functionality (if you want it to work):
 
    ```plaintext
-   EMAIL_HOST_USER=your_email@gmail.com
+   EMAIL_HOST_USER=your_email@example.com
    EMAIL_HOST_PASSWORD=your_password
+   ADMIN_NAME='Example Name'
+   ADMIN_EMAIL=django-appt@example.com
    ```
 
    > **Note:** The `.env` file is used to store sensitive information and should not be committed to version control.
 
 3. **Build and Run the Docker Containers**: Run the following command to build and run the Docker containers:
 
    ```bash
@@ -252,22 +293,15 @@
    docker-compose down
    # docker compose down
    ```
 
    > **Note:** I used the default database settings for the Docker container.
    > If you want to use a different database, you can modify the Dockerfile and docker-compose.yml files to use your
    > preferred database.
-
-## Customization 🔧
-
-1. In your Django project's `settings.py`, you can override the default values for the appointment scheduler. More
-   information regarding available configurations can be found in
-   the [documentation](https://github.com/adamspd/django-appointment/tree/main/docs/README.md#configuration).
-2. Modify these values as needed for your application, and the app will adapt to the new settings.
-3. For further customization, you can extend the provided models, views, and templates or create your own.
+   
 
 ## Compatibility Matrix 📊
 
 A compatibility matrix is available to help you determine which versions of Django and Python are compatible with the
 package.
 The matrix is updated regularly to reflect the latest compatibility test results. For more information, please
 refer to
```

### Comparing `django_appointment-3.5.2/appointment/__init__.py` & `django_appointment-3.6.0/appointment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,9 +2,9 @@
 __author_email__ = "django-appt@adamspierredavid.com"
 __author_website__ = "https://adamspierredavid.com/"
 __description__ = "Managing appointment scheduling with customizable slots, staff features, and conflict handling."
 __package_name__ = "django-appointment"
 __url__ = "https://github.com/adamspd/django-appointment"
 __package_website__ = "https://django-appt.adamspierredavid.com/"
 __package_doc_url__ = "https://django-appt-doc.adamspierredavid.com/overview.html"
-__version__ = "3.5.2"
+__version__ = "3.6.0"
 __test_version__ = False
```

### Comparing `django_appointment-3.5.2/appointment/admin.py` & `django_appointment-3.6.0/appointment/admin.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/decorators.py` & `django_appointment-3.6.0/appointment/decorators.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/email_sender/email_sender.py` & `django_appointment-3.6.0/appointment/tasks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,73 +1,65 @@
-from django.conf import settings
-from django.core.mail import mail_admins, send_mail
-from django.template import loader
-
-from appointment.settings import APP_DEFAULT_FROM_EMAIL
-
-
-def has_required_email_settings():
-    required_settings = [
-        'EMAIL_BACKEND',
-        'EMAIL_HOST',
-        'EMAIL_PORT',
-        'EMAIL_HOST_USER',
-        'EMAIL_HOST_PASSWORD',
-        'EMAIL_USE_TLS',
-        'EMAIL_USE_LOCALTIME',
-        'ADMINS',
-    ]
-
-    for setting_name in required_settings:
-        if not hasattr(settings, setting_name):
-            print(f"Warning: '{setting_name}' not found in settings. Email functionality will be disabled.")
-            return False
-    return True
-
-
-def send_email(recipient_list, subject: str, template_url: str = None, context: dict = None, from_email=None,
-               message: str = None):
-    if not has_required_email_settings():
-        return
-
-    if from_email is None:
-        from_email = APP_DEFAULT_FROM_EMAIL
-
-    html_message = ""
-
-    if template_url:
-        html_message = loader.render_to_string(
-            template_name=template_url,
-            context=context
-        )
+# tasks.py
+# Path: appointment/tasks.py
 
+"""
+Author: Adams Pierre David
+Since: 3.1.0
+"""
+from django.utils.translation import gettext as _
+
+from appointment.email_sender import notify_admin, send_email
+from appointment.logger_config import logger
+from appointment.models import Appointment
+
+
+def send_email_reminder(to_email, first_name, reschedule_link, appointment_id):
+    """
+    Send a reminder email to the client about the upcoming appointment.
+    """
+
+    # Fetch the appointment using appointment_id
+    logger.info(f"Sending reminder to {to_email} for appointment {appointment_id}")
+    appointment = Appointment.objects.get(id=appointment_id)
+    recipient_type = 'client'
+    email_context = {
+        'first_name': first_name,
+        'appointment': appointment,
+        'reschedule_link': reschedule_link,
+        'recipient_type': recipient_type,
+    }
+    send_email(
+            recipient_list=[to_email], subject=_("Reminder: Upcoming Appointment"),
+            template_url='email_sender/reminder_email.html', context=email_context
+    )
+    # Notify the admin
+    email_context['recipient_type'] = 'admin'
+    notify_admin(
+            subject=_("Admin Reminder: Upcoming Appointment"),
+            template_url='email_sender/reminder_email.html', context=email_context
+    )
+
+
+def send_email_task(recipient_list, subject, message, html_message, from_email):
+    """
+   Task function to send an email asynchronously using Django's send_mail function.
+   This function tries to send an email and logs an error if it fails.
+   """
     try:
+        from django.core.mail import send_mail
         send_mail(
-            subject=subject,
-            message=message if not template_url else "",
-            html_message=html_message if template_url else None,
-            from_email=from_email,
-            recipient_list=recipient_list,
-            fail_silently=False,
+                subject=subject, message=message, html_message=html_message, from_email=from_email,
+                recipient_list=recipient_list, fail_silently=False,
         )
     except Exception as e:
-        print(f"Error sending email: {e}")
+        print(f"Error sending email from task: {e}")
 
 
-def notify_admin(subject: str, template_url: str = None, context: dict = None, message: str = None):
-    if not has_required_email_settings():
-        return
-
-    html_message = ""
-    if template_url:
-        html_message = loader.render_to_string(
-            template_name=template_url,
-            context=context
-        )
+def notify_admin_task(subject, message, html_message):
+    """
+    Task function to send an admin email asynchronously.
+    """
     try:
-        mail_admins(
-            subject=subject,
-            message=message if not template_url else "",
-            html_message=html_message if template_url else None
-        )
+        from django.core.mail import mail_admins
+        mail_admins(subject=subject, message=message, html_message=html_message, fail_silently=False)
     except Exception as e:
-        print(f"Error sending email to admin: {e}")
+        print(f"Error sending admin email from task: {e}")
```

### Comparing `django_appointment-3.5.2/appointment/forms.py` & `django_appointment-3.6.0/appointment/forms.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/messages_.py` & `django_appointment-3.6.0/appointment/messages_.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/models.py` & `django_appointment-3.6.0/appointment/models.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/services.py` & `django_appointment-3.6.0/appointment/services.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/settings.py` & `django_appointment-3.6.0/appointment/settings.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/app_admin/admin.css` & `django_appointment-3.6.0/appointment/static/css/app_admin/admin.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/app_admin/btn.css` & `django_appointment-3.6.0/appointment/static/css/app_admin/btn.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/app_admin/days_off.css` & `django_appointment-3.6.0/appointment/static/css/app_admin/days_off.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/app_admin/display_appointment.css` & `django_appointment-3.6.0/appointment/static/css/app_admin/display_appointment.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/app_admin/service.css` & `django_appointment-3.6.0/appointment/static/css/app_admin/service.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/app_admin/staff_member.css` & `django_appointment-3.6.0/appointment/static/css/app_admin/staff_member.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/app_admin/user_profile.css` & `django_appointment-3.6.0/appointment/static/css/app_admin/user_profile.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/app_admin/working_hours.css` & `django_appointment-3.6.0/appointment/static/css/app_admin/working_hours.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/appointments-user-details.css` & `django_appointment-3.6.0/appointment/static/css/appointments-user-details.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/appt-common.css` & `django_appointment-3.6.0/appointment/static/css/appt-common.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/thank_you.css` & `django_appointment-3.6.0/appointment/static/css/thank_you.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/css/verification_code.css` & `django_appointment-3.6.0/appointment/static/css/verification_code.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/img/email_hd_bg.jpg` & `django_appointment-3.6.0/appointment/static/img/email_hd_bg.jpg`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/js/app_admin/staff_index.js` & `django_appointment-3.6.0/appointment/static/js/app_admin/staff_index.js`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/js/appointments.js` & `django_appointment-3.6.0/appointment/static/js/appointments.js`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/js/modal/error_modal.js` & `django_appointment-3.6.0/appointment/static/js/modal/error_modal.js`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/static/js/modal/show_modal.js` & `django_appointment-3.6.0/appointment/static/js/modal/show_modal.js`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/display_appointment.html` & `django_appointment-3.6.0/appointment/templates/administration/display_appointment.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/email_change_verification_code.html` & `django_appointment-3.6.0/appointment/templates/administration/email_change_verification_code.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/manage_day_off.html` & `django_appointment-3.6.0/appointment/templates/administration/manage_day_off.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/manage_service.html` & `django_appointment-3.6.0/appointment/templates/administration/manage_service.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/manage_staff_member.html` & `django_appointment-3.6.0/appointment/templates/administration/manage_staff_member.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/manage_staff_personal_info.html` & `django_appointment-3.6.0/appointment/templates/administration/manage_staff_personal_info.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/manage_working_hours.html` & `django_appointment-3.6.0/appointment/templates/administration/manage_working_hours.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/service_list.html` & `django_appointment-3.6.0/appointment/templates/administration/service_list.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/staff_index.html` & `django_appointment-3.6.0/appointment/templates/administration/staff_index.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/staff_list.html` & `django_appointment-3.6.0/appointment/templates/administration/staff_list.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/administration/user_profile.html` & `django_appointment-3.6.0/appointment/templates/administration/user_profile.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/appointment/appointment_client_information.html` & `django_appointment-3.6.0/appointment/templates/appointment/appointment_client_information.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/appointment/appointments.html` & `django_appointment-3.6.0/appointment/templates/appointment/appointments.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/appointment/default_thank_you.html` & `django_appointment-3.6.0/appointment/templates/appointment/default_thank_you.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/appointment/enter_verification_code.html` & `django_appointment-3.6.0/appointment/templates/appointment/enter_verification_code.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/appointment/rescheduling_thank_you.html` & `django_appointment-3.6.0/appointment/templates/appointment/rescheduling_thank_you.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/appointment/set_password.html` & `django_appointment-3.6.0/appointment/templates/appointment/set_password.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/appointment/thank_you.html` & `django_appointment-3.6.0/appointment/templates/appointment/thank_you.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/base_templates/base.html` & `django_appointment-3.6.0/appointment/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/email_sender/admin_new_appointment_email.html` & `django_appointment-3.6.0/appointment/templates/email_sender/admin_new_appointment_email.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/email_sender/reminder_email.html` & `django_appointment-3.6.0/appointment/templates/email_sender/reminder_email.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/email_sender/reschedule_email.html` & `django_appointment-3.6.0/appointment/templates/email_sender/reschedule_email.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/email_sender/thank_you_email.html` & `django_appointment-3.6.0/appointment/templates/email_sender/thank_you_email.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/error_pages/304_already_submitted.html` & `django_appointment-3.6.0/appointment/templates/error_pages/304_already_submitted.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/error_pages/403_forbidden.html` & `django_appointment-3.6.0/appointment/templates/error_pages/403_forbidden.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/error_pages/403_forbidden_rescheduling.html` & `django_appointment-3.6.0/appointment/templates/error_pages/403_forbidden_rescheduling.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/error_pages/404_not_found.html` & `django_appointment-3.6.0/appointment/templates/error_pages/404_not_found.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/modal/confirm_modal.html` & `django_appointment-3.6.0/appointment/templates/modal/confirm_modal.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/modal/error_modal.html` & `django_appointment-3.6.0/appointment/templates/modal/error_modal.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/templates/modal/event_details_modal.html` & `django_appointment-3.6.0/appointment/templates/modal/event_details_modal.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/base/base_test.py` & `django_appointment-3.6.0/appointment/tests/base/base_test.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/mixins/base_mixin.py` & `django_appointment-3.6.0/appointment/tests/mixins/base_mixin.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_appointment.py` & `django_appointment-3.6.0/appointment/tests/models/test_appointment.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_appointment_request.py` & `django_appointment-3.6.0/appointment/tests/models/test_appointment_request.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_appointment_reschedule_history.py` & `django_appointment-3.6.0/appointment/tests/models/test_appointment_reschedule_history.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_config.py` & `django_appointment-3.6.0/appointment/tests/models/test_config.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_day_off.py` & `django_appointment-3.6.0/appointment/tests/models/test_day_off.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_email_verification.py` & `django_appointment-3.6.0/appointment/tests/models/test_email_verification.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_password_reset_token.py` & `django_appointment-3.6.0/appointment/tests/models/test_password_reset_token.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_payment_info.py` & `django_appointment-3.6.0/appointment/tests/models/test_payment_info.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_service.py` & `django_appointment-3.6.0/appointment/tests/models/test_service.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_staff_member.py` & `django_appointment-3.6.0/appointment/tests/models/test_staff_member.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/models/test_working_hours.py` & `django_appointment-3.6.0/appointment/tests/models/test_working_hours.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/test_services.py` & `django_appointment-3.6.0/appointment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/test_settings.py` & `django_appointment-3.6.0/appointment/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/test_tasks.py` & `django_appointment-3.6.0/appointment/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/test_views.py` & `django_appointment-3.6.0/appointment/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1235,14 +1235,15 @@
         self.client_data = {'name': 'Orlin Ascended', 'email': 'orlin.ascended@django-appointment.com'}
         self.appointment_data = {'phone': '1234567890', 'want_reminder': True, 'address': '123 Ancient St, Velona',
                                  'additional_info': 'Test info'}
         self.request = RequestFactory().get('/')
 
     @patch('appointment.views.create_and_save_appointment')
     @patch('appointment.views.redirect_to_payment_or_thank_you_page')
+    @patch('django.conf.settings.USE_DJANGO_Q_FOR_EMAILS', new=False)
     def test_create_appointment_success(self, mock_redirect, mock_create_and_save):
         """Test successful creation of an appointment and redirection."""
         # Mock the appointment creation to return an Appointment instance
         mock_appointment = MagicMock()
         mock_create_and_save.return_value = mock_appointment
 
         # Mock the redirection function to simulate a successful redirection
```

### Comparing `django_appointment-3.5.2/appointment/tests/utils/test_date_time.py` & `django_appointment-3.6.0/appointment/tests/utils/test_date_time.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/utils/test_db_helpers.py` & `django_appointment-3.6.0/appointment/tests/utils/test_db_helpers.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/utils/test_email_ops.py` & `django_appointment-3.6.0/appointment/tests/utils/test_email_ops.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/utils/test_json_context.py` & `django_appointment-3.6.0/appointment/tests/utils/test_json_context.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/utils/test_permissions.py` & `django_appointment-3.6.0/appointment/tests/utils/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/utils/test_session.py` & `django_appointment-3.6.0/appointment/tests/utils/test_session.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/utils/test_staff_member_time.py` & `django_appointment-3.6.0/appointment/tests/utils/test_staff_member_time.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/utils/test_validators.py` & `django_appointment-3.6.0/appointment/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/tests/utils/test_view_helpers.py` & `django_appointment-3.6.0/appointment/tests/utils/test_view_helpers.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/urls.py` & `django_appointment-3.6.0/appointment/urls.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/utils/date_time.py` & `django_appointment-3.6.0/appointment/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/utils/db_helpers.py` & `django_appointment-3.6.0/appointment/utils/db_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,16 @@
     user = get_user_by_email(client_data['email'])
     appointment = Appointment.objects.create(
             client=user, appointment_request=ar,
             **appointment_data
     )
     appointment.save()
     logger.info(f"New appointment created: {appointment.to_dict()}")
-    schedule_email_reminder(appointment, request)
+    if appointment.want_reminder:
+        schedule_email_reminder(appointment, request)
     return appointment
 
 
 def schedule_email_reminder(appointment, request, appointment_datetime=None):
     """Schedule an email reminder for the given appointment."""
     # Check if the Django-Q cluster is running
     from appointment.settings import check_q_cluster
@@ -175,15 +176,16 @@
         cancel_existing_reminder(appointment.id_request)
 
         # If a reminder is still desired and the appointment is in the future, schedule a new one
         if want_reminder and new_datetime > timezone.now():
             schedule_email_reminder(appointment, request, new_datetime)
         else:
             logger.info(
-                    f"Reminder for appointment {appointment.id} is not scheduled per user's preference or past datetime.")
+                    f"Reminder for appointment {appointment.id} is not scheduled per "
+                    f"user's preference or past datetime.")
 
     # Update the appointment's reminder preference
     appointment.want_reminder = want_reminder
     appointment.save()
 
 
 def cancel_existing_reminder(appointment_id_request):
```

### Comparing `django_appointment-3.5.2/appointment/utils/email_ops.py` & `django_appointment-3.6.0/appointment/utils/email_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     :return: None
     """
     # Month and year like "J A N 2 0 2 1"
     token = PasswordResetToken.create_token(user=user, expiration_minutes=10080)  # 7 days expiration
     ui_db64 = urlsafe_base64_encode(force_bytes(user.pk))
     relative_set_passwd_link = reverse('appointment:set_passwd', args=[ui_db64, token.token])
     set_passwd_link = get_absolute_url_(relative_set_passwd_link, request=request)
+    website_name = get_website_name()
 
     message = _("""
         Hello {first_name},
 
         A request has been received to set a password for your staff account for the year {current_year} at {company}.
 
         Please click the link below to set up your new password:
@@ -118,24 +119,24 @@
         {account_details}
 
         Regards,
         {company}
         """).format(
         first_name=user.first_name,
         current_year=datetime.datetime.now().year,
-        company=get_website_name(),
+        company=website_name,
         activation_link=set_passwd_link,
         account_details=account_details if account_details else _("No additional details provided."),
         username=user.username
     )
 
     # Assuming send_email is a method you have that sends an email
     send_email(
         recipient_list=[email],
-        subject=_("Set Your Password for {company}").format(company=get_website_name()),
+        subject=_("Set Your Password for {company}").format(company=website_name),
         message=message,
     )
 
 
 def notify_admin_about_appointment(appointment, client_name: str):
     """Notify the admin and the staff member about a new appointment request."""
     email_context = {
```

### Comparing `django_appointment-3.5.2/appointment/utils/error_codes.py` & `django_appointment-3.6.0/appointment/utils/error_codes.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/utils/json_context.py` & `django_appointment-3.6.0/appointment/utils/json_context.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/utils/permissions.py` & `django_appointment-3.6.0/appointment/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/utils/session.py` & `django_appointment-3.6.0/appointment/utils/session.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/utils/view_helpers.py` & `django_appointment-3.6.0/appointment/utils/view_helpers.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/views.py` & `django_appointment-3.6.0/appointment/views.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/appointment/views_admin.py` & `django_appointment-3.6.0/appointment/views_admin.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/django_appointment.egg-info/PKG-INFO` & `django_appointment-3.6.0/django_appointment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 3.5.2
+Version: 3.6.0
 Summary: Managing appointment scheduling with customizable slots, staff features, and conflict handling.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: django-appt@adamspierredavid.com
 License: Apache License 2.0
 Project-URL: Author's Website, https://adamspierredavid.com/
 Project-URL: Package's demo Website, https://django-appt.adamspierredavid.com/
@@ -164,29 +164,30 @@
    It will be used in the footer of the emails sent to clients upon scheduling an appointment:
 
    ```html
    <p>® 2023 {{ APPOINTMENT_WEBSITE_NAME }}. All Rights Reserved.</p>
    ```
 
    To be able to send email reminders after adding `django_q` to your `INSTALLED_APPS`, you must add this variable
-   `Q_CLUSTER` in your Django's `settings.py`. If done, and users check the box to receive reminders, you and them
+   `Q_CLUSTER` in your Django's `settings.py`. If done, and users check the box to receive reminders, you and they
    will receive an email reminder 24 hours before the appointment.
 
-   Here's a configuration example, that you can use without modification (if you don't want to do much research):
+   Here's a configuration example that you can use without modification (if you don't want to do much research):
 
    ```python
    Q_CLUSTER = {
       'name': 'DjangORM',
       'workers': 4,
       'timeout': 90,
       'retry': 120,
       'queue_limit': 50,
       'bulk': 10,
       'orm': 'default',
    }
+   USE_DJANGO_Q_FOR_EMAILS = True  # 🆕 Use Django Q for sending ALL email.
    ```
 
 5. Next would be to create the migrations and run them by doing `python manage.py makemigrations appointment` and right
    after, run `python manage.py migrate` to create the appointment models.
 
 6. Start the Django Q cluster with `python manage.py qcluster`.
 
@@ -194,14 +195,52 @@
    configurations, and handle appointment conflicts (the Admin app must be enabled).
 8. You must create at least one service before using the application on the admin page. If your service is free, input 0
    as the price. If your service is paid, input the price in the price field. You may also provide a description for
    your service.
 9. Visit http://127.0.0.1:8000/appointment/request/<service_id>/ to view the available time slots and schedule an
    appointment.
 
+## Template Configuration 📝
+
+If you're using a base.html template, you must include the following block in your template:
+
+```
+{% block customCSS %}
+{% endblock %}
+
+{% block title %}
+{% endblock %}
+
+{% block description %}
+{% endblock %}
+
+{% block body %}
+{% endblock %}
+
+{% block customJS %}
+{% endblock %}
+```
+
+At least the block for css, body and js are required; otherwise the application will not work properly. 
+Jquery is also required to be included in the template.
+
+The title and description are optional but recommended for SEO purposes.
+
+See an example of a base.html template [here](https://github.com/adamspd/django-appointment/blob/main/appointment/templates/base_templates/base.html).
+
+
+## Customization 🔧
+
+1. In your Django project's `settings.py`, you can override the default values for the appointment scheduler.
+   More information regarding available configurations can be found in
+   the [documentation](https://github.com/adamspd/django-appointment/tree/main/docs/README.md#configuration).
+2. Modify these values as needed for your application, and the app will adapt to the new settings.
+3. For further customization, you can extend the provided models, views, and templates or create your own.
+
+
 ## Docker Support 🐳
 
 Django-Appointment now supports Docker, making it easier to set up, develop, and test.
 
 ### Getting Started with Docker for Development or Local Testing
 
 Using Django-Appointment with Docker is primarily intended for **development purposes** or **local testing**.
@@ -226,16 +265,18 @@
    ```
 
 2. **Prepare an .env File**: Create an `.env` file in the root directory of your project with your configuration
    settings.
    You should include your email host user and password for Django's email functionality (if you want it to work):
 
    ```plaintext
-   EMAIL_HOST_USER=your_email@gmail.com
+   EMAIL_HOST_USER=your_email@example.com
    EMAIL_HOST_PASSWORD=your_password
+   ADMIN_NAME='Example Name'
+   ADMIN_EMAIL=django-appt@example.com
    ```
 
    > **Note:** The `.env` file is used to store sensitive information and should not be committed to version control.
 
 3. **Build and Run the Docker Containers**: Run the following command to build and run the Docker containers:
 
    ```bash
@@ -288,22 +329,15 @@
    docker-compose down
    # docker compose down
    ```
 
    > **Note:** I used the default database settings for the Docker container.
    > If you want to use a different database, you can modify the Dockerfile and docker-compose.yml files to use your
    > preferred database.
-
-## Customization 🔧
-
-1. In your Django project's `settings.py`, you can override the default values for the appointment scheduler. More
-   information regarding available configurations can be found in
-   the [documentation](https://github.com/adamspd/django-appointment/tree/main/docs/README.md#configuration).
-2. Modify these values as needed for your application, and the app will adapt to the new settings.
-3. For further customization, you can extend the provided models, views, and templates or create your own.
+   
 
 ## Compatibility Matrix 📊
 
 A compatibility matrix is available to help you determine which versions of Django and Python are compatible with the
 package.
 The matrix is updated regularly to reflect the latest compatibility test results. For more information, please
 refer to
```

### Comparing `django_appointment-3.5.2/django_appointment.egg-info/SOURCES.txt` & `django_appointment-3.6.0/django_appointment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/setup.cfg` & `django_appointment-3.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.2/setup.py` & `django_appointment-3.6.0/setup.py`

 * *Files identical despite different names*

