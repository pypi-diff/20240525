# Comparing `tmp/pluggy_sdk-1.0.0.post8.tar.gz` & `tmp/pluggy_sdk-1.0.0.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluggy_sdk-1.0.0.post8.tar", last modified: Mon May  6 20:30:26 2024, max compression
+gzip compressed data, was "pluggy_sdk-1.0.0.post9.tar", last modified: Sat May 18 01:08:38 2024, max compression
```

## Comparing `pluggy_sdk-1.0.0.post8.tar` & `pluggy_sdk-1.0.0.post9.tar`

### file list

```diff
@@ -1,335 +1,343 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:30:26.538095 pluggy_sdk-1.0.0.post8/
--rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-05-06 20:30:26.538095 pluggy_sdk-1.0.0.post8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20469 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:30:26.486095 pluggy_sdk-1.0.0.post8/pluggy_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:30:26.490095 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22047 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26206 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/acquirer_anticipation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26120 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/acquirer_receivable_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25869 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/acquirer_sale_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22882 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20960 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/bill_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32808 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/bulk_payment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41577 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/category_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41008 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/connector_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21602 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/identity_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/income_report_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35989 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/investment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54593 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/items_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/loan_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54784 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/payment_customer_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32020 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/payment_intent_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    77933 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/payment_recipient_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    94243 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/payment_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22320 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/portfolio_yield_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    43323 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/smart_account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37553 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55525 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api/webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:30:26.510095 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/accounts_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_anticipation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_anticipation_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable_data_establishment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable_destination_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable_related_sale.py
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_sale.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_sale_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_sale_installment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_sale_installment_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/aggregated_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/aggregated_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/asset_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/auth_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bank_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bill_finance_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bills_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bulk_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bulk_payments_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/client_category_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connect_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connect_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_health_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_user_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_bulk_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_client_category_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_item_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_or_update_payment_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_payment_customer_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_pix_qr_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_smart_account_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-06 20:29:38.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/credential_select_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/credit_card_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/credit_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/global_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/i_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/identity_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/income_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/income_reports_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investment_expenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investment_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investment_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investments_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/item_creation_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/item_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/item_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_contracted_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_contracted_finance_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_installment_balloon_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_installment_balloon_payment_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_installments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_interest_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payment_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payment_release_over_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payment_release_over_parcel_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payment_release_over_parcel_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_warranty.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loans_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/merchant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/monthly_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/monthly_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/not_authenticated_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_acquirer_anticipations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_acquirer_receivables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_acquirer_sales.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_category_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_investment_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/parameter_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/parameter_validation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_customers_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_data_participant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_institution.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_intent_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_intents_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_receipt_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_receipt_person.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_recipient_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_recipients_institution_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_recipients_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_request_callback_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_request_receipt_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_requests_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/percentage_over_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/pix_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/smart_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/smart_account_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/smart_account_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/smart_accounts_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/status_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/status_detail_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/status_detail_product_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_item_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/webhook_creation_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/models/webhooks_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:30:26.538095 pluggy_sdk-1.0.0.post8/pluggy_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-05-06 20:30:26.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-05-06 20:30:26.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:30:26.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 20:30:26.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 20:30:26.000000 pluggy_sdk-1.0.0.post8/pluggy_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-06 20:29:39.000000 pluggy_sdk-1.0.0.post8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 20:30:26.538095 pluggy_sdk-1.0.0.post8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-06 20:30:24.000000 pluggy_sdk-1.0.0.post8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:30:26.538095 pluggy_sdk-1.0.0.post8/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_accounts_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_anticipation.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_anticipation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_anticipation_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_data_establishment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_destination_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_related_sale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_sale.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_sale_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_sale_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_sale_installment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_acquirer_sale_installment_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_aggregated_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_aggregated_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_asset_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_auth_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_auth_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_auth_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_bank_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_bill_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_bill_finance_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_bills_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_bulk_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_bulk_payment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_bulk_payments_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_category_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_client_category_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_company.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_connect_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_connect_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_connector_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_connector_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_connector_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_connector_health_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_connector_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_connector_user_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_bulk_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_client_category_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_item_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_or_update_payment_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_payment_customer_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_pix_qr_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_smart_account_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_create_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_credential_select_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_credit_card_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_credit_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_global_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_i_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_identity_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_identity_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_income_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_income_report_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_income_reports_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_investment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_investment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_investment_expenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_investment_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_investment_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_investments_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_item_creation_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_item_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_item_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_items_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_contracted_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_contracted_finance_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_installment_balloon_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_installment_balloon_payment_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_installments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_interest_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_payment_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_payment_release_over_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_payment_release_over_parcel_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_payment_release_over_parcel_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loan_warranty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_loans_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_merchant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_monthly_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_monthly_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_not_authenticated_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_page_response_acquirer_anticipations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_page_response_acquirer_receivables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_page_response_acquirer_sales.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_page_response_category_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_page_response_investment_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_page_response_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_parameter_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_parameter_validation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_customer_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_customers_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_data_participant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_institution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_intent_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_intent_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_intents_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_receipt_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_receipt_person.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_recipient_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_recipient_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_recipients_institution_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_recipients_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_request_callback_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_request_receipt_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_payment_requests_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_percentage_over_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_pix_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_portfolio_yield_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_smart_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_smart_account_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_smart_account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_smart_account_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_smart_accounts_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_status_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_status_detail_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_status_detail_product_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_update_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_update_item_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_update_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_update_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_update_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_webhook_creation_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-06 20:28:58.000000 pluggy_sdk-1.0.0.post8/test/test_webhooks_list200_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:08:38.944934 pluggy_sdk-1.0.0.post9/
+-rw-r--r--   0 runner    (1001) docker     (127)    21246 2024-05-18 01:08:38.944934 pluggy_sdk-1.0.0.post9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20833 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:08:38.892934 pluggy_sdk-1.0.0.post9/pluggy_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:08:38.896934 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22047 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26206 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/acquirer_anticipation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26120 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/acquirer_receivable_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25869 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/acquirer_sale_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22882 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20960 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/bill_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32808 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/bulk_payment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41577 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/category_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41008 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21602 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/identity_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/income_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35989 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/investment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54593 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/items_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/loan_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54784 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/payment_customer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32020 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/payment_intent_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77933 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/payment_recipient_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105085 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/payment_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22320 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/portfolio_yield_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43323 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/smart_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37553 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/transaction_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55525 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api/webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:08:38.920934 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/accounts_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_anticipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_anticipation_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable_data_establishment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable_destination_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable_related_sale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_sale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_sale_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_sale_installment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_sale_installment_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/aggregated_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/aggregated_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/asset_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bank_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bill_finance_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bills_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/boleto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/boleto_payer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/boleto_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bulk_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bulk_payments_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/client_category_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connect_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connect_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_health_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_user_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_boleto_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_bulk_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_client_category_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_item_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_or_update_payment_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_payment_customer_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_pix_qr_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_smart_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/credential_select_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/credit_card_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/credit_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/global_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/i_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/identity_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/income_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/income_reports_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investment_expenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investment_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investment_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investments_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/item_creation_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/item_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/item_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_contracted_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_contracted_finance_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_installment_balloon_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_installment_balloon_payment_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_installments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_interest_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payment_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payment_release_over_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payment_release_over_parcel_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payment_release_over_parcel_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_warranty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loans_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/merchant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/monthly_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/monthly_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/not_authenticated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_acquirer_anticipations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_acquirer_receivables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_acquirer_sales.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_category_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_investment_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/parameter_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/parameter_validation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_customers_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_data_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_institution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_intent_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_intents_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_receipt_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_receipt_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_recipient_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_recipients_institution_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_recipients_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_request_callback_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_request_receipt_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_requests_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/percentage_over_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/pix_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/smart_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/smart_account_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/smart_account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/smart_accounts_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/status_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/status_detail_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/status_detail_product_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_item_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/webhook_creation_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/models/webhooks_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:08:38.944934 pluggy_sdk-1.0.0.post9/pluggy_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21246 2024-05-18 01:08:38.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-18 01:08:38.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:08:38.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-18 01:08:38.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 01:08:38.000000 pluggy_sdk-1.0.0.post9/pluggy_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-18 01:08:28.000000 pluggy_sdk-1.0.0.post9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-18 01:08:38.944934 pluggy_sdk-1.0.0.post9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-18 01:08:35.000000 pluggy_sdk-1.0.0.post9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:08:38.944934 pluggy_sdk-1.0.0.post9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_accounts_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_anticipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_anticipation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_anticipation_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_data_establishment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_destination_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_related_sale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_sale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_sale_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_sale_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_sale_installment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_acquirer_sale_installment_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_aggregated_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_aggregated_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_asset_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_bank_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_bill_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_bill_finance_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_bills_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/test/test_boleto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/test/test_boleto_payer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/test/test_boleto_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_bulk_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_bulk_payment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_bulk_payments_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_category_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_client_category_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_connect_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_connect_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_connector_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_connector_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_connector_health_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_connector_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_connector_user_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-18 01:08:27.000000 pluggy_sdk-1.0.0.post9/test/test_create_boleto_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_bulk_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_client_category_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_item_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_or_update_payment_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_payment_customer_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_pix_qr_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_smart_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_create_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_credential_select_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_credit_card_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_credit_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_global_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_i_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_identity_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_identity_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_income_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_income_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_income_reports_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_investment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_investment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_investment_expenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_investment_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_investment_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_investments_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_item_creation_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_item_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_item_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_contracted_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_contracted_finance_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_installment_balloon_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_installment_balloon_payment_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_installments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_interest_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_payment_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_payment_release_over_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_payment_release_over_parcel_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_payment_release_over_parcel_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loan_warranty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_loans_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_monthly_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_monthly_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_not_authenticated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_page_response_acquirer_anticipations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_page_response_acquirer_receivables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_page_response_acquirer_sales.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_page_response_category_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_page_response_investment_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_page_response_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_parameter_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_parameter_validation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_customer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_customers_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_data_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_institution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_intent_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_intent_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_intents_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_receipt_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_receipt_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_recipient_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_recipient_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_recipients_institution_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_recipients_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_request_callback_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_request_receipt_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_payment_requests_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_percentage_over_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_pix_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_portfolio_yield_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_smart_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_smart_account_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_smart_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_smart_account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_smart_accounts_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_status_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_status_detail_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_status_detail_product_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_transaction_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_update_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_update_item_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_update_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_update_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_update_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_webhook_creation_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-18 01:07:48.000000 pluggy_sdk-1.0.0.post9/test/test_webhooks_list200_response.py
```

### Comparing `pluggy_sdk-1.0.0.post8/PKG-INFO` & `pluggy_sdk-1.0.0.post9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluggy-sdk
-Version: 1.0.0.post8
+Version: 1.0.0.post9
 Summary: Pluggy API
 Home-page: https://github.com/diraol/pluggy-python
 Author: Pluggy
 Author-email: hello@pluggy.ai
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Pluggy API
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 # pluggy-sdk
 Pluggy's main API to review data and execute connectors
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0.post8
+- Package version: 1.0.0.post9
 - Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pluggy.ai](https://pluggy.ai)
 
 ## Requirements.
 
 Python 3.7+
@@ -159,14 +159,15 @@
 *PaymentRecipientApi* | [**payment_recipient_delete**](docs/PaymentRecipientApi.md#payment_recipient_delete) | **DELETE** /payments/recipients/{id} | Delete
 *PaymentRecipientApi* | [**payment_recipient_institutions_retrieve**](docs/PaymentRecipientApi.md#payment_recipient_institutions_retrieve) | **GET** /payments/recipients/institutions/{id} | Retrieve Institution
 *PaymentRecipientApi* | [**payment_recipient_retrieve**](docs/PaymentRecipientApi.md#payment_recipient_retrieve) | **GET** /payments/recipients/{id} | Retrieve
 *PaymentRecipientApi* | [**payment_recipient_update**](docs/PaymentRecipientApi.md#payment_recipient_update) | **PATCH** /payments/recipients/{id} | Update
 *PaymentRecipientApi* | [**payment_recipients_institution_list**](docs/PaymentRecipientApi.md#payment_recipients_institution_list) | **GET** /payments/recipients/institutions | List Institutions
 *PaymentRecipientApi* | [**payment_recipients_list**](docs/PaymentRecipientApi.md#payment_recipients_list) | **GET** /payments/recipients | List
 *PaymentRequestApi* | [**payment_request_create**](docs/PaymentRequestApi.md#payment_request_create) | **POST** /payments/requests | Create
+*PaymentRequestApi* | [**payment_request_create_boleto**](docs/PaymentRequestApi.md#payment_request_create_boleto) | **POST** /payments/requests/boleto | Create boleto payment request
 *PaymentRequestApi* | [**payment_request_create_pix_qr**](docs/PaymentRequestApi.md#payment_request_create_pix_qr) | **POST** /payments/requests/pix-qr | Create PIX QR payment request
 *PaymentRequestApi* | [**payment_request_delete**](docs/PaymentRequestApi.md#payment_request_delete) | **DELETE** /payments/requests/{id} | Delete
 *PaymentRequestApi* | [**payment_request_receipt_create**](docs/PaymentRequestApi.md#payment_request_receipt_create) | **POST** /payments/requests/{id}/receipts | Create
 *PaymentRequestApi* | [**payment_request_receipt_list**](docs/PaymentRequestApi.md#payment_request_receipt_list) | **GET** /payments/requests/{id}/receipts | List
 *PaymentRequestApi* | [**payment_request_receipt_retrieve**](docs/PaymentRequestApi.md#payment_request_receipt_retrieve) | **GET** /payments/requests/{payment-request-id}/receipts/{payment-receipt-id} | Retrieve
 *PaymentRequestApi* | [**payment_request_retrieve**](docs/PaymentRequestApi.md#payment_request_retrieve) | **GET** /payments/requests/{id} | Retrieve
 *PaymentRequestApi* | [**payment_request_update**](docs/PaymentRequestApi.md#payment_request_update) | **PATCH** /payments/requests/{id} | Update
@@ -209,27 +210,31 @@
  - [AssetDistribution](docs/AssetDistribution.md)
  - [AuthRequest](docs/AuthRequest.md)
  - [AuthResponse](docs/AuthResponse.md)
  - [BankData](docs/BankData.md)
  - [Bill](docs/Bill.md)
  - [BillFinanceCharge](docs/BillFinanceCharge.md)
  - [BillsList200Response](docs/BillsList200Response.md)
+ - [Boleto](docs/Boleto.md)
+ - [BoletoPayer](docs/BoletoPayer.md)
+ - [BoletoRecipient](docs/BoletoRecipient.md)
  - [BulkPayment](docs/BulkPayment.md)
  - [BulkPaymentsList200Response](docs/BulkPaymentsList200Response.md)
  - [Category](docs/Category.md)
  - [ClientCategoryRule](docs/ClientCategoryRule.md)
  - [Company](docs/Company.md)
  - [ConnectTokenRequest](docs/ConnectTokenRequest.md)
  - [ConnectTokenResponse](docs/ConnectTokenResponse.md)
  - [Connector](docs/Connector.md)
  - [ConnectorCredential](docs/ConnectorCredential.md)
  - [ConnectorHealth](docs/ConnectorHealth.md)
  - [ConnectorHealthDetails](docs/ConnectorHealthDetails.md)
  - [ConnectorListResponse](docs/ConnectorListResponse.md)
  - [ConnectorUserAction](docs/ConnectorUserAction.md)
+ - [CreateBoletoPaymentRequest](docs/CreateBoletoPaymentRequest.md)
  - [CreateBulkPayment](docs/CreateBulkPayment.md)
  - [CreateClientCategoryRule](docs/CreateClientCategoryRule.md)
  - [CreateItem](docs/CreateItem.md)
  - [CreateItemParameters](docs/CreateItemParameters.md)
  - [CreateOrUpdatePaymentCustomer](docs/CreateOrUpdatePaymentCustomer.md)
  - [CreatePaymentCustomerRequestBody](docs/CreatePaymentCustomerRequestBody.md)
  - [CreatePaymentIntent](docs/CreatePaymentIntent.md)
```

### Comparing `pluggy_sdk-1.0.0.post8/README.md` & `pluggy_sdk-1.0.0.post9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pluggy-sdk
 Pluggy's main API to review data and execute connectors
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0.post8
+- Package version: 1.0.0.post9
 - Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pluggy.ai](https://pluggy.ai)
 
 ## Requirements.
 
 Python 3.7+
@@ -144,14 +144,15 @@
 *PaymentRecipientApi* | [**payment_recipient_delete**](docs/PaymentRecipientApi.md#payment_recipient_delete) | **DELETE** /payments/recipients/{id} | Delete
 *PaymentRecipientApi* | [**payment_recipient_institutions_retrieve**](docs/PaymentRecipientApi.md#payment_recipient_institutions_retrieve) | **GET** /payments/recipients/institutions/{id} | Retrieve Institution
 *PaymentRecipientApi* | [**payment_recipient_retrieve**](docs/PaymentRecipientApi.md#payment_recipient_retrieve) | **GET** /payments/recipients/{id} | Retrieve
 *PaymentRecipientApi* | [**payment_recipient_update**](docs/PaymentRecipientApi.md#payment_recipient_update) | **PATCH** /payments/recipients/{id} | Update
 *PaymentRecipientApi* | [**payment_recipients_institution_list**](docs/PaymentRecipientApi.md#payment_recipients_institution_list) | **GET** /payments/recipients/institutions | List Institutions
 *PaymentRecipientApi* | [**payment_recipients_list**](docs/PaymentRecipientApi.md#payment_recipients_list) | **GET** /payments/recipients | List
 *PaymentRequestApi* | [**payment_request_create**](docs/PaymentRequestApi.md#payment_request_create) | **POST** /payments/requests | Create
+*PaymentRequestApi* | [**payment_request_create_boleto**](docs/PaymentRequestApi.md#payment_request_create_boleto) | **POST** /payments/requests/boleto | Create boleto payment request
 *PaymentRequestApi* | [**payment_request_create_pix_qr**](docs/PaymentRequestApi.md#payment_request_create_pix_qr) | **POST** /payments/requests/pix-qr | Create PIX QR payment request
 *PaymentRequestApi* | [**payment_request_delete**](docs/PaymentRequestApi.md#payment_request_delete) | **DELETE** /payments/requests/{id} | Delete
 *PaymentRequestApi* | [**payment_request_receipt_create**](docs/PaymentRequestApi.md#payment_request_receipt_create) | **POST** /payments/requests/{id}/receipts | Create
 *PaymentRequestApi* | [**payment_request_receipt_list**](docs/PaymentRequestApi.md#payment_request_receipt_list) | **GET** /payments/requests/{id}/receipts | List
 *PaymentRequestApi* | [**payment_request_receipt_retrieve**](docs/PaymentRequestApi.md#payment_request_receipt_retrieve) | **GET** /payments/requests/{payment-request-id}/receipts/{payment-receipt-id} | Retrieve
 *PaymentRequestApi* | [**payment_request_retrieve**](docs/PaymentRequestApi.md#payment_request_retrieve) | **GET** /payments/requests/{id} | Retrieve
 *PaymentRequestApi* | [**payment_request_update**](docs/PaymentRequestApi.md#payment_request_update) | **PATCH** /payments/requests/{id} | Update
@@ -194,27 +195,31 @@
  - [AssetDistribution](docs/AssetDistribution.md)
  - [AuthRequest](docs/AuthRequest.md)
  - [AuthResponse](docs/AuthResponse.md)
  - [BankData](docs/BankData.md)
  - [Bill](docs/Bill.md)
  - [BillFinanceCharge](docs/BillFinanceCharge.md)
  - [BillsList200Response](docs/BillsList200Response.md)
+ - [Boleto](docs/Boleto.md)
+ - [BoletoPayer](docs/BoletoPayer.md)
+ - [BoletoRecipient](docs/BoletoRecipient.md)
  - [BulkPayment](docs/BulkPayment.md)
  - [BulkPaymentsList200Response](docs/BulkPaymentsList200Response.md)
  - [Category](docs/Category.md)
  - [ClientCategoryRule](docs/ClientCategoryRule.md)
  - [Company](docs/Company.md)
  - [ConnectTokenRequest](docs/ConnectTokenRequest.md)
  - [ConnectTokenResponse](docs/ConnectTokenResponse.md)
  - [Connector](docs/Connector.md)
  - [ConnectorCredential](docs/ConnectorCredential.md)
  - [ConnectorHealth](docs/ConnectorHealth.md)
  - [ConnectorHealthDetails](docs/ConnectorHealthDetails.md)
  - [ConnectorListResponse](docs/ConnectorListResponse.md)
  - [ConnectorUserAction](docs/ConnectorUserAction.md)
+ - [CreateBoletoPaymentRequest](docs/CreateBoletoPaymentRequest.md)
  - [CreateBulkPayment](docs/CreateBulkPayment.md)
  - [CreateClientCategoryRule](docs/CreateClientCategoryRule.md)
  - [CreateItem](docs/CreateItem.md)
  - [CreateItemParameters](docs/CreateItemParameters.md)
  - [CreateOrUpdatePaymentCustomer](docs/CreateOrUpdatePaymentCustomer.md)
  - [CreatePaymentCustomerRequestBody](docs/CreatePaymentCustomerRequestBody.md)
  - [CreatePaymentIntent](docs/CreatePaymentIntent.md)
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/__init__.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: hello@pluggy.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.0.post8"
+__version__ = "1.0.0.post9"
 
 # import apis into sdk package
 from pluggy_sdk.api.account_api import AccountApi
 from pluggy_sdk.api.acquirer_anticipation_api import AcquirerAnticipationApi
 from pluggy_sdk.api.acquirer_receivable_api import AcquirerReceivableApi
 from pluggy_sdk.api.acquirer_sale_api import AcquirerSaleApi
 from pluggy_sdk.api.auth_api import AuthApi
@@ -73,27 +73,31 @@
 from pluggy_sdk.models.asset_distribution import AssetDistribution
 from pluggy_sdk.models.auth_request import AuthRequest
 from pluggy_sdk.models.auth_response import AuthResponse
 from pluggy_sdk.models.bank_data import BankData
 from pluggy_sdk.models.bill import Bill
 from pluggy_sdk.models.bill_finance_charge import BillFinanceCharge
 from pluggy_sdk.models.bills_list200_response import BillsList200Response
+from pluggy_sdk.models.boleto import Boleto
+from pluggy_sdk.models.boleto_payer import BoletoPayer
+from pluggy_sdk.models.boleto_recipient import BoletoRecipient
 from pluggy_sdk.models.bulk_payment import BulkPayment
 from pluggy_sdk.models.bulk_payments_list200_response import BulkPaymentsList200Response
 from pluggy_sdk.models.category import Category
 from pluggy_sdk.models.client_category_rule import ClientCategoryRule
 from pluggy_sdk.models.company import Company
 from pluggy_sdk.models.connect_token_request import ConnectTokenRequest
 from pluggy_sdk.models.connect_token_response import ConnectTokenResponse
 from pluggy_sdk.models.connector import Connector
 from pluggy_sdk.models.connector_credential import ConnectorCredential
 from pluggy_sdk.models.connector_health import ConnectorHealth
 from pluggy_sdk.models.connector_health_details import ConnectorHealthDetails
 from pluggy_sdk.models.connector_list_response import ConnectorListResponse
 from pluggy_sdk.models.connector_user_action import ConnectorUserAction
+from pluggy_sdk.models.create_boleto_payment_request import CreateBoletoPaymentRequest
 from pluggy_sdk.models.create_bulk_payment import CreateBulkPayment
 from pluggy_sdk.models.create_client_category_rule import CreateClientCategoryRule
 from pluggy_sdk.models.create_item import CreateItem
 from pluggy_sdk.models.create_item_parameters import CreateItemParameters
 from pluggy_sdk.models.create_or_update_payment_customer import CreateOrUpdatePaymentCustomer
 from pluggy_sdk.models.create_payment_customer_request_body import CreatePaymentCustomerRequestBody
 from pluggy_sdk.models.create_payment_intent import CreatePaymentIntent
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/__init__.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/account_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/account_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/acquirer_anticipation_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/acquirer_anticipation_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/acquirer_receivable_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/acquirer_receivable_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/acquirer_sale_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/acquirer_sale_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/auth_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/bill_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/bill_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/bulk_payment_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/bulk_payment_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/category_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/category_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/connector_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/connector_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/identity_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/identity_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/income_report_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/income_report_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/investment_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/investment_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/items_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/items_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/loan_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/loan_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/payment_customer_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/payment_customer_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/payment_intent_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/payment_intent_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/payment_recipient_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/payment_recipient_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/payment_request_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/payment_request_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr
 from typing_extensions import Annotated
+from pluggy_sdk.models.create_boleto_payment_request import CreateBoletoPaymentRequest
 from pluggy_sdk.models.create_payment_request import CreatePaymentRequest
 from pluggy_sdk.models.create_pix_qr_payment_request import CreatePixQrPaymentRequest
 from pluggy_sdk.models.payment_receipt import PaymentReceipt
 from pluggy_sdk.models.payment_request import PaymentRequest
 from pluggy_sdk.models.payment_request_receipt_list200_response import PaymentRequestReceiptList200Response
 from pluggy_sdk.models.payment_requests_list200_response import PaymentRequestsList200Response
 from pluggy_sdk.models.update_payment_request import UpdatePaymentRequest
@@ -304,14 +305,285 @@
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def payment_request_create_boleto(
+        self,
+        create_boleto_payment_request: CreateBoletoPaymentRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> PaymentRequest:
+        """Create boleto payment request
+
+        Creates the boleto payment request resource
+
+        :param create_boleto_payment_request: (required)
+        :type create_boleto_payment_request: CreateBoletoPaymentRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._payment_request_create_boleto_serialize(
+            create_boleto_payment_request=create_boleto_payment_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PaymentRequest",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def payment_request_create_boleto_with_http_info(
+        self,
+        create_boleto_payment_request: CreateBoletoPaymentRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[PaymentRequest]:
+        """Create boleto payment request
+
+        Creates the boleto payment request resource
+
+        :param create_boleto_payment_request: (required)
+        :type create_boleto_payment_request: CreateBoletoPaymentRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._payment_request_create_boleto_serialize(
+            create_boleto_payment_request=create_boleto_payment_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PaymentRequest",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def payment_request_create_boleto_without_preload_content(
+        self,
+        create_boleto_payment_request: CreateBoletoPaymentRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """Create boleto payment request
+
+        Creates the boleto payment request resource
+
+        :param create_boleto_payment_request: (required)
+        :type create_boleto_payment_request: CreateBoletoPaymentRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._payment_request_create_boleto_serialize(
+            create_boleto_payment_request=create_boleto_payment_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PaymentRequest",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _payment_request_create_boleto_serialize(
+        self,
+        create_boleto_payment_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> RequestSerialized:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, Union[str, bytes]] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if create_boleto_payment_request is not None:
+            _body_params = create_boleto_payment_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'default'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/payments/requests/boleto',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth
         )
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/portfolio_yield_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/portfolio_yield_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/smart_account_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/smart_account_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/transaction_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/transaction_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api/webhook_api.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api/webhook_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api_client.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0.post8/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.0.post9/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/api_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/api_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/configuration.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.0.post8".\
+               "SDK Package Version: 1.0.0.post9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/exceptions.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/__init__.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,27 +35,31 @@
 from pluggy_sdk.models.asset_distribution import AssetDistribution
 from pluggy_sdk.models.auth_request import AuthRequest
 from pluggy_sdk.models.auth_response import AuthResponse
 from pluggy_sdk.models.bank_data import BankData
 from pluggy_sdk.models.bill import Bill
 from pluggy_sdk.models.bill_finance_charge import BillFinanceCharge
 from pluggy_sdk.models.bills_list200_response import BillsList200Response
+from pluggy_sdk.models.boleto import Boleto
+from pluggy_sdk.models.boleto_payer import BoletoPayer
+from pluggy_sdk.models.boleto_recipient import BoletoRecipient
 from pluggy_sdk.models.bulk_payment import BulkPayment
 from pluggy_sdk.models.bulk_payments_list200_response import BulkPaymentsList200Response
 from pluggy_sdk.models.category import Category
 from pluggy_sdk.models.client_category_rule import ClientCategoryRule
 from pluggy_sdk.models.company import Company
 from pluggy_sdk.models.connect_token_request import ConnectTokenRequest
 from pluggy_sdk.models.connect_token_response import ConnectTokenResponse
 from pluggy_sdk.models.connector import Connector
 from pluggy_sdk.models.connector_credential import ConnectorCredential
 from pluggy_sdk.models.connector_health import ConnectorHealth
 from pluggy_sdk.models.connector_health_details import ConnectorHealthDetails
 from pluggy_sdk.models.connector_list_response import ConnectorListResponse
 from pluggy_sdk.models.connector_user_action import ConnectorUserAction
+from pluggy_sdk.models.create_boleto_payment_request import CreateBoletoPaymentRequest
 from pluggy_sdk.models.create_bulk_payment import CreateBulkPayment
 from pluggy_sdk.models.create_client_category_rule import CreateClientCategoryRule
 from pluggy_sdk.models.create_item import CreateItem
 from pluggy_sdk.models.create_item_parameters import CreateItemParameters
 from pluggy_sdk.models.create_or_update_payment_customer import CreateOrUpdatePaymentCustomer
 from pluggy_sdk.models.create_payment_customer_request_body import CreatePaymentCustomerRequestBody
 from pluggy_sdk.models.create_payment_intent import CreatePaymentIntent
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/account.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/accounts_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/accounts_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_anticipation.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_anticipation.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_anticipation_data.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_anticipation_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_data.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable_data.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable_data_establishment.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable_data_establishment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable_destination_account.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable_destination_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_receivable_related_sale.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_receivable_related_sale.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_sale.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_sale.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_sale_data.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_sale_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_sale_installment.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_sale_installment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/acquirer_sale_installment_data.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/acquirer_sale_installment_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/address.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/address.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/aggregated_portfolio.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/aggregated_portfolio.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/aggregated_portfolio_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/aggregated_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/asset_distribution.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/asset_distribution.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/auth_request.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/auth_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/auth_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/auth_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bank_data.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bank_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bill.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bill.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bill_finance_charge.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bill_finance_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bills_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bills_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bulk_payment.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bulk_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/bulk_payments_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/bulk_payments_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/category.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/category.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/client_category_rule.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/client_category_rule.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/company.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/company.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connect_token_request.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connect_token_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connect_token_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connect_token_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_credential.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_credential.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_health.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_health.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_health_details.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_health_details.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_list_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_list_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/connector_user_action.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/connector_user_action.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_bulk_payment.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_bulk_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_client_category_rule.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_client_category_rule.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_item.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_item_parameters.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_item_parameters.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_or_update_payment_customer.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_or_update_payment_customer.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_payment_customer_request_body.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_payment_customer_request_body.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_payment_intent.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_payment_intent.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     """
     Request with information to create a payment intent
     """ # noqa: E501
     payment_request_id: Optional[StrictStr] = Field(default=None, description="Primary identifier of the payment request associated to the payment intent", alias="paymentRequestId")
     bulk_payment_id: Optional[StrictStr] = Field(default=None, description="Primary identifier of the bulk payment associated to the payment intent", alias="bulkPaymentId")
     parameters: Optional[PaymentIntentParameter] = None
     connector_id: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="Primary identifier of the connector associated to the payment intent", alias="connectorId")
-    payment_method: Optional[StrictStr] = Field(default=None, description="Payment method can be PIS (Payment Initiation) or PIX (PIX QR flow), if PIX selected only `bulkPaymentId` is required, if PIS selected only `paymentRequestId` or `bulkPaymentId` are required with `connectorId`, `parameters` and `paymentMethod`", alias="paymentMethod")
+    payment_method: Optional[StrictStr] = Field(default=None, description="Payment method can be PIS (Payment Initiation) or PIX (PIX QR flow), if PIX selected `bulkPaymentId` or a `paymentRequest` with smartAccountId attached will be accepted", alias="paymentMethod")
     __properties: ClassVar[List[str]] = ["paymentRequestId", "bulkPaymentId", "parameters", "connectorId", "paymentMethod"]
 
     @field_validator('payment_method')
     def payment_method_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_payment_recipient.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_payment_request.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_payment_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 
 from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from pluggy_sdk.models.payment_request_callback_urls import PaymentRequestCallbackUrls
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreatePaymentRequest(BaseModel):
+class UpdatePaymentRequest(BaseModel):
     """
-    Request with information to create a payment request
+    Request with information to update a payment request
     """ # noqa: E501
-    amount: Union[StrictFloat, StrictInt] = Field(description="Requested amount")
+    amount: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="Requested amount")
     description: Optional[StrictStr] = Field(default=None, description="Payment description")
     callback_urls: Optional[PaymentRequestCallbackUrls] = Field(default=None, alias="callbackUrls")
     recipient_id: Optional[StrictStr] = Field(default=None, description="Payment receiver identifier", alias="recipientId")
     customer_id: Optional[StrictStr] = Field(default=None, description="Customer identifier associated to the payment", alias="customerId")
     client_payment_id: Optional[StrictStr] = Field(default=None, description="Your payment identifier", alias="clientPaymentId")
     __properties: ClassVar[List[str]] = ["amount", "description", "callbackUrls", "recipientId", "customerId", "clientPaymentId"]
 
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreatePaymentRequest from a JSON string"""
+        """Create an instance of UpdatePaymentRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,15 +78,15 @@
         # override the default output from pydantic by calling `to_dict()` of callback_urls
         if self.callback_urls:
             _dict['callbackUrls'] = self.callback_urls.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreatePaymentRequest from a dict"""
+        """Create an instance of UpdatePaymentRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_pix_qr_payment_request.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_pix_qr_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_smart_account_request.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_smart_account_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/create_webhook.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_webhook.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/credential_select_option.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/credential_select_option.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/credit_card_metadata.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/credit_card_metadata.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/credit_data.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/credit_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/document.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/document.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/email.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/email.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/global_error_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/global_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/i_count_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/i_count_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/identity_relation.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/identity_relation.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/identity_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/identity_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/income_report.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/income_report.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/income_reports_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/income_reports_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investment.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investment_expenses.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investment_expenses.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investment_metadata.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investment_metadata.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investment_transaction.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investment_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/investments_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/investments_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/item.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/item_creation_error_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/item_creation_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/item_error.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/item_error.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/item_options.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/item_options.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_contracted_fee.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_contracted_fee.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_contracted_finance_charge.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_contracted_finance_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_installment_balloon_payment.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_installment_balloon_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_installment_balloon_payment_amount.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_installment_balloon_payment_amount.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_installments.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_installments.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_interest_rate.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_interest_rate.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payment_release.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payment_release.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payment_release_over_parcel.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payment_release_over_parcel.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payment_release_over_parcel_charge.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payment_release_over_parcel_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payment_release_over_parcel_fee.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payment_release_over_parcel_fee.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_payments.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_payments.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loan_warranty.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loan_warranty.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/loans_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/loans_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/merchant.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/merchant.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/monthly_portfolio.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/monthly_portfolio.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/monthly_portfolio_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/monthly_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/not_authenticated_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/not_authenticated_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_acquirer_anticipations.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_acquirer_anticipations.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_acquirer_receivables.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_acquirer_receivables.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_acquirer_sales.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_acquirer_sales.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_category_rules.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_category_rules.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_investment_transactions.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_investment_transactions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/page_response_transactions.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/page_response_transactions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/parameter_validation_error.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/parameter_validation_error.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/parameter_validation_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/parameter_validation_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_customer.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_customer.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_customers_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_customers_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_data.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_data_participant.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_data_participant.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_institution.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_institution.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_intent.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_intent_parameter.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_intent_parameter.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_intents_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_intents_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_receipt.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_receipt.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_receipt_bank_account.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_receipt_bank_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_receipt_person.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_receipt_person.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_recipient.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_recipient_account.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_recipient_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_recipients_institution_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_recipients_institution_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_recipients_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_recipients_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_request.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional, Union
+from pluggy_sdk.models.boleto import Boleto
 from pluggy_sdk.models.payment_request_callback_urls import PaymentRequestCallbackUrls
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PaymentRequest(BaseModel):
     """
     Response with information related to a payment request
@@ -36,15 +37,16 @@
     client_payment_id: Optional[StrictStr] = Field(default=None, description="Client payment identifier", alias="clientPaymentId")
     created_at: datetime = Field(description="Date when the payment request was created", alias="createdAt")
     updated_at: datetime = Field(description="Date when the payment request was updated", alias="updatedAt")
     callback_urls: Optional[PaymentRequestCallbackUrls] = Field(default=None, alias="callbackUrls")
     recipient_id: Optional[StrictStr] = Field(default=None, description="Payment receiver identifier", alias="recipientId")
     payment_url: StrictStr = Field(description="URL to begin the payment intent creation flow for this payment request", alias="paymentUrl")
     pix_qr_code: Optional[StrictStr] = Field(default=None, description="Pix QR code generated by the payment receiver", alias="pixQrCode")
-    __properties: ClassVar[List[str]] = ["id", "amount", "description", "status", "clientPaymentId", "createdAt", "updatedAt", "callbackUrls", "recipientId", "paymentUrl", "pixQrCode"]
+    boleto: Optional[Boleto] = None
+    __properties: ClassVar[List[str]] = ["id", "amount", "description", "status", "clientPaymentId", "createdAt", "updatedAt", "callbackUrls", "recipientId", "paymentUrl", "pixQrCode", "boleto"]
 
     @field_validator('status')
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value not in set(['CREATED', 'IN_PROGRESS', 'COMPLETED', 'ERROR']):
             raise ValueError("must be one of enum values ('CREATED', 'IN_PROGRESS', 'COMPLETED', 'ERROR')")
         return value
@@ -87,14 +89,17 @@
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         # override the default output from pydantic by calling `to_dict()` of callback_urls
         if self.callback_urls:
             _dict['callbackUrls'] = self.callback_urls.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of boleto
+        if self.boleto:
+            _dict['boleto'] = self.boleto.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of PaymentRequest from a dict"""
         if obj is None:
             return None
@@ -109,12 +114,13 @@
             "status": obj.get("status"),
             "clientPaymentId": obj.get("clientPaymentId"),
             "createdAt": obj.get("createdAt"),
             "updatedAt": obj.get("updatedAt"),
             "callbackUrls": PaymentRequestCallbackUrls.from_dict(obj["callbackUrls"]) if obj.get("callbackUrls") is not None else None,
             "recipientId": obj.get("recipientId"),
             "paymentUrl": obj.get("paymentUrl"),
-            "pixQrCode": obj.get("pixQrCode")
+            "pixQrCode": obj.get("pixQrCode"),
+            "boleto": Boleto.from_dict(obj["boleto"]) if obj.get("boleto") is not None else None
         })
         return _obj
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_request_callback_urls.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_request_callback_urls.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_request_receipt_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_request_receipt_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/payment_requests_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/payment_requests_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/percentage_over_index.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/percentage_over_index.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/phone_number.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/phone_number.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/pix_data.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/pix_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/smart_account.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/smart_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/smart_account_address.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/smart_account_address.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/smart_account_balance.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/smart_account_balance.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/smart_accounts_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/smart_accounts_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/status_detail.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/status_detail.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/status_detail_product.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/status_detail_product.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/status_detail_product_warning.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/status_detail_product_warning.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/transaction.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_item.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_item_parameters.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_item_parameters.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_payment_recipient.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_payment_request.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/create_payment_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,25 +20,26 @@
 
 from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from pluggy_sdk.models.payment_request_callback_urls import PaymentRequestCallbackUrls
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UpdatePaymentRequest(BaseModel):
+class CreatePaymentRequest(BaseModel):
     """
-    Request with information to update a payment request
+    Request with information to create a payment request
     """ # noqa: E501
-    amount: Optional[Union[StrictFloat, StrictInt]] = Field(default=None, description="Requested amount")
+    amount: Union[StrictFloat, StrictInt] = Field(description="Requested amount")
     description: Optional[StrictStr] = Field(default=None, description="Payment description")
     callback_urls: Optional[PaymentRequestCallbackUrls] = Field(default=None, alias="callbackUrls")
     recipient_id: Optional[StrictStr] = Field(default=None, description="Payment receiver identifier", alias="recipientId")
     customer_id: Optional[StrictStr] = Field(default=None, description="Customer identifier associated to the payment", alias="customerId")
     client_payment_id: Optional[StrictStr] = Field(default=None, description="Your payment identifier", alias="clientPaymentId")
-    __properties: ClassVar[List[str]] = ["amount", "description", "callbackUrls", "recipientId", "customerId", "clientPaymentId"]
+    smart_account_id: Optional[StrictStr] = Field(default=None, description="Smart account identifier associated to the payment, used to be able to use PIX Qr method", alias="smartAccountId")
+    __properties: ClassVar[List[str]] = ["amount", "description", "callbackUrls", "recipientId", "customerId", "clientPaymentId", "smartAccountId"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -50,15 +51,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UpdatePaymentRequest from a JSON string"""
+        """Create an instance of CreatePaymentRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,25 +79,26 @@
         # override the default output from pydantic by calling `to_dict()` of callback_urls
         if self.callback_urls:
             _dict['callbackUrls'] = self.callback_urls.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UpdatePaymentRequest from a dict"""
+        """Create an instance of CreatePaymentRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "amount": obj.get("amount"),
             "description": obj.get("description"),
             "callbackUrls": PaymentRequestCallbackUrls.from_dict(obj["callbackUrls"]) if obj.get("callbackUrls") is not None else None,
             "recipientId": obj.get("recipientId"),
             "customerId": obj.get("customerId"),
-            "clientPaymentId": obj.get("clientPaymentId")
+            "clientPaymentId": obj.get("clientPaymentId"),
+            "smartAccountId": obj.get("smartAccountId")
         })
         return _obj
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/update_transaction.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/update_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/webhook.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/webhook.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/webhook_creation_error_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/webhook_creation_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/models/webhooks_list200_response.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/models/webhooks_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk/rest.py` & `pluggy_sdk-1.0.0.post9/pluggy_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk.egg-info/PKG-INFO` & `pluggy_sdk-1.0.0.post9/pluggy_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluggy-sdk
-Version: 1.0.0.post8
+Version: 1.0.0.post9
 Summary: Pluggy API
 Home-page: https://github.com/diraol/pluggy-python
 Author: Pluggy
 Author-email: hello@pluggy.ai
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Pluggy API
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 # pluggy-sdk
 Pluggy's main API to review data and execute connectors
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0.post8
+- Package version: 1.0.0.post9
 - Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pluggy.ai](https://pluggy.ai)
 
 ## Requirements.
 
 Python 3.7+
@@ -159,14 +159,15 @@
 *PaymentRecipientApi* | [**payment_recipient_delete**](docs/PaymentRecipientApi.md#payment_recipient_delete) | **DELETE** /payments/recipients/{id} | Delete
 *PaymentRecipientApi* | [**payment_recipient_institutions_retrieve**](docs/PaymentRecipientApi.md#payment_recipient_institutions_retrieve) | **GET** /payments/recipients/institutions/{id} | Retrieve Institution
 *PaymentRecipientApi* | [**payment_recipient_retrieve**](docs/PaymentRecipientApi.md#payment_recipient_retrieve) | **GET** /payments/recipients/{id} | Retrieve
 *PaymentRecipientApi* | [**payment_recipient_update**](docs/PaymentRecipientApi.md#payment_recipient_update) | **PATCH** /payments/recipients/{id} | Update
 *PaymentRecipientApi* | [**payment_recipients_institution_list**](docs/PaymentRecipientApi.md#payment_recipients_institution_list) | **GET** /payments/recipients/institutions | List Institutions
 *PaymentRecipientApi* | [**payment_recipients_list**](docs/PaymentRecipientApi.md#payment_recipients_list) | **GET** /payments/recipients | List
 *PaymentRequestApi* | [**payment_request_create**](docs/PaymentRequestApi.md#payment_request_create) | **POST** /payments/requests | Create
+*PaymentRequestApi* | [**payment_request_create_boleto**](docs/PaymentRequestApi.md#payment_request_create_boleto) | **POST** /payments/requests/boleto | Create boleto payment request
 *PaymentRequestApi* | [**payment_request_create_pix_qr**](docs/PaymentRequestApi.md#payment_request_create_pix_qr) | **POST** /payments/requests/pix-qr | Create PIX QR payment request
 *PaymentRequestApi* | [**payment_request_delete**](docs/PaymentRequestApi.md#payment_request_delete) | **DELETE** /payments/requests/{id} | Delete
 *PaymentRequestApi* | [**payment_request_receipt_create**](docs/PaymentRequestApi.md#payment_request_receipt_create) | **POST** /payments/requests/{id}/receipts | Create
 *PaymentRequestApi* | [**payment_request_receipt_list**](docs/PaymentRequestApi.md#payment_request_receipt_list) | **GET** /payments/requests/{id}/receipts | List
 *PaymentRequestApi* | [**payment_request_receipt_retrieve**](docs/PaymentRequestApi.md#payment_request_receipt_retrieve) | **GET** /payments/requests/{payment-request-id}/receipts/{payment-receipt-id} | Retrieve
 *PaymentRequestApi* | [**payment_request_retrieve**](docs/PaymentRequestApi.md#payment_request_retrieve) | **GET** /payments/requests/{id} | Retrieve
 *PaymentRequestApi* | [**payment_request_update**](docs/PaymentRequestApi.md#payment_request_update) | **PATCH** /payments/requests/{id} | Update
@@ -209,27 +210,31 @@
  - [AssetDistribution](docs/AssetDistribution.md)
  - [AuthRequest](docs/AuthRequest.md)
  - [AuthResponse](docs/AuthResponse.md)
  - [BankData](docs/BankData.md)
  - [Bill](docs/Bill.md)
  - [BillFinanceCharge](docs/BillFinanceCharge.md)
  - [BillsList200Response](docs/BillsList200Response.md)
+ - [Boleto](docs/Boleto.md)
+ - [BoletoPayer](docs/BoletoPayer.md)
+ - [BoletoRecipient](docs/BoletoRecipient.md)
  - [BulkPayment](docs/BulkPayment.md)
  - [BulkPaymentsList200Response](docs/BulkPaymentsList200Response.md)
  - [Category](docs/Category.md)
  - [ClientCategoryRule](docs/ClientCategoryRule.md)
  - [Company](docs/Company.md)
  - [ConnectTokenRequest](docs/ConnectTokenRequest.md)
  - [ConnectTokenResponse](docs/ConnectTokenResponse.md)
  - [Connector](docs/Connector.md)
  - [ConnectorCredential](docs/ConnectorCredential.md)
  - [ConnectorHealth](docs/ConnectorHealth.md)
  - [ConnectorHealthDetails](docs/ConnectorHealthDetails.md)
  - [ConnectorListResponse](docs/ConnectorListResponse.md)
  - [ConnectorUserAction](docs/ConnectorUserAction.md)
+ - [CreateBoletoPaymentRequest](docs/CreateBoletoPaymentRequest.md)
  - [CreateBulkPayment](docs/CreateBulkPayment.md)
  - [CreateClientCategoryRule](docs/CreateClientCategoryRule.md)
  - [CreateItem](docs/CreateItem.md)
  - [CreateItemParameters](docs/CreateItemParameters.md)
  - [CreateOrUpdatePaymentCustomer](docs/CreateOrUpdatePaymentCustomer.md)
  - [CreatePaymentCustomerRequestBody](docs/CreatePaymentCustomerRequestBody.md)
  - [CreatePaymentIntent](docs/CreatePaymentIntent.md)
```

### Comparing `pluggy_sdk-1.0.0.post8/pluggy_sdk.egg-info/SOURCES.txt` & `pluggy_sdk-1.0.0.post9/pluggy_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,27 +58,31 @@
 pluggy_sdk/models/asset_distribution.py
 pluggy_sdk/models/auth_request.py
 pluggy_sdk/models/auth_response.py
 pluggy_sdk/models/bank_data.py
 pluggy_sdk/models/bill.py
 pluggy_sdk/models/bill_finance_charge.py
 pluggy_sdk/models/bills_list200_response.py
+pluggy_sdk/models/boleto.py
+pluggy_sdk/models/boleto_payer.py
+pluggy_sdk/models/boleto_recipient.py
 pluggy_sdk/models/bulk_payment.py
 pluggy_sdk/models/bulk_payments_list200_response.py
 pluggy_sdk/models/category.py
 pluggy_sdk/models/client_category_rule.py
 pluggy_sdk/models/company.py
 pluggy_sdk/models/connect_token_request.py
 pluggy_sdk/models/connect_token_response.py
 pluggy_sdk/models/connector.py
 pluggy_sdk/models/connector_credential.py
 pluggy_sdk/models/connector_health.py
 pluggy_sdk/models/connector_health_details.py
 pluggy_sdk/models/connector_list_response.py
 pluggy_sdk/models/connector_user_action.py
+pluggy_sdk/models/create_boleto_payment_request.py
 pluggy_sdk/models/create_bulk_payment.py
 pluggy_sdk/models/create_client_category_rule.py
 pluggy_sdk/models/create_item.py
 pluggy_sdk/models/create_item_parameters.py
 pluggy_sdk/models/create_or_update_payment_customer.py
 pluggy_sdk/models/create_payment_customer_request_body.py
 pluggy_sdk/models/create_payment_intent.py
@@ -197,14 +201,17 @@
 test/test_auth_request.py
 test/test_auth_response.py
 test/test_bank_data.py
 test/test_bill.py
 test/test_bill_api.py
 test/test_bill_finance_charge.py
 test/test_bills_list200_response.py
+test/test_boleto.py
+test/test_boleto_payer.py
+test/test_boleto_recipient.py
 test/test_bulk_payment.py
 test/test_bulk_payment_api.py
 test/test_bulk_payments_list200_response.py
 test/test_category.py
 test/test_category_api.py
 test/test_client_category_rule.py
 test/test_company.py
@@ -213,14 +220,15 @@
 test/test_connector.py
 test/test_connector_api.py
 test/test_connector_credential.py
 test/test_connector_health.py
 test/test_connector_health_details.py
 test/test_connector_list_response.py
 test/test_connector_user_action.py
+test/test_create_boleto_payment_request.py
 test/test_create_bulk_payment.py
 test/test_create_client_category_rule.py
 test/test_create_item.py
 test/test_create_item_parameters.py
 test/test_create_or_update_payment_customer.py
 test/test_create_payment_customer_request_body.py
 test/test_create_payment_intent.py
```

### Comparing `pluggy_sdk-1.0.0.post8/pyproject.toml` & `pluggy_sdk-1.0.0.post9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pluggy_sdk"
-version = "1.0.0.post8"
+version = "1.0.0.post9"
 description = "Pluggy API"
 authors = ["Pluggy <hello@pluggy.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Pluggy API"]
 include = ["pluggy_sdk/py.typed"]
```

### Comparing `pluggy_sdk-1.0.0.post8/setup.py` & `pluggy_sdk-1.0.0.post9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "pluggy-sdk"
-VERSION = "1.0.0.post8"
+VERSION = "1.0.0.post9"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `pluggy_sdk-1.0.0.post8/test/test_account.py` & `pluggy_sdk-1.0.0.post9/test/test_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_account_api.py` & `pluggy_sdk-1.0.0.post9/test/test_account_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_accounts_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_accounts_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_anticipation.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_anticipation.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_anticipation_api.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_anticipation_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_anticipation_data.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_anticipation_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_data.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_api.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_data.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_data_establishment.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_data_establishment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_destination_account.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_destination_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_receivable_related_sale.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_receivable_related_sale.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_sale.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_sale.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_sale_api.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_sale_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_sale_data.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_sale_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_sale_installment.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_sale_installment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_acquirer_sale_installment_data.py` & `pluggy_sdk-1.0.0.post9/test/test_acquirer_sale_installment_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_address.py` & `pluggy_sdk-1.0.0.post9/test/test_address.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_aggregated_portfolio.py` & `pluggy_sdk-1.0.0.post9/test/test_aggregated_portfolio.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_aggregated_portfolio_response.py` & `pluggy_sdk-1.0.0.post9/test/test_aggregated_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_asset_distribution.py` & `pluggy_sdk-1.0.0.post9/test/test_asset_distribution.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_auth_api.py` & `pluggy_sdk-1.0.0.post9/test/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_auth_request.py` & `pluggy_sdk-1.0.0.post9/test/test_auth_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_auth_response.py` & `pluggy_sdk-1.0.0.post9/test/test_auth_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_bank_data.py` & `pluggy_sdk-1.0.0.post9/test/test_bank_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_bill.py` & `pluggy_sdk-1.0.0.post9/test/test_bill.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_bill_api.py` & `pluggy_sdk-1.0.0.post9/test/test_bill_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_bill_finance_charge.py` & `pluggy_sdk-1.0.0.post9/test/test_bill_finance_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_bills_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_bills_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_bulk_payment.py` & `pluggy_sdk-1.0.0.post9/test/test_bulk_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_bulk_payment_api.py` & `pluggy_sdk-1.0.0.post9/test/test_bulk_payment_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_bulk_payments_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_bulk_payments_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_category.py` & `pluggy_sdk-1.0.0.post9/test/test_category.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_category_api.py` & `pluggy_sdk-1.0.0.post9/test/test_category_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_client_category_rule.py` & `pluggy_sdk-1.0.0.post9/test/test_client_category_rule.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_company.py` & `pluggy_sdk-1.0.0.post9/test/test_company.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_connect_token_request.py` & `pluggy_sdk-1.0.0.post9/test/test_connect_token_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_connect_token_response.py` & `pluggy_sdk-1.0.0.post9/test/test_connect_token_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_connector.py` & `pluggy_sdk-1.0.0.post9/test/test_connector.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_connector_api.py` & `pluggy_sdk-1.0.0.post9/test/test_connector_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_connector_credential.py` & `pluggy_sdk-1.0.0.post9/test/test_connector_credential.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_connector_health.py` & `pluggy_sdk-1.0.0.post9/test/test_connector_health.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_connector_health_details.py` & `pluggy_sdk-1.0.0.post9/test/test_connector_health_details.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_connector_list_response.py` & `pluggy_sdk-1.0.0.post9/test/test_connector_list_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_connector_user_action.py` & `pluggy_sdk-1.0.0.post9/test/test_connector_user_action.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_bulk_payment.py` & `pluggy_sdk-1.0.0.post9/test/test_create_bulk_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_client_category_rule.py` & `pluggy_sdk-1.0.0.post9/test/test_create_client_category_rule.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_item.py` & `pluggy_sdk-1.0.0.post9/test/test_create_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_item_parameters.py` & `pluggy_sdk-1.0.0.post9/test/test_create_item_parameters.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_or_update_payment_customer.py` & `pluggy_sdk-1.0.0.post9/test/test_create_or_update_payment_customer.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_payment_customer_request_body.py` & `pluggy_sdk-1.0.0.post9/test/test_create_payment_customer_request_body.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_payment_intent.py` & `pluggy_sdk-1.0.0.post9/test/test_create_payment_intent.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_payment_recipient.py` & `pluggy_sdk-1.0.0.post9/test/test_create_payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_payment_request.py` & `pluggy_sdk-1.0.0.post9/test/test_create_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_pix_qr_payment_request.py` & `pluggy_sdk-1.0.0.post9/test/test_create_pix_qr_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_smart_account_request.py` & `pluggy_sdk-1.0.0.post9/test/test_create_smart_account_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_create_webhook.py` & `pluggy_sdk-1.0.0.post9/test/test_create_webhook.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_credential_select_option.py` & `pluggy_sdk-1.0.0.post9/test/test_credential_select_option.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_credit_card_metadata.py` & `pluggy_sdk-1.0.0.post9/test/test_credit_card_metadata.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_credit_data.py` & `pluggy_sdk-1.0.0.post9/test/test_credit_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_document.py` & `pluggy_sdk-1.0.0.post9/test/test_document.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_email.py` & `pluggy_sdk-1.0.0.post9/test/test_email.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_global_error_response.py` & `pluggy_sdk-1.0.0.post9/test/test_global_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_i_count_response.py` & `pluggy_sdk-1.0.0.post9/test/test_i_count_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_identity_api.py` & `pluggy_sdk-1.0.0.post9/test/test_identity_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_identity_relation.py` & `pluggy_sdk-1.0.0.post9/test/test_identity_relation.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_identity_response.py` & `pluggy_sdk-1.0.0.post9/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_income_report.py` & `pluggy_sdk-1.0.0.post9/test/test_income_report.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_income_report_api.py` & `pluggy_sdk-1.0.0.post9/test/test_income_report_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_income_reports_response.py` & `pluggy_sdk-1.0.0.post9/test/test_income_reports_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_investment.py` & `pluggy_sdk-1.0.0.post9/test/test_investment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_investment_api.py` & `pluggy_sdk-1.0.0.post9/test/test_investment_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_investment_expenses.py` & `pluggy_sdk-1.0.0.post9/test/test_investment_expenses.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_investment_metadata.py` & `pluggy_sdk-1.0.0.post9/test/test_investment_metadata.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_investment_transaction.py` & `pluggy_sdk-1.0.0.post9/test/test_investment_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_investments_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_investments_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_item.py` & `pluggy_sdk-1.0.0.post9/test/test_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_item_creation_error_response.py` & `pluggy_sdk-1.0.0.post9/test/test_item_creation_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_item_error.py` & `pluggy_sdk-1.0.0.post9/test/test_item_error.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_item_options.py` & `pluggy_sdk-1.0.0.post9/test/test_item_options.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_items_api.py` & `pluggy_sdk-1.0.0.post9/test/test_items_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan.py` & `pluggy_sdk-1.0.0.post9/test/test_loan.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_api.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_contracted_fee.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_contracted_fee.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_contracted_finance_charge.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_contracted_finance_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_installment_balloon_payment.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_installment_balloon_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_installment_balloon_payment_amount.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_installment_balloon_payment_amount.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_installments.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_installments.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_interest_rate.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_interest_rate.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_payment_release.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_payment_release.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_payment_release_over_parcel.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_payment_release_over_parcel.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_payment_release_over_parcel_charge.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_payment_release_over_parcel_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_payment_release_over_parcel_fee.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_payment_release_over_parcel_fee.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_payments.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_payments.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loan_warranty.py` & `pluggy_sdk-1.0.0.post9/test/test_loan_warranty.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_loans_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_loans_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_merchant.py` & `pluggy_sdk-1.0.0.post9/test/test_merchant.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_monthly_portfolio.py` & `pluggy_sdk-1.0.0.post9/test/test_monthly_portfolio.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_monthly_portfolio_response.py` & `pluggy_sdk-1.0.0.post9/test/test_monthly_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_not_authenticated_response.py` & `pluggy_sdk-1.0.0.post9/test/test_not_authenticated_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_page_response_acquirer_anticipations.py` & `pluggy_sdk-1.0.0.post9/test/test_page_response_acquirer_anticipations.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_page_response_acquirer_receivables.py` & `pluggy_sdk-1.0.0.post9/test/test_page_response_acquirer_receivables.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_page_response_acquirer_sales.py` & `pluggy_sdk-1.0.0.post9/test/test_page_response_acquirer_sales.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_page_response_category_rules.py` & `pluggy_sdk-1.0.0.post9/test/test_page_response_category_rules.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_page_response_investment_transactions.py` & `pluggy_sdk-1.0.0.post9/test/test_page_response_investment_transactions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_page_response_transactions.py` & `pluggy_sdk-1.0.0.post9/test/test_page_response_transactions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_parameter_validation_error.py` & `pluggy_sdk-1.0.0.post9/test/test_parameter_validation_error.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_parameter_validation_response.py` & `pluggy_sdk-1.0.0.post9/test/test_parameter_validation_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_customer.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_customer.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_customer_api.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_customer_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_customers_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_customers_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_data.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_data_participant.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_data_participant.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_institution.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_institution.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_intent.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_intent.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_intent_api.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_intent_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_intent_parameter.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_intent_parameter.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_intents_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_intents_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_receipt.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_receipt.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_receipt_bank_account.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_receipt_bank_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_receipt_person.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_receipt_person.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_recipient.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_recipient_account.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_recipient_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_recipient_api.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_recipient_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_recipients_institution_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_recipients_institution_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_recipients_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_recipients_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_request.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_request_api.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_request_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_request_callback_urls.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_request_callback_urls.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_request_receipt_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_request_receipt_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_payment_requests_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_payment_requests_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_percentage_over_index.py` & `pluggy_sdk-1.0.0.post9/test/test_percentage_over_index.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_phone_number.py` & `pluggy_sdk-1.0.0.post9/test/test_phone_number.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_pix_data.py` & `pluggy_sdk-1.0.0.post9/test/test_pix_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_portfolio_yield_api.py` & `pluggy_sdk-1.0.0.post9/test/test_portfolio_yield_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_smart_account.py` & `pluggy_sdk-1.0.0.post9/test/test_smart_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_smart_account_address.py` & `pluggy_sdk-1.0.0.post9/test/test_smart_account_address.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_smart_account_api.py` & `pluggy_sdk-1.0.0.post9/test/test_smart_account_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_smart_account_balance.py` & `pluggy_sdk-1.0.0.post9/test/test_smart_account_balance.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_smart_accounts_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_smart_accounts_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_status_detail.py` & `pluggy_sdk-1.0.0.post9/test/test_status_detail.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_status_detail_product.py` & `pluggy_sdk-1.0.0.post9/test/test_status_detail_product.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_status_detail_product_warning.py` & `pluggy_sdk-1.0.0.post9/test/test_status_detail_product_warning.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_transaction.py` & `pluggy_sdk-1.0.0.post9/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_transaction_api.py` & `pluggy_sdk-1.0.0.post9/test/test_transaction_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_update_item.py` & `pluggy_sdk-1.0.0.post9/test/test_update_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_update_item_parameters.py` & `pluggy_sdk-1.0.0.post9/test/test_update_item_parameters.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_update_payment_recipient.py` & `pluggy_sdk-1.0.0.post9/test/test_update_payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_update_payment_request.py` & `pluggy_sdk-1.0.0.post9/test/test_update_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_update_transaction.py` & `pluggy_sdk-1.0.0.post9/test/test_update_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_webhook.py` & `pluggy_sdk-1.0.0.post9/test/test_webhook.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_webhook_api.py` & `pluggy_sdk-1.0.0.post9/test/test_webhook_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_webhook_creation_error_response.py` & `pluggy_sdk-1.0.0.post9/test/test_webhook_creation_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post8/test/test_webhooks_list200_response.py` & `pluggy_sdk-1.0.0.post9/test/test_webhooks_list200_response.py`

 * *Files identical despite different names*

