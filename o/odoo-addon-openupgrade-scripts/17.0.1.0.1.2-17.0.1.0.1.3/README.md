# Comparing `tmp/odoo_addon_openupgrade_scripts-17.0.1.0.1.2-py3-none-any.whl.zip` & `tmp/odoo_addon_openupgrade_scripts-17.0.1.0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,444 +1,482 @@
-Zip file size: 471946 bytes, number of entries: 442
--rw-r--r--  2.0 unx     3182 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/README.rst
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/__init__.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/__manifest__.py
--rw-r--r--  2.0 unx     1591 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/apriori.py
--rw-r--r--  2.0 unx      238 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/readme/CONFIGURE.md
--rw-r--r--  2.0 unx       86 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/readme/DESCRIPTION.md
--rw-r--r--  2.0 unx      113 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/readme/INSTALL.md
--rw-r--r--  2.0 unx     8333 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/noupdate_changes.xml
--rw-r--r--  2.0 unx    37610 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      601 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_audit_trail/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      189 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_check_printing/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      202 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_debit_note/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      186 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_edi/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      429 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_edi/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      785 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_edi_proxy_client/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     3209 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_edi_ubl_cii/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      162 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_fleet/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_payment/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      532 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_payment_term/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2637 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_peppol/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      516 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_qr_code_emv/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      469 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/account_tax_python/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1252 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/analytic/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      150 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/auth_ldap/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      206 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/auth_oauth/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    12678 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/auth_signup/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/auth_signup/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      150 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/auth_totp/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      188 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/auth_totp_mail/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      189 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/auth_totp_mail_enforce/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      147 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/barcodes/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      198 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/barcodes_gs1_nomenclature/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1097 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/noupdate_changes.xml
--rw-r--r--  2.0 unx    13341 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_analysis.txt
--rw-r--r--  2.0 unx    47834 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_general_log.txt
--rw-r--r--  2.0 unx      198 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base_address_extended/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      200 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base_automation/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     2474 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base_automation/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      187 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base_geolocalize/17.0.2.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     4560 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base_import/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      539 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base_import_module/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      183 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base_install_request/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      174 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base_sparse_field/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      283 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/base_vat/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      198 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/board/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      138 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/board/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      132 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/bus/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    23184 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/calendar/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx     1633 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/calendar/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      199 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/calendar_sms/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1632 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/crm/17.0.1.8/upgrade_analysis.txt
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/crm_iap_enrich/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx      165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/crm_iap_enrich/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      465 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/crm_iap_mine/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      159 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/crm_livechat/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      169 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/crm_sms/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      204 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/data_recycle/17.0.1.3/upgrade_analysis.txt
--rw-r--r--  2.0 unx      540 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     6693 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      186 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/delivery_mondialrelay/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      207 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/delivery_stock_picking_batch/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    19989 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/digest/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx      396 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/digest/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    51945 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/event/17.0.1.8/noupdate_changes.xml
--rw-r--r--  2.0 unx     4074 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/event/17.0.1.8/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2381 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/event_booth/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx      588 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/event_booth/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      650 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/event_booth_sale/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      150 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/event_crm/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1134 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/event_sale/17.0.1.3/upgrade_analysis.txt
--rw-r--r--  2.0 unx      690 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/event_sms/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      150 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/event_sms/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2889 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/fleet/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     8753 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     1843 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/google_account/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      457 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/google_calendar/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      296 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/google_gmail/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1783 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx     8407 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5377 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_attendance/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      518 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_contract/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     1400 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_contract/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2462 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_expense/17.0.2.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     4765 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_expense/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      361 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_fleet/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      168 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_gamification/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1399 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_holidays/17.0.1.6/noupdate_changes.xml
--rw-r--r--  2.0 unx     9856 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_holidays/17.0.1.6/upgrade_analysis.txt
--rw-r--r--  2.0 unx      439 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_holidays_attendance/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2519 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_homeworking/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_hourly_cost/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      172 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_livechat/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_maintenance/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      421 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_org_chart/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      156 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_presence/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1438 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx     2913 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_recruitment_skills/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      581 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_recruitment_survey/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      681 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_recruitment_survey/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1217 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_skills/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_skills_slides/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      715 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_skills_survey/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1862 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_timesheet/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      222 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_timesheet_attendance/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx      233 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_timesheet_attendance/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      738 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_work_entry/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      189 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_work_entry_contract/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      220 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/hr_work_entry_holidays/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      485 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/iap/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      144 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/iap_crm/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     6236 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/im_livechat/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     5508 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/im_livechat/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      183 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/im_livechat_mail_bot/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    12145 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ae/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    34529 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ar/17.0.3.5/upgrade_analysis.txt
--rw-r--r--  2.0 unx      169 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ar_pos/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      979 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ar_withholding/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    79751 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_at/17.0.3.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     9905 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_au/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    45436 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_be/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    23622 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_bg/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    11394 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_bo/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    79062 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_br/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      361 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_br_sales/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      250 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_br_website_sale/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    30677 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ca/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    14425 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ch/17.0.11.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      887 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/noupdate_changes.xml
--rw-r--r--  2.0 unx    14277 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     4790 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_cn/17.0.1.8/upgrade_analysis.txt
--rw-r--r--  2.0 unx    24365 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_co/17.0.0.8/upgrade_analysis.txt
--rw-r--r--  2.0 unx     7396 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_cr/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    31915 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_cz/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx   165698 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_de/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      159 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_din5008/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      186 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_purchase/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      180 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_repair/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      174 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_sale/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      177 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_stock/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     4165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_dk/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx    27657 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_dk/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      391 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_dk_bookkeeping/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      432 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_dk_oioubl/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    36437 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_do/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    54666 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_dz/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    37793 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ec/17.0.3.5/upgrade_analysis.txt
--rw-r--r--  2.0 unx    22251 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ee/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    13603 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_eg/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      220 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_eg_edi_eta/17.0.0.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx   210204 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_es/17.0.5.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx     3975 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_facturae/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2620 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_facturae_adm_centers/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      479 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_facturae_invoice_period/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1541 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_sii/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_tbai/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      625 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_es_pos/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5955 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_et/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    22062 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_fi/17.0.13.0.1/noupdate_changes.xml
--rw-r--r--  2.0 unx    17560 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_fi/17.0.13.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    56284 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_fr/17.0.2.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      201 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_fr_facturx_chorus_pro/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      156 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_fr_fec/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      479 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_fr_hr_holidays/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_fr_pos_cert/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      193 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_gcc_invoice/17.0.1.0.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    71841 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_gr/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1890 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_gt/17.0.3.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     4020 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_hk/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1986 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_hn/17.0.0.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx   169033 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_hr/17.0.13.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    27037 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_hu/17.0.3.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     6289 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_id/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      168 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_id_efaktur/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     7279 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ie/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     7752 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_il/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    38104 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_in/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      156 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_in_edi/17.0.1.03.00/upgrade_analysis.txt
--rw-r--r--  2.0 unx      183 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_in_edi_ewaybill/17.0.1.03.00/upgrade_analysis.txt
--rw-r--r--  2.0 unx      239 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_in_purchase/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      353 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_in_purchase_stock/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      323 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_in_sale/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      329 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_in_sale_stock/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    12277 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_it/17.0.0.5/upgrade_analysis.txt
--rw-r--r--  2.0 unx     4193 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_it_edi/17.0.0.3/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1913 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_it_edi_withholding/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      174 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_it_stock_ddt/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    10154 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_jp/17.0.2.3/upgrade_analysis.txt
--rw-r--r--  2.0 unx      368 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_jp_ubl_pint/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    23082 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ke/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      460 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ke_edi_tremol/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     8080 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_kz/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      282 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_latam_base/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_latam_check/17.0.1.0.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      818 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_latam_invoice_document/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    15271 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_lt/17.0.1.0.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx   122361 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_lu/17.0.2.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx    18165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_lv/17.0.1.0.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    55975 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ma/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    39171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_mn/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx   105353 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_mx/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      153 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_mx_hr/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5852 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_my/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    26131 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_mz/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    23323 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_nl/17.0.3.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx    24279 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_no/17.0.2.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5850 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_nz/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5072 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_pa/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    66374 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_pe/17.0.3.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      223 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_pe_pos/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      418 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_pe_website_sale/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    14223 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ph/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     9396 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_pk/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    50948 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_pl/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    32597 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_pt/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    43740 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ro/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      372 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ro_edi/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    24804 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_rs/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    11074 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_sa/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      754 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_sa_edi/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    59152 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_se/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    11360 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_sg/17.0.2.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx    31221 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_si/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    29204 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_sk/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    61515 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_syscohada/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2918 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_th/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5715 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_tn/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    15173 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_tr/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     6370 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_tw/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    24232 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ua/17.0.1.4/upgrade_analysis.txt
--rw-r--r--  2.0 unx     4525 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ug/17.0.1.0.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5043 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_uk/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      144 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_us/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    12484 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_uy/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    19110 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_ve/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    10061 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_vn/17.0.2.0.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5865 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/l10n_za/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      191 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/link_tracker/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1166 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/loyalty/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      645 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/lunch/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      295 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/noupdate_changes.xml
--rw-r--r--  2.0 unx    29124 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/upgrade_analysis.txt
--rw-r--r--  2.0 unx      147 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mail_bot/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      660 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mail_group/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      236 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mail_plugin/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      324 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/maintenance/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     2646 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/maintenance/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1285 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mass_mailing/17.0.2.7/noupdate_changes.xml
--rw-r--r--  2.0 unx     7962 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mass_mailing/17.0.2.7/upgrade_analysis.txt
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mass_mailing_crm/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      183 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mass_mailing_crm_sms/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      174 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mass_mailing_sale/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      186 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mass_mailing_sale_sms/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1452 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mass_mailing_sms/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1032 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mass_mailing_themes/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      388 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/membership/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      174 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/microsoft_account/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1511 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/microsoft_calendar/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      338 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/microsoft_outlook/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5891 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mrp/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     3346 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mrp_account/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mrp_landed_costs/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      228 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      216 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting_dropshipping/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      204 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting_purchase/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      334 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting_repair/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2393 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/onboarding/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      226 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/partner_autocomplete/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    17137 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/noupdate_changes.xml
--rw-r--r--  2.0 unx    19599 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      616 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_adyen/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      156 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_aps/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      397 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_asiapay/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      526 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_authorize/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_buckaroo/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      304 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_custom/17.0.2.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      384 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_custom/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      502 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_demo/17.0.2.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      471 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_demo/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      180 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_flutterwave/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      183 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_mercado_pago/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_mollie/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      362 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_paypal/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_razorpay/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      159 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_sips/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      197 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_stripe/17.0.2.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      450 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_stripe/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      670 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/payment_xendit/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      327 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/phone_validation/17.0.2.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1703 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/point_of_sale/17.0.1.0.1/noupdate_changes.xml
--rw-r--r--  2.0 unx     8810 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/point_of_sale/17.0.1.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     6652 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/portal/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      976 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/portal/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      162 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/portal_rating/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      150 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_adyen/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      159 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_discount/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      428 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_epson_printer/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      404 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_hr/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      161 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_loyalty/17.0.2.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      269 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_mercury/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1452 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_online_payment/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      524 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_online_payment_self_order/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1403 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_paytm/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2288 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_restaurant/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      183 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_restaurant_adyen/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      147 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_sale/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     4099 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_self_order/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      271 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_self_order_sale/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      191 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_self_order_stripe/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      144 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_six/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      153 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_stripe/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      983 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/pos_viva_wallet/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/privacy_lookup/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      990 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/product/17.0.1.2/noupdate_changes.xml
--rw-r--r--  2.0 unx     4946 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/product/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      189 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/product_email_template/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      611 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/product_expiry/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/product_images/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/product_margin/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     6545 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/noupdate_changes.xml
--rw-r--r--  2.0 unx    14255 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/upgrade_analysis.txt
--rw-r--r--  2.0 unx      651 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/project_account/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      177 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/project_hr_expense/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      156 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/project_mrp/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      171 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/project_purchase/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      156 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/project_sms/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      225 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/project_timesheet_holidays/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5194 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/project_todo/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     3109 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/purchase/17.0.1.2/noupdate_changes.xml
--rw-r--r--  2.0 unx     1174 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/purchase/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      188 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/purchase_mrp/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      192 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/purchase_product_matrix/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      642 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/purchase_requisition/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      201 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/purchase_requisition_stock/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1159 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/purchase_stock/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx     2029 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/rating/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      202 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/repair/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     9355 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/repair/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      939 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/resource/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx    13187 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/noupdate_changes.xml
--rw-r--r--  2.0 unx     5986 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      147 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_crm/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      159 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_expense/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      180 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_expense_margin/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      259 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_loyalty/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      492 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_loyalty_delivery/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      998 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_management/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      156 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_margin/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      147 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_mrp/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1366 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_pdf_quote_builder/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      477 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_product_configurator/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      180 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_product_matrix/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      284 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_project/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     1191 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_project/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      162 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_purchase/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      227 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_service/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      454 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_stock/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      172 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_timesheet/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx     1361 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sale_timesheet/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      644 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sales_team/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     3165 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/sms/17.0.3.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1610 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/snailmail/17.0.0.4/upgrade_analysis.txt
--rw-r--r--  2.0 unx      412 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/snailmail_account/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      197 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/social_media/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      209 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/spreadsheet/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1397 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/spreadsheet_dashboard/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/spreadsheet_dashboard_website_sale/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      358 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/stock/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx     9797 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/stock/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      965 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/stock_account/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     6177 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/stock_delivery/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      555 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/stock_dropshipping/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      677 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/stock_landed_costs/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      297 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/stock_landed_costs_company/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      696 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/stock_picking_batch/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      150 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/stock_sms/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     3699 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/survey/17.0.3.6/upgrade_analysis.txt
--rw-r--r--  2.0 unx      150 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/transifex/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      292 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/uom/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      479 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/utm/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      628 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/web/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      265 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/web_editor/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      430 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/web_hierarchy/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      147 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/web_tour/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx     4998 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx    15644 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1522 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_blog/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      210 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_cf_turnstile/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      156 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_crm/17.0.2.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      245 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_crm_iap_reveal/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      183 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_crm_livechat/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      300 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_crm_partner_assign/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      617 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_customer/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     8026 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event/17.0.1.4/upgrade_analysis.txt
--rw-r--r--  2.0 unx      615 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_booth/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      210 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_booth_exhibitor/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      297 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_booth_sale/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      225 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_booth_sale_exhibitor/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1080 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_exhibitor/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      424 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_meet/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      443 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_sale/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1615 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_track/17.0.1.3/upgrade_analysis.txt
--rw-r--r--  2.0 unx      195 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_track_live/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      195 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_event_track_quiz/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      266 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_form_project/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      203 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_forum/17.0.1.2/noupdate_changes.xml
--rw-r--r--  2.0 unx     4871 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_forum/17.0.1.2/upgrade_analysis.txt
--rw-r--r--  2.0 unx      799 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_hr_recruitment/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      162 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_jitsi/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      871 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_livechat/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      203 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_mass_mailing/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      299 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_membership/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      168 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_partner/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      406 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_payment/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5763 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_profile/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      334 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_profile/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      183 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale/17.0.1.1/noupdate_changes.xml
--rw-r--r--  2.0 unx    10047 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale/17.0.1.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      198 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_autocomplete/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      519 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_comparison/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      183 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_loyalty/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_mondialrelay/17.0.0.1/upgrade_analysis.txt
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_picking/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      811 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_product_configurator/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      462 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_slides/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      177 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_stock/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      204 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_stock_wishlist/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1073 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_sale_wishlist/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx     5201 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_slides/17.0.2.7/noupdate_changes.xml
--rw-r--r--  2.0 unx     5765 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_slides/17.0.2.7/upgrade_analysis.txt
--rw-r--r--  2.0 unx     1172 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_slides_forum/17.0.1.0/noupdate_changes.xml
--rw-r--r--  2.0 unx      790 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_slides_forum/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      394 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_slides_survey/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx      443 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/scripts/website_twitter/17.0.1.0/upgrade_analysis.txt
--rw-r--r--  2.0 unx    26859 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/static/description/banner.png
--rw-r--r--  2.0 unx     9455 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/static/description/icon.png
--rw-r--r--  2.0 unx    12639 b- defN 24-Apr-15 04:58 odoo/addons/openupgrade_scripts/static/description/index.html
--rw-r--r--  2.0 unx     3784 b- defN 24-Apr-15 04:58 odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       83 b- defN 24-Apr-15 04:58 odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-15 04:58 odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    61261 b- defN 24-Apr-15 04:58 odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/RECORD
-442 files, 3313358 bytes uncompressed, 365714 bytes compressed:  89.0%
+Zip file size: 513141 bytes, number of entries: 480
+-rw-r--r--  2.0 unx     3182 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/README.rst
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/__init__.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/__manifest__.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/apriori.py
+-rw-r--r--  2.0 unx      238 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/readme/CONFIGURE.md
+-rw-r--r--  2.0 unx       86 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/readme/DESCRIPTION.md
+-rw-r--r--  2.0 unx      113 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/readme/INSTALL.md
+-rw-r--r--  2.0 unx     8378 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/noupdate_changes.xml
+-rw-r--r--  2.0 unx    36863 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      601 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_audit_trail/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      189 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_check_printing/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      202 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_debit_note/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      186 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_edi/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      429 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_edi/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      920 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_edi_proxy_client/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3209 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_edi_ubl_cii/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      162 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_fleet/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      908 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_payment/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      532 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_payment_term/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2666 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_peppol/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      516 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_qr_code_emv/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      469 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/account_tax_python/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1252 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/analytic/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      150 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/auth_ldap/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      153 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/auth_oauth/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    12678 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/auth_signup/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      279 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/auth_signup/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      150 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/auth_totp/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      188 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/auth_totp_mail/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      189 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/auth_totp_mail_enforce/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      147 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/barcodes/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      198 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/barcodes_gs1_nomenclature/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1372 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/noupdate_changes.xml
+-rw-r--r--  2.0 unx    13821 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_analysis.txt
+-rw-r--r--  2.0 unx   293354 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_general_log.txt
+-rw-r--r--  2.0 unx      198 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base_address_extended/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      200 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base_automation/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     2474 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base_automation/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      187 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base_geolocalize/17.0.2.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4560 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base_import/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      539 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base_import_module/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      183 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base_install_request/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      174 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base_sparse_field/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      283 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/base_vat/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      198 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/board/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      138 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/board/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      132 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/bus/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    16199 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/calendar/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx     1633 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/calendar/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      199 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/calendar_sms/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1483 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/crm/17.0.1.8/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      645 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/crm_iap_enrich/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx      165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/crm_iap_enrich/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      225 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/crm_iap_mine/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      159 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/crm_livechat/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      169 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/crm_sms/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      159 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/data_recycle/17.0.1.3/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      517 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     6596 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      186 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/delivery_mondialrelay/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      207 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/delivery_stock_picking_batch/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    19965 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/digest/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx      396 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/digest/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    51945 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/event/17.0.1.8/noupdate_changes.xml
+-rw-r--r--  2.0 unx     4154 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/event/17.0.1.8/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2381 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/event_booth/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx      588 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/event_booth/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      552 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/event_booth_sale/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      150 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/event_crm/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1134 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/event_sale/17.0.1.3/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      690 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/event_sms/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      150 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/event_sms/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2652 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/fleet/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    10428 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     1754 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/google_account/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      377 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/google_calendar/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      296 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/google_gmail/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1783 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5377 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_attendance/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      518 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_contract/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_contract/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2462 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_expense/17.0.2.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     4674 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_expense/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      361 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_fleet/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      168 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_gamification/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1399 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_holidays/17.0.1.6/noupdate_changes.xml
+-rw-r--r--  2.0 unx    10388 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_holidays/17.0.1.6/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      439 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_holidays_attendance/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2616 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_homeworking/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_hourly_cost/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      172 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_livechat/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_maintenance/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      421 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_org_chart/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      156 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_presence/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1399 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx     2549 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      362 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_recruitment_skills/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      581 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_recruitment_survey/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      681 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_recruitment_survey/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      899 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_skills/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_skills_slides/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      715 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_skills_survey/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_timesheet/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      222 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_timesheet_attendance/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx      233 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_timesheet_attendance/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      264 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_work_entry/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      189 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_work_entry_contract/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      220 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/hr_work_entry_holidays/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      485 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/iap/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      144 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/iap_crm/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     6236 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/im_livechat/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     5505 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/im_livechat/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      183 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/im_livechat_mail_bot/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    12145 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ae/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    34365 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ar/17.0.3.5/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      169 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ar_pos/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1000 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ar_withholding/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    79751 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_at/17.0.3.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     9905 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_au/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3156 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_bd/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    45436 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_be/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     6101 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_bf/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    23622 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_bg/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3115 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_bj/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    11394 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_bo/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    79062 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_br/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      451 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_br_pix/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      361 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_br_sales/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      250 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_br_website_sale/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    30677 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ca/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     8459 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_cd/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2917 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_cf/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2587 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_cg/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    14425 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ch/17.0.11.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    14425 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ch/17.0.11.3/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4822 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ci/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      887 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx    14330 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4948 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_cm/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4790 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_cn/17.0.1.8/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    24365 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_co/17.0.0.8/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    24365 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_co/17.0.0.9/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     7396 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_cr/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    31915 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_cz/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      182 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_de/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      159 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_din5008/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      186 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_purchase/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      180 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_repair/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      174 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_sale/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      177 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_stock/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_dk/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx    27657 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_dk/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      391 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_dk_bookkeeping/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      443 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_dk_oioubl/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    36437 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_do/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    54636 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_dz/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    37793 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ec/17.0.3.5/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    42096 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ec/17.0.3.8/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      476 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ec_website_sale/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    22251 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ee/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    13603 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_eg/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      168 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_eg_edi_eta/17.0.0.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx   210204 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_es/17.0.5.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3975 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_facturae/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2620 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_facturae_adm_centers/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      479 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_facturae_invoice_period/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1541 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_sii/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_tbai/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      625 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_es_pos/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5955 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_et/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    22062 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_fi/17.0.13.0.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx    17560 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_fi/17.0.13.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    56284 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_fr/17.0.2.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      201 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_fr_facturx_chorus_pro/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      156 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_fr_fec/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      479 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_fr_hr_holidays/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_fr_pos_cert/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    13592 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ga/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      193 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_gcc_invoice/17.0.1.0.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2994 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_gn/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2822 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_gq/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    71841 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_gr/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1890 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_gt/17.0.3.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2991 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_gw/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4020 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_hk/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1986 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_hn/17.0.0.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx   117045 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_hr/17.0.13.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    27037 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_hu/17.0.3.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4915 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_hu_edi/17.0.1.0.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     6289 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_id/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      168 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_id_efaktur/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     7279 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ie/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     7752 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_il/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    23012 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_in/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      156 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_in_edi/17.0.1.03.00/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      183 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_in_edi_ewaybill/17.0.1.03.00/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5323 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_in_ewaybill_stock/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      239 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_in_purchase/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      353 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_in_purchase_stock/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      323 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_in_sale/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      329 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_in_sale_stock/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    12277 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_it/17.0.0.5/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    12277 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_it/17.0.0.6/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4193 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_it_edi/17.0.0.3/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4086 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_it_edi/17.0.0.4/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1913 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_it_edi_withholding/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      174 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_it_stock_ddt/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    10154 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_jp/17.0.2.3/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      368 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_jp_ubl_pint/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    23082 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ke/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      545 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ke_edi_tremol/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2666 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_km/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     8080 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_kz/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      282 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_latam_base/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_latam_check/17.0.1.0.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      918 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_latam_invoice_document/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    15271 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_lt/17.0.1.0.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx   124845 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_lu/17.0.2.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    18165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_lv/17.0.1.0.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    55975 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ma/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4112 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ml/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    39171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_mn/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5919 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_mt/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5012 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_mu_account/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx   105353 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_mx/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx   105353 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_mx/17.0.2.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      153 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_mx_hr/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5905 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_my/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1052 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_my_ubl_pint/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    26131 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_mz/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3978 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ne/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3079 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ng/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    23323 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_nl/17.0.3.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    24279 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_no/17.0.2.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5850 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_nz/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5072 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_pa/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    66374 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_pe/17.0.3.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      223 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_pe_pos/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      418 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_pe_website_sale/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    14223 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ph/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     9396 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_pk/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    51037 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_pl/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    32597 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_pt/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    43740 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ro/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      383 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ro_edi/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    24804 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_rs/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3031 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_rw/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    11074 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_sa/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      754 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_sa_edi/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    59152 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_se/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    11360 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_sg/17.0.2.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    31221 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_si/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    29204 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_sk/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4108 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_sn/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    61515 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_syscohada/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2624 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_td/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4249 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_tg/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2918 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_th/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5710 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_tn/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    15173 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_tr/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     6370 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_tw/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    24232 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ua/17.0.1.4/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4525 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ug/17.0.1.0.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5043 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_uk/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      144 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_us/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    12484 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_uy/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    19110 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_ve/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    10061 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_vn/17.0.2.0.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    10357 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_vn/17.0.2.0.3/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5865 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_za/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     6759 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/l10n_zm_account/17.0.1.0.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      159 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/link_tracker/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      689 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/loyalty/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      483 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/lunch/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      571 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/noupdate_changes.xml
+-rw-r--r--  2.0 unx    29205 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      147 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mail_bot/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      489 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mail_group/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      154 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mail_plugin/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      324 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/maintenance/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     2566 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/maintenance/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1285 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mass_mailing/17.0.2.7/noupdate_changes.xml
+-rw-r--r--  2.0 unx     7887 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mass_mailing/17.0.2.7/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mass_mailing_crm/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      183 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mass_mailing_crm_sms/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      174 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mass_mailing_sale/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      186 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mass_mailing_sale_sms/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1452 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mass_mailing_sms/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mass_mailing_themes/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      254 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/membership/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      174 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/microsoft_account/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1597 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/microsoft_calendar/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      338 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/microsoft_outlook/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5460 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mrp/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3346 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mrp_account/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mrp_landed_costs/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      228 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      216 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting_dropshipping/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      204 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting_purchase/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      334 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting_repair/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2308 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/onboarding/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      226 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/partner_autocomplete/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    17009 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx    19520 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      616 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_adyen/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      156 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_aps/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      397 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_asiapay/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      526 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_authorize/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_buckaroo/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      304 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_custom/17.0.2.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      384 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_custom/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      502 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_demo/17.0.2.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      471 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_demo/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      180 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_flutterwave/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      183 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_mercado_pago/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_mollie/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      362 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_paypal/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_razorpay/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      159 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_sips/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      197 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_stripe/17.0.2.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      450 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_stripe/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      670 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/payment_xendit/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      244 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/phone_validation/17.0.2.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1703 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/point_of_sale/17.0.1.0.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx     7525 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/point_of_sale/17.0.1.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     6652 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/portal/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      976 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/portal/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      162 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/portal_rating/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      150 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_adyen/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      159 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_discount/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      428 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_epson_printer/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      404 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_hr/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      161 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_loyalty/17.0.2.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      548 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_mercado_pago/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      269 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_mercury/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1452 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_online_payment/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      524 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_online_payment_self_order/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1403 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_paytm/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1368 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_razorpay/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2288 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_restaurant/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      183 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_restaurant_adyen/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      147 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_sale/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     4099 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_self_order/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      271 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_self_order_sale/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      191 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_self_order_stripe/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      144 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_six/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      153 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_stripe/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      983 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/pos_viva_wallet/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/privacy_lookup/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      990 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/product/17.0.1.2/noupdate_changes.xml
+-rw-r--r--  2.0 unx     4637 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/product/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      189 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/product_email_template/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      611 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/product_expiry/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/product_images/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/product_margin/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     6665 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/noupdate_changes.xml
+-rw-r--r--  2.0 unx    14096 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      651 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/project_account/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      177 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/project_hr_expense/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      156 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/project_mrp/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      171 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/project_purchase/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      156 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/project_sms/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      225 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/project_timesheet_holidays/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2038 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/project_todo/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3109 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/purchase/17.0.1.2/noupdate_changes.xml
+-rw-r--r--  2.0 unx      988 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/purchase/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      188 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/purchase_mrp/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      192 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/purchase_product_matrix/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      642 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/purchase_requisition/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      201 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/purchase_requisition_stock/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1458 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/purchase_stock/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1959 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/rating/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      202 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/repair/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     9290 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/repair/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      939 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/resource/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    13187 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/noupdate_changes.xml
+-rw-r--r--  2.0 unx     6014 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      361 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_async_emails/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      147 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_crm/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      159 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_expense/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      180 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_expense_margin/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      165 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_loyalty/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      445 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_loyalty_delivery/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      784 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_management/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      156 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_margin/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      147 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_mrp/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_pdf_quote_builder/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      477 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_product_configurator/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      180 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_product_matrix/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      284 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_project/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     1191 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_project/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      162 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_purchase/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      227 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_service/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      454 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_stock/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      172 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_timesheet/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx     1150 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sale_timesheet/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      579 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sales_team/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     3309 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/sms/17.0.3.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1626 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/snailmail/17.0.0.4/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      412 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/snailmail_account/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      197 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/social_media/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      209 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/spreadsheet/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1397 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/spreadsheet_dashboard/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      279 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/spreadsheet_dashboard_website_sale/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      358 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/stock/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx     9017 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/stock/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1191 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/stock_account/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     6177 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/stock_delivery/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      555 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/stock_dropshipping/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      677 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/stock_landed_costs/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      297 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/stock_landed_costs_company/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      696 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/stock_picking_batch/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      150 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/stock_sms/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     2379 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/survey/17.0.3.6/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      150 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/transifex/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      132 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/uom/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      230 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/utm/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      628 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/web/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      265 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/web_editor/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      430 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/web_hierarchy/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      147 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/web_tour/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      362 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx    23040 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1377 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_blog/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      210 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_cf_turnstile/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      156 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_crm/17.0.2.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      189 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_crm_iap_reveal/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      183 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_crm_livechat/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      300 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_crm_partner_assign/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      617 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_customer/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     8160 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event/17.0.1.4/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      615 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_booth/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      210 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_booth_exhibitor/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      297 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_booth_sale/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      225 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_booth_sale_exhibitor/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1080 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_exhibitor/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      424 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_meet/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      443 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_sale/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1533 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_track/17.0.1.3/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      195 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_track_live/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      195 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_event_track_quiz/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      266 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_form_project/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      203 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_forum/17.0.1.2/noupdate_changes.xml
+-rw-r--r--  2.0 unx     4725 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_forum/17.0.1.2/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      799 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_hr_recruitment/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      162 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_jitsi/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      871 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_livechat/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      203 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_mass_mailing/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      299 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_membership/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      168 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_partner/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      406 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_payment/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_profile/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      334 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_profile/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      183 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale/17.0.1.1/noupdate_changes.xml
+-rw-r--r--  2.0 unx    10086 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale/17.0.1.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      198 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_autocomplete/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      519 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_comparison/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      183 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_loyalty/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      471 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_mondialrelay/17.0.0.1/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      322 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_picking/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      730 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_product_configurator/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      375 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_slides/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      177 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_stock/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      204 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_stock_wishlist/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      972 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_sale_wishlist/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     5201 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_slides/17.0.2.7/noupdate_changes.xml
+-rw-r--r--  2.0 unx     5145 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_slides/17.0.2.7/upgrade_analysis.txt
+-rw-r--r--  2.0 unx     1172 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_slides_forum/17.0.1.0/noupdate_changes.xml
+-rw-r--r--  2.0 unx      708 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_slides_forum/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      210 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_slides_survey/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx      443 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/scripts/website_twitter/17.0.1.0/upgrade_analysis.txt
+-rw-r--r--  2.0 unx    26859 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/static/description/banner.png
+-rw-r--r--  2.0 unx     9455 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/static/description/icon.png
+-rw-r--r--  2.0 unx    12639 b- defN 24-May-24 06:21 odoo/addons/openupgrade_scripts/static/description/index.html
+-rw-r--r--  2.0 unx     3784 b- defN 24-May-24 06:21 odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       83 b- defN 24-May-24 06:21 odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-May-24 06:21 odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    66448 b- defN 24-May-24 06:21 odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/RECORD
+480 files, 3649900 bytes uncompressed, 397977 bytes compressed:  89.1%
```

## zipnote {}

```diff
@@ -357,50 +357,83 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_at/17.0.3.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_au/17.0.1.1/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_bd/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_be/17.0.2.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_bf/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_bg/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_bj/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_bo/17.0.2.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_br/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_br_pix/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_br_sales/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_br_website_sale/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ca/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_cd/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_cf/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_cg/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ch/17.0.11.2/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ch/17.0.11.3/upgrade_analysis.txt
+Comment: 
+
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ci/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/noupdate_changes.xml
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_cm/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_cn/17.0.1.8/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_co/17.0.0.8/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_co/17.0.0.9/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_cr/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_cz/17.0.1.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_de/17.0.2.0/upgrade_analysis.txt
@@ -438,14 +471,20 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_dz/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ec/17.0.3.5/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ec/17.0.3.8/upgrade_analysis.txt
+Comment: 
+
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ec_website_sale/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ee/17.0.1.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_eg/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_eg_edi_eta/17.0.0.2/upgrade_analysis.txt
@@ -492,35 +531,50 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_fr_hr_holidays/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_fr_pos_cert/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ga/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_gcc_invoice/17.0.1.0.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_gn/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_gq/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_gr/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_gt/17.0.3.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_gw/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_hk/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_hn/17.0.0.2/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_hr/17.0.13.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_hu/17.0.3.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_hu_edi/17.0.1.0.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_id/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_id_efaktur/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ie/17.0.2.0/upgrade_analysis.txt
@@ -534,14 +588,17 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_in_edi/17.0.1.03.00/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_in_edi_ewaybill/17.0.1.03.00/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_in_ewaybill_stock/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_in_purchase/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_in_purchase_stock/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_in_sale/17.0.1.0/upgrade_analysis.txt
@@ -549,17 +606,23 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_in_sale_stock/17.0.0.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_it/17.0.0.5/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_it/17.0.0.6/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_it_edi/17.0.0.3/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_it_edi/17.0.0.4/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_it_edi_withholding/17.0.0.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_it_stock_ddt/17.0.0.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_jp/17.0.2.3/upgrade_analysis.txt
@@ -570,14 +633,17 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ke/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ke_edi_tremol/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_km/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_kz/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_latam_base/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_latam_check/17.0.1.0.0/upgrade_analysis.txt
@@ -594,29 +660,50 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_lv/17.0.1.0.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ma/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ml/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_mn/17.0.1.1/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_mt/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_mu_account/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_mx/17.0.2.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_mx/17.0.2.1/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_mx_hr/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_my/17.0.1.1/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_my_ubl_pint/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_mz/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ne/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ng/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_nl/17.0.3.2/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_no/17.0.2.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_nz/17.0.1.1/upgrade_analysis.txt
@@ -651,14 +738,17 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ro_edi/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_rs/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_rw/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_sa/17.0.2.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_sa_edi/17.0.0.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_se/17.0.1.0/upgrade_analysis.txt
@@ -669,17 +759,26 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_si/17.0.1.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_sk/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_sn/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_syscohada/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_td/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_tg/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_th/17.0.2.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_tn/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_tr/17.0.1.1/upgrade_analysis.txt
@@ -705,17 +804,23 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_ve/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_vn/17.0.2.0.2/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_vn/17.0.2.0.3/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/l10n_za/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/l10n_zm_account/17.0.1.0.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/link_tracker/17.0.1.1/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/loyalty/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/lunch/17.0.1.0/upgrade_analysis.txt
@@ -894,26 +999,32 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/pos_hr/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/pos_loyalty/17.0.2.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/pos_mercado_pago/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/pos_mercury/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/pos_online_payment/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/pos_online_payment_self_order/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/pos_paytm/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/pos_razorpay/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/pos_restaurant/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/pos_restaurant_adyen/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/pos_sale/17.0.1.1/upgrade_analysis.txt
@@ -1020,14 +1131,17 @@
 
 Filename: odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/noupdate_changes.xml
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/upgrade_analysis.txt
 Comment: 
 
+Filename: odoo/addons/openupgrade_scripts/scripts/sale_async_emails/17.0.1.0/upgrade_analysis.txt
+Comment: 
+
 Filename: odoo/addons/openupgrade_scripts/scripts/sale_crm/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/sale_expense/17.0.1.0/upgrade_analysis.txt
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/scripts/sale_expense_margin/17.0.1.0/upgrade_analysis.txt
@@ -1308,20 +1422,20 @@
 
 Filename: odoo/addons/openupgrade_scripts/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/openupgrade_scripts/static/description/index.html
 Comment: 
 
-Filename: odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/METADATA
+Filename: odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/WHEEL
+Filename: odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/top_level.txt
+Filename: odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/RECORD
+Filename: odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/noupdate_changes.xml

```diff
@@ -14,17 +14,14 @@
   </record>
   <record id="account_move_comp_rule" model="ir.rule">
     <field name="domain_force">[('company_id', 'in', company_ids)]</field>
   </record>
   <record id="account_move_line_comp_rule" model="ir.rule">
     <field name="domain_force">[('company_id', 'in', company_ids)]</field>
   </record>
-  <record id="account_payment_comp_rule" model="ir.rule">
-    <field name="domain_force">[('company_id', 'in', company_ids)]</field>
-  </record>
   <record id="account_payment_term_15days" model="account.payment.term">
     <field name="line_ids" eval="[Command.clear(), Command.create({'value': 'percent', 'value_amount': 100.0, 'nb_days': 15})]"/>
   </record>
   <record id="account_payment_term_21days" model="account.payment.term">
     <field name="line_ids" eval="[Command.clear(), Command.create({'value': 'percent', 'value_amount': 100.0, 'nb_days': 21})]"/>
   </record>
   <record id="account_payment_term_30_days_end_month_the_10" model="account.payment.term">
@@ -43,14 +40,17 @@
   </record>
   <record id="account_payment_term_45days" model="account.payment.term">
     <field name="line_ids" eval="[Command.clear(), Command.create({'value': 'percent', 'value_amount': 100.0, 'nb_days': 45})]"/>
   </record>
   <record id="account_payment_term_advance_60days" model="account.payment.term">
     <field name="line_ids" eval="[                 Command.clear(),                 Command.create({'value': 'percent', 'value_amount': 30.0, 'nb_days': 0}),                 Command.create({'value': 'percent', 'value_amount': 70.0, 'nb_days': 60})]"/>
   </record>
+  <record id="account_payment_term_comp_rule" model="ir.rule">
+    <field name="domain_force">['|', ('company_id', '=', False), ('company_id', 'parent_of', company_ids)]</field>
+  </record>
   <record id="account_payment_term_end_following_month" model="account.payment.term">
     <field name="line_ids" eval="[Command.clear(), Command.create({'value': 'percent', 'value_amount': 100.0, 'delay_type':'days_after_end_of_next_month', 'nb_days': 0})]"/>
   </record>
   <record id="account_payment_term_immediate" model="account.payment.term">
     <field name="line_ids" eval="[Command.clear(), Command.create({'value': 'percent', 'value_amount': 100.0, 'nb_days': 0})]"/>
   </record>
   <record id="account_reconcile_model_line_template_comp_rule" model="ir.rule">
```

## odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/upgrade_analysis.txt

```diff
@@ -103,29 +103,29 @@
 account      / account.journal          / rating_ids (one2many)         : NEW relation: rating.rating
 account      / account.move             / _order                        : _order is now 'date desc, name desc, invoice_date desc, id desc' ('date desc, name desc, id desc')
 account      / account.move             / activity_user_id (many2one)   : not related anymore
 account      / account.move             / activity_user_id (many2one)   : now a function
 account      / account.move             / amount_total_words (char)     : previously in module l10n_dz
 account      / account.move             / delivery_date (date)          : NEW isfunction: function, stored
 account      / account.move             / incoterm_location (char)      : NEW hasdefault: compute
+account      / account.move             / invoice_payment_term_id (many2one): now a function
 account      / account.move             / invoice_pdf_report_file (binary): NEW attachment: True
 account      / account.move             / rating_ids (one2many)         : NEW relation: rating.rating
 account      / account.move             / send_and_print_values (json)  : NEW
 account      / account.move.line        / discount_percentage (float)   : DEL
 account      / account.move.line        / display_type (selection)      : selection_keys is now '['cogs', 'discount', 'epd', 'line_note', 'line_section', 'payment_term', 'product', 'rounding', 'tax']' ('['cogs', 'epd', 'line_note', 'line_section', 'payment_term', 'product', 'rounding', 'tax']')
 account      / account.move.line        / invoice_date (date)           : NEW isrelated: related, stored
 account      / account.move.line        / matching_number (char)        : not a function anymore
 account      / account.move.line        / tax_audit (char)              : DEL
 account      / account.partial.reconcile / company_id (many2one)         : not related anymore
 account      / account.payment          / activity_user_id (many2one)   : not related anymore
 account      / account.payment          / activity_user_id (many2one)   : now a function
 account      / account.payment          / amount_total_words (char)     : previously in module l10n_dz
 account      / account.payment          / qr_code (char)                : type is now 'html' ('char')
 account      / account.payment          / rating_ids (one2many)         : NEW relation: rating.rating
-account      / account.payment.term     / currency_id (many2one)        : NEW relation: res.currency, hasdefault: default
 account      / account.payment.term     / discount_days (integer)       : NEW hasdefault: default
 account      / account.payment.term     / discount_percentage (float)   : NEW hasdefault: default
 account      / account.payment.term     / early_discount (boolean)      : NEW
 account      / account.payment.term     / early_pay_discount_computation (selection): NEW selection_keys: ['excluded', 'included', 'mixed'], hasdefault: compute
 account      / account.payment.term.line / days (integer)                : DEL required
 account      / account.payment.term.line / days_after (integer)          : DEL
 account      / account.payment.term.line / delay_type (selection)        : NEW required, selection_keys: ['days_after', 'days_after_end_of_month', 'days_after_end_of_next_month'], hasdefault: default
@@ -189,15 +189,15 @@
 account      / account.report           / section_report_ids (many2many): NEW relation: account.report
 account      / account.report           / sequence (integer)            : NEW
 account      / account.report           / use_sections (boolean)        : NEW hasdefault: compute
 account      / account.report.column    / figure_type (selection)       : selection_keys is now '['boolean', 'date', 'datetime', 'float', 'integer', 'monetary', 'percentage', 'string']' ('['date', 'datetime', 'float', 'integer', 'monetary', 'none', 'percentage']')
 account      / account.report.expression / figure_type (selection)       : selection_keys is now '['boolean', 'date', 'datetime', 'float', 'integer', 'monetary', 'percentage', 'string']' ('['date', 'datetime', 'float', 'integer', 'monetary', 'none', 'percentage']')
 account      / account.report.external.value / text_value (char)             : NEW
 account      / account.report.line      / external_formula (char)       : NEW
-account      / account.report.line      / user_groupby (char)           : NEW
+account      / account.report.line      / user_groupby (char)           : NEW hasdefault: compute
 account      / account.tax              / invoice_label (char)          : NEW
 account      / account.tax              / message_follower_ids (one2many): NEW relation: mail.followers
 account      / account.tax              / message_ids (one2many)        : NEW relation: mail.message
 account      / account.tax              / rating_ids (one2many)         : NEW relation: rating.rating
 account      / account.tax              / real_amount (float)           : DEL
 account      / account.tax              / repartition_line_ids (one2many): NEW relation: account.tax.repartition.line
 account      / account.tax              / website_message_ids (one2many): NEW relation: mail.message
@@ -287,14 +287,15 @@
 DEL ir.actions.act_window: account.action_account_tax_template_form
 DEL ir.actions.act_window: account.action_open_account_onboarding_create_invoice
 DEL ir.actions.act_window: account.action_open_account_onboarding_sale_tax
 NEW ir.actions.server: account.action_automatic_entry_change_account
 NEW ir.actions.server: account.action_automatic_entry_change_period
 NEW ir.actions.server: account.action_move_switch_move_type
 DEL ir.actions.server: account.action_automatic_entry
+DEL ir.actions.server: account.action_duplicate_account
 DEL ir.actions.server: account.action_move_switch_invoice_to_credit_note
 NEW ir.cron: account.ir_cron_account_move_send
 NEW ir.model.access: account.access_account_journal_group_invoice
 NEW ir.model.access: account.access_account_journal_group_readonly
 NEW ir.model.access: account.access_account_move_send
 DEL ir.model.access: account.access_account_account_template
 DEL ir.model.access: account.access_account_chart_template
@@ -306,41 +307,30 @@
 DEL ir.model.access: account.access_account_journal_group_all
 DEL ir.model.access: account.access_account_reconcile_model_line_template
 DEL ir.model.access: account.access_account_reconcile_model_template
 DEL ir.model.access: account.access_account_tag_internal_user
 DEL ir.model.access: account.access_account_tax_repartition_line_template_manager
 DEL ir.model.access: account.access_account_tax_template
 DEL ir.model.access: account.access_product_template_account_manager
+NEW ir.model.constraint: account.constraint_account_account_tag_name_uniq
+NEW ir.model.constraint: account.constraint_account_move_unique_name [renamed from account_sequence module]
+NEW ir.model.constraint: account.constraint_account_report_expression_domain_engine_subformula_required
+NEW ir.model.constraint: account.constraint_account_report_expression_line_label_uniq
+ir.model.constraint: account.constraint_account_report_line_code_uniq (changed definition: is now 'unique(report_id,code)' ('unique(code)'))
 DEL ir.model.constraint: account.constraint_account_account_code_company_uniq
-DEL ir.model.constraint: account.constraint_account_fiscal_position_account_account_src_dest_uniq
-DEL ir.model.constraint: account.constraint_account_fiscal_position_tax_tax_src_dest_uniq
-DEL ir.model.constraint: account.constraint_account_group_check_length_prefix
-DEL ir.model.constraint: account.constraint_account_journal_code_company_uniq
-DEL ir.model.constraint: account.constraint_account_journal_group_uniq_name
-DEL ir.model.constraint: account.constraint_account_move_line_check_accountable_required_fields
-DEL ir.model.constraint: account.constraint_account_move_line_check_amount_currency_balance_sign
-DEL ir.model.constraint: account.constraint_account_move_line_check_credit_debit
-DEL ir.model.constraint: account.constraint_account_move_line_check_non_accountable_fields_null
-DEL ir.model.constraint: account.constraint_account_payment_check_amount_not_negative
-DEL ir.model.constraint: account.constraint_account_payment_method_name_code_unique
-DEL ir.model.constraint: account.constraint_account_reconcile_model_name_unique
-DEL ir.model.constraint: account.constraint_account_report_line_code_uniq
 DEL ir.model.constraint: account.constraint_account_tax_name_company_uniq
 DEL ir.model.constraint: account.constraint_account_tax_template_name_company_uniq
-DEL ir.model.constraint: account_sequence.constraint_account_move_unique_name
 NEW ir.module.category: account.module_category_accounting_bank
 NEW ir.rule: account.account_move_send_rule_group_invoice (noupdate)
 NEW ir.rule: account.ir_rule_res_partner_bank_billing_officers (noupdate)
 NEW ir.rule: account.tax_group_comp_rule (noupdate)
 DEL ir.rule: account.account_invoice_send_rule_group_invoice (noupdate)
 DEL ir.sequence: account.sequence_reconcile_seq (noupdate)
 NEW ir.ui.menu: account.menu_account_supplier_accounts
 NEW ir.ui.menu: account.menu_action_analytic_reporting
-NEW ir.ui.menu: account.menu_action_open_payment_items
-NEW ir.ui.menu: account.menu_action_open_sale_payment_items
 NEW ir.ui.view: account.account_move_send_form
 NEW ir.ui.view: account.account_move_view_activity
 NEW ir.ui.view: account.document_tax_totals_company_currency_template
 NEW ir.ui.view: account.document_tax_totals_template
 NEW ir.ui.view: account.product_uom_form_view_inherit
 NEW ir.ui.view: account.report_statement_internal_layout
 NEW ir.ui.view: account.res_company_form_view_onboarding
```

## odoo/addons/openupgrade_scripts/scripts/account_edi_proxy_client/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,8 +1,9 @@
 ---Models in module 'account_edi_proxy_client'---
 ---Fields in module 'account_edi_proxy_client'---
 account_edi_proxy_client / account_edi_proxy_client.user / edi_format_id (many2one)      : DEL relation: account.edi.format, required
 account_edi_proxy_client / account_edi_proxy_client.user / edi_mode (selection)          : NEW selection_keys: ['demo', 'prod', 'test']
 account_edi_proxy_client / account_edi_proxy_client.user / proxy_type (selection)        : NEW required, selection_keys: []
 ---XML records in module 'account_edi_proxy_client'---
+NEW ir.model.constraint: account_edi_proxy_client.constraint_account_edi_proxy_client_user_unique_active_company_proxy
+NEW ir.model.constraint: account_edi_proxy_client.constraint_account_edi_proxy_client_user_unique_active_edi_identification
 DEL ir.model.constraint: account_edi_proxy_client.constraint_account_edi_proxy_client_user_unique_edi_identification_per_format
-DEL ir.model.constraint: account_edi_proxy_client.constraint_account_edi_proxy_client_user_unique_id_client
```

## odoo/addons/openupgrade_scripts/scripts/account_payment/17.0.2.0/upgrade_analysis.txt

```diff
@@ -1,16 +1,13 @@
 ---Models in module 'account_payment'---
 ---Fields in module 'account_payment'---
+account_payment / account.payment.method.line / payment_provider_id (many2one): now a function
 ---XML records in module 'account_payment'---
 NEW ir.config_parameter: account_payment.enable_portal_payment [renamed from account_payment_invoice_online_payment_patch module] (noupdate)
-DEL ir.config_parameter: account_payment_invoice_online_payment_patch.enable_portal_payment [renamed to account_payment module] (noupdate)
 NEW ir.model.access: account_payment.payment_transaction_user [renamed from payment module]
 DEL ir.rule: account_payment.payment_transaction_billing_rule (noupdate)
 NEW ir.ui.menu: account_payment.payment_method_menu
 DEL ir.ui.menu: account_payment.payment_icon_menu
 NEW ir.ui.view: account_payment.res_config_settings_view_form
 DEL ir.ui.view: account_payment.payment_checkout_inherit
 DEL ir.ui.view: account_payment.payment_manage_inherit
-DEL ir.ui.view: account_payment_invoice_online_payment_patch.portal_invoice_page_inherit_payment
-DEL ir.ui.view: account_payment_invoice_online_payment_patch.portal_my_invoices_payment
-DEL ir.ui.view: account_payment_invoice_online_payment_patch.res_config_settings_view_form
 NEW onboarding.onboarding.step: account_payment.onboarding_onboarding_step_payment_provider (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/account_peppol/17.0.1.0/upgrade_analysis.txt

```diff
@@ -8,15 +8,15 @@
 account_peppol / res.company              / account_peppol_contact_email (char): NEW hasdefault: compute
 account_peppol / res.company              / account_peppol_migration_key (char): NEW
 account_peppol / res.company              / account_peppol_phone_number (char): NEW hasdefault: compute
 account_peppol / res.company              / account_peppol_proxy_state (selection): NEW required, selection_keys: ['active', 'canceled', 'not_registered', 'not_verified', 'pending', 'rejected', 'sent_verification'], hasdefault: default
 account_peppol / res.company              / is_account_peppol_participant (boolean): NEW
 account_peppol / res.company              / peppol_purchase_journal_id (many2one): NEW relation: account.journal, isfunction: function, stored
 account_peppol / res.partner              / account_peppol_is_endpoint_valid (boolean): NEW isfunction: function, stored
-account_peppol / res.partner              / account_peppol_validity_last_check (date): NEW
+account_peppol / res.partner              / account_peppol_validity_last_check (date): NEW isfunction: function, stored
 ---XML records in module 'account_peppol'---
 NEW ir.actions.server: account_peppol.partner_action_verify_peppol
 NEW ir.cron: account_peppol.ir_cron_peppol_get_message_status
 NEW ir.cron: account_peppol.ir_cron_peppol_get_new_documents
 NEW ir.cron: account_peppol.ir_cron_peppol_get_participant_status
 NEW ir.ui.view: account_peppol.account_journal_dashboard_kanban_view
 NEW ir.ui.view: account_peppol.account_move_send_inherit_account_peppol
```

## odoo/addons/openupgrade_scripts/scripts/auth_oauth/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,4 +1,4 @@
 ---Models in module 'auth_oauth'---
 ---Fields in module 'auth_oauth'---
 ---XML records in module 'auth_oauth'---
-DEL ir.model.constraint: auth_oauth.constraint_res_users_uniq_users_oauth_provider_oauth_uid
+---nothing has changed in this module--
```

## odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/noupdate_changes.xml

```diff
@@ -8,26 +8,35 @@
   </record>
   <record id="UYI" model="res.currency">
     <field name="rounding">0.0001</field>
   </record>
   <record id="ca" model="res.country">
     <field name="vat_label">GST/HST number</field>
   </record>
+  <record id="ec" model="res.country">
+    <field name="zip_required">0</field>
+  </record>
   <record id="es" model="res.country">
     <field eval="'%(street)s\n%(street2)s\n%(zip)s %(city)s\n%(state_name)s\n%(country_name)s'" name="address_format"/>
   </record>
   <record id="europe" model="res.country.group">
     <field name="name">European Union</field>
   </record>
   <record id="main_company" model="res.company">
     <field name="currency_id" ref="base.USD"/>
   </record>
+  <record id="nz" model="res.country">
+    <field name="vat_label">GST</field>
+  </record>
   <record id="sl" model="res.country">
     <field name="currency_id" ref="SLE"/>
   </record>
   <record id="ug" model="res.country">
     <field name="vat_label">TIN</field>
   </record>
   <record id="uy" model="res.country">
     <field name="vat_label">RUT</field>
   </record>
+  <record id="zm" model="res.country">
+    <field name="vat_label">TPIN</field>
+  </record>
 </odoo>
```

## odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_analysis.txt

```diff
@@ -132,14 +132,26 @@
 DEL ir.ui.view: base.onboarding_container
 DEL ir.ui.view: base.onboarding_step
 DEL ir.ui.view: base.view_module_category_tree
 NEW res.country.group: base.eurasian_economic_union (noupdate)
 NEW res.country.state: base.state_hk_hk
 NEW res.country.state: base.state_hk_kln
 NEW res.country.state: base.state_hk_nt
+NEW res.country.state: base.state_jo_aj
+NEW res.country.state: base.state_jo_am
+NEW res.country.state: base.state_jo_aq
+NEW res.country.state: base.state_jo_at
+NEW res.country.state: base.state_jo_az
+NEW res.country.state: base.state_jo_ba
+NEW res.country.state: base.state_jo_ir
+NEW res.country.state: base.state_jo_ja
+NEW res.country.state: base.state_jo_ka
+NEW res.country.state: base.state_jo_ma
+NEW res.country.state: base.state_jo_md
+NEW res.country.state: base.state_jo_mn
 NEW res.country.state: base.state_ke_01
 NEW res.country.state: base.state_ke_02
 NEW res.country.state: base.state_ke_03
 NEW res.country.state: base.state_ke_04
 NEW res.country.state: base.state_ke_05
 NEW res.country.state: base.state_ke_06
 NEW res.country.state: base.state_ke_07
```

## odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_general_log.txt

```diff
@@ -55,14 +55,15 @@
 obsolete model sms.api [module module_map(column['module'])]
 obsolete model snailmail.confirm [module module_map(column['module'])]
 obsolete model snailmail.confirm.invoice [module module_map(column['module'])]
 obsolete model stock.immediate.transfer [module module_map(column['module'])]
 obsolete model stock.immediate.transfer.line [module module_map(column['module'])]
 new model account.edi.xml.oioubl_201 [module l10n_dk_oioubl]
 new model account.edi.xml.pint_jp [module l10n_jp_ubl_pint]
+new model account.edi.xml.pint_my [module l10n_my_ubl_pint]
 new model account.edi.xml.ubl_ro [module l10n_ro_edi]
 new model account.move.send [module account]
 new model calendar.popover.delete.wizard [module calendar]
 new model discuss.channel [module mail]
 new model discuss.channel.member [module mail]
 new model discuss.channel.rtc.session [module mail]
 new model discuss.gif.favorite [module mail]
@@ -74,14 +75,18 @@
 new model hr.leave.mandatory.day [module hr_holidays]
 new model html.field.history.mixin [module web_editor]
 new model iap.account.info [module iap]
 new model ir.model.inherit [module base]
 new model l10n_ar.payment.register.withholding [module l10n_ar_withholding]
 new model l10n_es_edi_facturae_adm_centers.ac_role_type [module l10n_es_edi_facturae_adm_centers]
 new model l10n_es_edi_facturae.certificate [module l10n_es_edi_facturae]
+new model l10n_hu_edi.cancellation [module l10n_hu_edi]
+new model l10n_hu_edi.tax_audit_export [module l10n_hu_edi]
+new model l10n.in.ewaybill [module l10n_in_ewaybill_stock]
+new model l10n.in.ewaybill.cancel [module l10n_in_ewaybill_stock]
 new model l10n_ke.item.code [module l10n_ke]
 new model l10n_pl.l10n_pl_tax_office [module l10n_pl]
 new model mail.activity.plan [module mail]
 new model mail.activity.plan.template [module mail]
 new model mail.activity.schedule [module mail]
 new model mail.activity.todo.create [module project_todo]
 new model mail.alias.domain [module mail]
@@ -117,23 +122,2744 @@
 new model spreadsheet.dashboard.share [module spreadsheet_dashboard]
 new model spreadsheet.mixin [module spreadsheet]
 new model stock.forecasted_product_product [module stock]
 new model stock.forecasted_product_template [module stock]
 new model stock.quant.relocate [module stock]
 new model website.controller.page [module website]
 ---Fields in module 'general'---
-# 11977 fields matched,
-# Direct match: 11861
-# Found in other module: 116
+# 11979 fields matched,
+# Direct match: 11847
+# Found in other module: 132
 # Found with different type: 0
 # In obsolete models: 529
-# New columns: 1521
+# New columns: 1670
 # Not matched: 1547
 ---XML records in module 'general'---
 ERROR: module not in list of installed modules:
+---Models in module 'account_payment_invoice_online_payment_patch'---
+---Fields in module 'account_payment_invoice_online_payment_patch'---
+---XML records in module 'account_payment_invoice_online_payment_patch'---
+DEL ir.config_parameter: account_payment_invoice_online_payment_patch.enable_portal_payment [renamed to account_payment module] (noupdate)
+DEL ir.ui.view: account_payment_invoice_online_payment_patch.portal_invoice_page_inherit_payment
+DEL ir.ui.view: account_payment_invoice_online_payment_patch.portal_my_invoices_payment
+DEL ir.ui.view: account_payment_invoice_online_payment_patch.res_config_settings_view_form
+ERROR: module not in list of installed modules:
+---Models in module 'association'---
+---Fields in module 'association'---
+---XML records in module 'association'---
+DEL ir.ui.menu: association.menu_event_config
+ERROR: module not in list of installed modules:
+---Models in module 'l10n_de_skr03'---
+---Fields in module 'l10n_de_skr03'---
+---XML records in module 'l10n_de_skr03'---
+DEL account.account.template: l10n_de_skr03.account_0005
+DEL account.account.template: l10n_de_skr03.account_0010
+DEL account.account.template: l10n_de_skr03.account_0015
+DEL account.account.template: l10n_de_skr03.account_0020
+DEL account.account.template: l10n_de_skr03.account_0025
+DEL account.account.template: l10n_de_skr03.account_0027
+DEL account.account.template: l10n_de_skr03.account_0030
+DEL account.account.template: l10n_de_skr03.account_0035
+DEL account.account.template: l10n_de_skr03.account_0038
+DEL account.account.template: l10n_de_skr03.account_0039
+DEL account.account.template: l10n_de_skr03.account_0040
+DEL account.account.template: l10n_de_skr03.account_0043
+DEL account.account.template: l10n_de_skr03.account_0045
+DEL account.account.template: l10n_de_skr03.account_0046
+DEL account.account.template: l10n_de_skr03.account_0047
+DEL account.account.template: l10n_de_skr03.account_0048
+DEL account.account.template: l10n_de_skr03.account_0050
+DEL account.account.template: l10n_de_skr03.account_0059
+DEL account.account.template: l10n_de_skr03.account_0060
+DEL account.account.template: l10n_de_skr03.account_0065
+DEL account.account.template: l10n_de_skr03.account_0070
+DEL account.account.template: l10n_de_skr03.account_0075
+DEL account.account.template: l10n_de_skr03.account_0079
+DEL account.account.template: l10n_de_skr03.account_0080
+DEL account.account.template: l10n_de_skr03.account_0085
+DEL account.account.template: l10n_de_skr03.account_0090
+DEL account.account.template: l10n_de_skr03.account_0100
+DEL account.account.template: l10n_de_skr03.account_0110
+DEL account.account.template: l10n_de_skr03.account_0111
+DEL account.account.template: l10n_de_skr03.account_0112
+DEL account.account.template: l10n_de_skr03.account_0113
+DEL account.account.template: l10n_de_skr03.account_0115
+DEL account.account.template: l10n_de_skr03.account_0120
+DEL account.account.template: l10n_de_skr03.account_0129
+DEL account.account.template: l10n_de_skr03.account_0140
+DEL account.account.template: l10n_de_skr03.account_0145
+DEL account.account.template: l10n_de_skr03.account_0146
+DEL account.account.template: l10n_de_skr03.account_0147
+DEL account.account.template: l10n_de_skr03.account_0148
+DEL account.account.template: l10n_de_skr03.account_0149
+DEL account.account.template: l10n_de_skr03.account_0150
+DEL account.account.template: l10n_de_skr03.account_0159
+DEL account.account.template: l10n_de_skr03.account_0160
+DEL account.account.template: l10n_de_skr03.account_0165
+DEL account.account.template: l10n_de_skr03.account_0170
+DEL account.account.template: l10n_de_skr03.account_0175
+DEL account.account.template: l10n_de_skr03.account_0176
+DEL account.account.template: l10n_de_skr03.account_0177
+DEL account.account.template: l10n_de_skr03.account_0178
+DEL account.account.template: l10n_de_skr03.account_0179
+DEL account.account.template: l10n_de_skr03.account_0180
+DEL account.account.template: l10n_de_skr03.account_0189
+DEL account.account.template: l10n_de_skr03.account_0190
+DEL account.account.template: l10n_de_skr03.account_0191
+DEL account.account.template: l10n_de_skr03.account_0192
+DEL account.account.template: l10n_de_skr03.account_0193
+DEL account.account.template: l10n_de_skr03.account_0194
+DEL account.account.template: l10n_de_skr03.account_0195
+DEL account.account.template: l10n_de_skr03.account_0199
+DEL account.account.template: l10n_de_skr03.account_0200
+DEL account.account.template: l10n_de_skr03.account_0210
+DEL account.account.template: l10n_de_skr03.account_0220
+DEL account.account.template: l10n_de_skr03.account_0240
+DEL account.account.template: l10n_de_skr03.account_0260
+DEL account.account.template: l10n_de_skr03.account_0280
+DEL account.account.template: l10n_de_skr03.account_0290
+DEL account.account.template: l10n_de_skr03.account_0299
+DEL account.account.template: l10n_de_skr03.account_0300
+DEL account.account.template: l10n_de_skr03.account_0310
+DEL account.account.template: l10n_de_skr03.account_0320
+DEL account.account.template: l10n_de_skr03.account_0350
+DEL account.account.template: l10n_de_skr03.account_0380
+DEL account.account.template: l10n_de_skr03.account_0400
+DEL account.account.template: l10n_de_skr03.account_0410
+DEL account.account.template: l10n_de_skr03.account_0420
+DEL account.account.template: l10n_de_skr03.account_0430
+DEL account.account.template: l10n_de_skr03.account_0440
+DEL account.account.template: l10n_de_skr03.account_0450
+DEL account.account.template: l10n_de_skr03.account_0460
+DEL account.account.template: l10n_de_skr03.account_0480
+DEL account.account.template: l10n_de_skr03.account_0485
+DEL account.account.template: l10n_de_skr03.account_0490
+DEL account.account.template: l10n_de_skr03.account_0498
+DEL account.account.template: l10n_de_skr03.account_0499
+DEL account.account.template: l10n_de_skr03.account_0500
+DEL account.account.template: l10n_de_skr03.account_0501
+DEL account.account.template: l10n_de_skr03.account_0502
+DEL account.account.template: l10n_de_skr03.account_0503
+DEL account.account.template: l10n_de_skr03.account_0504
+DEL account.account.template: l10n_de_skr03.account_0505
+DEL account.account.template: l10n_de_skr03.account_0506
+DEL account.account.template: l10n_de_skr03.account_0507
+DEL account.account.template: l10n_de_skr03.account_0508
+DEL account.account.template: l10n_de_skr03.account_0509
+DEL account.account.template: l10n_de_skr03.account_0510
+DEL account.account.template: l10n_de_skr03.account_0513
+DEL account.account.template: l10n_de_skr03.account_0516
+DEL account.account.template: l10n_de_skr03.account_0517
+DEL account.account.template: l10n_de_skr03.account_0518
+DEL account.account.template: l10n_de_skr03.account_0519
+DEL account.account.template: l10n_de_skr03.account_0520
+DEL account.account.template: l10n_de_skr03.account_0523
+DEL account.account.template: l10n_de_skr03.account_0524
+DEL account.account.template: l10n_de_skr03.account_0525
+DEL account.account.template: l10n_de_skr03.account_0530
+DEL account.account.template: l10n_de_skr03.account_0535
+DEL account.account.template: l10n_de_skr03.account_0540
+DEL account.account.template: l10n_de_skr03.account_0550
+DEL account.account.template: l10n_de_skr03.account_0570
+DEL account.account.template: l10n_de_skr03.account_0580
+DEL account.account.template: l10n_de_skr03.account_0582
+DEL account.account.template: l10n_de_skr03.account_0584
+DEL account.account.template: l10n_de_skr03.account_0586
+DEL account.account.template: l10n_de_skr03.account_0590
+DEL account.account.template: l10n_de_skr03.account_0595
+DEL account.account.template: l10n_de_skr03.account_0600
+DEL account.account.template: l10n_de_skr03.account_0601
+DEL account.account.template: l10n_de_skr03.account_0605
+DEL account.account.template: l10n_de_skr03.account_0610
+DEL account.account.template: l10n_de_skr03.account_0615
+DEL account.account.template: l10n_de_skr03.account_0616
+DEL account.account.template: l10n_de_skr03.account_0620
+DEL account.account.template: l10n_de_skr03.account_0625
+DEL account.account.template: l10n_de_skr03.account_0630
+DEL account.account.template: l10n_de_skr03.account_0631
+DEL account.account.template: l10n_de_skr03.account_0640
+DEL account.account.template: l10n_de_skr03.account_0650
+DEL account.account.template: l10n_de_skr03.account_0660
+DEL account.account.template: l10n_de_skr03.account_0661
+DEL account.account.template: l10n_de_skr03.account_0670
+DEL account.account.template: l10n_de_skr03.account_0680
+DEL account.account.template: l10n_de_skr03.account_0699
+DEL account.account.template: l10n_de_skr03.account_0700
+DEL account.account.template: l10n_de_skr03.account_0701
+DEL account.account.template: l10n_de_skr03.account_0705
+DEL account.account.template: l10n_de_skr03.account_0710
+DEL account.account.template: l10n_de_skr03.account_0715
+DEL account.account.template: l10n_de_skr03.account_0716
+DEL account.account.template: l10n_de_skr03.account_0720
+DEL account.account.template: l10n_de_skr03.account_0725
+DEL account.account.template: l10n_de_skr03.account_0730
+DEL account.account.template: l10n_de_skr03.account_0731
+DEL account.account.template: l10n_de_skr03.account_0740
+DEL account.account.template: l10n_de_skr03.account_0750
+DEL account.account.template: l10n_de_skr03.account_0755
+DEL account.account.template: l10n_de_skr03.account_0760
+DEL account.account.template: l10n_de_skr03.account_0761
+DEL account.account.template: l10n_de_skr03.account_0764
+DEL account.account.template: l10n_de_skr03.account_0767
+DEL account.account.template: l10n_de_skr03.account_0770
+DEL account.account.template: l10n_de_skr03.account_0771
+DEL account.account.template: l10n_de_skr03.account_0774
+DEL account.account.template: l10n_de_skr03.account_0777
+DEL account.account.template: l10n_de_skr03.account_0780
+DEL account.account.template: l10n_de_skr03.account_0781
+DEL account.account.template: l10n_de_skr03.account_0784
+DEL account.account.template: l10n_de_skr03.account_0787
+DEL account.account.template: l10n_de_skr03.account_0799
+DEL account.account.template: l10n_de_skr03.account_0809
+DEL account.account.template: l10n_de_skr03.account_0810
+DEL account.account.template: l10n_de_skr03.account_0811
+DEL account.account.template: l10n_de_skr03.account_0812
+DEL account.account.template: l10n_de_skr03.account_0813
+DEL account.account.template: l10n_de_skr03.account_0815
+DEL account.account.template: l10n_de_skr03.account_0819
+DEL account.account.template: l10n_de_skr03.account_0839
+DEL account.account.template: l10n_de_skr03.account_0845
+DEL account.account.template: l10n_de_skr03.account_0848
+DEL account.account.template: l10n_de_skr03.account_0849
+DEL account.account.template: l10n_de_skr03.account_0852
+DEL account.account.template: l10n_de_skr03.account_0853
+DEL account.account.template: l10n_de_skr03.account_0854
+DEL account.account.template: l10n_de_skr03.account_0857
+DEL account.account.template: l10n_de_skr03.account_0858
+DEL account.account.template: l10n_de_skr03.account_0859
+DEL account.account.template: l10n_de_skr03.account_0865
+DEL account.account.template: l10n_de_skr03.account_0867
+DEL account.account.template: l10n_de_skr03.account_0870
+DEL account.account.template: l10n_de_skr03.account_0880
+DEL account.account.template: l10n_de_skr03.account_0890
+DEL account.account.template: l10n_de_skr03.account_0900
+DEL account.account.template: l10n_de_skr03.account_0910
+DEL account.account.template: l10n_de_skr03.account_0920
+DEL account.account.template: l10n_de_skr03.account_0950
+DEL account.account.template: l10n_de_skr03.account_0951
+DEL account.account.template: l10n_de_skr03.account_0952
+DEL account.account.template: l10n_de_skr03.account_0953
+DEL account.account.template: l10n_de_skr03.account_0954
+DEL account.account.template: l10n_de_skr03.account_0955
+DEL account.account.template: l10n_de_skr03.account_0956
+DEL account.account.template: l10n_de_skr03.account_0957
+DEL account.account.template: l10n_de_skr03.account_0961
+DEL account.account.template: l10n_de_skr03.account_0962
+DEL account.account.template: l10n_de_skr03.account_0963
+DEL account.account.template: l10n_de_skr03.account_0964
+DEL account.account.template: l10n_de_skr03.account_0965
+DEL account.account.template: l10n_de_skr03.account_0966
+DEL account.account.template: l10n_de_skr03.account_0967
+DEL account.account.template: l10n_de_skr03.account_0968
+DEL account.account.template: l10n_de_skr03.account_0969
+DEL account.account.template: l10n_de_skr03.account_0970
+DEL account.account.template: l10n_de_skr03.account_0971
+DEL account.account.template: l10n_de_skr03.account_0973
+DEL account.account.template: l10n_de_skr03.account_0974
+DEL account.account.template: l10n_de_skr03.account_0976
+DEL account.account.template: l10n_de_skr03.account_0977
+DEL account.account.template: l10n_de_skr03.account_0978
+DEL account.account.template: l10n_de_skr03.account_0979
+DEL account.account.template: l10n_de_skr03.account_0980
+DEL account.account.template: l10n_de_skr03.account_0983
+DEL account.account.template: l10n_de_skr03.account_0984
+DEL account.account.template: l10n_de_skr03.account_0985
+DEL account.account.template: l10n_de_skr03.account_0986
+DEL account.account.template: l10n_de_skr03.account_0987
+DEL account.account.template: l10n_de_skr03.account_0988
+DEL account.account.template: l10n_de_skr03.account_0989
+DEL account.account.template: l10n_de_skr03.account_0990
+DEL account.account.template: l10n_de_skr03.account_0996
+DEL account.account.template: l10n_de_skr03.account_0997
+DEL account.account.template: l10n_de_skr03.account_0998
+DEL account.account.template: l10n_de_skr03.account_0999
+DEL account.account.template: l10n_de_skr03.account_1010
+DEL account.account.template: l10n_de_skr03.account_1020
+DEL account.account.template: l10n_de_skr03.account_1100
+DEL account.account.template: l10n_de_skr03.account_1110
+DEL account.account.template: l10n_de_skr03.account_1120
+DEL account.account.template: l10n_de_skr03.account_1130
+DEL account.account.template: l10n_de_skr03.account_1190
+DEL account.account.template: l10n_de_skr03.account_1195
+DEL account.account.template: l10n_de_skr03.account_1210
+DEL account.account.template: l10n_de_skr03.account_1220
+DEL account.account.template: l10n_de_skr03.account_1230
+DEL account.account.template: l10n_de_skr03.account_1240
+DEL account.account.template: l10n_de_skr03.account_1250
+DEL account.account.template: l10n_de_skr03.account_1290
+DEL account.account.template: l10n_de_skr03.account_1295
+DEL account.account.template: l10n_de_skr03.account_1300
+DEL account.account.template: l10n_de_skr03.account_1301
+DEL account.account.template: l10n_de_skr03.account_1302
+DEL account.account.template: l10n_de_skr03.account_1305
+DEL account.account.template: l10n_de_skr03.account_1310
+DEL account.account.template: l10n_de_skr03.account_1311
+DEL account.account.template: l10n_de_skr03.account_1312
+DEL account.account.template: l10n_de_skr03.account_1315
+DEL account.account.template: l10n_de_skr03.account_1320
+DEL account.account.template: l10n_de_skr03.account_1321
+DEL account.account.template: l10n_de_skr03.account_1322
+DEL account.account.template: l10n_de_skr03.account_1325
+DEL account.account.template: l10n_de_skr03.account_1327
+DEL account.account.template: l10n_de_skr03.account_1329
+DEL account.account.template: l10n_de_skr03.account_1330
+DEL account.account.template: l10n_de_skr03.account_1340
+DEL account.account.template: l10n_de_skr03.account_1344
+DEL account.account.template: l10n_de_skr03.account_1348
+DEL account.account.template: l10n_de_skr03.account_1349
+DEL account.account.template: l10n_de_skr03.account_1350
+DEL account.account.template: l10n_de_skr03.account_1352
+DEL account.account.template: l10n_de_skr03.account_1353
+DEL account.account.template: l10n_de_skr03.account_1354
+DEL account.account.template: l10n_de_skr03.account_1355
+DEL account.account.template: l10n_de_skr03.account_1356
+DEL account.account.template: l10n_de_skr03.account_1357
+DEL account.account.template: l10n_de_skr03.account_1370
+DEL account.account.template: l10n_de_skr03.account_1371
+DEL account.account.template: l10n_de_skr03.account_1372
+DEL account.account.template: l10n_de_skr03.account_1373
+DEL account.account.template: l10n_de_skr03.account_1374
+DEL account.account.template: l10n_de_skr03.account_1375
+DEL account.account.template: l10n_de_skr03.account_1376
+DEL account.account.template: l10n_de_skr03.account_1377
+DEL account.account.template: l10n_de_skr03.account_1378
+DEL account.account.template: l10n_de_skr03.account_1380
+DEL account.account.template: l10n_de_skr03.account_1381
+DEL account.account.template: l10n_de_skr03.account_1382
+DEL account.account.template: l10n_de_skr03.account_1383
+DEL account.account.template: l10n_de_skr03.account_1385
+DEL account.account.template: l10n_de_skr03.account_1386
+DEL account.account.template: l10n_de_skr03.account_1387
+DEL account.account.template: l10n_de_skr03.account_1389
+DEL account.account.template: l10n_de_skr03.account_1390
+DEL account.account.template: l10n_de_skr03.account_1400
+DEL account.account.template: l10n_de_skr03.account_1401
+DEL account.account.template: l10n_de_skr03.account_1410
+DEL account.account.template: l10n_de_skr03.account_1411
+DEL account.account.template: l10n_de_skr03.account_1445
+DEL account.account.template: l10n_de_skr03.account_1446
+DEL account.account.template: l10n_de_skr03.account_1447
+DEL account.account.template: l10n_de_skr03.account_1448
+DEL account.account.template: l10n_de_skr03.account_1449
+DEL account.account.template: l10n_de_skr03.account_1450
+DEL account.account.template: l10n_de_skr03.account_1451
+DEL account.account.template: l10n_de_skr03.account_1455
+DEL account.account.template: l10n_de_skr03.account_1460
+DEL account.account.template: l10n_de_skr03.account_1461
+DEL account.account.template: l10n_de_skr03.account_1465
+DEL account.account.template: l10n_de_skr03.account_1470
+DEL account.account.template: l10n_de_skr03.account_1471
+DEL account.account.template: l10n_de_skr03.account_1475
+DEL account.account.template: l10n_de_skr03.account_1478
+DEL account.account.template: l10n_de_skr03.account_1479
+DEL account.account.template: l10n_de_skr03.account_1480
+DEL account.account.template: l10n_de_skr03.account_1481
+DEL account.account.template: l10n_de_skr03.account_1485
+DEL account.account.template: l10n_de_skr03.account_1488
+DEL account.account.template: l10n_de_skr03.account_1489
+DEL account.account.template: l10n_de_skr03.account_1490
+DEL account.account.template: l10n_de_skr03.account_1491
+DEL account.account.template: l10n_de_skr03.account_1495
+DEL account.account.template: l10n_de_skr03.account_1498
+DEL account.account.template: l10n_de_skr03.account_1499
+DEL account.account.template: l10n_de_skr03.account_1500
+DEL account.account.template: l10n_de_skr03.account_1501
+DEL account.account.template: l10n_de_skr03.account_1502
+DEL account.account.template: l10n_de_skr03.account_1503
+DEL account.account.template: l10n_de_skr03.account_1504
+DEL account.account.template: l10n_de_skr03.account_1505
+DEL account.account.template: l10n_de_skr03.account_1506
+DEL account.account.template: l10n_de_skr03.account_1507
+DEL account.account.template: l10n_de_skr03.account_1508
+DEL account.account.template: l10n_de_skr03.account_1510
+DEL account.account.template: l10n_de_skr03.account_1511
+DEL account.account.template: l10n_de_skr03.account_1518
+DEL account.account.template: l10n_de_skr03.account_1519
+DEL account.account.template: l10n_de_skr03.account_1520
+DEL account.account.template: l10n_de_skr03.account_1521
+DEL account.account.template: l10n_de_skr03.account_1522
+DEL account.account.template: l10n_de_skr03.account_1524
+DEL account.account.template: l10n_de_skr03.account_1525
+DEL account.account.template: l10n_de_skr03.account_1526
+DEL account.account.template: l10n_de_skr03.account_1527
+DEL account.account.template: l10n_de_skr03.account_1528
+DEL account.account.template: l10n_de_skr03.account_1529
+DEL account.account.template: l10n_de_skr03.account_1530
+DEL account.account.template: l10n_de_skr03.account_1531
+DEL account.account.template: l10n_de_skr03.account_1537
+DEL account.account.template: l10n_de_skr03.account_1538
+DEL account.account.template: l10n_de_skr03.account_1539
+DEL account.account.template: l10n_de_skr03.account_1540
+DEL account.account.template: l10n_de_skr03.account_1542
+DEL account.account.template: l10n_de_skr03.account_1543
+DEL account.account.template: l10n_de_skr03.account_1544
+DEL account.account.template: l10n_de_skr03.account_1545
+DEL account.account.template: l10n_de_skr03.account_1547
+DEL account.account.template: l10n_de_skr03.account_1548
+DEL account.account.template: l10n_de_skr03.account_1549
+DEL account.account.template: l10n_de_skr03.account_1550
+DEL account.account.template: l10n_de_skr03.account_1551
+DEL account.account.template: l10n_de_skr03.account_1555
+DEL account.account.template: l10n_de_skr03.account_1556
+DEL account.account.template: l10n_de_skr03.account_1557
+DEL account.account.template: l10n_de_skr03.account_1558
+DEL account.account.template: l10n_de_skr03.account_1559
+DEL account.account.template: l10n_de_skr03.account_1560
+DEL account.account.template: l10n_de_skr03.account_1561
+DEL account.account.template: l10n_de_skr03.account_1562
+DEL account.account.template: l10n_de_skr03.account_1563
+DEL account.account.template: l10n_de_skr03.account_1566
+DEL account.account.template: l10n_de_skr03.account_1567
+DEL account.account.template: l10n_de_skr03.account_1569
+DEL account.account.template: l10n_de_skr03.account_1570
+DEL account.account.template: l10n_de_skr03.account_1571
+DEL account.account.template: l10n_de_skr03.account_1572
+DEL account.account.template: l10n_de_skr03.account_1574
+DEL account.account.template: l10n_de_skr03.account_1576
+DEL account.account.template: l10n_de_skr03.account_1577
+DEL account.account.template: l10n_de_skr03.account_1578
+DEL account.account.template: l10n_de_skr03.account_1580
+DEL account.account.template: l10n_de_skr03.account_1581
+DEL account.account.template: l10n_de_skr03.account_1582
+DEL account.account.template: l10n_de_skr03.account_1583
+DEL account.account.template: l10n_de_skr03.account_1584
+DEL account.account.template: l10n_de_skr03.account_1585
+DEL account.account.template: l10n_de_skr03.account_1587
+DEL account.account.template: l10n_de_skr03.account_1588
+DEL account.account.template: l10n_de_skr03.account_1590
+DEL account.account.template: l10n_de_skr03.account_1592
+DEL account.account.template: l10n_de_skr03.account_1593
+DEL account.account.template: l10n_de_skr03.account_1594
+DEL account.account.template: l10n_de_skr03.account_1595
+DEL account.account.template: l10n_de_skr03.account_1596
+DEL account.account.template: l10n_de_skr03.account_1597
+DEL account.account.template: l10n_de_skr03.account_1598
+DEL account.account.template: l10n_de_skr03.account_1599
+DEL account.account.template: l10n_de_skr03.account_1600
+DEL account.account.template: l10n_de_skr03.account_1601
+DEL account.account.template: l10n_de_skr03.account_1605
+DEL account.account.template: l10n_de_skr03.account_1606
+DEL account.account.template: l10n_de_skr03.account_1607
+DEL account.account.template: l10n_de_skr03.account_1609
+DEL account.account.template: l10n_de_skr03.account_1610
+DEL account.account.template: l10n_de_skr03.account_1624
+DEL account.account.template: l10n_de_skr03.account_1625
+DEL account.account.template: l10n_de_skr03.account_1626
+DEL account.account.template: l10n_de_skr03.account_1628
+DEL account.account.template: l10n_de_skr03.account_1630
+DEL account.account.template: l10n_de_skr03.account_1631
+DEL account.account.template: l10n_de_skr03.account_1635
+DEL account.account.template: l10n_de_skr03.account_1638
+DEL account.account.template: l10n_de_skr03.account_1640
+DEL account.account.template: l10n_de_skr03.account_1641
+DEL account.account.template: l10n_de_skr03.account_1645
+DEL account.account.template: l10n_de_skr03.account_1648
+DEL account.account.template: l10n_de_skr03.account_1650
+DEL account.account.template: l10n_de_skr03.account_1651
+DEL account.account.template: l10n_de_skr03.account_1655
+DEL account.account.template: l10n_de_skr03.account_1658
+DEL account.account.template: l10n_de_skr03.account_1659
+DEL account.account.template: l10n_de_skr03.account_1660
+DEL account.account.template: l10n_de_skr03.account_1661
+DEL account.account.template: l10n_de_skr03.account_1662
+DEL account.account.template: l10n_de_skr03.account_1663
+DEL account.account.template: l10n_de_skr03.account_1665
+DEL account.account.template: l10n_de_skr03.account_1666
+DEL account.account.template: l10n_de_skr03.account_1667
+DEL account.account.template: l10n_de_skr03.account_1668
+DEL account.account.template: l10n_de_skr03.account_1670
+DEL account.account.template: l10n_de_skr03.account_1671
+DEL account.account.template: l10n_de_skr03.account_1672
+DEL account.account.template: l10n_de_skr03.account_1673
+DEL account.account.template: l10n_de_skr03.account_1675
+DEL account.account.template: l10n_de_skr03.account_1676
+DEL account.account.template: l10n_de_skr03.account_1677
+DEL account.account.template: l10n_de_skr03.account_1678
+DEL account.account.template: l10n_de_skr03.account_1691
+DEL account.account.template: l10n_de_skr03.account_1695
+DEL account.account.template: l10n_de_skr03.account_1696
+DEL account.account.template: l10n_de_skr03.account_1697
+DEL account.account.template: l10n_de_skr03.account_1698
+DEL account.account.template: l10n_de_skr03.account_1700
+DEL account.account.template: l10n_de_skr03.account_1701
+DEL account.account.template: l10n_de_skr03.account_1702
+DEL account.account.template: l10n_de_skr03.account_1703
+DEL account.account.template: l10n_de_skr03.account_1704
+DEL account.account.template: l10n_de_skr03.account_1705
+DEL account.account.template: l10n_de_skr03.account_1706
+DEL account.account.template: l10n_de_skr03.account_1707
+DEL account.account.template: l10n_de_skr03.account_1708
+DEL account.account.template: l10n_de_skr03.account_1709
+DEL account.account.template: l10n_de_skr03.account_1710
+DEL account.account.template: l10n_de_skr03.account_1711
+DEL account.account.template: l10n_de_skr03.account_1716
+DEL account.account.template: l10n_de_skr03.account_1718
+DEL account.account.template: l10n_de_skr03.account_1719
+DEL account.account.template: l10n_de_skr03.account_1720
+DEL account.account.template: l10n_de_skr03.account_1721
+DEL account.account.template: l10n_de_skr03.account_1722
+DEL account.account.template: l10n_de_skr03.account_1725
+DEL account.account.template: l10n_de_skr03.account_1728
+DEL account.account.template: l10n_de_skr03.account_1729
+DEL account.account.template: l10n_de_skr03.account_1730
+DEL account.account.template: l10n_de_skr03.account_1731
+DEL account.account.template: l10n_de_skr03.account_1732
+DEL account.account.template: l10n_de_skr03.account_1733
+DEL account.account.template: l10n_de_skr03.account_1734
+DEL account.account.template: l10n_de_skr03.account_1735
+DEL account.account.template: l10n_de_skr03.account_1736
+DEL account.account.template: l10n_de_skr03.account_1737
+DEL account.account.template: l10n_de_skr03.account_1738
+DEL account.account.template: l10n_de_skr03.account_1739
+DEL account.account.template: l10n_de_skr03.account_1740
+DEL account.account.template: l10n_de_skr03.account_1741
+DEL account.account.template: l10n_de_skr03.account_1742
+DEL account.account.template: l10n_de_skr03.account_1743
+DEL account.account.template: l10n_de_skr03.account_1744
+DEL account.account.template: l10n_de_skr03.account_1745
+DEL account.account.template: l10n_de_skr03.account_1746
+DEL account.account.template: l10n_de_skr03.account_1747
+DEL account.account.template: l10n_de_skr03.account_1748
+DEL account.account.template: l10n_de_skr03.account_1749
+DEL account.account.template: l10n_de_skr03.account_1750
+DEL account.account.template: l10n_de_skr03.account_1751
+DEL account.account.template: l10n_de_skr03.account_1752
+DEL account.account.template: l10n_de_skr03.account_1753
+DEL account.account.template: l10n_de_skr03.account_1754
+DEL account.account.template: l10n_de_skr03.account_1755
+DEL account.account.template: l10n_de_skr03.account_1756
+DEL account.account.template: l10n_de_skr03.account_1758
+DEL account.account.template: l10n_de_skr03.account_1759
+DEL account.account.template: l10n_de_skr03.account_1760
+DEL account.account.template: l10n_de_skr03.account_1761
+DEL account.account.template: l10n_de_skr03.account_1762
+DEL account.account.template: l10n_de_skr03.account_1764
+DEL account.account.template: l10n_de_skr03.account_1766
+DEL account.account.template: l10n_de_skr03.account_1767
+DEL account.account.template: l10n_de_skr03.account_1768
+DEL account.account.template: l10n_de_skr03.account_1769
+DEL account.account.template: l10n_de_skr03.account_1770
+DEL account.account.template: l10n_de_skr03.account_1771
+DEL account.account.template: l10n_de_skr03.account_1772
+DEL account.account.template: l10n_de_skr03.account_1774
+DEL account.account.template: l10n_de_skr03.account_1776
+DEL account.account.template: l10n_de_skr03.account_1777
+DEL account.account.template: l10n_de_skr03.account_1778
+DEL account.account.template: l10n_de_skr03.account_1779
+DEL account.account.template: l10n_de_skr03.account_1780
+DEL account.account.template: l10n_de_skr03.account_1781
+DEL account.account.template: l10n_de_skr03.account_1782
+DEL account.account.template: l10n_de_skr03.account_1783
+DEL account.account.template: l10n_de_skr03.account_1784
+DEL account.account.template: l10n_de_skr03.account_1785
+DEL account.account.template: l10n_de_skr03.account_1787
+DEL account.account.template: l10n_de_skr03.account_1788
+DEL account.account.template: l10n_de_skr03.account_1789
+DEL account.account.template: l10n_de_skr03.account_1790
+DEL account.account.template: l10n_de_skr03.account_1791
+DEL account.account.template: l10n_de_skr03.account_1792
+DEL account.account.template: l10n_de_skr03.account_1793
+DEL account.account.template: l10n_de_skr03.account_1794
+DEL account.account.template: l10n_de_skr03.account_1795
+DEL account.account.template: l10n_de_skr03.account_1796
+DEL account.account.template: l10n_de_skr03.account_1797
+DEL account.account.template: l10n_de_skr03.account_1800
+DEL account.account.template: l10n_de_skr03.account_1810
+DEL account.account.template: l10n_de_skr03.account_1820
+DEL account.account.template: l10n_de_skr03.account_1830
+DEL account.account.template: l10n_de_skr03.account_1840
+DEL account.account.template: l10n_de_skr03.account_1850
+DEL account.account.template: l10n_de_skr03.account_1860
+DEL account.account.template: l10n_de_skr03.account_1869
+DEL account.account.template: l10n_de_skr03.account_1870
+DEL account.account.template: l10n_de_skr03.account_1879
+DEL account.account.template: l10n_de_skr03.account_1880
+DEL account.account.template: l10n_de_skr03.account_1890
+DEL account.account.template: l10n_de_skr03.account_1900
+DEL account.account.template: l10n_de_skr03.account_1910
+DEL account.account.template: l10n_de_skr03.account_1920
+DEL account.account.template: l10n_de_skr03.account_1930
+DEL account.account.template: l10n_de_skr03.account_1940
+DEL account.account.template: l10n_de_skr03.account_1950
+DEL account.account.template: l10n_de_skr03.account_1960
+DEL account.account.template: l10n_de_skr03.account_1970
+DEL account.account.template: l10n_de_skr03.account_1980
+DEL account.account.template: l10n_de_skr03.account_1990
+DEL account.account.template: l10n_de_skr03.account_2000
+DEL account.account.template: l10n_de_skr03.account_2001
+DEL account.account.template: l10n_de_skr03.account_2004
+DEL account.account.template: l10n_de_skr03.account_2005
+DEL account.account.template: l10n_de_skr03.account_2006
+DEL account.account.template: l10n_de_skr03.account_2007
+DEL account.account.template: l10n_de_skr03.account_2008
+DEL account.account.template: l10n_de_skr03.account_2010
+DEL account.account.template: l10n_de_skr03.account_2020
+DEL account.account.template: l10n_de_skr03.account_2090
+DEL account.account.template: l10n_de_skr03.account_2091
+DEL account.account.template: l10n_de_skr03.account_2092
+DEL account.account.template: l10n_de_skr03.account_2094
+DEL account.account.template: l10n_de_skr03.account_2100
+DEL account.account.template: l10n_de_skr03.account_2102
+DEL account.account.template: l10n_de_skr03.account_2103
+DEL account.account.template: l10n_de_skr03.account_2104
+DEL account.account.template: l10n_de_skr03.account_2105
+DEL account.account.template: l10n_de_skr03.account_2106
+DEL account.account.template: l10n_de_skr03.account_2107
+DEL account.account.template: l10n_de_skr03.account_2108
+DEL account.account.template: l10n_de_skr03.account_2109
+DEL account.account.template: l10n_de_skr03.account_2110
+DEL account.account.template: l10n_de_skr03.account_2113
+DEL account.account.template: l10n_de_skr03.account_2114
+DEL account.account.template: l10n_de_skr03.account_2115
+DEL account.account.template: l10n_de_skr03.account_2116
+DEL account.account.template: l10n_de_skr03.account_2117
+DEL account.account.template: l10n_de_skr03.account_2118
+DEL account.account.template: l10n_de_skr03.account_2119
+DEL account.account.template: l10n_de_skr03.account_2120
+DEL account.account.template: l10n_de_skr03.account_2123
+DEL account.account.template: l10n_de_skr03.account_2124
+DEL account.account.template: l10n_de_skr03.account_2125
+DEL account.account.template: l10n_de_skr03.account_2126
+DEL account.account.template: l10n_de_skr03.account_2127
+DEL account.account.template: l10n_de_skr03.account_2128
+DEL account.account.template: l10n_de_skr03.account_2129
+DEL account.account.template: l10n_de_skr03.account_2130
+DEL account.account.template: l10n_de_skr03.account_2139
+DEL account.account.template: l10n_de_skr03.account_2140
+DEL account.account.template: l10n_de_skr03.account_2141
+DEL account.account.template: l10n_de_skr03.account_2142
+DEL account.account.template: l10n_de_skr03.account_2143
+DEL account.account.template: l10n_de_skr03.account_2144
+DEL account.account.template: l10n_de_skr03.account_2145
+DEL account.account.template: l10n_de_skr03.account_2146
+DEL account.account.template: l10n_de_skr03.account_2147
+DEL account.account.template: l10n_de_skr03.account_2148
+DEL account.account.template: l10n_de_skr03.account_2149
+DEL account.account.template: l10n_de_skr03.account_2150
+DEL account.account.template: l10n_de_skr03.account_2151
+DEL account.account.template: l10n_de_skr03.account_2166
+DEL account.account.template: l10n_de_skr03.account_2170
+DEL account.account.template: l10n_de_skr03.account_2171
+DEL account.account.template: l10n_de_skr03.account_2176
+DEL account.account.template: l10n_de_skr03.account_2200
+DEL account.account.template: l10n_de_skr03.account_2203
+DEL account.account.template: l10n_de_skr03.account_2204
+DEL account.account.template: l10n_de_skr03.account_2208
+DEL account.account.template: l10n_de_skr03.account_2209
+DEL account.account.template: l10n_de_skr03.account_2210
+DEL account.account.template: l10n_de_skr03.account_2213
+DEL account.account.template: l10n_de_skr03.account_2216
+DEL account.account.template: l10n_de_skr03.account_2219
+DEL account.account.template: l10n_de_skr03.account_2250
+DEL account.account.template: l10n_de_skr03.account_2255
+DEL account.account.template: l10n_de_skr03.account_2260
+DEL account.account.template: l10n_de_skr03.account_2265
+DEL account.account.template: l10n_de_skr03.account_2280
+DEL account.account.template: l10n_de_skr03.account_2281
+DEL account.account.template: l10n_de_skr03.account_2282
+DEL account.account.template: l10n_de_skr03.account_2283
+DEL account.account.template: l10n_de_skr03.account_2284
+DEL account.account.template: l10n_de_skr03.account_2285
+DEL account.account.template: l10n_de_skr03.account_2287
+DEL account.account.template: l10n_de_skr03.account_2289
+DEL account.account.template: l10n_de_skr03.account_2300
+DEL account.account.template: l10n_de_skr03.account_2307
+DEL account.account.template: l10n_de_skr03.account_2308
+DEL account.account.template: l10n_de_skr03.account_2309
+DEL account.account.template: l10n_de_skr03.account_2310
+DEL account.account.template: l10n_de_skr03.account_2311
+DEL account.account.template: l10n_de_skr03.account_2312
+DEL account.account.template: l10n_de_skr03.account_2313
+DEL account.account.template: l10n_de_skr03.account_2315
+DEL account.account.template: l10n_de_skr03.account_2316
+DEL account.account.template: l10n_de_skr03.account_2317
+DEL account.account.template: l10n_de_skr03.account_2318
+DEL account.account.template: l10n_de_skr03.account_2320
+DEL account.account.template: l10n_de_skr03.account_2323
+DEL account.account.template: l10n_de_skr03.account_2325
+DEL account.account.template: l10n_de_skr03.account_2326
+DEL account.account.template: l10n_de_skr03.account_2327
+DEL account.account.template: l10n_de_skr03.account_2328
+DEL account.account.template: l10n_de_skr03.account_2339
+DEL account.account.template: l10n_de_skr03.account_2340
+DEL account.account.template: l10n_de_skr03.account_2341
+DEL account.account.template: l10n_de_skr03.account_2342
+DEL account.account.template: l10n_de_skr03.account_2344
+DEL account.account.template: l10n_de_skr03.account_2345
+DEL account.account.template: l10n_de_skr03.account_2347
+DEL account.account.template: l10n_de_skr03.account_2350
+DEL account.account.template: l10n_de_skr03.account_2375
+DEL account.account.template: l10n_de_skr03.account_2380
+DEL account.account.template: l10n_de_skr03.account_2381
+DEL account.account.template: l10n_de_skr03.account_2382
+DEL account.account.template: l10n_de_skr03.account_2383
+DEL account.account.template: l10n_de_skr03.account_2384
+DEL account.account.template: l10n_de_skr03.account_2385
+DEL account.account.template: l10n_de_skr03.account_2386
+DEL account.account.template: l10n_de_skr03.account_2387
+DEL account.account.template: l10n_de_skr03.account_2388
+DEL account.account.template: l10n_de_skr03.account_2389
+DEL account.account.template: l10n_de_skr03.account_2390
+DEL account.account.template: l10n_de_skr03.account_2400
+DEL account.account.template: l10n_de_skr03.account_2401
+DEL account.account.template: l10n_de_skr03.account_2402
+DEL account.account.template: l10n_de_skr03.account_2403
+DEL account.account.template: l10n_de_skr03.account_2406
+DEL account.account.template: l10n_de_skr03.account_2408
+DEL account.account.template: l10n_de_skr03.account_2430
+DEL account.account.template: l10n_de_skr03.account_2431
+DEL account.account.template: l10n_de_skr03.account_2436
+DEL account.account.template: l10n_de_skr03.account_2440
+DEL account.account.template: l10n_de_skr03.account_2441
+DEL account.account.template: l10n_de_skr03.account_2450
+DEL account.account.template: l10n_de_skr03.account_2451
+DEL account.account.template: l10n_de_skr03.account_2480
+DEL account.account.template: l10n_de_skr03.account_2481
+DEL account.account.template: l10n_de_skr03.account_2485
+DEL account.account.template: l10n_de_skr03.account_2490
+DEL account.account.template: l10n_de_skr03.account_2492
+DEL account.account.template: l10n_de_skr03.account_2493
+DEL account.account.template: l10n_de_skr03.account_2494
+DEL account.account.template: l10n_de_skr03.account_2498
+DEL account.account.template: l10n_de_skr03.account_2500
+DEL account.account.template: l10n_de_skr03.account_2501
+DEL account.account.template: l10n_de_skr03.account_2504
+DEL account.account.template: l10n_de_skr03.account_2505
+DEL account.account.template: l10n_de_skr03.account_2506
+DEL account.account.template: l10n_de_skr03.account_2507
+DEL account.account.template: l10n_de_skr03.account_2508
+DEL account.account.template: l10n_de_skr03.account_2510
+DEL account.account.template: l10n_de_skr03.account_2520
+DEL account.account.template: l10n_de_skr03.account_2590
+DEL account.account.template: l10n_de_skr03.account_2591
+DEL account.account.template: l10n_de_skr03.account_2592
+DEL account.account.template: l10n_de_skr03.account_2593
+DEL account.account.template: l10n_de_skr03.account_2594
+DEL account.account.template: l10n_de_skr03.account_2600
+DEL account.account.template: l10n_de_skr03.account_2603
+DEL account.account.template: l10n_de_skr03.account_2615
+DEL account.account.template: l10n_de_skr03.account_2616
+DEL account.account.template: l10n_de_skr03.account_2617
+DEL account.account.template: l10n_de_skr03.account_2618
+DEL account.account.template: l10n_de_skr03.account_2619
+DEL account.account.template: l10n_de_skr03.account_2620
+DEL account.account.template: l10n_de_skr03.account_2621
+DEL account.account.template: l10n_de_skr03.account_2622
+DEL account.account.template: l10n_de_skr03.account_2623
+DEL account.account.template: l10n_de_skr03.account_2625
+DEL account.account.template: l10n_de_skr03.account_2626
+DEL account.account.template: l10n_de_skr03.account_2640
+DEL account.account.template: l10n_de_skr03.account_2641
+DEL account.account.template: l10n_de_skr03.account_2646
+DEL account.account.template: l10n_de_skr03.account_2647
+DEL account.account.template: l10n_de_skr03.account_2648
+DEL account.account.template: l10n_de_skr03.account_2649
+DEL account.account.template: l10n_de_skr03.account_2650
+DEL account.account.template: l10n_de_skr03.account_2652
+DEL account.account.template: l10n_de_skr03.account_2653
+DEL account.account.template: l10n_de_skr03.account_2654
+DEL account.account.template: l10n_de_skr03.account_2655
+DEL account.account.template: l10n_de_skr03.account_2656
+DEL account.account.template: l10n_de_skr03.account_2657
+DEL account.account.template: l10n_de_skr03.account_2658
+DEL account.account.template: l10n_de_skr03.account_2659
+DEL account.account.template: l10n_de_skr03.account_2660
+DEL account.account.template: l10n_de_skr03.account_2661
+DEL account.account.template: l10n_de_skr03.account_2666
+DEL account.account.template: l10n_de_skr03.account_2670
+DEL account.account.template: l10n_de_skr03.account_2679
+DEL account.account.template: l10n_de_skr03.account_2680
+DEL account.account.template: l10n_de_skr03.account_2682
+DEL account.account.template: l10n_de_skr03.account_2683
+DEL account.account.template: l10n_de_skr03.account_2684
+DEL account.account.template: l10n_de_skr03.account_2685
+DEL account.account.template: l10n_de_skr03.account_2686
+DEL account.account.template: l10n_de_skr03.account_2687
+DEL account.account.template: l10n_de_skr03.account_2688
+DEL account.account.template: l10n_de_skr03.account_2689
+DEL account.account.template: l10n_de_skr03.account_2700
+DEL account.account.template: l10n_de_skr03.account_2705
+DEL account.account.template: l10n_de_skr03.account_2707
+DEL account.account.template: l10n_de_skr03.account_2709
+DEL account.account.template: l10n_de_skr03.account_2710
+DEL account.account.template: l10n_de_skr03.account_2711
+DEL account.account.template: l10n_de_skr03.account_2712
+DEL account.account.template: l10n_de_skr03.account_2713
+DEL account.account.template: l10n_de_skr03.account_2714
+DEL account.account.template: l10n_de_skr03.account_2715
+DEL account.account.template: l10n_de_skr03.account_2716
+DEL account.account.template: l10n_de_skr03.account_2720
+DEL account.account.template: l10n_de_skr03.account_2723
+DEL account.account.template: l10n_de_skr03.account_2725
+DEL account.account.template: l10n_de_skr03.account_2726
+DEL account.account.template: l10n_de_skr03.account_2727
+DEL account.account.template: l10n_de_skr03.account_2728
+DEL account.account.template: l10n_de_skr03.account_2729
+DEL account.account.template: l10n_de_skr03.account_2730
+DEL account.account.template: l10n_de_skr03.account_2731
+DEL account.account.template: l10n_de_skr03.account_2732
+DEL account.account.template: l10n_de_skr03.account_2733
+DEL account.account.template: l10n_de_skr03.account_2734
+DEL account.account.template: l10n_de_skr03.account_2735
+DEL account.account.template: l10n_de_skr03.account_2736
+DEL account.account.template: l10n_de_skr03.account_2738
+DEL account.account.template: l10n_de_skr03.account_2739
+DEL account.account.template: l10n_de_skr03.account_2740
+DEL account.account.template: l10n_de_skr03.account_2741
+DEL account.account.template: l10n_de_skr03.account_2742
+DEL account.account.template: l10n_de_skr03.account_2743
+DEL account.account.template: l10n_de_skr03.account_2744
+DEL account.account.template: l10n_de_skr03.account_2746
+DEL account.account.template: l10n_de_skr03.account_2747
+DEL account.account.template: l10n_de_skr03.account_2749
+DEL account.account.template: l10n_de_skr03.account_2750
+DEL account.account.template: l10n_de_skr03.account_2751
+DEL account.account.template: l10n_de_skr03.account_2752
+DEL account.account.template: l10n_de_skr03.account_2760
+DEL account.account.template: l10n_de_skr03.account_2762
+DEL account.account.template: l10n_de_skr03.account_2764
+DEL account.account.template: l10n_de_skr03.account_2790
+DEL account.account.template: l10n_de_skr03.account_2792
+DEL account.account.template: l10n_de_skr03.account_2794
+DEL account.account.template: l10n_de_skr03.account_2798
+DEL account.account.template: l10n_de_skr03.account_2840
+DEL account.account.template: l10n_de_skr03.account_2841
+DEL account.account.template: l10n_de_skr03.account_2850
+DEL account.account.template: l10n_de_skr03.account_2865
+DEL account.account.template: l10n_de_skr03.account_2867
+DEL account.account.template: l10n_de_skr03.account_2870
+DEL account.account.template: l10n_de_skr03.account_2890
+DEL account.account.template: l10n_de_skr03.account_2891
+DEL account.account.template: l10n_de_skr03.account_2892
+DEL account.account.template: l10n_de_skr03.account_2893
+DEL account.account.template: l10n_de_skr03.account_2894
+DEL account.account.template: l10n_de_skr03.account_2895
+DEL account.account.template: l10n_de_skr03.account_2990
+DEL account.account.template: l10n_de_skr03.account_3000
+DEL account.account.template: l10n_de_skr03.account_3010
+DEL account.account.template: l10n_de_skr03.account_3030
+DEL account.account.template: l10n_de_skr03.account_3060
+DEL account.account.template: l10n_de_skr03.account_3062
+DEL account.account.template: l10n_de_skr03.account_3066
+DEL account.account.template: l10n_de_skr03.account_3067
+DEL account.account.template: l10n_de_skr03.account_3070
+DEL account.account.template: l10n_de_skr03.account_3071
+DEL account.account.template: l10n_de_skr03.account_3075
+DEL account.account.template: l10n_de_skr03.account_3076
+DEL account.account.template: l10n_de_skr03.account_3089
+DEL account.account.template: l10n_de_skr03.account_3090
+DEL account.account.template: l10n_de_skr03.account_3091
+DEL account.account.template: l10n_de_skr03.account_3092
+DEL account.account.template: l10n_de_skr03.account_3100
+DEL account.account.template: l10n_de_skr03.account_3106
+DEL account.account.template: l10n_de_skr03.account_3108
+DEL account.account.template: l10n_de_skr03.account_3109
+DEL account.account.template: l10n_de_skr03.account_3110
+DEL account.account.template: l10n_de_skr03.account_3113
+DEL account.account.template: l10n_de_skr03.account_3115
+DEL account.account.template: l10n_de_skr03.account_3120
+DEL account.account.template: l10n_de_skr03.account_3123
+DEL account.account.template: l10n_de_skr03.account_3125
+DEL account.account.template: l10n_de_skr03.account_3130
+DEL account.account.template: l10n_de_skr03.account_3133
+DEL account.account.template: l10n_de_skr03.account_3135
+DEL account.account.template: l10n_de_skr03.account_3140
+DEL account.account.template: l10n_de_skr03.account_3143
+DEL account.account.template: l10n_de_skr03.account_3145
+DEL account.account.template: l10n_de_skr03.account_3150
+DEL account.account.template: l10n_de_skr03.account_3151
+DEL account.account.template: l10n_de_skr03.account_3153
+DEL account.account.template: l10n_de_skr03.account_3154
+DEL account.account.template: l10n_de_skr03.account_3160
+DEL account.account.template: l10n_de_skr03.account_3165
+DEL account.account.template: l10n_de_skr03.account_3170
+DEL account.account.template: l10n_de_skr03.account_3175
+DEL account.account.template: l10n_de_skr03.account_3180
+DEL account.account.template: l10n_de_skr03.account_3185
+DEL account.account.template: l10n_de_skr03.account_3200
+DEL account.account.template: l10n_de_skr03.account_3300
+DEL account.account.template: l10n_de_skr03.account_3349
+DEL account.account.template: l10n_de_skr03.account_3400
+DEL account.account.template: l10n_de_skr03.account_3420
+DEL account.account.template: l10n_de_skr03.account_3425
+DEL account.account.template: l10n_de_skr03.account_3430
+DEL account.account.template: l10n_de_skr03.account_3435
+DEL account.account.template: l10n_de_skr03.account_3440
+DEL account.account.template: l10n_de_skr03.account_3505
+DEL account.account.template: l10n_de_skr03.account_3540
+DEL account.account.template: l10n_de_skr03.account_3550
+DEL account.account.template: l10n_de_skr03.account_3551
+DEL account.account.template: l10n_de_skr03.account_3552
+DEL account.account.template: l10n_de_skr03.account_3553
+DEL account.account.template: l10n_de_skr03.account_3557
+DEL account.account.template: l10n_de_skr03.account_3558
+DEL account.account.template: l10n_de_skr03.account_3559
+DEL account.account.template: l10n_de_skr03.account_3560
+DEL account.account.template: l10n_de_skr03.account_3565
+DEL account.account.template: l10n_de_skr03.account_3600
+DEL account.account.template: l10n_de_skr03.account_3610
+DEL account.account.template: l10n_de_skr03.account_3660
+DEL account.account.template: l10n_de_skr03.account_3700
+DEL account.account.template: l10n_de_skr03.account_3701
+DEL account.account.template: l10n_de_skr03.account_3710
+DEL account.account.template: l10n_de_skr03.account_3714
+DEL account.account.template: l10n_de_skr03.account_3715
+DEL account.account.template: l10n_de_skr03.account_3717
+DEL account.account.template: l10n_de_skr03.account_3718
+DEL account.account.template: l10n_de_skr03.account_3720
+DEL account.account.template: l10n_de_skr03.account_3724
+DEL account.account.template: l10n_de_skr03.account_3725
+DEL account.account.template: l10n_de_skr03.account_3730
+DEL account.account.template: l10n_de_skr03.account_3731
+DEL account.account.template: l10n_de_skr03.account_3733
+DEL account.account.template: l10n_de_skr03.account_3734
+DEL account.account.template: l10n_de_skr03.account_3736
+DEL account.account.template: l10n_de_skr03.account_3738
+DEL account.account.template: l10n_de_skr03.account_3741
+DEL account.account.template: l10n_de_skr03.account_3743
+DEL account.account.template: l10n_de_skr03.account_3744
+DEL account.account.template: l10n_de_skr03.account_3745
+DEL account.account.template: l10n_de_skr03.account_3746
+DEL account.account.template: l10n_de_skr03.account_3748
+DEL account.account.template: l10n_de_skr03.account_3750
+DEL account.account.template: l10n_de_skr03.account_3753
+DEL account.account.template: l10n_de_skr03.account_3754
+DEL account.account.template: l10n_de_skr03.account_3755
+DEL account.account.template: l10n_de_skr03.account_3760
+DEL account.account.template: l10n_de_skr03.account_3769
+DEL account.account.template: l10n_de_skr03.account_3770
+DEL account.account.template: l10n_de_skr03.account_3780
+DEL account.account.template: l10n_de_skr03.account_3783
+DEL account.account.template: l10n_de_skr03.account_3784
+DEL account.account.template: l10n_de_skr03.account_3785
+DEL account.account.template: l10n_de_skr03.account_3788
+DEL account.account.template: l10n_de_skr03.account_3790
+DEL account.account.template: l10n_de_skr03.account_3792
+DEL account.account.template: l10n_de_skr03.account_3793
+DEL account.account.template: l10n_de_skr03.account_3794
+DEL account.account.template: l10n_de_skr03.account_3796
+DEL account.account.template: l10n_de_skr03.account_3798
+DEL account.account.template: l10n_de_skr03.account_3800
+DEL account.account.template: l10n_de_skr03.account_3830
+DEL account.account.template: l10n_de_skr03.account_3850
+DEL account.account.template: l10n_de_skr03.account_3950
+DEL account.account.template: l10n_de_skr03.account_3955
+DEL account.account.template: l10n_de_skr03.account_3960
+DEL account.account.template: l10n_de_skr03.account_3970
+DEL account.account.template: l10n_de_skr03.account_3980
+DEL account.account.template: l10n_de_skr03.account_4100
+DEL account.account.template: l10n_de_skr03.account_4110
+DEL account.account.template: l10n_de_skr03.account_4120
+DEL account.account.template: l10n_de_skr03.account_4124
+DEL account.account.template: l10n_de_skr03.account_4125
+DEL account.account.template: l10n_de_skr03.account_4126
+DEL account.account.template: l10n_de_skr03.account_4127
+DEL account.account.template: l10n_de_skr03.account_4128
+DEL account.account.template: l10n_de_skr03.account_4129
+DEL account.account.template: l10n_de_skr03.account_4130
+DEL account.account.template: l10n_de_skr03.account_4137
+DEL account.account.template: l10n_de_skr03.account_4138
+DEL account.account.template: l10n_de_skr03.account_4139
+DEL account.account.template: l10n_de_skr03.account_4140
+DEL account.account.template: l10n_de_skr03.account_4141
+DEL account.account.template: l10n_de_skr03.account_4144
+DEL account.account.template: l10n_de_skr03.account_4145
+DEL account.account.template: l10n_de_skr03.account_4146
+DEL account.account.template: l10n_de_skr03.account_4147
+DEL account.account.template: l10n_de_skr03.account_4148
+DEL account.account.template: l10n_de_skr03.account_4149
+DEL account.account.template: l10n_de_skr03.account_4150
+DEL account.account.template: l10n_de_skr03.account_4151
+DEL account.account.template: l10n_de_skr03.account_4152
+DEL account.account.template: l10n_de_skr03.account_4153
+DEL account.account.template: l10n_de_skr03.account_4154
+DEL account.account.template: l10n_de_skr03.account_4155
+DEL account.account.template: l10n_de_skr03.account_4156
+DEL account.account.template: l10n_de_skr03.account_4157
+DEL account.account.template: l10n_de_skr03.account_4158
+DEL account.account.template: l10n_de_skr03.account_4159
+DEL account.account.template: l10n_de_skr03.account_4160
+DEL account.account.template: l10n_de_skr03.account_4165
+DEL account.account.template: l10n_de_skr03.account_4166
+DEL account.account.template: l10n_de_skr03.account_4167
+DEL account.account.template: l10n_de_skr03.account_4168
+DEL account.account.template: l10n_de_skr03.account_4169
+DEL account.account.template: l10n_de_skr03.account_4170
+DEL account.account.template: l10n_de_skr03.account_4175
+DEL account.account.template: l10n_de_skr03.account_4180
+DEL account.account.template: l10n_de_skr03.account_4190
+DEL account.account.template: l10n_de_skr03.account_4194
+DEL account.account.template: l10n_de_skr03.account_4195
+DEL account.account.template: l10n_de_skr03.account_4196
+DEL account.account.template: l10n_de_skr03.account_4197
+DEL account.account.template: l10n_de_skr03.account_4198
+DEL account.account.template: l10n_de_skr03.account_4199
+DEL account.account.template: l10n_de_skr03.account_4200
+DEL account.account.template: l10n_de_skr03.account_4210
+DEL account.account.template: l10n_de_skr03.account_4211
+DEL account.account.template: l10n_de_skr03.account_4212
+DEL account.account.template: l10n_de_skr03.account_4215
+DEL account.account.template: l10n_de_skr03.account_4219
+DEL account.account.template: l10n_de_skr03.account_4220
+DEL account.account.template: l10n_de_skr03.account_4222
+DEL account.account.template: l10n_de_skr03.account_4228
+DEL account.account.template: l10n_de_skr03.account_4229
+DEL account.account.template: l10n_de_skr03.account_4230
+DEL account.account.template: l10n_de_skr03.account_4240
+DEL account.account.template: l10n_de_skr03.account_4250
+DEL account.account.template: l10n_de_skr03.account_4260
+DEL account.account.template: l10n_de_skr03.account_4270
+DEL account.account.template: l10n_de_skr03.account_4280
+DEL account.account.template: l10n_de_skr03.account_4288
+DEL account.account.template: l10n_de_skr03.account_4289
+DEL account.account.template: l10n_de_skr03.account_4290
+DEL account.account.template: l10n_de_skr03.account_4300
+DEL account.account.template: l10n_de_skr03.account_4301
+DEL account.account.template: l10n_de_skr03.account_4306
+DEL account.account.template: l10n_de_skr03.account_4320
+DEL account.account.template: l10n_de_skr03.account_4340
+DEL account.account.template: l10n_de_skr03.account_4350
+DEL account.account.template: l10n_de_skr03.account_4355
+DEL account.account.template: l10n_de_skr03.account_4360
+DEL account.account.template: l10n_de_skr03.account_4366
+DEL account.account.template: l10n_de_skr03.account_4370
+DEL account.account.template: l10n_de_skr03.account_4380
+DEL account.account.template: l10n_de_skr03.account_4390
+DEL account.account.template: l10n_de_skr03.account_4396
+DEL account.account.template: l10n_de_skr03.account_4397
+DEL account.account.template: l10n_de_skr03.account_4500
+DEL account.account.template: l10n_de_skr03.account_4510
+DEL account.account.template: l10n_de_skr03.account_4520
+DEL account.account.template: l10n_de_skr03.account_4530
+DEL account.account.template: l10n_de_skr03.account_4540
+DEL account.account.template: l10n_de_skr03.account_4550
+DEL account.account.template: l10n_de_skr03.account_4560
+DEL account.account.template: l10n_de_skr03.account_4570
+DEL account.account.template: l10n_de_skr03.account_4580
+DEL account.account.template: l10n_de_skr03.account_4590
+DEL account.account.template: l10n_de_skr03.account_4595
+DEL account.account.template: l10n_de_skr03.account_4600
+DEL account.account.template: l10n_de_skr03.account_4605
+DEL account.account.template: l10n_de_skr03.account_4630
+DEL account.account.template: l10n_de_skr03.account_4631
+DEL account.account.template: l10n_de_skr03.account_4632
+DEL account.account.template: l10n_de_skr03.account_4633
+DEL account.account.template: l10n_de_skr03.account_4635
+DEL account.account.template: l10n_de_skr03.account_4636
+DEL account.account.template: l10n_de_skr03.account_4637
+DEL account.account.template: l10n_de_skr03.account_4638
+DEL account.account.template: l10n_de_skr03.account_4639
+DEL account.account.template: l10n_de_skr03.account_4640
+DEL account.account.template: l10n_de_skr03.account_4650
+DEL account.account.template: l10n_de_skr03.account_4651
+DEL account.account.template: l10n_de_skr03.account_4652
+DEL account.account.template: l10n_de_skr03.account_4653
+DEL account.account.template: l10n_de_skr03.account_4654
+DEL account.account.template: l10n_de_skr03.account_4655
+DEL account.account.template: l10n_de_skr03.account_4660
+DEL account.account.template: l10n_de_skr03.account_4663
+DEL account.account.template: l10n_de_skr03.account_4664
+DEL account.account.template: l10n_de_skr03.account_4666
+DEL account.account.template: l10n_de_skr03.account_4668
+DEL account.account.template: l10n_de_skr03.account_4670
+DEL account.account.template: l10n_de_skr03.account_4672
+DEL account.account.template: l10n_de_skr03.account_4673
+DEL account.account.template: l10n_de_skr03.account_4674
+DEL account.account.template: l10n_de_skr03.account_4676
+DEL account.account.template: l10n_de_skr03.account_4678
+DEL account.account.template: l10n_de_skr03.account_4679
+DEL account.account.template: l10n_de_skr03.account_4680
+DEL account.account.template: l10n_de_skr03.account_4681
+DEL account.account.template: l10n_de_skr03.account_4700
+DEL account.account.template: l10n_de_skr03.account_4710
+DEL account.account.template: l10n_de_skr03.account_4730
+DEL account.account.template: l10n_de_skr03.account_4750
+DEL account.account.template: l10n_de_skr03.account_4760
+DEL account.account.template: l10n_de_skr03.account_4780
+DEL account.account.template: l10n_de_skr03.account_4790
+DEL account.account.template: l10n_de_skr03.account_4800
+DEL account.account.template: l10n_de_skr03.account_4801
+DEL account.account.template: l10n_de_skr03.account_4805
+DEL account.account.template: l10n_de_skr03.account_4806
+DEL account.account.template: l10n_de_skr03.account_4808
+DEL account.account.template: l10n_de_skr03.account_4809
+DEL account.account.template: l10n_de_skr03.account_4810
+DEL account.account.template: l10n_de_skr03.account_4815
+DEL account.account.template: l10n_de_skr03.account_4820
+DEL account.account.template: l10n_de_skr03.account_4822
+DEL account.account.template: l10n_de_skr03.account_4823
+DEL account.account.template: l10n_de_skr03.account_4824
+DEL account.account.template: l10n_de_skr03.account_4825
+DEL account.account.template: l10n_de_skr03.account_4826
+DEL account.account.template: l10n_de_skr03.account_4827
+DEL account.account.template: l10n_de_skr03.account_4830
+DEL account.account.template: l10n_de_skr03.account_4831
+DEL account.account.template: l10n_de_skr03.account_4832
+DEL account.account.template: l10n_de_skr03.account_4833
+DEL account.account.template: l10n_de_skr03.account_4840
+DEL account.account.template: l10n_de_skr03.account_4841
+DEL account.account.template: l10n_de_skr03.account_4842
+DEL account.account.template: l10n_de_skr03.account_4843
+DEL account.account.template: l10n_de_skr03.account_4850
+DEL account.account.template: l10n_de_skr03.account_4851
+DEL account.account.template: l10n_de_skr03.account_4852
+DEL account.account.template: l10n_de_skr03.account_4853
+DEL account.account.template: l10n_de_skr03.account_4854
+DEL account.account.template: l10n_de_skr03.account_4855
+DEL account.account.template: l10n_de_skr03.account_4860
+DEL account.account.template: l10n_de_skr03.account_4862
+DEL account.account.template: l10n_de_skr03.account_4865
+DEL account.account.template: l10n_de_skr03.account_4866
+DEL account.account.template: l10n_de_skr03.account_4870
+DEL account.account.template: l10n_de_skr03.account_4871
+DEL account.account.template: l10n_de_skr03.account_4872
+DEL account.account.template: l10n_de_skr03.account_4873
+DEL account.account.template: l10n_de_skr03.account_4874
+DEL account.account.template: l10n_de_skr03.account_4875
+DEL account.account.template: l10n_de_skr03.account_4876
+DEL account.account.template: l10n_de_skr03.account_4877
+DEL account.account.template: l10n_de_skr03.account_4878
+DEL account.account.template: l10n_de_skr03.account_4880
+DEL account.account.template: l10n_de_skr03.account_4882
+DEL account.account.template: l10n_de_skr03.account_4886
+DEL account.account.template: l10n_de_skr03.account_4887
+DEL account.account.template: l10n_de_skr03.account_4892
+DEL account.account.template: l10n_de_skr03.account_4893
+DEL account.account.template: l10n_de_skr03.account_4900
+DEL account.account.template: l10n_de_skr03.account_4902
+DEL account.account.template: l10n_de_skr03.account_4905
+DEL account.account.template: l10n_de_skr03.account_4909
+DEL account.account.template: l10n_de_skr03.account_4910
+DEL account.account.template: l10n_de_skr03.account_4920
+DEL account.account.template: l10n_de_skr03.account_4925
+DEL account.account.template: l10n_de_skr03.account_4930
+DEL account.account.template: l10n_de_skr03.account_4940
+DEL account.account.template: l10n_de_skr03.account_4945
+DEL account.account.template: l10n_de_skr03.account_4946
+DEL account.account.template: l10n_de_skr03.account_4948
+DEL account.account.template: l10n_de_skr03.account_4949
+DEL account.account.template: l10n_de_skr03.account_4950
+DEL account.account.template: l10n_de_skr03.account_4955
+DEL account.account.template: l10n_de_skr03.account_4957
+DEL account.account.template: l10n_de_skr03.account_4958
+DEL account.account.template: l10n_de_skr03.account_4959
+DEL account.account.template: l10n_de_skr03.account_4960
+DEL account.account.template: l10n_de_skr03.account_4961
+DEL account.account.template: l10n_de_skr03.account_4963
+DEL account.account.template: l10n_de_skr03.account_4964
+DEL account.account.template: l10n_de_skr03.account_4965
+DEL account.account.template: l10n_de_skr03.account_4969
+DEL account.account.template: l10n_de_skr03.account_4970
+DEL account.account.template: l10n_de_skr03.account_4975
+DEL account.account.template: l10n_de_skr03.account_4976
+DEL account.account.template: l10n_de_skr03.account_4980
+DEL account.account.template: l10n_de_skr03.account_4984
+DEL account.account.template: l10n_de_skr03.account_4985
+DEL account.account.template: l10n_de_skr03.account_4990
+DEL account.account.template: l10n_de_skr03.account_4991
+DEL account.account.template: l10n_de_skr03.account_4992
+DEL account.account.template: l10n_de_skr03.account_4993
+DEL account.account.template: l10n_de_skr03.account_4994
+DEL account.account.template: l10n_de_skr03.account_4995
+DEL account.account.template: l10n_de_skr03.account_4996
+DEL account.account.template: l10n_de_skr03.account_4997
+DEL account.account.template: l10n_de_skr03.account_4998
+DEL account.account.template: l10n_de_skr03.account_4999
+DEL account.account.template: l10n_de_skr03.account_7000
+DEL account.account.template: l10n_de_skr03.account_7050
+DEL account.account.template: l10n_de_skr03.account_7080
+DEL account.account.template: l10n_de_skr03.account_7090
+DEL account.account.template: l10n_de_skr03.account_7095
+DEL account.account.template: l10n_de_skr03.account_7100
+DEL account.account.template: l10n_de_skr03.account_7110
+DEL account.account.template: l10n_de_skr03.account_7140
+DEL account.account.template: l10n_de_skr03.account_7200
+DEL account.account.template: l10n_de_skr03.account_8100
+DEL account.account.template: l10n_de_skr03.account_8105
+DEL account.account.template: l10n_de_skr03.account_8110
+DEL account.account.template: l10n_de_skr03.account_8120
+DEL account.account.template: l10n_de_skr03.account_8125
+DEL account.account.template: l10n_de_skr03.account_8130
+DEL account.account.template: l10n_de_skr03.account_8135
+DEL account.account.template: l10n_de_skr03.account_8140
+DEL account.account.template: l10n_de_skr03.account_8150
+DEL account.account.template: l10n_de_skr03.account_8160
+DEL account.account.template: l10n_de_skr03.account_8165
+DEL account.account.template: l10n_de_skr03.account_8190
+DEL account.account.template: l10n_de_skr03.account_8191
+DEL account.account.template: l10n_de_skr03.account_8193
+DEL account.account.template: l10n_de_skr03.account_8194
+DEL account.account.template: l10n_de_skr03.account_8195
+DEL account.account.template: l10n_de_skr03.account_8196
+DEL account.account.template: l10n_de_skr03.account_8200
+DEL account.account.template: l10n_de_skr03.account_8300
+DEL account.account.template: l10n_de_skr03.account_8310
+DEL account.account.template: l10n_de_skr03.account_8315
+DEL account.account.template: l10n_de_skr03.account_8320
+DEL account.account.template: l10n_de_skr03.account_8331
+DEL account.account.template: l10n_de_skr03.account_8335
+DEL account.account.template: l10n_de_skr03.account_8336
+DEL account.account.template: l10n_de_skr03.account_8337
+DEL account.account.template: l10n_de_skr03.account_8338
+DEL account.account.template: l10n_de_skr03.account_8339
+DEL account.account.template: l10n_de_skr03.account_8400
+DEL account.account.template: l10n_de_skr03.account_8410
+DEL account.account.template: l10n_de_skr03.account_8499
+DEL account.account.template: l10n_de_skr03.account_8500
+DEL account.account.template: l10n_de_skr03.account_8501
+DEL account.account.template: l10n_de_skr03.account_8502
+DEL account.account.template: l10n_de_skr03.account_8503
+DEL account.account.template: l10n_de_skr03.account_8504
+DEL account.account.template: l10n_de_skr03.account_8505
+DEL account.account.template: l10n_de_skr03.account_8510
+DEL account.account.template: l10n_de_skr03.account_8514
+DEL account.account.template: l10n_de_skr03.account_8515
+DEL account.account.template: l10n_de_skr03.account_8516
+DEL account.account.template: l10n_de_skr03.account_8519
+DEL account.account.template: l10n_de_skr03.account_8520
+DEL account.account.template: l10n_de_skr03.account_8540
+DEL account.account.template: l10n_de_skr03.account_8570
+DEL account.account.template: l10n_de_skr03.account_8574
+DEL account.account.template: l10n_de_skr03.account_8575
+DEL account.account.template: l10n_de_skr03.account_8576
+DEL account.account.template: l10n_de_skr03.account_8579
+DEL account.account.template: l10n_de_skr03.account_8589
+DEL account.account.template: l10n_de_skr03.account_8590
+DEL account.account.template: l10n_de_skr03.account_8591
+DEL account.account.template: l10n_de_skr03.account_8595
+DEL account.account.template: l10n_de_skr03.account_8600
+DEL account.account.template: l10n_de_skr03.account_8603
+DEL account.account.template: l10n_de_skr03.account_8604
+DEL account.account.template: l10n_de_skr03.account_8605
+DEL account.account.template: l10n_de_skr03.account_8606
+DEL account.account.template: l10n_de_skr03.account_8607
+DEL account.account.template: l10n_de_skr03.account_8609
+DEL account.account.template: l10n_de_skr03.account_8610
+DEL account.account.template: l10n_de_skr03.account_8611
+DEL account.account.template: l10n_de_skr03.account_8613
+DEL account.account.template: l10n_de_skr03.account_8614
+DEL account.account.template: l10n_de_skr03.account_8625
+DEL account.account.template: l10n_de_skr03.account_8630
+DEL account.account.template: l10n_de_skr03.account_8640
+DEL account.account.template: l10n_de_skr03.account_8650
+DEL account.account.template: l10n_de_skr03.account_8660
+DEL account.account.template: l10n_de_skr03.account_8700
+DEL account.account.template: l10n_de_skr03.account_8701
+DEL account.account.template: l10n_de_skr03.account_8702
+DEL account.account.template: l10n_de_skr03.account_8703
+DEL account.account.template: l10n_de_skr03.account_8704
+DEL account.account.template: l10n_de_skr03.account_8705
+DEL account.account.template: l10n_de_skr03.account_8710
+DEL account.account.template: l10n_de_skr03.account_8720
+DEL account.account.template: l10n_de_skr03.account_8724
+DEL account.account.template: l10n_de_skr03.account_8725
+DEL account.account.template: l10n_de_skr03.account_8726
+DEL account.account.template: l10n_de_skr03.account_8727
+DEL account.account.template: l10n_de_skr03.account_8730
+DEL account.account.template: l10n_de_skr03.account_8731
+DEL account.account.template: l10n_de_skr03.account_8736
+DEL account.account.template: l10n_de_skr03.account_8738
+DEL account.account.template: l10n_de_skr03.account_8741
+DEL account.account.template: l10n_de_skr03.account_8742
+DEL account.account.template: l10n_de_skr03.account_8743
+DEL account.account.template: l10n_de_skr03.account_8745
+DEL account.account.template: l10n_de_skr03.account_8746
+DEL account.account.template: l10n_de_skr03.account_8748
+DEL account.account.template: l10n_de_skr03.account_8750
+DEL account.account.template: l10n_de_skr03.account_8760
+DEL account.account.template: l10n_de_skr03.account_8769
+DEL account.account.template: l10n_de_skr03.account_8770
+DEL account.account.template: l10n_de_skr03.account_8780
+DEL account.account.template: l10n_de_skr03.account_8790
+DEL account.account.template: l10n_de_skr03.account_8800
+DEL account.account.template: l10n_de_skr03.account_8801
+DEL account.account.template: l10n_de_skr03.account_8807
+DEL account.account.template: l10n_de_skr03.account_8808
+DEL account.account.template: l10n_de_skr03.account_8817
+DEL account.account.template: l10n_de_skr03.account_8818
+DEL account.account.template: l10n_de_skr03.account_8819
+DEL account.account.template: l10n_de_skr03.account_8820
+DEL account.account.template: l10n_de_skr03.account_8827
+DEL account.account.template: l10n_de_skr03.account_8828
+DEL account.account.template: l10n_de_skr03.account_8829
+DEL account.account.template: l10n_de_skr03.account_8837
+DEL account.account.template: l10n_de_skr03.account_8838
+DEL account.account.template: l10n_de_skr03.account_8839
+DEL account.account.template: l10n_de_skr03.account_8850
+DEL account.account.template: l10n_de_skr03.account_8851
+DEL account.account.template: l10n_de_skr03.account_8852
+DEL account.account.template: l10n_de_skr03.account_8853
+DEL account.account.template: l10n_de_skr03.account_8900
+DEL account.account.template: l10n_de_skr03.account_8905
+DEL account.account.template: l10n_de_skr03.account_8906
+DEL account.account.template: l10n_de_skr03.account_8910
+DEL account.account.template: l10n_de_skr03.account_8915
+DEL account.account.template: l10n_de_skr03.account_8918
+DEL account.account.template: l10n_de_skr03.account_8919
+DEL account.account.template: l10n_de_skr03.account_8920
+DEL account.account.template: l10n_de_skr03.account_8921
+DEL account.account.template: l10n_de_skr03.account_8922
+DEL account.account.template: l10n_de_skr03.account_8924
+DEL account.account.template: l10n_de_skr03.account_8925
+DEL account.account.template: l10n_de_skr03.account_8929
+DEL account.account.template: l10n_de_skr03.account_8930
+DEL account.account.template: l10n_de_skr03.account_8932
+DEL account.account.template: l10n_de_skr03.account_8935
+DEL account.account.template: l10n_de_skr03.account_8939
+DEL account.account.template: l10n_de_skr03.account_8940
+DEL account.account.template: l10n_de_skr03.account_8945
+DEL account.account.template: l10n_de_skr03.account_8949
+DEL account.account.template: l10n_de_skr03.account_8950
+DEL account.account.template: l10n_de_skr03.account_8955
+DEL account.account.template: l10n_de_skr03.account_8959
+DEL account.account.template: l10n_de_skr03.account_8960
+DEL account.account.template: l10n_de_skr03.account_8970
+DEL account.account.template: l10n_de_skr03.account_8975
+DEL account.account.template: l10n_de_skr03.account_8977
+DEL account.account.template: l10n_de_skr03.account_8980
+DEL account.account.template: l10n_de_skr03.account_8990
+DEL account.account.template: l10n_de_skr03.account_8994
+DEL account.account.template: l10n_de_skr03.account_8995
+DEL account.account.template: l10n_de_skr03.account_9000
+DEL account.account.template: l10n_de_skr03.account_9001
+DEL account.account.template: l10n_de_skr03.account_9008
+DEL account.account.template: l10n_de_skr03.account_9009
+DEL account.account.template: l10n_de_skr03.account_9089
+DEL account.account.template: l10n_de_skr03.account_9090
+DEL account.chart.template: l10n_de_skr03.l10n_de_chart_template
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_no_id_partner_19a_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_no_id_partner_19b_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_no_id_partner_7b_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_no_id_partner_afa7a_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_partner_19b_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_partner_afa19a_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_partner_afa7a_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_partner_afa7b_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_purchase_service_19_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_purchase_service_7_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_non_eu_purchase_services_19_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_no_id_purchase_19_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_no_id_sale_19_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_vat_id_purchase_19_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_vat_id_purchase_7_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_vat_id_sale_19_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_vat_id_sale_7_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_no_id_purchase_7_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_no_id_sale_7_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_purchase_19_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_purchase_7_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_sale_19_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_sale_7_skr03
+DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_sale_services_19_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_no_id_purchase_19_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_no_id_purchase_7_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_no_id_sale_19_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_purchase_19_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_purchase_7_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_purchase_services_19_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_purchase_services_7_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_sale_19_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_sale_7_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_purchase_19_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_purchase_7_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_purchase_services_19_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_sale_19_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_sale_7_skr03
+DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_sale_services_19_skr03
+DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_domestic_skr03
+DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_eu_no_id_partner_skr03
+DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_eu_vat_id_partner_service_skr03
+DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_eu_vat_id_partner_skr03
+DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_non_eu_partner_service_skr03
+DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_non_eu_partner_skr03
+DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_2401_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_2406_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_3731_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_3736_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_8731_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_8736_line (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr03.reconcile_2401 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr03.reconcile_2406 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr03.reconcile_3731 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr03.reconcile_3736 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr03.reconcile_8731 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr03.reconcile_8736 (noupdate)
+DEL account.tax.group: l10n_de_skr03.tax_group_0 (noupdate)
+DEL account.tax.group: l10n_de_skr03.tax_group_107 (noupdate)
+DEL account.tax.group: l10n_de_skr03.tax_group_19 (noupdate)
+DEL account.tax.group: l10n_de_skr03.tax_group_55 (noupdate)
+DEL account.tax.group: l10n_de_skr03.tax_group_7 (noupdate)
+DEL account.tax.group: l10n_de_skr03.tax_group_x (noupdate)
+DEL account.tax.template: l10n_de_skr03.tax_eu_19_purchase_goods_skr03
+DEL account.tax.template: l10n_de_skr03.tax_eu_19_purchase_no_vst_skr03
+DEL account.tax.template: l10n_de_skr03.tax_eu_19_purchase_skr03
+DEL account.tax.template: l10n_de_skr03.tax_eu_7_purchase_goods_skr03
+DEL account.tax.template: l10n_de_skr03.tax_eu_7_purchase_no_vst_skr03
+DEL account.tax.template: l10n_de_skr03.tax_eu_7_purchase_skr03
+DEL account.tax.template: l10n_de_skr03.tax_eu_car_purchase_skr03
+DEL account.tax.template: l10n_de_skr03.tax_eu_purchase_tax_free_skr03
+DEL account.tax.template: l10n_de_skr03.tax_eu_sale_skr03
+DEL account.tax.template: l10n_de_skr03.tax_export_skr03
+DEL account.tax.template: l10n_de_skr03.tax_free_eu_skr03
+DEL account.tax.template: l10n_de_skr03.tax_free_newcar_skr03
+DEL account.tax.template: l10n_de_skr03.tax_free_skr03_mit_vst
+DEL account.tax.template: l10n_de_skr03.tax_free_skr03_ohne_vst
+DEL account.tax.template: l10n_de_skr03.tax_free_third_country_skr03
+DEL account.tax.template: l10n_de_skr03.tax_import_19_and_payable_skr03
+DEL account.tax.template: l10n_de_skr03.tax_import_7_and_payable_skr03
+DEL account.tax.template: l10n_de_skr03.tax_not_taxable_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_107_farmer_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_19_13b_ausland_ohne_vst_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_19_13b_bau_ohne_vst_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_19_13b_eu_ohne_vst_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_19_3eck_first_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_19_eu_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_19_farmer_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_19_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_19_taxinclusive_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_55_farmer_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_7_13b_ausland_ohne_vst_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_7_13b_bau_ohne_vst_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_7_13b_eu_ohne_vst_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_7_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_7_taxinclusive_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_eu_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_free_bau_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_free_mobil_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_no_ustpflicht_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_vst_19_purchase_13b_bau_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_vst_7_purchase_13b_bau_skr03
+DEL account.tax.template: l10n_de_skr03.tax_ust_x_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_107_farmer_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_19_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_19_taxinclusive_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_55_farmer_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_7_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_7_taxinclusive_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_no_ustpflicht_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_ust_19_purchase_13a_auslagerung_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_ust_19_purchase_13b_mobil_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_ust_19_purchase_13b_werk_ausland_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_ust_19_purchase_3eck_last_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_ust_7_purchase_13a_auslagerung_skr03
+DEL account.tax.template: l10n_de_skr03.tax_vst_ust_7_purchase_13b_werk_ausland_skr03
+ERROR: module not in list of installed modules:
+---Models in module 'l10n_de_skr04'---
+---Fields in module 'l10n_de_skr04'---
+---XML records in module 'l10n_de_skr04'---
+DEL account.account.template: l10n_de_skr04.chart_skr04_100
+DEL account.account.template: l10n_de_skr04.chart_skr04_1000
+DEL account.account.template: l10n_de_skr04.chart_skr04_1040
+DEL account.account.template: l10n_de_skr04.chart_skr04_1050
+DEL account.account.template: l10n_de_skr04.chart_skr04_1080
+DEL account.account.template: l10n_de_skr04.chart_skr04_1090
+DEL account.account.template: l10n_de_skr04.chart_skr04_1095
+DEL account.account.template: l10n_de_skr04.chart_skr04_110
+DEL account.account.template: l10n_de_skr04.chart_skr04_1100
+DEL account.account.template: l10n_de_skr04.chart_skr04_1110
+DEL account.account.template: l10n_de_skr04.chart_skr04_1140
+DEL account.account.template: l10n_de_skr04.chart_skr04_1180
+DEL account.account.template: l10n_de_skr04.chart_skr04_1181
+DEL account.account.template: l10n_de_skr04.chart_skr04_1186
+DEL account.account.template: l10n_de_skr04.chart_skr04_1190
+DEL account.account.template: l10n_de_skr04.chart_skr04_120
+DEL account.account.template: l10n_de_skr04.chart_skr04_1200
+DEL account.account.template: l10n_de_skr04.chart_skr04_1205
+DEL account.account.template: l10n_de_skr04.chart_skr04_1206
+DEL account.account.template: l10n_de_skr04.chart_skr04_1210
+DEL account.account.template: l10n_de_skr04.chart_skr04_1215
+DEL account.account.template: l10n_de_skr04.chart_skr04_1216
+DEL account.account.template: l10n_de_skr04.chart_skr04_1217
+DEL account.account.template: l10n_de_skr04.chart_skr04_1218
+DEL account.account.template: l10n_de_skr04.chart_skr04_1219
+DEL account.account.template: l10n_de_skr04.chart_skr04_1220
+DEL account.account.template: l10n_de_skr04.chart_skr04_1221
+DEL account.account.template: l10n_de_skr04.chart_skr04_1225
+DEL account.account.template: l10n_de_skr04.chart_skr04_1230
+DEL account.account.template: l10n_de_skr04.chart_skr04_1231
+DEL account.account.template: l10n_de_skr04.chart_skr04_1232
+DEL account.account.template: l10n_de_skr04.chart_skr04_1235
+DEL account.account.template: l10n_de_skr04.chart_skr04_1240
+DEL account.account.template: l10n_de_skr04.chart_skr04_1241
+DEL account.account.template: l10n_de_skr04.chart_skr04_1245
+DEL account.account.template: l10n_de_skr04.chart_skr04_1246
+DEL account.account.template: l10n_de_skr04.chart_skr04_1247
+DEL account.account.template: l10n_de_skr04.chart_skr04_1248
+DEL account.account.template: l10n_de_skr04.chart_skr04_1249
+DEL account.account.template: l10n_de_skr04.chart_skr04_1250
+DEL account.account.template: l10n_de_skr04.chart_skr04_1251
+DEL account.account.template: l10n_de_skr04.chart_skr04_1255
+DEL account.account.template: l10n_de_skr04.chart_skr04_1260
+DEL account.account.template: l10n_de_skr04.chart_skr04_1261
+DEL account.account.template: l10n_de_skr04.chart_skr04_1265
+DEL account.account.template: l10n_de_skr04.chart_skr04_1266
+DEL account.account.template: l10n_de_skr04.chart_skr04_1267
+DEL account.account.template: l10n_de_skr04.chart_skr04_1268
+DEL account.account.template: l10n_de_skr04.chart_skr04_1269
+DEL account.account.template: l10n_de_skr04.chart_skr04_1270
+DEL account.account.template: l10n_de_skr04.chart_skr04_1271
+DEL account.account.template: l10n_de_skr04.chart_skr04_1275
+DEL account.account.template: l10n_de_skr04.chart_skr04_1276
+DEL account.account.template: l10n_de_skr04.chart_skr04_1277
+DEL account.account.template: l10n_de_skr04.chart_skr04_1280
+DEL account.account.template: l10n_de_skr04.chart_skr04_1281
+DEL account.account.template: l10n_de_skr04.chart_skr04_1285
+DEL account.account.template: l10n_de_skr04.chart_skr04_1286
+DEL account.account.template: l10n_de_skr04.chart_skr04_1287
+DEL account.account.template: l10n_de_skr04.chart_skr04_1288
+DEL account.account.template: l10n_de_skr04.chart_skr04_1289
+DEL account.account.template: l10n_de_skr04.chart_skr04_1290
+DEL account.account.template: l10n_de_skr04.chart_skr04_1291
+DEL account.account.template: l10n_de_skr04.chart_skr04_1295
+DEL account.account.template: l10n_de_skr04.chart_skr04_1296
+DEL account.account.template: l10n_de_skr04.chart_skr04_1297
+DEL account.account.template: l10n_de_skr04.chart_skr04_1298
+DEL account.account.template: l10n_de_skr04.chart_skr04_1299
+DEL account.account.template: l10n_de_skr04.chart_skr04_130
+DEL account.account.template: l10n_de_skr04.chart_skr04_1300
+DEL account.account.template: l10n_de_skr04.chart_skr04_1301
+DEL account.account.template: l10n_de_skr04.chart_skr04_1305
+DEL account.account.template: l10n_de_skr04.chart_skr04_1307
+DEL account.account.template: l10n_de_skr04.chart_skr04_1308
+DEL account.account.template: l10n_de_skr04.chart_skr04_1309
+DEL account.account.template: l10n_de_skr04.chart_skr04_1310
+DEL account.account.template: l10n_de_skr04.chart_skr04_1311
+DEL account.account.template: l10n_de_skr04.chart_skr04_1315
+DEL account.account.template: l10n_de_skr04.chart_skr04_1317
+DEL account.account.template: l10n_de_skr04.chart_skr04_1318
+DEL account.account.template: l10n_de_skr04.chart_skr04_1319
+DEL account.account.template: l10n_de_skr04.chart_skr04_1320
+DEL account.account.template: l10n_de_skr04.chart_skr04_1321
+DEL account.account.template: l10n_de_skr04.chart_skr04_1325
+DEL account.account.template: l10n_de_skr04.chart_skr04_1327
+DEL account.account.template: l10n_de_skr04.chart_skr04_1328
+DEL account.account.template: l10n_de_skr04.chart_skr04_1329
+DEL account.account.template: l10n_de_skr04.chart_skr04_1330
+DEL account.account.template: l10n_de_skr04.chart_skr04_1331
+DEL account.account.template: l10n_de_skr04.chart_skr04_1335
+DEL account.account.template: l10n_de_skr04.chart_skr04_1337
+DEL account.account.template: l10n_de_skr04.chart_skr04_1338
+DEL account.account.template: l10n_de_skr04.chart_skr04_1339
+DEL account.account.template: l10n_de_skr04.chart_skr04_1340
+DEL account.account.template: l10n_de_skr04.chart_skr04_1341
+DEL account.account.template: l10n_de_skr04.chart_skr04_1345
+DEL account.account.template: l10n_de_skr04.chart_skr04_135
+DEL account.account.template: l10n_de_skr04.chart_skr04_1350
+DEL account.account.template: l10n_de_skr04.chart_skr04_1351
+DEL account.account.template: l10n_de_skr04.chart_skr04_1355
+DEL account.account.template: l10n_de_skr04.chart_skr04_1360
+DEL account.account.template: l10n_de_skr04.chart_skr04_1361
+DEL account.account.template: l10n_de_skr04.chart_skr04_1365
+DEL account.account.template: l10n_de_skr04.chart_skr04_1369
+DEL account.account.template: l10n_de_skr04.chart_skr04_1370
+DEL account.account.template: l10n_de_skr04.chart_skr04_1374
+DEL account.account.template: l10n_de_skr04.chart_skr04_1375
+DEL account.account.template: l10n_de_skr04.chart_skr04_1378
+DEL account.account.template: l10n_de_skr04.chart_skr04_1380
+DEL account.account.template: l10n_de_skr04.chart_skr04_1381
+DEL account.account.template: l10n_de_skr04.chart_skr04_1382
+DEL account.account.template: l10n_de_skr04.chart_skr04_1383
+DEL account.account.template: l10n_de_skr04.chart_skr04_1390
+DEL account.account.template: l10n_de_skr04.chart_skr04_1391
+DEL account.account.template: l10n_de_skr04.chart_skr04_1393
+DEL account.account.template: l10n_de_skr04.chart_skr04_1394
+DEL account.account.template: l10n_de_skr04.chart_skr04_1395
+DEL account.account.template: l10n_de_skr04.chart_skr04_1396
+DEL account.account.template: l10n_de_skr04.chart_skr04_1397
+DEL account.account.template: l10n_de_skr04.chart_skr04_1398
+DEL account.account.template: l10n_de_skr04.chart_skr04_1399
+DEL account.account.template: l10n_de_skr04.chart_skr04_140
+DEL account.account.template: l10n_de_skr04.chart_skr04_1400
+DEL account.account.template: l10n_de_skr04.chart_skr04_1401
+DEL account.account.template: l10n_de_skr04.chart_skr04_1402
+DEL account.account.template: l10n_de_skr04.chart_skr04_1404
+DEL account.account.template: l10n_de_skr04.chart_skr04_1406
+DEL account.account.template: l10n_de_skr04.chart_skr04_1407
+DEL account.account.template: l10n_de_skr04.chart_skr04_1408
+DEL account.account.template: l10n_de_skr04.chart_skr04_1410
+DEL account.account.template: l10n_de_skr04.chart_skr04_1411
+DEL account.account.template: l10n_de_skr04.chart_skr04_1412
+DEL account.account.template: l10n_de_skr04.chart_skr04_1413
+DEL account.account.template: l10n_de_skr04.chart_skr04_1416
+DEL account.account.template: l10n_de_skr04.chart_skr04_1417
+DEL account.account.template: l10n_de_skr04.chart_skr04_1419
+DEL account.account.template: l10n_de_skr04.chart_skr04_1420
+DEL account.account.template: l10n_de_skr04.chart_skr04_1421
+DEL account.account.template: l10n_de_skr04.chart_skr04_1422
+DEL account.account.template: l10n_de_skr04.chart_skr04_1425
+DEL account.account.template: l10n_de_skr04.chart_skr04_1427
+DEL account.account.template: l10n_de_skr04.chart_skr04_143
+DEL account.account.template: l10n_de_skr04.chart_skr04_1431
+DEL account.account.template: l10n_de_skr04.chart_skr04_1432
+DEL account.account.template: l10n_de_skr04.chart_skr04_1433
+DEL account.account.template: l10n_de_skr04.chart_skr04_1434
+DEL account.account.template: l10n_de_skr04.chart_skr04_1435
+DEL account.account.template: l10n_de_skr04.chart_skr04_1436
+DEL account.account.template: l10n_de_skr04.chart_skr04_144
+DEL account.account.template: l10n_de_skr04.chart_skr04_1440
+DEL account.account.template: l10n_de_skr04.chart_skr04_145
+DEL account.account.template: l10n_de_skr04.chart_skr04_1450
+DEL account.account.template: l10n_de_skr04.chart_skr04_1456
+DEL account.account.template: l10n_de_skr04.chart_skr04_1457
+DEL account.account.template: l10n_de_skr04.chart_skr04_146
+DEL account.account.template: l10n_de_skr04.chart_skr04_147
+DEL account.account.template: l10n_de_skr04.chart_skr04_148
+DEL account.account.template: l10n_de_skr04.chart_skr04_1480
+DEL account.account.template: l10n_de_skr04.chart_skr04_1481
+DEL account.account.template: l10n_de_skr04.chart_skr04_1482
+DEL account.account.template: l10n_de_skr04.chart_skr04_1483
+DEL account.account.template: l10n_de_skr04.chart_skr04_1485
+DEL account.account.template: l10n_de_skr04.chart_skr04_1486
+DEL account.account.template: l10n_de_skr04.chart_skr04_1490
+DEL account.account.template: l10n_de_skr04.chart_skr04_1495
+DEL account.account.template: l10n_de_skr04.chart_skr04_1498
+DEL account.account.template: l10n_de_skr04.chart_skr04_150
+DEL account.account.template: l10n_de_skr04.chart_skr04_1500
+DEL account.account.template: l10n_de_skr04.chart_skr04_1504
+DEL account.account.template: l10n_de_skr04.chart_skr04_1510
+DEL account.account.template: l10n_de_skr04.chart_skr04_1520
+DEL account.account.template: l10n_de_skr04.chart_skr04_1525
+DEL account.account.template: l10n_de_skr04.chart_skr04_1530
+DEL account.account.template: l10n_de_skr04.chart_skr04_1550
+DEL account.account.template: l10n_de_skr04.chart_skr04_1610
+DEL account.account.template: l10n_de_skr04.chart_skr04_1620
+DEL account.account.template: l10n_de_skr04.chart_skr04_170
+DEL account.account.template: l10n_de_skr04.chart_skr04_1700
+DEL account.account.template: l10n_de_skr04.chart_skr04_1710
+DEL account.account.template: l10n_de_skr04.chart_skr04_1720
+DEL account.account.template: l10n_de_skr04.chart_skr04_1730
+DEL account.account.template: l10n_de_skr04.chart_skr04_1780
+DEL account.account.template: l10n_de_skr04.chart_skr04_179
+DEL account.account.template: l10n_de_skr04.chart_skr04_1790
+DEL account.account.template: l10n_de_skr04.chart_skr04_1810
+DEL account.account.template: l10n_de_skr04.chart_skr04_1820
+DEL account.account.template: l10n_de_skr04.chart_skr04_1830
+DEL account.account.template: l10n_de_skr04.chart_skr04_1840
+DEL account.account.template: l10n_de_skr04.chart_skr04_1850
+DEL account.account.template: l10n_de_skr04.chart_skr04_1890
+DEL account.account.template: l10n_de_skr04.chart_skr04_1900
+DEL account.account.template: l10n_de_skr04.chart_skr04_1920
+DEL account.account.template: l10n_de_skr04.chart_skr04_1930
+DEL account.account.template: l10n_de_skr04.chart_skr04_1940
+DEL account.account.template: l10n_de_skr04.chart_skr04_1950
+DEL account.account.template: l10n_de_skr04.chart_skr04_200
+DEL account.account.template: l10n_de_skr04.chart_skr04_2000
+DEL account.account.template: l10n_de_skr04.chart_skr04_2010
+DEL account.account.template: l10n_de_skr04.chart_skr04_2020
+DEL account.account.template: l10n_de_skr04.chart_skr04_2050
+DEL account.account.template: l10n_de_skr04.chart_skr04_2060
+DEL account.account.template: l10n_de_skr04.chart_skr04_2070
+DEL account.account.template: l10n_de_skr04.chart_skr04_210
+DEL account.account.template: l10n_de_skr04.chart_skr04_2100
+DEL account.account.template: l10n_de_skr04.chart_skr04_2130
+DEL account.account.template: l10n_de_skr04.chart_skr04_215
+DEL account.account.template: l10n_de_skr04.chart_skr04_2150
+DEL account.account.template: l10n_de_skr04.chart_skr04_2180
+DEL account.account.template: l10n_de_skr04.chart_skr04_220
+DEL account.account.template: l10n_de_skr04.chart_skr04_2200
+DEL account.account.template: l10n_de_skr04.chart_skr04_2230
+DEL account.account.template: l10n_de_skr04.chart_skr04_225
+DEL account.account.template: l10n_de_skr04.chart_skr04_2250
+DEL account.account.template: l10n_de_skr04.chart_skr04_2280
+DEL account.account.template: l10n_de_skr04.chart_skr04_230
+DEL account.account.template: l10n_de_skr04.chart_skr04_2300
+DEL account.account.template: l10n_de_skr04.chart_skr04_2349
+DEL account.account.template: l10n_de_skr04.chart_skr04_235
+DEL account.account.template: l10n_de_skr04.chart_skr04_2350
+DEL account.account.template: l10n_de_skr04.chart_skr04_2399
+DEL account.account.template: l10n_de_skr04.chart_skr04_240
+DEL account.account.template: l10n_de_skr04.chart_skr04_250
+DEL account.account.template: l10n_de_skr04.chart_skr04_2500
+DEL account.account.template: l10n_de_skr04.chart_skr04_2530
+DEL account.account.template: l10n_de_skr04.chart_skr04_2550
+DEL account.account.template: l10n_de_skr04.chart_skr04_2580
+DEL account.account.template: l10n_de_skr04.chart_skr04_260
+DEL account.account.template: l10n_de_skr04.chart_skr04_2600
+DEL account.account.template: l10n_de_skr04.chart_skr04_2630
+DEL account.account.template: l10n_de_skr04.chart_skr04_2650
+DEL account.account.template: l10n_de_skr04.chart_skr04_2680
+DEL account.account.template: l10n_de_skr04.chart_skr04_270
+DEL account.account.template: l10n_de_skr04.chart_skr04_2700
+DEL account.account.template: l10n_de_skr04.chart_skr04_2750
+DEL account.account.template: l10n_de_skr04.chart_skr04_280
+DEL account.account.template: l10n_de_skr04.chart_skr04_285
+DEL account.account.template: l10n_de_skr04.chart_skr04_290
+DEL account.account.template: l10n_de_skr04.chart_skr04_2900
+DEL account.account.template: l10n_de_skr04.chart_skr04_2901
+DEL account.account.template: l10n_de_skr04.chart_skr04_2902
+DEL account.account.template: l10n_de_skr04.chart_skr04_2903
+DEL account.account.template: l10n_de_skr04.chart_skr04_2906
+DEL account.account.template: l10n_de_skr04.chart_skr04_2907
+DEL account.account.template: l10n_de_skr04.chart_skr04_2908
+DEL account.account.template: l10n_de_skr04.chart_skr04_2909
+DEL account.account.template: l10n_de_skr04.chart_skr04_2910
+DEL account.account.template: l10n_de_skr04.chart_skr04_2920
+DEL account.account.template: l10n_de_skr04.chart_skr04_2925
+DEL account.account.template: l10n_de_skr04.chart_skr04_2926
+DEL account.account.template: l10n_de_skr04.chart_skr04_2927
+DEL account.account.template: l10n_de_skr04.chart_skr04_2928
+DEL account.account.template: l10n_de_skr04.chart_skr04_2929
+DEL account.account.template: l10n_de_skr04.chart_skr04_2930
+DEL account.account.template: l10n_de_skr04.chart_skr04_2935
+DEL account.account.template: l10n_de_skr04.chart_skr04_2937
+DEL account.account.template: l10n_de_skr04.chart_skr04_2950
+DEL account.account.template: l10n_de_skr04.chart_skr04_2959
+DEL account.account.template: l10n_de_skr04.chart_skr04_2960
+DEL account.account.template: l10n_de_skr04.chart_skr04_2961
+DEL account.account.template: l10n_de_skr04.chart_skr04_2962
+DEL account.account.template: l10n_de_skr04.chart_skr04_2963
+DEL account.account.template: l10n_de_skr04.chart_skr04_2964
+DEL account.account.template: l10n_de_skr04.chart_skr04_2965
+DEL account.account.template: l10n_de_skr04.chart_skr04_2966
+DEL account.account.template: l10n_de_skr04.chart_skr04_2967
+DEL account.account.template: l10n_de_skr04.chart_skr04_2968
+DEL account.account.template: l10n_de_skr04.chart_skr04_2969
+DEL account.account.template: l10n_de_skr04.chart_skr04_2970
+DEL account.account.template: l10n_de_skr04.chart_skr04_2975
+DEL account.account.template: l10n_de_skr04.chart_skr04_2977
+DEL account.account.template: l10n_de_skr04.chart_skr04_2978
+DEL account.account.template: l10n_de_skr04.chart_skr04_2979
+DEL account.account.template: l10n_de_skr04.chart_skr04_300
+DEL account.account.template: l10n_de_skr04.chart_skr04_3000
+DEL account.account.template: l10n_de_skr04.chart_skr04_3005
+DEL account.account.template: l10n_de_skr04.chart_skr04_3009
+DEL account.account.template: l10n_de_skr04.chart_skr04_3010
+DEL account.account.template: l10n_de_skr04.chart_skr04_3011
+DEL account.account.template: l10n_de_skr04.chart_skr04_3015
+DEL account.account.template: l10n_de_skr04.chart_skr04_3020
+DEL account.account.template: l10n_de_skr04.chart_skr04_3030
+DEL account.account.template: l10n_de_skr04.chart_skr04_3035
+DEL account.account.template: l10n_de_skr04.chart_skr04_3040
+DEL account.account.template: l10n_de_skr04.chart_skr04_305
+DEL account.account.template: l10n_de_skr04.chart_skr04_3050
+DEL account.account.template: l10n_de_skr04.chart_skr04_3060
+DEL account.account.template: l10n_de_skr04.chart_skr04_3065
+DEL account.account.template: l10n_de_skr04.chart_skr04_3070
+DEL account.account.template: l10n_de_skr04.chart_skr04_3075
+DEL account.account.template: l10n_de_skr04.chart_skr04_3076
+DEL account.account.template: l10n_de_skr04.chart_skr04_3077
+DEL account.account.template: l10n_de_skr04.chart_skr04_3079
+DEL account.account.template: l10n_de_skr04.chart_skr04_3085
+DEL account.account.template: l10n_de_skr04.chart_skr04_3090
+DEL account.account.template: l10n_de_skr04.chart_skr04_3092
+DEL account.account.template: l10n_de_skr04.chart_skr04_3095
+DEL account.account.template: l10n_de_skr04.chart_skr04_3098
+DEL account.account.template: l10n_de_skr04.chart_skr04_3099
+DEL account.account.template: l10n_de_skr04.chart_skr04_310
+DEL account.account.template: l10n_de_skr04.chart_skr04_3100
+DEL account.account.template: l10n_de_skr04.chart_skr04_3101
+DEL account.account.template: l10n_de_skr04.chart_skr04_3105
+DEL account.account.template: l10n_de_skr04.chart_skr04_3110
+DEL account.account.template: l10n_de_skr04.chart_skr04_3120
+DEL account.account.template: l10n_de_skr04.chart_skr04_3121
+DEL account.account.template: l10n_de_skr04.chart_skr04_3125
+DEL account.account.template: l10n_de_skr04.chart_skr04_3130
+DEL account.account.template: l10n_de_skr04.chart_skr04_315
+DEL account.account.template: l10n_de_skr04.chart_skr04_3150
+DEL account.account.template: l10n_de_skr04.chart_skr04_3151
+DEL account.account.template: l10n_de_skr04.chart_skr04_3160
+DEL account.account.template: l10n_de_skr04.chart_skr04_3170
+DEL account.account.template: l10n_de_skr04.chart_skr04_3180
+DEL account.account.template: l10n_de_skr04.chart_skr04_3181
+DEL account.account.template: l10n_de_skr04.chart_skr04_3190
+DEL account.account.template: l10n_de_skr04.chart_skr04_320
+DEL account.account.template: l10n_de_skr04.chart_skr04_3200
+DEL account.account.template: l10n_de_skr04.chart_skr04_3250
+DEL account.account.template: l10n_de_skr04.chart_skr04_3260
+DEL account.account.template: l10n_de_skr04.chart_skr04_3272
+DEL account.account.template: l10n_de_skr04.chart_skr04_3280
+DEL account.account.template: l10n_de_skr04.chart_skr04_3284
+DEL account.account.template: l10n_de_skr04.chart_skr04_3285
+DEL account.account.template: l10n_de_skr04.chart_skr04_329
+DEL account.account.template: l10n_de_skr04.chart_skr04_330
+DEL account.account.template: l10n_de_skr04.chart_skr04_3300
+DEL account.account.template: l10n_de_skr04.chart_skr04_3301
+DEL account.account.template: l10n_de_skr04.chart_skr04_3305
+DEL account.account.template: l10n_de_skr04.chart_skr04_3306
+DEL account.account.template: l10n_de_skr04.chart_skr04_3307
+DEL account.account.template: l10n_de_skr04.chart_skr04_3309
+DEL account.account.template: l10n_de_skr04.chart_skr04_3310
+DEL account.account.template: l10n_de_skr04.chart_skr04_3334
+DEL account.account.template: l10n_de_skr04.chart_skr04_3335
+DEL account.account.template: l10n_de_skr04.chart_skr04_3337
+DEL account.account.template: l10n_de_skr04.chart_skr04_3338
+DEL account.account.template: l10n_de_skr04.chart_skr04_3340
+DEL account.account.template: l10n_de_skr04.chart_skr04_3341
+DEL account.account.template: l10n_de_skr04.chart_skr04_3345
+DEL account.account.template: l10n_de_skr04.chart_skr04_3348
+DEL account.account.template: l10n_de_skr04.chart_skr04_3350
+DEL account.account.template: l10n_de_skr04.chart_skr04_3351
+DEL account.account.template: l10n_de_skr04.chart_skr04_3380
+DEL account.account.template: l10n_de_skr04.chart_skr04_3390
+DEL account.account.template: l10n_de_skr04.chart_skr04_340
+DEL account.account.template: l10n_de_skr04.chart_skr04_3400
+DEL account.account.template: l10n_de_skr04.chart_skr04_3401
+DEL account.account.template: l10n_de_skr04.chart_skr04_3405
+DEL account.account.template: l10n_de_skr04.chart_skr04_3410
+DEL account.account.template: l10n_de_skr04.chart_skr04_3420
+DEL account.account.template: l10n_de_skr04.chart_skr04_3421
+DEL account.account.template: l10n_de_skr04.chart_skr04_3425
+DEL account.account.template: l10n_de_skr04.chart_skr04_3430
+DEL account.account.template: l10n_de_skr04.chart_skr04_3450
+DEL account.account.template: l10n_de_skr04.chart_skr04_3451
+DEL account.account.template: l10n_de_skr04.chart_skr04_3455
+DEL account.account.template: l10n_de_skr04.chart_skr04_3460
+DEL account.account.template: l10n_de_skr04.chart_skr04_3470
+DEL account.account.template: l10n_de_skr04.chart_skr04_3471
+DEL account.account.template: l10n_de_skr04.chart_skr04_3475
+DEL account.account.template: l10n_de_skr04.chart_skr04_3480
+DEL account.account.template: l10n_de_skr04.chart_skr04_350
+DEL account.account.template: l10n_de_skr04.chart_skr04_3500
+DEL account.account.template: l10n_de_skr04.chart_skr04_3501
+DEL account.account.template: l10n_de_skr04.chart_skr04_3504
+DEL account.account.template: l10n_de_skr04.chart_skr04_3507
+DEL account.account.template: l10n_de_skr04.chart_skr04_3509
+DEL account.account.template: l10n_de_skr04.chart_skr04_3510
+DEL account.account.template: l10n_de_skr04.chart_skr04_3511
+DEL account.account.template: l10n_de_skr04.chart_skr04_3514
+DEL account.account.template: l10n_de_skr04.chart_skr04_3517
+DEL account.account.template: l10n_de_skr04.chart_skr04_3519
+DEL account.account.template: l10n_de_skr04.chart_skr04_3520
+DEL account.account.template: l10n_de_skr04.chart_skr04_3521
+DEL account.account.template: l10n_de_skr04.chart_skr04_3524
+DEL account.account.template: l10n_de_skr04.chart_skr04_3527
+DEL account.account.template: l10n_de_skr04.chart_skr04_3530
+DEL account.account.template: l10n_de_skr04.chart_skr04_3531
+DEL account.account.template: l10n_de_skr04.chart_skr04_3534
+DEL account.account.template: l10n_de_skr04.chart_skr04_3537
+DEL account.account.template: l10n_de_skr04.chart_skr04_3540
+DEL account.account.template: l10n_de_skr04.chart_skr04_3541
+DEL account.account.template: l10n_de_skr04.chart_skr04_3544
+DEL account.account.template: l10n_de_skr04.chart_skr04_3547
+DEL account.account.template: l10n_de_skr04.chart_skr04_3550
+DEL account.account.template: l10n_de_skr04.chart_skr04_3551
+DEL account.account.template: l10n_de_skr04.chart_skr04_3554
+DEL account.account.template: l10n_de_skr04.chart_skr04_3557
+DEL account.account.template: l10n_de_skr04.chart_skr04_3560
+DEL account.account.template: l10n_de_skr04.chart_skr04_3561
+DEL account.account.template: l10n_de_skr04.chart_skr04_3564
+DEL account.account.template: l10n_de_skr04.chart_skr04_3567
+DEL account.account.template: l10n_de_skr04.chart_skr04_360
+DEL account.account.template: l10n_de_skr04.chart_skr04_3600
+DEL account.account.template: l10n_de_skr04.chart_skr04_3610
+DEL account.account.template: l10n_de_skr04.chart_skr04_3611
+DEL account.account.template: l10n_de_skr04.chart_skr04_3620
+DEL account.account.template: l10n_de_skr04.chart_skr04_3630
+DEL account.account.template: l10n_de_skr04.chart_skr04_3635
+DEL account.account.template: l10n_de_skr04.chart_skr04_3640
+DEL account.account.template: l10n_de_skr04.chart_skr04_3641
+DEL account.account.template: l10n_de_skr04.chart_skr04_3642
+DEL account.account.template: l10n_de_skr04.chart_skr04_3643
+DEL account.account.template: l10n_de_skr04.chart_skr04_3645
+DEL account.account.template: l10n_de_skr04.chart_skr04_3646
+DEL account.account.template: l10n_de_skr04.chart_skr04_3647
+DEL account.account.template: l10n_de_skr04.chart_skr04_3648
+DEL account.account.template: l10n_de_skr04.chart_skr04_3650
+DEL account.account.template: l10n_de_skr04.chart_skr04_3651
+DEL account.account.template: l10n_de_skr04.chart_skr04_3652
+DEL account.account.template: l10n_de_skr04.chart_skr04_3653
+DEL account.account.template: l10n_de_skr04.chart_skr04_3655
+DEL account.account.template: l10n_de_skr04.chart_skr04_3656
+DEL account.account.template: l10n_de_skr04.chart_skr04_3657
+DEL account.account.template: l10n_de_skr04.chart_skr04_3658
+DEL account.account.template: l10n_de_skr04.chart_skr04_3695
+DEL account.account.template: l10n_de_skr04.chart_skr04_370
+DEL account.account.template: l10n_de_skr04.chart_skr04_3700
+DEL account.account.template: l10n_de_skr04.chart_skr04_3701
+DEL account.account.template: l10n_de_skr04.chart_skr04_3710
+DEL account.account.template: l10n_de_skr04.chart_skr04_3715
+DEL account.account.template: l10n_de_skr04.chart_skr04_3720
+DEL account.account.template: l10n_de_skr04.chart_skr04_3725
+DEL account.account.template: l10n_de_skr04.chart_skr04_3726
+DEL account.account.template: l10n_de_skr04.chart_skr04_3730
+DEL account.account.template: l10n_de_skr04.chart_skr04_3740
+DEL account.account.template: l10n_de_skr04.chart_skr04_3741
+DEL account.account.template: l10n_de_skr04.chart_skr04_3750
+DEL account.account.template: l10n_de_skr04.chart_skr04_3755
+DEL account.account.template: l10n_de_skr04.chart_skr04_3759
+DEL account.account.template: l10n_de_skr04.chart_skr04_3760
+DEL account.account.template: l10n_de_skr04.chart_skr04_3761
+DEL account.account.template: l10n_de_skr04.chart_skr04_3770
+DEL account.account.template: l10n_de_skr04.chart_skr04_3771
+DEL account.account.template: l10n_de_skr04.chart_skr04_3780
+DEL account.account.template: l10n_de_skr04.chart_skr04_3785
+DEL account.account.template: l10n_de_skr04.chart_skr04_3786
+DEL account.account.template: l10n_de_skr04.chart_skr04_3790
+DEL account.account.template: l10n_de_skr04.chart_skr04_3796
+DEL account.account.template: l10n_de_skr04.chart_skr04_3798
+DEL account.account.template: l10n_de_skr04.chart_skr04_3799
+DEL account.account.template: l10n_de_skr04.chart_skr04_380
+DEL account.account.template: l10n_de_skr04.chart_skr04_3800
+DEL account.account.template: l10n_de_skr04.chart_skr04_3801
+DEL account.account.template: l10n_de_skr04.chart_skr04_3802
+DEL account.account.template: l10n_de_skr04.chart_skr04_3804
+DEL account.account.template: l10n_de_skr04.chart_skr04_3806
+DEL account.account.template: l10n_de_skr04.chart_skr04_3807
+DEL account.account.template: l10n_de_skr04.chart_skr04_3808
+DEL account.account.template: l10n_de_skr04.chart_skr04_3809
+DEL account.account.template: l10n_de_skr04.chart_skr04_3810
+DEL account.account.template: l10n_de_skr04.chart_skr04_3811
+DEL account.account.template: l10n_de_skr04.chart_skr04_3812
+DEL account.account.template: l10n_de_skr04.chart_skr04_3814
+DEL account.account.template: l10n_de_skr04.chart_skr04_3816
+DEL account.account.template: l10n_de_skr04.chart_skr04_3817
+DEL account.account.template: l10n_de_skr04.chart_skr04_3818
+DEL account.account.template: l10n_de_skr04.chart_skr04_3819
+DEL account.account.template: l10n_de_skr04.chart_skr04_3820
+DEL account.account.template: l10n_de_skr04.chart_skr04_3830
+DEL account.account.template: l10n_de_skr04.chart_skr04_3832
+DEL account.account.template: l10n_de_skr04.chart_skr04_3834
+DEL account.account.template: l10n_de_skr04.chart_skr04_3835
+DEL account.account.template: l10n_de_skr04.chart_skr04_3837
+DEL account.account.template: l10n_de_skr04.chart_skr04_3840
+DEL account.account.template: l10n_de_skr04.chart_skr04_3841
+DEL account.account.template: l10n_de_skr04.chart_skr04_3845
+DEL account.account.template: l10n_de_skr04.chart_skr04_3850
+DEL account.account.template: l10n_de_skr04.chart_skr04_3851
+DEL account.account.template: l10n_de_skr04.chart_skr04_3854
+DEL account.account.template: l10n_de_skr04.chart_skr04_3860
+DEL account.account.template: l10n_de_skr04.chart_skr04_3865
+DEL account.account.template: l10n_de_skr04.chart_skr04_390
+DEL account.account.template: l10n_de_skr04.chart_skr04_3900
+DEL account.account.template: l10n_de_skr04.chart_skr04_395
+DEL account.account.template: l10n_de_skr04.chart_skr04_3950
+DEL account.account.template: l10n_de_skr04.chart_skr04_398
+DEL account.account.template: l10n_de_skr04.chart_skr04_400
+DEL account.account.template: l10n_de_skr04.chart_skr04_4000
+DEL account.account.template: l10n_de_skr04.chart_skr04_4100
+DEL account.account.template: l10n_de_skr04.chart_skr04_4110
+DEL account.account.template: l10n_de_skr04.chart_skr04_4120
+DEL account.account.template: l10n_de_skr04.chart_skr04_4125
+DEL account.account.template: l10n_de_skr04.chart_skr04_4130
+DEL account.account.template: l10n_de_skr04.chart_skr04_4135
+DEL account.account.template: l10n_de_skr04.chart_skr04_4136
+DEL account.account.template: l10n_de_skr04.chart_skr04_4138
+DEL account.account.template: l10n_de_skr04.chart_skr04_4139
+DEL account.account.template: l10n_de_skr04.chart_skr04_4140
+DEL account.account.template: l10n_de_skr04.chart_skr04_4150
+DEL account.account.template: l10n_de_skr04.chart_skr04_4160
+DEL account.account.template: l10n_de_skr04.chart_skr04_4165
+DEL account.account.template: l10n_de_skr04.chart_skr04_4180
+DEL account.account.template: l10n_de_skr04.chart_skr04_4185
+DEL account.account.template: l10n_de_skr04.chart_skr04_4186
+DEL account.account.template: l10n_de_skr04.chart_skr04_420
+DEL account.account.template: l10n_de_skr04.chart_skr04_4200
+DEL account.account.template: l10n_de_skr04.chart_skr04_4300
+DEL account.account.template: l10n_de_skr04.chart_skr04_4310
+DEL account.account.template: l10n_de_skr04.chart_skr04_4315
+DEL account.account.template: l10n_de_skr04.chart_skr04_4320
+DEL account.account.template: l10n_de_skr04.chart_skr04_4331
+DEL account.account.template: l10n_de_skr04.chart_skr04_4335
+DEL account.account.template: l10n_de_skr04.chart_skr04_4336
+DEL account.account.template: l10n_de_skr04.chart_skr04_4337
+DEL account.account.template: l10n_de_skr04.chart_skr04_4338
+DEL account.account.template: l10n_de_skr04.chart_skr04_4339
+DEL account.account.template: l10n_de_skr04.chart_skr04_440
+DEL account.account.template: l10n_de_skr04.chart_skr04_4400
+DEL account.account.template: l10n_de_skr04.chart_skr04_4499
+DEL account.account.template: l10n_de_skr04.chart_skr04_450
+DEL account.account.template: l10n_de_skr04.chart_skr04_4510
+DEL account.account.template: l10n_de_skr04.chart_skr04_4520
+DEL account.account.template: l10n_de_skr04.chart_skr04_4560
+DEL account.account.template: l10n_de_skr04.chart_skr04_4564
+DEL account.account.template: l10n_de_skr04.chart_skr04_4566
+DEL account.account.template: l10n_de_skr04.chart_skr04_4569
+DEL account.account.template: l10n_de_skr04.chart_skr04_4570
+DEL account.account.template: l10n_de_skr04.chart_skr04_4574
+DEL account.account.template: l10n_de_skr04.chart_skr04_4575
+DEL account.account.template: l10n_de_skr04.chart_skr04_4576
+DEL account.account.template: l10n_de_skr04.chart_skr04_4579
+DEL account.account.template: l10n_de_skr04.chart_skr04_460
+DEL account.account.template: l10n_de_skr04.chart_skr04_4600
+DEL account.account.template: l10n_de_skr04.chart_skr04_4605
+DEL account.account.template: l10n_de_skr04.chart_skr04_4610
+DEL account.account.template: l10n_de_skr04.chart_skr04_4616
+DEL account.account.template: l10n_de_skr04.chart_skr04_4619
+DEL account.account.template: l10n_de_skr04.chart_skr04_4620
+DEL account.account.template: l10n_de_skr04.chart_skr04_4630
+DEL account.account.template: l10n_de_skr04.chart_skr04_4639
+DEL account.account.template: l10n_de_skr04.chart_skr04_4640
+DEL account.account.template: l10n_de_skr04.chart_skr04_4645
+DEL account.account.template: l10n_de_skr04.chart_skr04_4646
+DEL account.account.template: l10n_de_skr04.chart_skr04_4650
+DEL account.account.template: l10n_de_skr04.chart_skr04_4659
+DEL account.account.template: l10n_de_skr04.chart_skr04_4660
+DEL account.account.template: l10n_de_skr04.chart_skr04_4670
+DEL account.account.template: l10n_de_skr04.chart_skr04_4679
+DEL account.account.template: l10n_de_skr04.chart_skr04_4680
+DEL account.account.template: l10n_de_skr04.chart_skr04_4686
+DEL account.account.template: l10n_de_skr04.chart_skr04_4689
+DEL account.account.template: l10n_de_skr04.chart_skr04_4690
+DEL account.account.template: l10n_de_skr04.chart_skr04_4695
+DEL account.account.template: l10n_de_skr04.chart_skr04_4699
+DEL account.account.template: l10n_de_skr04.chart_skr04_470
+DEL account.account.template: l10n_de_skr04.chart_skr04_4700
+DEL account.account.template: l10n_de_skr04.chart_skr04_4701
+DEL account.account.template: l10n_de_skr04.chart_skr04_4702
+DEL account.account.template: l10n_de_skr04.chart_skr04_4703
+DEL account.account.template: l10n_de_skr04.chart_skr04_4704
+DEL account.account.template: l10n_de_skr04.chart_skr04_4705
+DEL account.account.template: l10n_de_skr04.chart_skr04_4710
+DEL account.account.template: l10n_de_skr04.chart_skr04_4720
+DEL account.account.template: l10n_de_skr04.chart_skr04_4724
+DEL account.account.template: l10n_de_skr04.chart_skr04_4725
+DEL account.account.template: l10n_de_skr04.chart_skr04_4726
+DEL account.account.template: l10n_de_skr04.chart_skr04_4727
+DEL account.account.template: l10n_de_skr04.chart_skr04_4730
+DEL account.account.template: l10n_de_skr04.chart_skr04_4731
+DEL account.account.template: l10n_de_skr04.chart_skr04_4736
+DEL account.account.template: l10n_de_skr04.chart_skr04_4738
+DEL account.account.template: l10n_de_skr04.chart_skr04_4741
+DEL account.account.template: l10n_de_skr04.chart_skr04_4742
+DEL account.account.template: l10n_de_skr04.chart_skr04_4743
+DEL account.account.template: l10n_de_skr04.chart_skr04_4745
+DEL account.account.template: l10n_de_skr04.chart_skr04_4746
+DEL account.account.template: l10n_de_skr04.chart_skr04_4748
+DEL account.account.template: l10n_de_skr04.chart_skr04_4750
+DEL account.account.template: l10n_de_skr04.chart_skr04_4760
+DEL account.account.template: l10n_de_skr04.chart_skr04_4770
+DEL account.account.template: l10n_de_skr04.chart_skr04_4780
+DEL account.account.template: l10n_de_skr04.chart_skr04_4790
+DEL account.account.template: l10n_de_skr04.chart_skr04_4800
+DEL account.account.template: l10n_de_skr04.chart_skr04_4810
+DEL account.account.template: l10n_de_skr04.chart_skr04_4815
+DEL account.account.template: l10n_de_skr04.chart_skr04_4816
+DEL account.account.template: l10n_de_skr04.chart_skr04_4818
+DEL account.account.template: l10n_de_skr04.chart_skr04_4820
+DEL account.account.template: l10n_de_skr04.chart_skr04_4824
+DEL account.account.template: l10n_de_skr04.chart_skr04_4825
+DEL account.account.template: l10n_de_skr04.chart_skr04_4830
+DEL account.account.template: l10n_de_skr04.chart_skr04_4832
+DEL account.account.template: l10n_de_skr04.chart_skr04_4833
+DEL account.account.template: l10n_de_skr04.chart_skr04_4835
+DEL account.account.template: l10n_de_skr04.chart_skr04_4836
+DEL account.account.template: l10n_de_skr04.chart_skr04_4837
+DEL account.account.template: l10n_de_skr04.chart_skr04_4838
+DEL account.account.template: l10n_de_skr04.chart_skr04_4839
+DEL account.account.template: l10n_de_skr04.chart_skr04_4840
+DEL account.account.template: l10n_de_skr04.chart_skr04_4841
+DEL account.account.template: l10n_de_skr04.chart_skr04_4842
+DEL account.account.template: l10n_de_skr04.chart_skr04_4843
+DEL account.account.template: l10n_de_skr04.chart_skr04_4844
+DEL account.account.template: l10n_de_skr04.chart_skr04_4845
+DEL account.account.template: l10n_de_skr04.chart_skr04_4847
+DEL account.account.template: l10n_de_skr04.chart_skr04_4848
+DEL account.account.template: l10n_de_skr04.chart_skr04_4849
+DEL account.account.template: l10n_de_skr04.chart_skr04_4850
+DEL account.account.template: l10n_de_skr04.chart_skr04_4851
+DEL account.account.template: l10n_de_skr04.chart_skr04_4852
+DEL account.account.template: l10n_de_skr04.chart_skr04_4855
+DEL account.account.template: l10n_de_skr04.chart_skr04_4856
+DEL account.account.template: l10n_de_skr04.chart_skr04_4857
+DEL account.account.template: l10n_de_skr04.chart_skr04_4858
+DEL account.account.template: l10n_de_skr04.chart_skr04_4860
+DEL account.account.template: l10n_de_skr04.chart_skr04_4861
+DEL account.account.template: l10n_de_skr04.chart_skr04_4862
+DEL account.account.template: l10n_de_skr04.chart_skr04_4900
+DEL account.account.template: l10n_de_skr04.chart_skr04_4901
+DEL account.account.template: l10n_de_skr04.chart_skr04_4905
+DEL account.account.template: l10n_de_skr04.chart_skr04_4906
+DEL account.account.template: l10n_de_skr04.chart_skr04_4910
+DEL account.account.template: l10n_de_skr04.chart_skr04_4911
+DEL account.account.template: l10n_de_skr04.chart_skr04_4912
+DEL account.account.template: l10n_de_skr04.chart_skr04_4913
+DEL account.account.template: l10n_de_skr04.chart_skr04_4914
+DEL account.account.template: l10n_de_skr04.chart_skr04_4915
+DEL account.account.template: l10n_de_skr04.chart_skr04_4916
+DEL account.account.template: l10n_de_skr04.chart_skr04_4920
+DEL account.account.template: l10n_de_skr04.chart_skr04_4923
+DEL account.account.template: l10n_de_skr04.chart_skr04_4925
+DEL account.account.template: l10n_de_skr04.chart_skr04_4927
+DEL account.account.template: l10n_de_skr04.chart_skr04_4928
+DEL account.account.template: l10n_de_skr04.chart_skr04_4929
+DEL account.account.template: l10n_de_skr04.chart_skr04_4930
+DEL account.account.template: l10n_de_skr04.chart_skr04_4932
+DEL account.account.template: l10n_de_skr04.chart_skr04_4934
+DEL account.account.template: l10n_de_skr04.chart_skr04_4935
+DEL account.account.template: l10n_de_skr04.chart_skr04_4936
+DEL account.account.template: l10n_de_skr04.chart_skr04_4937
+DEL account.account.template: l10n_de_skr04.chart_skr04_4938
+DEL account.account.template: l10n_de_skr04.chart_skr04_4939
+DEL account.account.template: l10n_de_skr04.chart_skr04_4940
+DEL account.account.template: l10n_de_skr04.chart_skr04_4941
+DEL account.account.template: l10n_de_skr04.chart_skr04_4945
+DEL account.account.template: l10n_de_skr04.chart_skr04_4947
+DEL account.account.template: l10n_de_skr04.chart_skr04_4948
+DEL account.account.template: l10n_de_skr04.chart_skr04_4949
+DEL account.account.template: l10n_de_skr04.chart_skr04_4960
+DEL account.account.template: l10n_de_skr04.chart_skr04_4970
+DEL account.account.template: l10n_de_skr04.chart_skr04_4972
+DEL account.account.template: l10n_de_skr04.chart_skr04_4975
+DEL account.account.template: l10n_de_skr04.chart_skr04_4980
+DEL account.account.template: l10n_de_skr04.chart_skr04_4981
+DEL account.account.template: l10n_de_skr04.chart_skr04_4982
+DEL account.account.template: l10n_de_skr04.chart_skr04_4987
+DEL account.account.template: l10n_de_skr04.chart_skr04_4989
+DEL account.account.template: l10n_de_skr04.chart_skr04_4992
+DEL account.account.template: l10n_de_skr04.chart_skr04_50
+DEL account.account.template: l10n_de_skr04.chart_skr04_500
+DEL account.account.template: l10n_de_skr04.chart_skr04_5000
+DEL account.account.template: l10n_de_skr04.chart_skr04_510
+DEL account.account.template: l10n_de_skr04.chart_skr04_5100
+DEL account.account.template: l10n_de_skr04.chart_skr04_5110
+DEL account.account.template: l10n_de_skr04.chart_skr04_5130
+DEL account.account.template: l10n_de_skr04.chart_skr04_5160
+DEL account.account.template: l10n_de_skr04.chart_skr04_5162
+DEL account.account.template: l10n_de_skr04.chart_skr04_5166
+DEL account.account.template: l10n_de_skr04.chart_skr04_5167
+DEL account.account.template: l10n_de_skr04.chart_skr04_5189
+DEL account.account.template: l10n_de_skr04.chart_skr04_5190
+DEL account.account.template: l10n_de_skr04.chart_skr04_5191
+DEL account.account.template: l10n_de_skr04.chart_skr04_5192
+DEL account.account.template: l10n_de_skr04.chart_skr04_520
+DEL account.account.template: l10n_de_skr04.chart_skr04_5200
+DEL account.account.template: l10n_de_skr04.chart_skr04_5300
+DEL account.account.template: l10n_de_skr04.chart_skr04_5349
+DEL account.account.template: l10n_de_skr04.chart_skr04_540
+DEL account.account.template: l10n_de_skr04.chart_skr04_5400
+DEL account.account.template: l10n_de_skr04.chart_skr04_5420
+DEL account.account.template: l10n_de_skr04.chart_skr04_5425
+DEL account.account.template: l10n_de_skr04.chart_skr04_5430
+DEL account.account.template: l10n_de_skr04.chart_skr04_5435
+DEL account.account.template: l10n_de_skr04.chart_skr04_5440
+DEL account.account.template: l10n_de_skr04.chart_skr04_5550
+DEL account.account.template: l10n_de_skr04.chart_skr04_5551
+DEL account.account.template: l10n_de_skr04.chart_skr04_5552
+DEL account.account.template: l10n_de_skr04.chart_skr04_5553
+DEL account.account.template: l10n_de_skr04.chart_skr04_5557
+DEL account.account.template: l10n_de_skr04.chart_skr04_5559
+DEL account.account.template: l10n_de_skr04.chart_skr04_560
+DEL account.account.template: l10n_de_skr04.chart_skr04_5600
+DEL account.account.template: l10n_de_skr04.chart_skr04_5610
+DEL account.account.template: l10n_de_skr04.chart_skr04_5660
+DEL account.account.template: l10n_de_skr04.chart_skr04_5700
+DEL account.account.template: l10n_de_skr04.chart_skr04_5701
+DEL account.account.template: l10n_de_skr04.chart_skr04_5710
+DEL account.account.template: l10n_de_skr04.chart_skr04_5714
+DEL account.account.template: l10n_de_skr04.chart_skr04_5715
+DEL account.account.template: l10n_de_skr04.chart_skr04_5717
+DEL account.account.template: l10n_de_skr04.chart_skr04_5718
+DEL account.account.template: l10n_de_skr04.chart_skr04_5720
+DEL account.account.template: l10n_de_skr04.chart_skr04_5724
+DEL account.account.template: l10n_de_skr04.chart_skr04_5725
+DEL account.account.template: l10n_de_skr04.chart_skr04_5730
+DEL account.account.template: l10n_de_skr04.chart_skr04_5731
+DEL account.account.template: l10n_de_skr04.chart_skr04_5733
+DEL account.account.template: l10n_de_skr04.chart_skr04_5734
+DEL account.account.template: l10n_de_skr04.chart_skr04_5736
+DEL account.account.template: l10n_de_skr04.chart_skr04_5738
+DEL account.account.template: l10n_de_skr04.chart_skr04_5741
+DEL account.account.template: l10n_de_skr04.chart_skr04_5743
+DEL account.account.template: l10n_de_skr04.chart_skr04_5744
+DEL account.account.template: l10n_de_skr04.chart_skr04_5750
+DEL account.account.template: l10n_de_skr04.chart_skr04_5753
+DEL account.account.template: l10n_de_skr04.chart_skr04_5754
+DEL account.account.template: l10n_de_skr04.chart_skr04_5755
+DEL account.account.template: l10n_de_skr04.chart_skr04_5760
+DEL account.account.template: l10n_de_skr04.chart_skr04_5770
+DEL account.account.template: l10n_de_skr04.chart_skr04_5780
+DEL account.account.template: l10n_de_skr04.chart_skr04_5783
+DEL account.account.template: l10n_de_skr04.chart_skr04_5784
+DEL account.account.template: l10n_de_skr04.chart_skr04_5785
+DEL account.account.template: l10n_de_skr04.chart_skr04_5788
+DEL account.account.template: l10n_de_skr04.chart_skr04_5790
+DEL account.account.template: l10n_de_skr04.chart_skr04_5792
+DEL account.account.template: l10n_de_skr04.chart_skr04_5793
+DEL account.account.template: l10n_de_skr04.chart_skr04_5794
+DEL account.account.template: l10n_de_skr04.chart_skr04_5796
+DEL account.account.template: l10n_de_skr04.chart_skr04_5798
+DEL account.account.template: l10n_de_skr04.chart_skr04_5800
+DEL account.account.template: l10n_de_skr04.chart_skr04_5820
+DEL account.account.template: l10n_de_skr04.chart_skr04_5840
+DEL account.account.template: l10n_de_skr04.chart_skr04_5880
+DEL account.account.template: l10n_de_skr04.chart_skr04_5881
+DEL account.account.template: l10n_de_skr04.chart_skr04_5885
+DEL account.account.template: l10n_de_skr04.chart_skr04_5900
+DEL account.account.template: l10n_de_skr04.chart_skr04_5906
+DEL account.account.template: l10n_de_skr04.chart_skr04_5908
+DEL account.account.template: l10n_de_skr04.chart_skr04_5909
+DEL account.account.template: l10n_de_skr04.chart_skr04_5910
+DEL account.account.template: l10n_de_skr04.chart_skr04_5913
+DEL account.account.template: l10n_de_skr04.chart_skr04_5915
+DEL account.account.template: l10n_de_skr04.chart_skr04_5920
+DEL account.account.template: l10n_de_skr04.chart_skr04_5923
+DEL account.account.template: l10n_de_skr04.chart_skr04_5925
+DEL account.account.template: l10n_de_skr04.chart_skr04_5950
+DEL account.account.template: l10n_de_skr04.chart_skr04_5951
+DEL account.account.template: l10n_de_skr04.chart_skr04_5970
+DEL account.account.template: l10n_de_skr04.chart_skr04_5975
+DEL account.account.template: l10n_de_skr04.chart_skr04_5980
+DEL account.account.template: l10n_de_skr04.chart_skr04_5985
+DEL account.account.template: l10n_de_skr04.chart_skr04_60
+DEL account.account.template: l10n_de_skr04.chart_skr04_6000
+DEL account.account.template: l10n_de_skr04.chart_skr04_6010
+DEL account.account.template: l10n_de_skr04.chart_skr04_6020
+DEL account.account.template: l10n_de_skr04.chart_skr04_6024
+DEL account.account.template: l10n_de_skr04.chart_skr04_6026
+DEL account.account.template: l10n_de_skr04.chart_skr04_6027
+DEL account.account.template: l10n_de_skr04.chart_skr04_6028
+DEL account.account.template: l10n_de_skr04.chart_skr04_6029
+DEL account.account.template: l10n_de_skr04.chart_skr04_6030
+DEL account.account.template: l10n_de_skr04.chart_skr04_6035
+DEL account.account.template: l10n_de_skr04.chart_skr04_6036
+DEL account.account.template: l10n_de_skr04.chart_skr04_6037
+DEL account.account.template: l10n_de_skr04.chart_skr04_6038
+DEL account.account.template: l10n_de_skr04.chart_skr04_6039
+DEL account.account.template: l10n_de_skr04.chart_skr04_6040
+DEL account.account.template: l10n_de_skr04.chart_skr04_6045
+DEL account.account.template: l10n_de_skr04.chart_skr04_6050
+DEL account.account.template: l10n_de_skr04.chart_skr04_6060
+DEL account.account.template: l10n_de_skr04.chart_skr04_6066
+DEL account.account.template: l10n_de_skr04.chart_skr04_6067
+DEL account.account.template: l10n_de_skr04.chart_skr04_6068
+DEL account.account.template: l10n_de_skr04.chart_skr04_6069
+DEL account.account.template: l10n_de_skr04.chart_skr04_6070
+DEL account.account.template: l10n_de_skr04.chart_skr04_6071
+DEL account.account.template: l10n_de_skr04.chart_skr04_6072
+DEL account.account.template: l10n_de_skr04.chart_skr04_6073
+DEL account.account.template: l10n_de_skr04.chart_skr04_6074
+DEL account.account.template: l10n_de_skr04.chart_skr04_6075
+DEL account.account.template: l10n_de_skr04.chart_skr04_6076
+DEL account.account.template: l10n_de_skr04.chart_skr04_6077
+DEL account.account.template: l10n_de_skr04.chart_skr04_6078
+DEL account.account.template: l10n_de_skr04.chart_skr04_6079
+DEL account.account.template: l10n_de_skr04.chart_skr04_6080
+DEL account.account.template: l10n_de_skr04.chart_skr04_6090
+DEL account.account.template: l10n_de_skr04.chart_skr04_6100
+DEL account.account.template: l10n_de_skr04.chart_skr04_6110
+DEL account.account.template: l10n_de_skr04.chart_skr04_6118
+DEL account.account.template: l10n_de_skr04.chart_skr04_6120
+DEL account.account.template: l10n_de_skr04.chart_skr04_6130
+DEL account.account.template: l10n_de_skr04.chart_skr04_6140
+DEL account.account.template: l10n_de_skr04.chart_skr04_6147
+DEL account.account.template: l10n_de_skr04.chart_skr04_6148
+DEL account.account.template: l10n_de_skr04.chart_skr04_6149
+DEL account.account.template: l10n_de_skr04.chart_skr04_6150
+DEL account.account.template: l10n_de_skr04.chart_skr04_6160
+DEL account.account.template: l10n_de_skr04.chart_skr04_6170
+DEL account.account.template: l10n_de_skr04.chart_skr04_6171
+DEL account.account.template: l10n_de_skr04.chart_skr04_620
+DEL account.account.template: l10n_de_skr04.chart_skr04_6200
+DEL account.account.template: l10n_de_skr04.chart_skr04_6201
+DEL account.account.template: l10n_de_skr04.chart_skr04_6205
+DEL account.account.template: l10n_de_skr04.chart_skr04_6209
+DEL account.account.template: l10n_de_skr04.chart_skr04_6210
+DEL account.account.template: l10n_de_skr04.chart_skr04_6211
+DEL account.account.template: l10n_de_skr04.chart_skr04_6220
+DEL account.account.template: l10n_de_skr04.chart_skr04_6221
+DEL account.account.template: l10n_de_skr04.chart_skr04_6222
+DEL account.account.template: l10n_de_skr04.chart_skr04_6223
+DEL account.account.template: l10n_de_skr04.chart_skr04_6230
+DEL account.account.template: l10n_de_skr04.chart_skr04_6231
+DEL account.account.template: l10n_de_skr04.chart_skr04_6232
+DEL account.account.template: l10n_de_skr04.chart_skr04_6233
+DEL account.account.template: l10n_de_skr04.chart_skr04_6240
+DEL account.account.template: l10n_de_skr04.chart_skr04_6241
+DEL account.account.template: l10n_de_skr04.chart_skr04_6242
+DEL account.account.template: l10n_de_skr04.chart_skr04_6243
+DEL account.account.template: l10n_de_skr04.chart_skr04_6244
+DEL account.account.template: l10n_de_skr04.chart_skr04_6250
+DEL account.account.template: l10n_de_skr04.chart_skr04_6260
+DEL account.account.template: l10n_de_skr04.chart_skr04_6262
+DEL account.account.template: l10n_de_skr04.chart_skr04_6264
+DEL account.account.template: l10n_de_skr04.chart_skr04_6266
+DEL account.account.template: l10n_de_skr04.chart_skr04_6268
+DEL account.account.template: l10n_de_skr04.chart_skr04_6270
+DEL account.account.template: l10n_de_skr04.chart_skr04_6272
+DEL account.account.template: l10n_de_skr04.chart_skr04_6278
+DEL account.account.template: l10n_de_skr04.chart_skr04_6279
+DEL account.account.template: l10n_de_skr04.chart_skr04_6280
+DEL account.account.template: l10n_de_skr04.chart_skr04_6281
+DEL account.account.template: l10n_de_skr04.chart_skr04_6286
+DEL account.account.template: l10n_de_skr04.chart_skr04_6290
+DEL account.account.template: l10n_de_skr04.chart_skr04_6291
+DEL account.account.template: l10n_de_skr04.chart_skr04_630
+DEL account.account.template: l10n_de_skr04.chart_skr04_6300
+DEL account.account.template: l10n_de_skr04.chart_skr04_6302
+DEL account.account.template: l10n_de_skr04.chart_skr04_6303
+DEL account.account.template: l10n_de_skr04.chart_skr04_6304
+DEL account.account.template: l10n_de_skr04.chart_skr04_6305
+DEL account.account.template: l10n_de_skr04.chart_skr04_6310
+DEL account.account.template: l10n_de_skr04.chart_skr04_6312
+DEL account.account.template: l10n_de_skr04.chart_skr04_6313
+DEL account.account.template: l10n_de_skr04.chart_skr04_6314
+DEL account.account.template: l10n_de_skr04.chart_skr04_6315
+DEL account.account.template: l10n_de_skr04.chart_skr04_6316
+DEL account.account.template: l10n_de_skr04.chart_skr04_6317
+DEL account.account.template: l10n_de_skr04.chart_skr04_6319
+DEL account.account.template: l10n_de_skr04.chart_skr04_6320
+DEL account.account.template: l10n_de_skr04.chart_skr04_6325
+DEL account.account.template: l10n_de_skr04.chart_skr04_6330
+DEL account.account.template: l10n_de_skr04.chart_skr04_6335
+DEL account.account.template: l10n_de_skr04.chart_skr04_6340
+DEL account.account.template: l10n_de_skr04.chart_skr04_6345
+DEL account.account.template: l10n_de_skr04.chart_skr04_6348
+DEL account.account.template: l10n_de_skr04.chart_skr04_6349
+DEL account.account.template: l10n_de_skr04.chart_skr04_635
+DEL account.account.template: l10n_de_skr04.chart_skr04_6350
+DEL account.account.template: l10n_de_skr04.chart_skr04_6390
+DEL account.account.template: l10n_de_skr04.chart_skr04_6391
+DEL account.account.template: l10n_de_skr04.chart_skr04_6392
+DEL account.account.template: l10n_de_skr04.chart_skr04_6393
+DEL account.account.template: l10n_de_skr04.chart_skr04_6394
+DEL account.account.template: l10n_de_skr04.chart_skr04_6395
+DEL account.account.template: l10n_de_skr04.chart_skr04_6396
+DEL account.account.template: l10n_de_skr04.chart_skr04_6397
+DEL account.account.template: l10n_de_skr04.chart_skr04_6398
+DEL account.account.template: l10n_de_skr04.chart_skr04_640
+DEL account.account.template: l10n_de_skr04.chart_skr04_6400
+DEL account.account.template: l10n_de_skr04.chart_skr04_6405
+DEL account.account.template: l10n_de_skr04.chart_skr04_6410
+DEL account.account.template: l10n_de_skr04.chart_skr04_6420
+DEL account.account.template: l10n_de_skr04.chart_skr04_6430
+DEL account.account.template: l10n_de_skr04.chart_skr04_6436
+DEL account.account.template: l10n_de_skr04.chart_skr04_6437
+DEL account.account.template: l10n_de_skr04.chart_skr04_6440
+DEL account.account.template: l10n_de_skr04.chart_skr04_6450
+DEL account.account.template: l10n_de_skr04.chart_skr04_6460
+DEL account.account.template: l10n_de_skr04.chart_skr04_6470
+DEL account.account.template: l10n_de_skr04.chart_skr04_6475
+DEL account.account.template: l10n_de_skr04.chart_skr04_6485
+DEL account.account.template: l10n_de_skr04.chart_skr04_6490
+DEL account.account.template: l10n_de_skr04.chart_skr04_6495
+DEL account.account.template: l10n_de_skr04.chart_skr04_6498
+DEL account.account.template: l10n_de_skr04.chart_skr04_650
+DEL account.account.template: l10n_de_skr04.chart_skr04_6500
+DEL account.account.template: l10n_de_skr04.chart_skr04_6520
+DEL account.account.template: l10n_de_skr04.chart_skr04_6530
+DEL account.account.template: l10n_de_skr04.chart_skr04_6540
+DEL account.account.template: l10n_de_skr04.chart_skr04_6550
+DEL account.account.template: l10n_de_skr04.chart_skr04_6560
+DEL account.account.template: l10n_de_skr04.chart_skr04_6570
+DEL account.account.template: l10n_de_skr04.chart_skr04_6580
+DEL account.account.template: l10n_de_skr04.chart_skr04_6590
+DEL account.account.template: l10n_de_skr04.chart_skr04_6595
+DEL account.account.template: l10n_de_skr04.chart_skr04_660
+DEL account.account.template: l10n_de_skr04.chart_skr04_6600
+DEL account.account.template: l10n_de_skr04.chart_skr04_6605
+DEL account.account.template: l10n_de_skr04.chart_skr04_6610
+DEL account.account.template: l10n_de_skr04.chart_skr04_6611
+DEL account.account.template: l10n_de_skr04.chart_skr04_6612
+DEL account.account.template: l10n_de_skr04.chart_skr04_6620
+DEL account.account.template: l10n_de_skr04.chart_skr04_6621
+DEL account.account.template: l10n_de_skr04.chart_skr04_6625
+DEL account.account.template: l10n_de_skr04.chart_skr04_6629
+DEL account.account.template: l10n_de_skr04.chart_skr04_6630
+DEL account.account.template: l10n_de_skr04.chart_skr04_6640
+DEL account.account.template: l10n_de_skr04.chart_skr04_6641
+DEL account.account.template: l10n_de_skr04.chart_skr04_6642
+DEL account.account.template: l10n_de_skr04.chart_skr04_6643
+DEL account.account.template: l10n_de_skr04.chart_skr04_6644
+DEL account.account.template: l10n_de_skr04.chart_skr04_6645
+DEL account.account.template: l10n_de_skr04.chart_skr04_6650
+DEL account.account.template: l10n_de_skr04.chart_skr04_6660
+DEL account.account.template: l10n_de_skr04.chart_skr04_6663
+DEL account.account.template: l10n_de_skr04.chart_skr04_6664
+DEL account.account.template: l10n_de_skr04.chart_skr04_6668
+DEL account.account.template: l10n_de_skr04.chart_skr04_6670
+DEL account.account.template: l10n_de_skr04.chart_skr04_6673
+DEL account.account.template: l10n_de_skr04.chart_skr04_6674
+DEL account.account.template: l10n_de_skr04.chart_skr04_6680
+DEL account.account.template: l10n_de_skr04.chart_skr04_6688
+DEL account.account.template: l10n_de_skr04.chart_skr04_6689
+DEL account.account.template: l10n_de_skr04.chart_skr04_6690
+DEL account.account.template: l10n_de_skr04.chart_skr04_6691
+DEL account.account.template: l10n_de_skr04.chart_skr04_670
+DEL account.account.template: l10n_de_skr04.chart_skr04_6700
+DEL account.account.template: l10n_de_skr04.chart_skr04_6710
+DEL account.account.template: l10n_de_skr04.chart_skr04_6740
+DEL account.account.template: l10n_de_skr04.chart_skr04_675
+DEL account.account.template: l10n_de_skr04.chart_skr04_6760
+DEL account.account.template: l10n_de_skr04.chart_skr04_6770
+DEL account.account.template: l10n_de_skr04.chart_skr04_6780
+DEL account.account.template: l10n_de_skr04.chart_skr04_6790
+DEL account.account.template: l10n_de_skr04.chart_skr04_680
+DEL account.account.template: l10n_de_skr04.chart_skr04_6800
+DEL account.account.template: l10n_de_skr04.chart_skr04_6805
+DEL account.account.template: l10n_de_skr04.chart_skr04_6810
+DEL account.account.template: l10n_de_skr04.chart_skr04_6815
+DEL account.account.template: l10n_de_skr04.chart_skr04_6820
+DEL account.account.template: l10n_de_skr04.chart_skr04_6821
+DEL account.account.template: l10n_de_skr04.chart_skr04_6822
+DEL account.account.template: l10n_de_skr04.chart_skr04_6823
+DEL account.account.template: l10n_de_skr04.chart_skr04_6824
+DEL account.account.template: l10n_de_skr04.chart_skr04_6825
+DEL account.account.template: l10n_de_skr04.chart_skr04_6827
+DEL account.account.template: l10n_de_skr04.chart_skr04_6830
+DEL account.account.template: l10n_de_skr04.chart_skr04_6833
+DEL account.account.template: l10n_de_skr04.chart_skr04_6834
+DEL account.account.template: l10n_de_skr04.chart_skr04_6835
+DEL account.account.template: l10n_de_skr04.chart_skr04_6837
+DEL account.account.template: l10n_de_skr04.chart_skr04_6838
+DEL account.account.template: l10n_de_skr04.chart_skr04_6840
+DEL account.account.template: l10n_de_skr04.chart_skr04_6845
+DEL account.account.template: l10n_de_skr04.chart_skr04_6850
+DEL account.account.template: l10n_de_skr04.chart_skr04_6854
+DEL account.account.template: l10n_de_skr04.chart_skr04_6855
+DEL account.account.template: l10n_de_skr04.chart_skr04_6856
+DEL account.account.template: l10n_de_skr04.chart_skr04_6857
+DEL account.account.template: l10n_de_skr04.chart_skr04_6859
+DEL account.account.template: l10n_de_skr04.chart_skr04_6860
+DEL account.account.template: l10n_de_skr04.chart_skr04_6865
+DEL account.account.template: l10n_de_skr04.chart_skr04_6871
+DEL account.account.template: l10n_de_skr04.chart_skr04_6875
+DEL account.account.template: l10n_de_skr04.chart_skr04_6876
+DEL account.account.template: l10n_de_skr04.chart_skr04_6880
+DEL account.account.template: l10n_de_skr04.chart_skr04_6881
+DEL account.account.template: l10n_de_skr04.chart_skr04_6883
+DEL account.account.template: l10n_de_skr04.chart_skr04_6884
+DEL account.account.template: l10n_de_skr04.chart_skr04_6885
+DEL account.account.template: l10n_de_skr04.chart_skr04_6888
+DEL account.account.template: l10n_de_skr04.chart_skr04_6889
+DEL account.account.template: l10n_de_skr04.chart_skr04_6890
+DEL account.account.template: l10n_de_skr04.chart_skr04_6891
+DEL account.account.template: l10n_de_skr04.chart_skr04_6892
+DEL account.account.template: l10n_de_skr04.chart_skr04_6895
+DEL account.account.template: l10n_de_skr04.chart_skr04_6896
+DEL account.account.template: l10n_de_skr04.chart_skr04_6897
+DEL account.account.template: l10n_de_skr04.chart_skr04_6898
+DEL account.account.template: l10n_de_skr04.chart_skr04_690
+DEL account.account.template: l10n_de_skr04.chart_skr04_6900
+DEL account.account.template: l10n_de_skr04.chart_skr04_6903
+DEL account.account.template: l10n_de_skr04.chart_skr04_6905
+DEL account.account.template: l10n_de_skr04.chart_skr04_6906
+DEL account.account.template: l10n_de_skr04.chart_skr04_6910
+DEL account.account.template: l10n_de_skr04.chart_skr04_6912
+DEL account.account.template: l10n_de_skr04.chart_skr04_6918
+DEL account.account.template: l10n_de_skr04.chart_skr04_6920
+DEL account.account.template: l10n_de_skr04.chart_skr04_6922
+DEL account.account.template: l10n_de_skr04.chart_skr04_6923
+DEL account.account.template: l10n_de_skr04.chart_skr04_6924
+DEL account.account.template: l10n_de_skr04.chart_skr04_6927
+DEL account.account.template: l10n_de_skr04.chart_skr04_6928
+DEL account.account.template: l10n_de_skr04.chart_skr04_6929
+DEL account.account.template: l10n_de_skr04.chart_skr04_6930
+DEL account.account.template: l10n_de_skr04.chart_skr04_6931
+DEL account.account.template: l10n_de_skr04.chart_skr04_6932
+DEL account.account.template: l10n_de_skr04.chart_skr04_6933
+DEL account.account.template: l10n_de_skr04.chart_skr04_6936
+DEL account.account.template: l10n_de_skr04.chart_skr04_6938
+DEL account.account.template: l10n_de_skr04.chart_skr04_6960
+DEL account.account.template: l10n_de_skr04.chart_skr04_6967
+DEL account.account.template: l10n_de_skr04.chart_skr04_6968
+DEL account.account.template: l10n_de_skr04.chart_skr04_6969
+DEL account.account.template: l10n_de_skr04.chart_skr04_70
+DEL account.account.template: l10n_de_skr04.chart_skr04_700
+DEL account.account.template: l10n_de_skr04.chart_skr04_7000
+DEL account.account.template: l10n_de_skr04.chart_skr04_7004
+DEL account.account.template: l10n_de_skr04.chart_skr04_7005
+DEL account.account.template: l10n_de_skr04.chart_skr04_7006
+DEL account.account.template: l10n_de_skr04.chart_skr04_7008
+DEL account.account.template: l10n_de_skr04.chart_skr04_7009
+DEL account.account.template: l10n_de_skr04.chart_skr04_7010
+DEL account.account.template: l10n_de_skr04.chart_skr04_7011
+DEL account.account.template: l10n_de_skr04.chart_skr04_7012
+DEL account.account.template: l10n_de_skr04.chart_skr04_7013
+DEL account.account.template: l10n_de_skr04.chart_skr04_7014
+DEL account.account.template: l10n_de_skr04.chart_skr04_7015
+DEL account.account.template: l10n_de_skr04.chart_skr04_7016
+DEL account.account.template: l10n_de_skr04.chart_skr04_7017
+DEL account.account.template: l10n_de_skr04.chart_skr04_7018
+DEL account.account.template: l10n_de_skr04.chart_skr04_7019
+DEL account.account.template: l10n_de_skr04.chart_skr04_7020
+DEL account.account.template: l10n_de_skr04.chart_skr04_7030
+DEL account.account.template: l10n_de_skr04.chart_skr04_705
+DEL account.account.template: l10n_de_skr04.chart_skr04_710
+DEL account.account.template: l10n_de_skr04.chart_skr04_7100
+DEL account.account.template: l10n_de_skr04.chart_skr04_7103
+DEL account.account.template: l10n_de_skr04.chart_skr04_7104
+DEL account.account.template: l10n_de_skr04.chart_skr04_7105
+DEL account.account.template: l10n_de_skr04.chart_skr04_7106
+DEL account.account.template: l10n_de_skr04.chart_skr04_7107
+DEL account.account.template: l10n_de_skr04.chart_skr04_7109
+DEL account.account.template: l10n_de_skr04.chart_skr04_7110
+DEL account.account.template: l10n_de_skr04.chart_skr04_7119
+DEL account.account.template: l10n_de_skr04.chart_skr04_7120
+DEL account.account.template: l10n_de_skr04.chart_skr04_7129
+DEL account.account.template: l10n_de_skr04.chart_skr04_7130
+DEL account.account.template: l10n_de_skr04.chart_skr04_7139
+DEL account.account.template: l10n_de_skr04.chart_skr04_7140
+DEL account.account.template: l10n_de_skr04.chart_skr04_7141
+DEL account.account.template: l10n_de_skr04.chart_skr04_7142
+DEL account.account.template: l10n_de_skr04.chart_skr04_7143
+DEL account.account.template: l10n_de_skr04.chart_skr04_7144
+DEL account.account.template: l10n_de_skr04.chart_skr04_7145
+DEL account.account.template: l10n_de_skr04.chart_skr04_7190
+DEL account.account.template: l10n_de_skr04.chart_skr04_7192
+DEL account.account.template: l10n_de_skr04.chart_skr04_7194
+DEL account.account.template: l10n_de_skr04.chart_skr04_720
+DEL account.account.template: l10n_de_skr04.chart_skr04_7200
+DEL account.account.template: l10n_de_skr04.chart_skr04_7201
+DEL account.account.template: l10n_de_skr04.chart_skr04_7204
+DEL account.account.template: l10n_de_skr04.chart_skr04_7207
+DEL account.account.template: l10n_de_skr04.chart_skr04_7208
+DEL account.account.template: l10n_de_skr04.chart_skr04_7210
+DEL account.account.template: l10n_de_skr04.chart_skr04_7214
+DEL account.account.template: l10n_de_skr04.chart_skr04_7217
+DEL account.account.template: l10n_de_skr04.chart_skr04_725
+DEL account.account.template: l10n_de_skr04.chart_skr04_7250
+DEL account.account.template: l10n_de_skr04.chart_skr04_7255
+DEL account.account.template: l10n_de_skr04.chart_skr04_7300
+DEL account.account.template: l10n_de_skr04.chart_skr04_7302
+DEL account.account.template: l10n_de_skr04.chart_skr04_7303
+DEL account.account.template: l10n_de_skr04.chart_skr04_7304
+DEL account.account.template: l10n_de_skr04.chart_skr04_7305
+DEL account.account.template: l10n_de_skr04.chart_skr04_7306
+DEL account.account.template: l10n_de_skr04.chart_skr04_7309
+DEL account.account.template: l10n_de_skr04.chart_skr04_7310
+DEL account.account.template: l10n_de_skr04.chart_skr04_7313
+DEL account.account.template: l10n_de_skr04.chart_skr04_7316
+DEL account.account.template: l10n_de_skr04.chart_skr04_7317
+DEL account.account.template: l10n_de_skr04.chart_skr04_7319
+DEL account.account.template: l10n_de_skr04.chart_skr04_7320
+DEL account.account.template: l10n_de_skr04.chart_skr04_7323
+DEL account.account.template: l10n_de_skr04.chart_skr04_7324
+DEL account.account.template: l10n_de_skr04.chart_skr04_7325
+DEL account.account.template: l10n_de_skr04.chart_skr04_7326
+DEL account.account.template: l10n_de_skr04.chart_skr04_7327
+DEL account.account.template: l10n_de_skr04.chart_skr04_7328
+DEL account.account.template: l10n_de_skr04.chart_skr04_7329
+DEL account.account.template: l10n_de_skr04.chart_skr04_7330
+DEL account.account.template: l10n_de_skr04.chart_skr04_7339
+DEL account.account.template: l10n_de_skr04.chart_skr04_7340
+DEL account.account.template: l10n_de_skr04.chart_skr04_7349
+DEL account.account.template: l10n_de_skr04.chart_skr04_735
+DEL account.account.template: l10n_de_skr04.chart_skr04_7350
+DEL account.account.template: l10n_de_skr04.chart_skr04_7351
+DEL account.account.template: l10n_de_skr04.chart_skr04_7355
+DEL account.account.template: l10n_de_skr04.chart_skr04_7360
+DEL account.account.template: l10n_de_skr04.chart_skr04_7361
+DEL account.account.template: l10n_de_skr04.chart_skr04_7362
+DEL account.account.template: l10n_de_skr04.chart_skr04_7363
+DEL account.account.template: l10n_de_skr04.chart_skr04_7364
+DEL account.account.template: l10n_de_skr04.chart_skr04_7365
+DEL account.account.template: l10n_de_skr04.chart_skr04_7366
+DEL account.account.template: l10n_de_skr04.chart_skr04_7390
+DEL account.account.template: l10n_de_skr04.chart_skr04_7392
+DEL account.account.template: l10n_de_skr04.chart_skr04_7394
+DEL account.account.template: l10n_de_skr04.chart_skr04_7399
+DEL account.account.template: l10n_de_skr04.chart_skr04_740
+DEL account.account.template: l10n_de_skr04.chart_skr04_7400
+DEL account.account.template: l10n_de_skr04.chart_skr04_7401
+DEL account.account.template: l10n_de_skr04.chart_skr04_7450
+DEL account.account.template: l10n_de_skr04.chart_skr04_7451
+DEL account.account.template: l10n_de_skr04.chart_skr04_7452
+DEL account.account.template: l10n_de_skr04.chart_skr04_7453
+DEL account.account.template: l10n_de_skr04.chart_skr04_7454
+DEL account.account.template: l10n_de_skr04.chart_skr04_7460
+DEL account.account.template: l10n_de_skr04.chart_skr04_7461
+DEL account.account.template: l10n_de_skr04.chart_skr04_7462
+DEL account.account.template: l10n_de_skr04.chart_skr04_7463
+DEL account.account.template: l10n_de_skr04.chart_skr04_7464
+DEL account.account.template: l10n_de_skr04.chart_skr04_7500
+DEL account.account.template: l10n_de_skr04.chart_skr04_7501
+DEL account.account.template: l10n_de_skr04.chart_skr04_755
+DEL account.account.template: l10n_de_skr04.chart_skr04_7550
+DEL account.account.template: l10n_de_skr04.chart_skr04_7551
+DEL account.account.template: l10n_de_skr04.chart_skr04_7552
+DEL account.account.template: l10n_de_skr04.chart_skr04_7553
+DEL account.account.template: l10n_de_skr04.chart_skr04_7554
+DEL account.account.template: l10n_de_skr04.chart_skr04_7560
+DEL account.account.template: l10n_de_skr04.chart_skr04_7561
+DEL account.account.template: l10n_de_skr04.chart_skr04_7562
+DEL account.account.template: l10n_de_skr04.chart_skr04_7563
+DEL account.account.template: l10n_de_skr04.chart_skr04_7600
+DEL account.account.template: l10n_de_skr04.chart_skr04_7603
+DEL account.account.template: l10n_de_skr04.chart_skr04_7604
+DEL account.account.template: l10n_de_skr04.chart_skr04_7607
+DEL account.account.template: l10n_de_skr04.chart_skr04_7608
+DEL account.account.template: l10n_de_skr04.chart_skr04_7609
+DEL account.account.template: l10n_de_skr04.chart_skr04_7610
+DEL account.account.template: l10n_de_skr04.chart_skr04_7630
+DEL account.account.template: l10n_de_skr04.chart_skr04_7633
+DEL account.account.template: l10n_de_skr04.chart_skr04_7639
+DEL account.account.template: l10n_de_skr04.chart_skr04_7640
+DEL account.account.template: l10n_de_skr04.chart_skr04_7641
+DEL account.account.template: l10n_de_skr04.chart_skr04_7642
+DEL account.account.template: l10n_de_skr04.chart_skr04_7643
+DEL account.account.template: l10n_de_skr04.chart_skr04_7644
+DEL account.account.template: l10n_de_skr04.chart_skr04_7646
+DEL account.account.template: l10n_de_skr04.chart_skr04_7648
+DEL account.account.template: l10n_de_skr04.chart_skr04_7649
+DEL account.account.template: l10n_de_skr04.chart_skr04_765
+DEL account.account.template: l10n_de_skr04.chart_skr04_7650
+DEL account.account.template: l10n_de_skr04.chart_skr04_7675
+DEL account.account.template: l10n_de_skr04.chart_skr04_7678
+DEL account.account.template: l10n_de_skr04.chart_skr04_7680
+DEL account.account.template: l10n_de_skr04.chart_skr04_7685
+DEL account.account.template: l10n_de_skr04.chart_skr04_7690
+DEL account.account.template: l10n_de_skr04.chart_skr04_7692
+DEL account.account.template: l10n_de_skr04.chart_skr04_7694
+DEL account.account.template: l10n_de_skr04.chart_skr04_770
+DEL account.account.template: l10n_de_skr04.chart_skr04_7705
+DEL account.account.template: l10n_de_skr04.chart_skr04_7725
+DEL account.account.template: l10n_de_skr04.chart_skr04_7744
+DEL account.account.template: l10n_de_skr04.chart_skr04_7751
+DEL account.account.template: l10n_de_skr04.chart_skr04_7781
+DEL account.account.template: l10n_de_skr04.chart_skr04_7785
+DEL account.account.template: l10n_de_skr04.chart_skr04_780
+DEL account.account.template: l10n_de_skr04.chart_skr04_785
+DEL account.account.template: l10n_de_skr04.chart_skr04_795
+DEL account.account.template: l10n_de_skr04.chart_skr04_80
+DEL account.account.template: l10n_de_skr04.chart_skr04_800
+DEL account.account.template: l10n_de_skr04.chart_skr04_803
+DEL account.account.template: l10n_de_skr04.chart_skr04_804
+DEL account.account.template: l10n_de_skr04.chart_skr04_805
+DEL account.account.template: l10n_de_skr04.chart_skr04_808
+DEL account.account.template: l10n_de_skr04.chart_skr04_809
+DEL account.account.template: l10n_de_skr04.chart_skr04_810
+DEL account.account.template: l10n_de_skr04.chart_skr04_813
+DEL account.account.template: l10n_de_skr04.chart_skr04_814
+DEL account.account.template: l10n_de_skr04.chart_skr04_815
+DEL account.account.template: l10n_de_skr04.chart_skr04_820
+DEL account.account.template: l10n_de_skr04.chart_skr04_829
+DEL account.account.template: l10n_de_skr04.chart_skr04_830
+DEL account.account.template: l10n_de_skr04.chart_skr04_840
+DEL account.account.template: l10n_de_skr04.chart_skr04_850
+DEL account.account.template: l10n_de_skr04.chart_skr04_860
+DEL account.account.template: l10n_de_skr04.chart_skr04_880
+DEL account.account.template: l10n_de_skr04.chart_skr04_883
+DEL account.account.template: l10n_de_skr04.chart_skr04_885
+DEL account.account.template: l10n_de_skr04.chart_skr04_90
+DEL account.account.template: l10n_de_skr04.chart_skr04_900
+DEL account.account.template: l10n_de_skr04.chart_skr04_9000
+DEL account.account.template: l10n_de_skr04.chart_skr04_9008
+DEL account.account.template: l10n_de_skr04.chart_skr04_9009
+DEL account.account.template: l10n_de_skr04.chart_skr04_9090
+DEL account.account.template: l10n_de_skr04.chart_skr04_910
+DEL account.account.template: l10n_de_skr04.chart_skr04_920
+DEL account.account.template: l10n_de_skr04.chart_skr04_930
+DEL account.account.template: l10n_de_skr04.chart_skr04_940
+DEL account.account.template: l10n_de_skr04.chart_skr04_960
+DEL account.account.template: l10n_de_skr04.chart_skr04_961
+DEL account.account.template: l10n_de_skr04.chart_skr04_962
+DEL account.account.template: l10n_de_skr04.chart_skr04_963
+DEL account.account.template: l10n_de_skr04.chart_skr04_964
+DEL account.account.template: l10n_de_skr04.chart_skr04_970
+DEL account.account.template: l10n_de_skr04.chart_skr04_980
+DEL account.account.template: l10n_de_skr04.chart_skr04_9991
+DEL account.account.template: l10n_de_skr04.chart_skr04_9994
+DEL account.chart.template: l10n_de_skr04.l10n_chart_de_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_no_id_partner_19a_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_no_id_partner_19b_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_no_id_partner_7b_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_no_id_partner_afa7a_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_partner_19b_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_partner_afa19a_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_partner_afa7a_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_partner_afa7b_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_purchase_service_19_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_purchase_service_7_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_non_eu_purchase_services_19_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_no_id_purchase_19_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_no_id_sale_19_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_vat_id_purchase_19_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_vat_id_purchase_7_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_vat_id_sale_19_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_vat_id_sale_7_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_no_id_purchase_7_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_no_id_sale_7_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_purchase_19_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_purchase_7_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_sale_19_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_sale_7_skr04
+DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_sale_services_19_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_no_id_purchase_19_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_no_id_purchase_7_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_no_id_sale_19_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_purchase_19_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_purchase_7_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_purchase_services_19_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_purchase_services_7_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_sale_19_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_sale_7_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_purchase_19_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_purchase_7_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_purchase_services_19_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_sale_19_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_sale_7_skr04
+DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_sale_services_19_skr04
+DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_domestic_skr04
+DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_eu_no_id_partner_skr04
+DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_eu_vat_id_partner_service_skr04
+DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_eu_vat_id_partner_skr04
+DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_non_eu_partner_service_skr04
+DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_non_eu_partner_skr04
+DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_4731_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_4736_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_5731_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_5736_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_6931_line (noupdate)
+DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_6936_line (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr04.reconcile_4731 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr04.reconcile_4736 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr04.reconcile_5731 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr04.reconcile_5736 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr04.reconcile_6931 (noupdate)
+DEL account.reconcile.model.template: l10n_de_skr04.reconcile_6936 (noupdate)
+DEL account.tax.group: l10n_de_skr04.tax_group_0 (noupdate)
+DEL account.tax.group: l10n_de_skr04.tax_group_107 (noupdate)
+DEL account.tax.group: l10n_de_skr04.tax_group_19 (noupdate)
+DEL account.tax.group: l10n_de_skr04.tax_group_55 (noupdate)
+DEL account.tax.group: l10n_de_skr04.tax_group_7 (noupdate)
+DEL account.tax.group: l10n_de_skr04.tax_group_x (noupdate)
+DEL account.tax.template: l10n_de_skr04.tax_eu_19_purchase_goods_skr04
+DEL account.tax.template: l10n_de_skr04.tax_eu_19_purchase_no_vst_skr04
+DEL account.tax.template: l10n_de_skr04.tax_eu_19_purchase_skr04
+DEL account.tax.template: l10n_de_skr04.tax_eu_7_purchase_goods_skr04
+DEL account.tax.template: l10n_de_skr04.tax_eu_7_purchase_no_vst_skr04
+DEL account.tax.template: l10n_de_skr04.tax_eu_7_purchase_skr04
+DEL account.tax.template: l10n_de_skr04.tax_eu_car_purchase_skr04
+DEL account.tax.template: l10n_de_skr04.tax_eu_purchase_tax_free_skr04
+DEL account.tax.template: l10n_de_skr04.tax_eu_sale_skr04
+DEL account.tax.template: l10n_de_skr04.tax_export_skr04
+DEL account.tax.template: l10n_de_skr04.tax_free_eu_skr04
+DEL account.tax.template: l10n_de_skr04.tax_free_newcar_skr04
+DEL account.tax.template: l10n_de_skr04.tax_free_skr04_mit_vst
+DEL account.tax.template: l10n_de_skr04.tax_free_skr04_ohne_vst
+DEL account.tax.template: l10n_de_skr04.tax_free_third_country_skr04
+DEL account.tax.template: l10n_de_skr04.tax_import_19_and_payable_skr04
+DEL account.tax.template: l10n_de_skr04.tax_import_7_and_payable_skr04
+DEL account.tax.template: l10n_de_skr04.tax_not_taxable_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_107_farmer_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_19_13b_ausland_ohne_vst_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_19_13b_bau_ohne_vst_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_19_13b_eu_ohne_vst_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_19_3eck_first_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_19_eu_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_19_farmer_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_19_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_19_taxinclusive_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_55_farmer_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_7_13b_ausland_ohne_vst_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_7_13b_bau_ohne_vst_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_7_13b_eu_ohne_vst_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_7_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_7_taxinclusive_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_eu_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_free_bau_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_free_mobil_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_no_ustpflicht_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_vst_19_purchase_13b_bau_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_vst_7_purchase_13b_bau_skr04
+DEL account.tax.template: l10n_de_skr04.tax_ust_x_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_107_farmer_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_19_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_19_taxinclusive_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_55_farmer_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_7_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_7_taxinclusive_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_no_ustpflicht_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_ust_19_purchase_13a_auslagerung_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_ust_19_purchase_13b_mobil_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_ust_19_purchase_13b_werk_ausland_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_ust_19_purchase_3eck_last_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_ust_7_purchase_13a_auslagerung_skr04
+DEL account.tax.template: l10n_de_skr04.tax_vst_ust_7_purchase_13b_werk_ausland_skr04
+ERROR: module not in list of installed modules:
 ---Models in module 'l10n_generic_coa'---
 ---Fields in module 'l10n_generic_coa'---
 ---XML records in module 'l10n_generic_coa'---
 DEL account.account.template: l10n_generic_coa.capital
 DEL account.account.template: l10n_generic_coa.cash_diff_expense
 DEL account.account.template: l10n_generic_coa.cash_diff_income
 DEL account.account.template: l10n_generic_coa.cash_discount_gain
@@ -170,14 +2896,1058 @@
 DEL account.account.template: l10n_generic_coa.to_receive_pay
 DEL account.account.template: l10n_generic_coa.to_receive_rec
 DEL account.chart.template: l10n_generic_coa.configurable_chart_template
 DEL account.tax.group: l10n_generic_coa.tax_group_15 (noupdate)
 DEL account.tax.template: l10n_generic_coa.purchase_tax_template
 DEL account.tax.template: l10n_generic_coa.sale_tax_template
 ERROR: module not in list of installed modules:
+---Models in module 'l10n_hr_euro'---
+---Fields in module 'l10n_hr_euro'---
+---XML records in module 'l10n_hr_euro'---
+DEL account.account.template: l10n_hr_euro.hr_000000
+DEL account.account.template: l10n_hr_euro.hr_001000
+DEL account.account.template: l10n_hr_euro.hr_002000
+DEL account.account.template: l10n_hr_euro.hr_003000
+DEL account.account.template: l10n_hr_euro.hr_004000
+DEL account.account.template: l10n_hr_euro.hr_010000
+DEL account.account.template: l10n_hr_euro.hr_011000
+DEL account.account.template: l10n_hr_euro.hr_012000
+DEL account.account.template: l10n_hr_euro.hr_013000
+DEL account.account.template: l10n_hr_euro.hr_014000
+DEL account.account.template: l10n_hr_euro.hr_015000
+DEL account.account.template: l10n_hr_euro.hr_016000
+DEL account.account.template: l10n_hr_euro.hr_017000
+DEL account.account.template: l10n_hr_euro.hr_018000
+DEL account.account.template: l10n_hr_euro.hr_019000
+DEL account.account.template: l10n_hr_euro.hr_020000
+DEL account.account.template: l10n_hr_euro.hr_021000
+DEL account.account.template: l10n_hr_euro.hr_023000
+DEL account.account.template: l10n_hr_euro.hr_024000
+DEL account.account.template: l10n_hr_euro.hr_026000
+DEL account.account.template: l10n_hr_euro.hr_027000
+DEL account.account.template: l10n_hr_euro.hr_028000
+DEL account.account.template: l10n_hr_euro.hr_029000
+DEL account.account.template: l10n_hr_euro.hr_030000
+DEL account.account.template: l10n_hr_euro.hr_031000
+DEL account.account.template: l10n_hr_euro.hr_032000
+DEL account.account.template: l10n_hr_euro.hr_033000
+DEL account.account.template: l10n_hr_euro.hr_034000
+DEL account.account.template: l10n_hr_euro.hr_035000
+DEL account.account.template: l10n_hr_euro.hr_036000
+DEL account.account.template: l10n_hr_euro.hr_037000
+DEL account.account.template: l10n_hr_euro.hr_038000
+DEL account.account.template: l10n_hr_euro.hr_039000
+DEL account.account.template: l10n_hr_euro.hr_040000
+DEL account.account.template: l10n_hr_euro.hr_041000
+DEL account.account.template: l10n_hr_euro.hr_046000
+DEL account.account.template: l10n_hr_euro.hr_047000
+DEL account.account.template: l10n_hr_euro.hr_048000
+DEL account.account.template: l10n_hr_euro.hr_049000
+DEL account.account.template: l10n_hr_euro.hr_050000
+DEL account.account.template: l10n_hr_euro.hr_051000
+DEL account.account.template: l10n_hr_euro.hr_056000
+DEL account.account.template: l10n_hr_euro.hr_057000
+DEL account.account.template: l10n_hr_euro.hr_058000
+DEL account.account.template: l10n_hr_euro.hr_059000
+DEL account.account.template: l10n_hr_euro.hr_060000
+DEL account.account.template: l10n_hr_euro.hr_060100
+DEL account.account.template: l10n_hr_euro.hr_061000
+DEL account.account.template: l10n_hr_euro.hr_062000
+DEL account.account.template: l10n_hr_euro.hr_062100
+DEL account.account.template: l10n_hr_euro.hr_063000
+DEL account.account.template: l10n_hr_euro.hr_064000
+DEL account.account.template: l10n_hr_euro.hr_065000
+DEL account.account.template: l10n_hr_euro.hr_066000
+DEL account.account.template: l10n_hr_euro.hr_067000
+DEL account.account.template: l10n_hr_euro.hr_068000
+DEL account.account.template: l10n_hr_euro.hr_069000
+DEL account.account.template: l10n_hr_euro.hr_070000
+DEL account.account.template: l10n_hr_euro.hr_071000
+DEL account.account.template: l10n_hr_euro.hr_072000
+DEL account.account.template: l10n_hr_euro.hr_073000
+DEL account.account.template: l10n_hr_euro.hr_074000
+DEL account.account.template: l10n_hr_euro.hr_075000
+DEL account.account.template: l10n_hr_euro.hr_076000
+DEL account.account.template: l10n_hr_euro.hr_077000
+DEL account.account.template: l10n_hr_euro.hr_078000
+DEL account.account.template: l10n_hr_euro.hr_079000
+DEL account.account.template: l10n_hr_euro.hr_080000
+DEL account.account.template: l10n_hr_euro.hr_081000
+DEL account.account.template: l10n_hr_euro.hr_100000
+DEL account.account.template: l10n_hr_euro.hr_101000
+DEL account.account.template: l10n_hr_euro.hr_102000
+DEL account.account.template: l10n_hr_euro.hr_103000
+DEL account.account.template: l10n_hr_euro.hr_104000
+DEL account.account.template: l10n_hr_euro.hr_105000
+DEL account.account.template: l10n_hr_euro.hr_106000
+DEL account.account.template: l10n_hr_euro.hr_108000
+DEL account.account.template: l10n_hr_euro.hr_109000
+DEL account.account.template: l10n_hr_euro.hr_110000
+DEL account.account.template: l10n_hr_euro.hr_110100
+DEL account.account.template: l10n_hr_euro.hr_111000
+DEL account.account.template: l10n_hr_euro.hr_112000
+DEL account.account.template: l10n_hr_euro.hr_112100
+DEL account.account.template: l10n_hr_euro.hr_113000
+DEL account.account.template: l10n_hr_euro.hr_114000
+DEL account.account.template: l10n_hr_euro.hr_115000
+DEL account.account.template: l10n_hr_euro.hr_116000
+DEL account.account.template: l10n_hr_euro.hr_117000
+DEL account.account.template: l10n_hr_euro.hr_118000
+DEL account.account.template: l10n_hr_euro.hr_119000
+DEL account.account.template: l10n_hr_euro.hr_120000
+DEL account.account.template: l10n_hr_euro.hr_120100
+DEL account.account.template: l10n_hr_euro.hr_121000
+DEL account.account.template: l10n_hr_euro.hr_122000
+DEL account.account.template: l10n_hr_euro.hr_123000
+DEL account.account.template: l10n_hr_euro.hr_124000
+DEL account.account.template: l10n_hr_euro.hr_125000
+DEL account.account.template: l10n_hr_euro.hr_126000
+DEL account.account.template: l10n_hr_euro.hr_127000
+DEL account.account.template: l10n_hr_euro.hr_128000
+DEL account.account.template: l10n_hr_euro.hr_129000
+DEL account.account.template: l10n_hr_euro.hr_130000
+DEL account.account.template: l10n_hr_euro.hr_131000
+DEL account.account.template: l10n_hr_euro.hr_133000
+DEL account.account.template: l10n_hr_euro.hr_134000
+DEL account.account.template: l10n_hr_euro.hr_135000
+DEL account.account.template: l10n_hr_euro.hr_136000
+DEL account.account.template: l10n_hr_euro.hr_137000
+DEL account.account.template: l10n_hr_euro.hr_138000
+DEL account.account.template: l10n_hr_euro.hr_139000
+DEL account.account.template: l10n_hr_euro.hr_140000
+DEL account.account.template: l10n_hr_euro.hr_140010
+DEL account.account.template: l10n_hr_euro.hr_140011
+DEL account.account.template: l10n_hr_euro.hr_140012
+DEL account.account.template: l10n_hr_euro.hr_140020
+DEL account.account.template: l10n_hr_euro.hr_140021
+DEL account.account.template: l10n_hr_euro.hr_140022
+DEL account.account.template: l10n_hr_euro.hr_140030
+DEL account.account.template: l10n_hr_euro.hr_140031
+DEL account.account.template: l10n_hr_euro.hr_140032
+DEL account.account.template: l10n_hr_euro.hr_140100
+DEL account.account.template: l10n_hr_euro.hr_140200
+DEL account.account.template: l10n_hr_euro.hr_140210
+DEL account.account.template: l10n_hr_euro.hr_140220
+DEL account.account.template: l10n_hr_euro.hr_140300
+DEL account.account.template: l10n_hr_euro.hr_140310
+DEL account.account.template: l10n_hr_euro.hr_140320
+DEL account.account.template: l10n_hr_euro.hr_140400
+DEL account.account.template: l10n_hr_euro.hr_140410
+DEL account.account.template: l10n_hr_euro.hr_140420
+DEL account.account.template: l10n_hr_euro.hr_140500
+DEL account.account.template: l10n_hr_euro.hr_140700
+DEL account.account.template: l10n_hr_euro.hr_140800
+DEL account.account.template: l10n_hr_euro.hr_141000
+DEL account.account.template: l10n_hr_euro.hr_142000
+DEL account.account.template: l10n_hr_euro.hr_143000
+DEL account.account.template: l10n_hr_euro.hr_144000
+DEL account.account.template: l10n_hr_euro.hr_145000
+DEL account.account.template: l10n_hr_euro.hr_146000
+DEL account.account.template: l10n_hr_euro.hr_147000
+DEL account.account.template: l10n_hr_euro.hr_148000
+DEL account.account.template: l10n_hr_euro.hr_149000
+DEL account.account.template: l10n_hr_euro.hr_150000
+DEL account.account.template: l10n_hr_euro.hr_151000
+DEL account.account.template: l10n_hr_euro.hr_152000
+DEL account.account.template: l10n_hr_euro.hr_153000
+DEL account.account.template: l10n_hr_euro.hr_154000
+DEL account.account.template: l10n_hr_euro.hr_155000
+DEL account.account.template: l10n_hr_euro.hr_156000
+DEL account.account.template: l10n_hr_euro.hr_159000
+DEL account.account.template: l10n_hr_euro.hr_190000
+DEL account.account.template: l10n_hr_euro.hr_191000
+DEL account.account.template: l10n_hr_euro.hr_192000
+DEL account.account.template: l10n_hr_euro.hr_193000
+DEL account.account.template: l10n_hr_euro.hr_194000
+DEL account.account.template: l10n_hr_euro.hr_195000
+DEL account.account.template: l10n_hr_euro.hr_196000
+DEL account.account.template: l10n_hr_euro.hr_197000
+DEL account.account.template: l10n_hr_euro.hr_199000
+DEL account.account.template: l10n_hr_euro.hr_200000
+DEL account.account.template: l10n_hr_euro.hr_200100
+DEL account.account.template: l10n_hr_euro.hr_201000
+DEL account.account.template: l10n_hr_euro.hr_210000
+DEL account.account.template: l10n_hr_euro.hr_211000
+DEL account.account.template: l10n_hr_euro.hr_212000
+DEL account.account.template: l10n_hr_euro.hr_213000
+DEL account.account.template: l10n_hr_euro.hr_213100
+DEL account.account.template: l10n_hr_euro.hr_214000
+DEL account.account.template: l10n_hr_euro.hr_215000
+DEL account.account.template: l10n_hr_euro.hr_216000
+DEL account.account.template: l10n_hr_euro.hr_217000
+DEL account.account.template: l10n_hr_euro.hr_218000
+DEL account.account.template: l10n_hr_euro.hr_220000
+DEL account.account.template: l10n_hr_euro.hr_221000
+DEL account.account.template: l10n_hr_euro.hr_222000
+DEL account.account.template: l10n_hr_euro.hr_223000
+DEL account.account.template: l10n_hr_euro.hr_224000
+DEL account.account.template: l10n_hr_euro.hr_225000
+DEL account.account.template: l10n_hr_euro.hr_230000
+DEL account.account.template: l10n_hr_euro.hr_231000
+DEL account.account.template: l10n_hr_euro.hr_232000
+DEL account.account.template: l10n_hr_euro.hr_233000
+DEL account.account.template: l10n_hr_euro.hr_234000
+DEL account.account.template: l10n_hr_euro.hr_235000
+DEL account.account.template: l10n_hr_euro.hr_236000
+DEL account.account.template: l10n_hr_euro.hr_237000
+DEL account.account.template: l10n_hr_euro.hr_238000
+DEL account.account.template: l10n_hr_euro.hr_239000
+DEL account.account.template: l10n_hr_euro.hr_240000
+DEL account.account.template: l10n_hr_euro.hr_240010
+DEL account.account.template: l10n_hr_euro.hr_240011
+DEL account.account.template: l10n_hr_euro.hr_240012
+DEL account.account.template: l10n_hr_euro.hr_240020
+DEL account.account.template: l10n_hr_euro.hr_240021
+DEL account.account.template: l10n_hr_euro.hr_240022
+DEL account.account.template: l10n_hr_euro.hr_240030
+DEL account.account.template: l10n_hr_euro.hr_240031
+DEL account.account.template: l10n_hr_euro.hr_240032
+DEL account.account.template: l10n_hr_euro.hr_240040
+DEL account.account.template: l10n_hr_euro.hr_240050
+DEL account.account.template: l10n_hr_euro.hr_240100
+DEL account.account.template: l10n_hr_euro.hr_240200
+DEL account.account.template: l10n_hr_euro.hr_240210
+DEL account.account.template: l10n_hr_euro.hr_240220
+DEL account.account.template: l10n_hr_euro.hr_240300
+DEL account.account.template: l10n_hr_euro.hr_240310
+DEL account.account.template: l10n_hr_euro.hr_240320
+DEL account.account.template: l10n_hr_euro.hr_240400
+DEL account.account.template: l10n_hr_euro.hr_240410
+DEL account.account.template: l10n_hr_euro.hr_240420
+DEL account.account.template: l10n_hr_euro.hr_240500
+DEL account.account.template: l10n_hr_euro.hr_240700
+DEL account.account.template: l10n_hr_euro.hr_240800
+DEL account.account.template: l10n_hr_euro.hr_241000
+DEL account.account.template: l10n_hr_euro.hr_242000
+DEL account.account.template: l10n_hr_euro.hr_243000
+DEL account.account.template: l10n_hr_euro.hr_244000
+DEL account.account.template: l10n_hr_euro.hr_245000
+DEL account.account.template: l10n_hr_euro.hr_246000
+DEL account.account.template: l10n_hr_euro.hr_247000
+DEL account.account.template: l10n_hr_euro.hr_248000
+DEL account.account.template: l10n_hr_euro.hr_249000
+DEL account.account.template: l10n_hr_euro.hr_250000
+DEL account.account.template: l10n_hr_euro.hr_250100
+DEL account.account.template: l10n_hr_euro.hr_251000
+DEL account.account.template: l10n_hr_euro.hr_251100
+DEL account.account.template: l10n_hr_euro.hr_252000
+DEL account.account.template: l10n_hr_euro.hr_253000
+DEL account.account.template: l10n_hr_euro.hr_254000
+DEL account.account.template: l10n_hr_euro.hr_255000
+DEL account.account.template: l10n_hr_euro.hr_256000
+DEL account.account.template: l10n_hr_euro.hr_257000
+DEL account.account.template: l10n_hr_euro.hr_258000
+DEL account.account.template: l10n_hr_euro.hr_259000
+DEL account.account.template: l10n_hr_euro.hr_260000
+DEL account.account.template: l10n_hr_euro.hr_280000
+DEL account.account.template: l10n_hr_euro.hr_281000
+DEL account.account.template: l10n_hr_euro.hr_282000
+DEL account.account.template: l10n_hr_euro.hr_283000
+DEL account.account.template: l10n_hr_euro.hr_284000
+DEL account.account.template: l10n_hr_euro.hr_285000
+DEL account.account.template: l10n_hr_euro.hr_290000
+DEL account.account.template: l10n_hr_euro.hr_291000
+DEL account.account.template: l10n_hr_euro.hr_292000
+DEL account.account.template: l10n_hr_euro.hr_293000
+DEL account.account.template: l10n_hr_euro.hr_294000
+DEL account.account.template: l10n_hr_euro.hr_295000
+DEL account.account.template: l10n_hr_euro.hr_296000
+DEL account.account.template: l10n_hr_euro.hr_297000
+DEL account.account.template: l10n_hr_euro.hr_298000
+DEL account.account.template: l10n_hr_euro.hr_299000
+DEL account.account.template: l10n_hr_euro.hr_300000
+DEL account.account.template: l10n_hr_euro.hr_301000
+DEL account.account.template: l10n_hr_euro.hr_302000
+DEL account.account.template: l10n_hr_euro.hr_303000
+DEL account.account.template: l10n_hr_euro.hr_309000
+DEL account.account.template: l10n_hr_euro.hr_310000
+DEL account.account.template: l10n_hr_euro.hr_311000
+DEL account.account.template: l10n_hr_euro.hr_312000
+DEL account.account.template: l10n_hr_euro.hr_313000
+DEL account.account.template: l10n_hr_euro.hr_318000
+DEL account.account.template: l10n_hr_euro.hr_319000
+DEL account.account.template: l10n_hr_euro.hr_320000
+DEL account.account.template: l10n_hr_euro.hr_328000
+DEL account.account.template: l10n_hr_euro.hr_329000
+DEL account.account.template: l10n_hr_euro.hr_350000
+DEL account.account.template: l10n_hr_euro.hr_351000
+DEL account.account.template: l10n_hr_euro.hr_352000
+DEL account.account.template: l10n_hr_euro.hr_358000
+DEL account.account.template: l10n_hr_euro.hr_359000
+DEL account.account.template: l10n_hr_euro.hr_360000
+DEL account.account.template: l10n_hr_euro.hr_361000
+DEL account.account.template: l10n_hr_euro.hr_362000
+DEL account.account.template: l10n_hr_euro.hr_363000
+DEL account.account.template: l10n_hr_euro.hr_364000
+DEL account.account.template: l10n_hr_euro.hr_365000
+DEL account.account.template: l10n_hr_euro.hr_369000
+DEL account.account.template: l10n_hr_euro.hr_370000
+DEL account.account.template: l10n_hr_euro.hr_371000
+DEL account.account.template: l10n_hr_euro.hr_372000
+DEL account.account.template: l10n_hr_euro.hr_373000
+DEL account.account.template: l10n_hr_euro.hr_374000
+DEL account.account.template: l10n_hr_euro.hr_379000
+DEL account.account.template: l10n_hr_euro.hr_400000
+DEL account.account.template: l10n_hr_euro.hr_401000
+DEL account.account.template: l10n_hr_euro.hr_402000
+DEL account.account.template: l10n_hr_euro.hr_403000
+DEL account.account.template: l10n_hr_euro.hr_404000
+DEL account.account.template: l10n_hr_euro.hr_405000
+DEL account.account.template: l10n_hr_euro.hr_406000
+DEL account.account.template: l10n_hr_euro.hr_407000
+DEL account.account.template: l10n_hr_euro.hr_408000
+DEL account.account.template: l10n_hr_euro.hr_409000
+DEL account.account.template: l10n_hr_euro.hr_410000
+DEL account.account.template: l10n_hr_euro.hr_411000
+DEL account.account.template: l10n_hr_euro.hr_412000
+DEL account.account.template: l10n_hr_euro.hr_413000
+DEL account.account.template: l10n_hr_euro.hr_414000
+DEL account.account.template: l10n_hr_euro.hr_415000
+DEL account.account.template: l10n_hr_euro.hr_416000
+DEL account.account.template: l10n_hr_euro.hr_417000
+DEL account.account.template: l10n_hr_euro.hr_418000
+DEL account.account.template: l10n_hr_euro.hr_419000
+DEL account.account.template: l10n_hr_euro.hr_420000
+DEL account.account.template: l10n_hr_euro.hr_421000
+DEL account.account.template: l10n_hr_euro.hr_422000
+DEL account.account.template: l10n_hr_euro.hr_423000
+DEL account.account.template: l10n_hr_euro.hr_424000
+DEL account.account.template: l10n_hr_euro.hr_430000
+DEL account.account.template: l10n_hr_euro.hr_431000
+DEL account.account.template: l10n_hr_euro.hr_432000
+DEL account.account.template: l10n_hr_euro.hr_433000
+DEL account.account.template: l10n_hr_euro.hr_434000
+DEL account.account.template: l10n_hr_euro.hr_435000
+DEL account.account.template: l10n_hr_euro.hr_436000
+DEL account.account.template: l10n_hr_euro.hr_440000
+DEL account.account.template: l10n_hr_euro.hr_441000
+DEL account.account.template: l10n_hr_euro.hr_442000
+DEL account.account.template: l10n_hr_euro.hr_444000
+DEL account.account.template: l10n_hr_euro.hr_445000
+DEL account.account.template: l10n_hr_euro.hr_446000
+DEL account.account.template: l10n_hr_euro.hr_447000
+DEL account.account.template: l10n_hr_euro.hr_448000
+DEL account.account.template: l10n_hr_euro.hr_449000
+DEL account.account.template: l10n_hr_euro.hr_450000
+DEL account.account.template: l10n_hr_euro.hr_451000
+DEL account.account.template: l10n_hr_euro.hr_452000
+DEL account.account.template: l10n_hr_euro.hr_453000
+DEL account.account.template: l10n_hr_euro.hr_454000
+DEL account.account.template: l10n_hr_euro.hr_455000
+DEL account.account.template: l10n_hr_euro.hr_456000
+DEL account.account.template: l10n_hr_euro.hr_457000
+DEL account.account.template: l10n_hr_euro.hr_460000
+DEL account.account.template: l10n_hr_euro.hr_461000
+DEL account.account.template: l10n_hr_euro.hr_462000
+DEL account.account.template: l10n_hr_euro.hr_463000
+DEL account.account.template: l10n_hr_euro.hr_464000
+DEL account.account.template: l10n_hr_euro.hr_465000
+DEL account.account.template: l10n_hr_euro.hr_466000
+DEL account.account.template: l10n_hr_euro.hr_467000
+DEL account.account.template: l10n_hr_euro.hr_468000
+DEL account.account.template: l10n_hr_euro.hr_469000
+DEL account.account.template: l10n_hr_euro.hr_470000
+DEL account.account.template: l10n_hr_euro.hr_471000
+DEL account.account.template: l10n_hr_euro.hr_472000
+DEL account.account.template: l10n_hr_euro.hr_473000
+DEL account.account.template: l10n_hr_euro.hr_474000
+DEL account.account.template: l10n_hr_euro.hr_475000
+DEL account.account.template: l10n_hr_euro.hr_476000
+DEL account.account.template: l10n_hr_euro.hr_477000
+DEL account.account.template: l10n_hr_euro.hr_478000
+DEL account.account.template: l10n_hr_euro.hr_478200
+DEL account.account.template: l10n_hr_euro.hr_479000
+DEL account.account.template: l10n_hr_euro.hr_480000
+DEL account.account.template: l10n_hr_euro.hr_481000
+DEL account.account.template: l10n_hr_euro.hr_482000
+DEL account.account.template: l10n_hr_euro.hr_483000
+DEL account.account.template: l10n_hr_euro.hr_484000
+DEL account.account.template: l10n_hr_euro.hr_485000
+DEL account.account.template: l10n_hr_euro.hr_486000
+DEL account.account.template: l10n_hr_euro.hr_487000
+DEL account.account.template: l10n_hr_euro.hr_488000
+DEL account.account.template: l10n_hr_euro.hr_489000
+DEL account.account.template: l10n_hr_euro.hr_490000
+DEL account.account.template: l10n_hr_euro.hr_491000
+DEL account.account.template: l10n_hr_euro.hr_500000
+DEL account.account.template: l10n_hr_euro.hr_501000
+DEL account.account.template: l10n_hr_euro.hr_502000
+DEL account.account.template: l10n_hr_euro.hr_505000
+DEL account.account.template: l10n_hr_euro.hr_510000
+DEL account.account.template: l10n_hr_euro.hr_511000
+DEL account.account.template: l10n_hr_euro.hr_512000
+DEL account.account.template: l10n_hr_euro.hr_513000
+DEL account.account.template: l10n_hr_euro.hr_515000
+DEL account.account.template: l10n_hr_euro.hr_590000
+DEL account.account.template: l10n_hr_euro.hr_591000
+DEL account.account.template: l10n_hr_euro.hr_600000
+DEL account.account.template: l10n_hr_euro.hr_601000
+DEL account.account.template: l10n_hr_euro.hr_602000
+DEL account.account.template: l10n_hr_euro.hr_605000
+DEL account.account.template: l10n_hr_euro.hr_606000
+DEL account.account.template: l10n_hr_euro.hr_607000
+DEL account.account.template: l10n_hr_euro.hr_608000
+DEL account.account.template: l10n_hr_euro.hr_609000
+DEL account.account.template: l10n_hr_euro.hr_610000
+DEL account.account.template: l10n_hr_euro.hr_611000
+DEL account.account.template: l10n_hr_euro.hr_619000
+DEL account.account.template: l10n_hr_euro.hr_620000
+DEL account.account.template: l10n_hr_euro.hr_621000
+DEL account.account.template: l10n_hr_euro.hr_629000
+DEL account.account.template: l10n_hr_euro.hr_630000
+DEL account.account.template: l10n_hr_euro.hr_631000
+DEL account.account.template: l10n_hr_euro.hr_632000
+DEL account.account.template: l10n_hr_euro.hr_633000
+DEL account.account.template: l10n_hr_euro.hr_634000
+DEL account.account.template: l10n_hr_euro.hr_635000
+DEL account.account.template: l10n_hr_euro.hr_636000
+DEL account.account.template: l10n_hr_euro.hr_637000
+DEL account.account.template: l10n_hr_euro.hr_638000
+DEL account.account.template: l10n_hr_euro.hr_639000
+DEL account.account.template: l10n_hr_euro.hr_640000
+DEL account.account.template: l10n_hr_euro.hr_641000
+DEL account.account.template: l10n_hr_euro.hr_648000
+DEL account.account.template: l10n_hr_euro.hr_649000
+DEL account.account.template: l10n_hr_euro.hr_660000
+DEL account.account.template: l10n_hr_euro.hr_661000
+DEL account.account.template: l10n_hr_euro.hr_662000
+DEL account.account.template: l10n_hr_euro.hr_663000
+DEL account.account.template: l10n_hr_euro.hr_664000
+DEL account.account.template: l10n_hr_euro.hr_665000
+DEL account.account.template: l10n_hr_euro.hr_666000
+DEL account.account.template: l10n_hr_euro.hr_667000
+DEL account.account.template: l10n_hr_euro.hr_668000
+DEL account.account.template: l10n_hr_euro.hr_669000
+DEL account.account.template: l10n_hr_euro.hr_670000
+DEL account.account.template: l10n_hr_euro.hr_671000
+DEL account.account.template: l10n_hr_euro.hr_672000
+DEL account.account.template: l10n_hr_euro.hr_673000
+DEL account.account.template: l10n_hr_euro.hr_679000
+DEL account.account.template: l10n_hr_euro.hr_680000
+DEL account.account.template: l10n_hr_euro.hr_681000
+DEL account.account.template: l10n_hr_euro.hr_682000
+DEL account.account.template: l10n_hr_euro.hr_683000
+DEL account.account.template: l10n_hr_euro.hr_684000
+DEL account.account.template: l10n_hr_euro.hr_685000
+DEL account.account.template: l10n_hr_euro.hr_687000
+DEL account.account.template: l10n_hr_euro.hr_688000
+DEL account.account.template: l10n_hr_euro.hr_689000
+DEL account.account.template: l10n_hr_euro.hr_690000
+DEL account.account.template: l10n_hr_euro.hr_691000
+DEL account.account.template: l10n_hr_euro.hr_699000
+DEL account.account.template: l10n_hr_euro.hr_700000
+DEL account.account.template: l10n_hr_euro.hr_701000
+DEL account.account.template: l10n_hr_euro.hr_702000
+DEL account.account.template: l10n_hr_euro.hr_703000
+DEL account.account.template: l10n_hr_euro.hr_704000
+DEL account.account.template: l10n_hr_euro.hr_705000
+DEL account.account.template: l10n_hr_euro.hr_706000
+DEL account.account.template: l10n_hr_euro.hr_707000
+DEL account.account.template: l10n_hr_euro.hr_708000
+DEL account.account.template: l10n_hr_euro.hr_710000
+DEL account.account.template: l10n_hr_euro.hr_711000
+DEL account.account.template: l10n_hr_euro.hr_712000
+DEL account.account.template: l10n_hr_euro.hr_713000
+DEL account.account.template: l10n_hr_euro.hr_714000
+DEL account.account.template: l10n_hr_euro.hr_715000
+DEL account.account.template: l10n_hr_euro.hr_718000
+DEL account.account.template: l10n_hr_euro.hr_719000
+DEL account.account.template: l10n_hr_euro.hr_720000
+DEL account.account.template: l10n_hr_euro.hr_721000
+DEL account.account.template: l10n_hr_euro.hr_730000
+DEL account.account.template: l10n_hr_euro.hr_731000
+DEL account.account.template: l10n_hr_euro.hr_732000
+DEL account.account.template: l10n_hr_euro.hr_733000
+DEL account.account.template: l10n_hr_euro.hr_734000
+DEL account.account.template: l10n_hr_euro.hr_735000
+DEL account.account.template: l10n_hr_euro.hr_736000
+DEL account.account.template: l10n_hr_euro.hr_737000
+DEL account.account.template: l10n_hr_euro.hr_738000
+DEL account.account.template: l10n_hr_euro.hr_740000
+DEL account.account.template: l10n_hr_euro.hr_740100
+DEL account.account.template: l10n_hr_euro.hr_745000
+DEL account.account.template: l10n_hr_euro.hr_745100
+DEL account.account.template: l10n_hr_euro.hr_750000
+DEL account.account.template: l10n_hr_euro.hr_751000
+DEL account.account.template: l10n_hr_euro.hr_752000
+DEL account.account.template: l10n_hr_euro.hr_753000
+DEL account.account.template: l10n_hr_euro.hr_754000
+DEL account.account.template: l10n_hr_euro.hr_755000
+DEL account.account.template: l10n_hr_euro.hr_756000
+DEL account.account.template: l10n_hr_euro.hr_757000
+DEL account.account.template: l10n_hr_euro.hr_758000
+DEL account.account.template: l10n_hr_euro.hr_759000
+DEL account.account.template: l10n_hr_euro.hr_760000
+DEL account.account.template: l10n_hr_euro.hr_761000
+DEL account.account.template: l10n_hr_euro.hr_762000
+DEL account.account.template: l10n_hr_euro.hr_763000
+DEL account.account.template: l10n_hr_euro.hr_764000
+DEL account.account.template: l10n_hr_euro.hr_765000
+DEL account.account.template: l10n_hr_euro.hr_766000
+DEL account.account.template: l10n_hr_euro.hr_767000
+DEL account.account.template: l10n_hr_euro.hr_768000
+DEL account.account.template: l10n_hr_euro.hr_769000
+DEL account.account.template: l10n_hr_euro.hr_770000
+DEL account.account.template: l10n_hr_euro.hr_770100
+DEL account.account.template: l10n_hr_euro.hr_770200
+DEL account.account.template: l10n_hr_euro.hr_770300
+DEL account.account.template: l10n_hr_euro.hr_771000
+DEL account.account.template: l10n_hr_euro.hr_772000
+DEL account.account.template: l10n_hr_euro.hr_773000
+DEL account.account.template: l10n_hr_euro.hr_774000
+DEL account.account.template: l10n_hr_euro.hr_775000
+DEL account.account.template: l10n_hr_euro.hr_776000
+DEL account.account.template: l10n_hr_euro.hr_777000
+DEL account.account.template: l10n_hr_euro.hr_778000
+DEL account.account.template: l10n_hr_euro.hr_779000
+DEL account.account.template: l10n_hr_euro.hr_780000
+DEL account.account.template: l10n_hr_euro.hr_780900
+DEL account.account.template: l10n_hr_euro.hr_781000
+DEL account.account.template: l10n_hr_euro.hr_782000
+DEL account.account.template: l10n_hr_euro.hr_783000
+DEL account.account.template: l10n_hr_euro.hr_783900
+DEL account.account.template: l10n_hr_euro.hr_784000
+DEL account.account.template: l10n_hr_euro.hr_785000
+DEL account.account.template: l10n_hr_euro.hr_786000
+DEL account.account.template: l10n_hr_euro.hr_787000
+DEL account.account.template: l10n_hr_euro.hr_788000
+DEL account.account.template: l10n_hr_euro.hr_789000
+DEL account.account.template: l10n_hr_euro.hr_803000
+DEL account.account.template: l10n_hr_euro.hr_900000
+DEL account.account.template: l10n_hr_euro.hr_901000
+DEL account.account.template: l10n_hr_euro.hr_902000
+DEL account.account.template: l10n_hr_euro.hr_903000
+DEL account.account.template: l10n_hr_euro.hr_904000
+DEL account.account.template: l10n_hr_euro.hr_905000
+DEL account.account.template: l10n_hr_euro.hr_906000
+DEL account.account.template: l10n_hr_euro.hr_910000
+DEL account.account.template: l10n_hr_euro.hr_911000
+DEL account.account.template: l10n_hr_euro.hr_912000
+DEL account.account.template: l10n_hr_euro.hr_913000
+DEL account.account.template: l10n_hr_euro.hr_914000
+DEL account.account.template: l10n_hr_euro.hr_915000
+DEL account.account.template: l10n_hr_euro.hr_916000
+DEL account.account.template: l10n_hr_euro.hr_917000
+DEL account.account.template: l10n_hr_euro.hr_918000
+DEL account.account.template: l10n_hr_euro.hr_919000
+DEL account.account.template: l10n_hr_euro.hr_920000
+DEL account.account.template: l10n_hr_euro.hr_921000
+DEL account.account.template: l10n_hr_euro.hr_922000
+DEL account.account.template: l10n_hr_euro.hr_923000
+DEL account.account.template: l10n_hr_euro.hr_924000
+DEL account.account.template: l10n_hr_euro.hr_930000
+DEL account.account.template: l10n_hr_euro.hr_931000
+DEL account.account.template: l10n_hr_euro.hr_931200
+DEL account.account.template: l10n_hr_euro.hr_931300
+DEL account.account.template: l10n_hr_euro.hr_932000
+DEL account.account.template: l10n_hr_euro.hr_933000
+DEL account.account.template: l10n_hr_euro.hr_934000
+DEL account.account.template: l10n_hr_euro.hr_935000
+DEL account.account.template: l10n_hr_euro.hr_940000
+DEL account.account.template: l10n_hr_euro.hr_941000
+DEL account.account.template: l10n_hr_euro.hr_960000
+DEL account.account.template: l10n_hr_euro.hr_990000
+DEL account.account.template: l10n_hr_euro.hr_991000
+DEL account.account.template: l10n_hr_euro.hr_992000
+DEL account.account.template: l10n_hr_euro.hr_993000
+DEL account.account.template: l10n_hr_euro.hr_994000
+DEL account.account.template: l10n_hr_euro.hr_995000
+DEL account.account.template: l10n_hr_euro.hr_996000
+DEL account.account.template: l10n_hr_euro.hr_997000
+DEL account.account.template: l10n_hr_euro.hr_998000
+DEL account.account.template: l10n_hr_euro.hr_999000
+DEL account.chart.template: l10n_hr_euro.l10n_hr_euro_chart_template
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_P_G_hr_eu_1
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_P_G_hr_eu_2
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_P_G_hr_eu_3
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_S_G_hr_eu_1
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_S_G_hr_eu_2
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_S_G_hr_eu_3
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_exempt_tax_1
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_exempt_tax_2
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_exempt_tax_3
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_out_eu_1
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_out_eu_2
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_out_eu_3
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_exempt_tax_1
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_exempt_tax_2
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_exempt_tax_3
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_out_eu_1
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_out_eu_2
+DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_out_eu_3
+DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_eu (noupdate)
+DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_eu_out (noupdate)
+DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_exempt (noupdate)
+DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_national (noupdate)
+DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_person_private (noupdate)
+DEL account.group.template: l10n_hr_euro.hr_group_0
+DEL account.group.template: l10n_hr_euro.hr_group_00
+DEL account.group.template: l10n_hr_euro.hr_group_01
+DEL account.group.template: l10n_hr_euro.hr_group_02
+DEL account.group.template: l10n_hr_euro.hr_group_03
+DEL account.group.template: l10n_hr_euro.hr_group_04
+DEL account.group.template: l10n_hr_euro.hr_group_05
+DEL account.group.template: l10n_hr_euro.hr_group_06
+DEL account.group.template: l10n_hr_euro.hr_group_07
+DEL account.group.template: l10n_hr_euro.hr_group_08
+DEL account.group.template: l10n_hr_euro.hr_group_1
+DEL account.group.template: l10n_hr_euro.hr_group_10
+DEL account.group.template: l10n_hr_euro.hr_group_11
+DEL account.group.template: l10n_hr_euro.hr_group_12
+DEL account.group.template: l10n_hr_euro.hr_group_13
+DEL account.group.template: l10n_hr_euro.hr_group_14
+DEL account.group.template: l10n_hr_euro.hr_group_15
+DEL account.group.template: l10n_hr_euro.hr_group_19
+DEL account.group.template: l10n_hr_euro.hr_group_2
+DEL account.group.template: l10n_hr_euro.hr_group_20
+DEL account.group.template: l10n_hr_euro.hr_group_21
+DEL account.group.template: l10n_hr_euro.hr_group_22
+DEL account.group.template: l10n_hr_euro.hr_group_23
+DEL account.group.template: l10n_hr_euro.hr_group_24
+DEL account.group.template: l10n_hr_euro.hr_group_25
+DEL account.group.template: l10n_hr_euro.hr_group_26
+DEL account.group.template: l10n_hr_euro.hr_group_28
+DEL account.group.template: l10n_hr_euro.hr_group_29
+DEL account.group.template: l10n_hr_euro.hr_group_3
+DEL account.group.template: l10n_hr_euro.hr_group_30
+DEL account.group.template: l10n_hr_euro.hr_group_31
+DEL account.group.template: l10n_hr_euro.hr_group_32
+DEL account.group.template: l10n_hr_euro.hr_group_35
+DEL account.group.template: l10n_hr_euro.hr_group_36
+DEL account.group.template: l10n_hr_euro.hr_group_37
+DEL account.group.template: l10n_hr_euro.hr_group_4
+DEL account.group.template: l10n_hr_euro.hr_group_40
+DEL account.group.template: l10n_hr_euro.hr_group_41
+DEL account.group.template: l10n_hr_euro.hr_group_42
+DEL account.group.template: l10n_hr_euro.hr_group_43
+DEL account.group.template: l10n_hr_euro.hr_group_44
+DEL account.group.template: l10n_hr_euro.hr_group_45
+DEL account.group.template: l10n_hr_euro.hr_group_46
+DEL account.group.template: l10n_hr_euro.hr_group_47
+DEL account.group.template: l10n_hr_euro.hr_group_48
+DEL account.group.template: l10n_hr_euro.hr_group_49
+DEL account.group.template: l10n_hr_euro.hr_group_5
+DEL account.group.template: l10n_hr_euro.hr_group_50
+DEL account.group.template: l10n_hr_euro.hr_group_51
+DEL account.group.template: l10n_hr_euro.hr_group_52
+DEL account.group.template: l10n_hr_euro.hr_group_53
+DEL account.group.template: l10n_hr_euro.hr_group_54
+DEL account.group.template: l10n_hr_euro.hr_group_59
+DEL account.group.template: l10n_hr_euro.hr_group_6
+DEL account.group.template: l10n_hr_euro.hr_group_60
+DEL account.group.template: l10n_hr_euro.hr_group_61
+DEL account.group.template: l10n_hr_euro.hr_group_62
+DEL account.group.template: l10n_hr_euro.hr_group_63
+DEL account.group.template: l10n_hr_euro.hr_group_64
+DEL account.group.template: l10n_hr_euro.hr_group_65
+DEL account.group.template: l10n_hr_euro.hr_group_66
+DEL account.group.template: l10n_hr_euro.hr_group_67
+DEL account.group.template: l10n_hr_euro.hr_group_68
+DEL account.group.template: l10n_hr_euro.hr_group_69
+DEL account.group.template: l10n_hr_euro.hr_group_7
+DEL account.group.template: l10n_hr_euro.hr_group_70
+DEL account.group.template: l10n_hr_euro.hr_group_71
+DEL account.group.template: l10n_hr_euro.hr_group_72
+DEL account.group.template: l10n_hr_euro.hr_group_73
+DEL account.group.template: l10n_hr_euro.hr_group_74
+DEL account.group.template: l10n_hr_euro.hr_group_75
+DEL account.group.template: l10n_hr_euro.hr_group_76
+DEL account.group.template: l10n_hr_euro.hr_group_77
+DEL account.group.template: l10n_hr_euro.hr_group_78
+DEL account.group.template: l10n_hr_euro.hr_group_79
+DEL account.group.template: l10n_hr_euro.hr_group_8
+DEL account.group.template: l10n_hr_euro.hr_group_80
+DEL account.group.template: l10n_hr_euro.hr_group_81
+DEL account.group.template: l10n_hr_euro.hr_group_82
+DEL account.group.template: l10n_hr_euro.hr_group_83
+DEL account.group.template: l10n_hr_euro.hr_group_9
+DEL account.group.template: l10n_hr_euro.hr_group_90
+DEL account.group.template: l10n_hr_euro.hr_group_91
+DEL account.group.template: l10n_hr_euro.hr_group_92
+DEL account.group.template: l10n_hr_euro.hr_group_93
+DEL account.group.template: l10n_hr_euro.hr_group_94
+DEL account.group.template: l10n_hr_euro.hr_group_95
+DEL account.group.template: l10n_hr_euro.hr_group_96
+DEL account.group.template: l10n_hr_euro.hr_group_99
+DEL account.report: l10n_hr_euro.tax_report [renamed to l10n_rw module]
+DEL account.report.column: l10n_hr_euro.tax_report_tax_amount [renamed to l10n_hr module]
+DEL account.report.column: l10n_hr_euro.tax_report_tax_base [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_0_0_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_0_0_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_0_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_0_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_10_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_10_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_11_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_11_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_12_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_12_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_13_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_13_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_14_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_14_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_15_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_1_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_1_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_2_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_2_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_3_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_3_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_4_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_4_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_5_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_5_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_6_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_6_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_7_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_7_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_8_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_8_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_9_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_III_9_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_0_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_0_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_10_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_10_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_11_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_11_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_12_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_12_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_13_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_13_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_14_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_14_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_15_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_15_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_1_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_1_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_2_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_2_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_3_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_3_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_4_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_4_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_5_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_5_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_6_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_6_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_7_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_7_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_8_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_8_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_9_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_II_9_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_IV_0_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_IV_1_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_IV_2_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_0_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_10_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_1_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_2_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_3_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_4_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_5_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_6_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_7_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_8_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_I_9_tag_column1 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_VI_0_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_VI_1_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_VI_2_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_V_0_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_V_1_tag_column2 [renamed to l10n_hr module]
+DEL account.report.expression: l10n_hr_euro.tax_report_line_V_2_tag_column2 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_1 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_10 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_11 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_12 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_13 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_14 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_15 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_2 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_3 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_4 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_5 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_6 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_7 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_8 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_III_9 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_1 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_10 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_11 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_12 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_13 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_14 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_15 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_2 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_3 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_4 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_5 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_6 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_7 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_8 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_II_9 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_IV_1 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_IV_2 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_1 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_10 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_2 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_3 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_4 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_5 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_6 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_7 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_8 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_I_9 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_VI_1 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_VI_2 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_V_1 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_line_V_2 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_title_annual_deductible [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_title_calculed_vat [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_title_prev_calculation [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_title_total_dif [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_title_transactions0 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_title_transactions1 [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_title_vat_calculation [renamed to l10n_hr module]
+DEL account.report.line: l10n_hr_euro.tax_report_title_vat_liab [renamed to l10n_hr module]
+DEL account.tax.group: l10n_hr_euro.tax_group_pdv_0
+DEL account.tax.group: l10n_hr_euro.tax_group_pdv_13
+DEL account.tax.group: l10n_hr_euro.tax_group_pdv_25
+DEL account.tax.group: l10n_hr_euro.tax_group_pdv_5
+DEL account.tax.template: l10n_hr_euro.VAT_P_G_IN_EU_13
+DEL account.tax.template: l10n_hr_euro.VAT_P_G_IN_EU_25
+DEL account.tax.template: l10n_hr_euro.VAT_P_G_IN_EU_5
+DEL account.tax.template: l10n_hr_euro.VAT_P_IN_ROC_13
+DEL account.tax.template: l10n_hr_euro.VAT_P_IN_ROC_25
+DEL account.tax.template: l10n_hr_euro.VAT_P_IN_ROC_5
+DEL account.tax.template: l10n_hr_euro.VAT_P_NOT_IN_EU_13
+DEL account.tax.template: l10n_hr_euro.VAT_P_NOT_IN_EU_25
+DEL account.tax.template: l10n_hr_euro.VAT_P_NOT_IN_EU_5
+DEL account.tax.template: l10n_hr_euro.VAT_P_O
+DEL account.tax.template: l10n_hr_euro.VAT_P_S_IN_EU_13
+DEL account.tax.template: l10n_hr_euro.VAT_P_S_IN_EU_25
+DEL account.tax.template: l10n_hr_euro.VAT_P_S_IN_EU_5
+DEL account.tax.template: l10n_hr_euro.VAT_P_install_assemb_goods_O
+DEL account.tax.template: l10n_hr_euro.VAT_P_reverse_charge
+DEL account.tax.template: l10n_hr_euro.VAT_S_EU_G
+DEL account.tax.template: l10n_hr_euro.VAT_S_EU_S
+DEL account.tax.template: l10n_hr_euro.VAT_S_EX_O
+DEL account.tax.template: l10n_hr_euro.VAT_S_IN_ROC_13
+DEL account.tax.template: l10n_hr_euro.VAT_S_IN_ROC_25
+DEL account.tax.template: l10n_hr_euro.VAT_S_IN_ROC_5
+DEL account.tax.template: l10n_hr_euro.VAT_S_TAX_PERSON_13%
+DEL account.tax.template: l10n_hr_euro.VAT_S_TAX_PERSON_25%
+DEL account.tax.template: l10n_hr_euro.VAT_S_TAX_PERSON_5%
+DEL account.tax.template: l10n_hr_euro.VAT_S_carried_other_state_O
+DEL account.tax.template: l10n_hr_euro.VAT_S_new_transport_other_state_O
+DEL account.tax.template: l10n_hr_euro.VAT_S_other_exempt_O
+DEL account.tax.template: l10n_hr_euro.VAT_S_person_not_in_ROC_O
+DEL account.tax.template: l10n_hr_euro.VAT_S_reverse_O
+DEL ir.ui.menu: l10n_hr_euro.account_reports_hr_statements_menu [renamed to l10n_hr module]
+ERROR: module not in list of installed modules:
+---Models in module 'l10n_in_tcs_tds'---
+---Fields in module 'l10n_in_tcs_tds'---
+l10n_in_tcs_tds / res.partner              / l10n_in_pan (char)            : module is now 'l10n_in' ('l10n_in_tcs_tds')
+l10n_in_tcs_tds / res.users                / l10n_in_pan (char)            : module is now 'l10n_in' ('l10n_in_tcs_tds')
+---XML records in module 'l10n_in_tcs_tds'---
+DEL account.account.template: l10n_in_tcs_tds.p11244
+DEL account.account.template: l10n_in_tcs_tds.p11245
+DEL account.report: l10n_in_tcs_tds.tcs_report [renamed to l10n_in module]
+DEL account.report: l10n_in_tcs_tds.tds_report [renamed to l10n_in module]
+DEL account.report.column: l10n_in_tcs_tds.tcs_report_balance [renamed to l10n_in module]
+DEL account.report.column: l10n_in_tcs_tds.tds_report_balance [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_alfhc_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_aofpnbtotl_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_mbcoloio_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_s_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_tl_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_tobaotuafl_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_touafl_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_maq_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_pl_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_tp_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1f_mv_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1g_soaotpp_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1g_som_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1h_sog_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_192_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_192a_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_193_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194a_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194b_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194bb_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194c_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194d_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194da_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194e_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194ee_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194f_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194g_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194h_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194i_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194ia_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194ib_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194ic_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194j_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194k_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194la_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194lb_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194lba_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194lbb_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194lbc_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194m_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194n_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194o_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194q_tag [renamed to l10n_in module]
+DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_195_tag [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_alfhc [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_aofpnbtotl [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_mbcoloio [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_s [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_tl [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_tobaotuafl [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_touafl [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_maq [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_pl [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_tp [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1f_mv [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1g_soaotpp [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1g_som [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1h_sog [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_192 [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_192a [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_193 [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194 [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194a [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194b [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194bb [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194c [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194d [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194da [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194e [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194ee [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194f [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194g [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194h [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194i [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194ia [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194ib [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194ic [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194j [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194k [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194la [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194lb [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194lba [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194lbb [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194lbc [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194m [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194n [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194o [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194q [renamed to l10n_in module]
+DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_195 [renamed to l10n_in module]
+DEL account.tax.group: l10n_in_tcs_tds.tcs_group (noupdate)
+DEL account.tax.group: l10n_in_tcs_tds.tds_group (noupdate)
+DEL account.tax.template: l10n_in_tcs_tds.tcs_0_1_us_206c_1h_sog
+DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1_alfhc
+DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1_mbcoloio
+DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1_s
+DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1f_mv
+DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1h_sog
+DEL account.tax.template: l10n_in_tcs_tds.tcs_2_5_us_206c_1_aofpnbtotl
+DEL account.tax.template: l10n_in_tcs_tds.tcs_2_5_us_206c_1_tobamotuafl
+DEL account.tax.template: l10n_in_tcs_tds.tcs_2_5_us_206c_1_touafl
+DEL account.tax.template: l10n_in_tcs_tds.tcs_2_us_206c_1c_maq
+DEL account.tax.template: l10n_in_tcs_tds.tcs_2_us_206c_1c_pl
+DEL account.tax.template: l10n_in_tcs_tds.tcs_2_us_206c_1c_tp
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_alfhc
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_aofpnbtotl
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_mbcoloio
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_s
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_tl
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_tobamotuafl
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_touafl
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1c_maq
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1c_pl
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1c_tp
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1f_mv
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1g_soaotpp
+DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1g_som
+DEL account.tax.template: l10n_in_tcs_tds.tds_01_us_194q
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_4_us_195
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_192a
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_193
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194a
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194d
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194ee
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194i
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194ic
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194j
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194k
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194la
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194lba
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194lbb
+DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194lbc
+DEL account.tax.template: l10n_in_tcs_tds.tds_15_6_us_195
+DEL account.tax.template: l10n_in_tcs_tds.tds_1_us_194c
+DEL account.tax.template: l10n_in_tcs_tds.tds_1_us_194ia
+DEL account.tax.template: l10n_in_tcs_tds.tds_1_us_194o
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_8_us_195
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_192a
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_193
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194a
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194c
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194d
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194da
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194e
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194ee
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194f
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194g
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194h
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194i
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194ia
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194ib
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194ic
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194j
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194k
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194la
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194lb
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194lba
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194lbb
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194m
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194n
+DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194o
+DEL account.tax.template: l10n_in_tcs_tds.tds_25_us_194lbc
+DEL account.tax.template: l10n_in_tcs_tds.tds_2_us_194c
+DEL account.tax.template: l10n_in_tcs_tds.tds_2_us_194i
+DEL account.tax.template: l10n_in_tcs_tds.tds_2_us_194j
+DEL account.tax.template: l10n_in_tcs_tds.tds_2_us_194n
+DEL account.tax.template: l10n_in_tcs_tds.tds_30_us_194b
+DEL account.tax.template: l10n_in_tcs_tds.tds_30_us_194bb
+DEL account.tax.template: l10n_in_tcs_tds.tds_30_us_194lbc
+DEL account.tax.template: l10n_in_tcs_tds.tds_31_2_us_195
+DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194d
+DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194da
+DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194g
+DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194h
+DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194ib
+DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194lb
+DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194m
+DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194n
+DEL ir.ui.view: l10n_in_tcs_tds.l10n_in_tcs_tds_view_partner_form
+ERROR: module not in list of installed modules:
+---Models in module 'l10n_in_upi'---
+---Fields in module 'l10n_in_upi'---
+l10n_in_upi  / res.company              / l10n_in_upi_id (char)         : module is now 'l10n_in' ('l10n_in_upi')
+---XML records in module 'l10n_in_upi'---
+DEL ir.ui.view: l10n_in_upi.view_company_form
+ERROR: module not in list of installed modules:
 ---Models in module 'l10n_it_edi_pa'---
 ---Fields in module 'l10n_it_edi_pa'---
 l10n_it_edi_pa / account.bank.statement.line / l10n_it_cig (char)            : module is now 'l10n_it_edi' ('l10n_it_edi_pa')
 l10n_it_edi_pa / account.bank.statement.line / l10n_it_cup (char)            : module is now 'l10n_it_edi' ('l10n_it_edi_pa')
 l10n_it_edi_pa / account.bank.statement.line / l10n_it_origin_document_date (date): module is now 'l10n_it_edi' ('l10n_it_edi_pa')
 l10n_it_edi_pa / account.bank.statement.line / l10n_it_origin_document_name (char): module is now 'l10n_it_edi' ('l10n_it_edi_pa')
 l10n_it_edi_pa / account.bank.statement.line / l10n_it_origin_document_type (selection): module is now 'l10n_it_edi' ('l10n_it_edi_pa')
@@ -640,14 +4410,119 @@
 DEL l10n_pl_tax_office: l10n_pl_jpk.pl_tax_office_3271
 ERROR: module not in list of installed modules:
 ---Models in module 'l10n_pl_sale_stock'---
 ---Fields in module 'l10n_pl_sale_stock'---
 ---XML records in module 'l10n_pl_sale_stock'---
 ---nothing has changed in this module--
 ERROR: module not in list of installed modules:
+---Models in module 'loyalty_delivery'---
+---Fields in module 'loyalty_delivery'---
+loyalty_delivery / loyalty.reward           / reward_type (False)           : module is now 'sale_loyalty_delivery' ('loyalty_delivery')
+---XML records in module 'loyalty_delivery'---
+DEL ir.ui.view: loyalty_delivery.loyalty_reward_view_form_inherit_loyalty_delivery
+DEL ir.ui.view: loyalty_delivery.loyalty_reward_view_kanban_inherit_loyalty_delivery
+ERROR: module not in list of installed modules:
+---Models in module 'note'---
+obsolete model note.note
+obsolete model note.stage
+obsolete model note.tag
+---Fields in module 'note'---
+note         / mail.activity            / note_id (many2one)            : DEL relation: note.note
+note         / mail.activity.type       / category (False)              : module is now 'project_todo' ('note')
+note         / note.note                / activity_ids (one2many)       : DEL relation: mail.activity
+note         / note.note                / color (integer)               : DEL
+note         / note.note                / company_id (many2one)         : DEL relation: res.company
+note         / note.note                / date_done (date)              : DEL
+note         / note.note                / memo (html)                   : DEL
+note         / note.note                / message_follower_ids (one2many): DEL relation: mail.followers
+note         / note.note                / message_ids (one2many)        : DEL relation: mail.message
+note         / note.note                / message_main_attachment_id (many2one): DEL relation: ir.attachment
+note         / note.note                / name (text)                   : DEL
+note         / note.note                / open (boolean)                : DEL
+note         / note.note                / sequence (integer)            : DEL
+note         / note.note                / stage_ids (many2many)         : DEL relation: note.stage
+note         / note.note                / tag_ids (many2many)           : DEL relation: note.tag
+note         / note.note                / user_id (many2one)            : DEL relation: res.users
+note         / note.stage               / fold (boolean)                : DEL
+note         / note.stage               / name (char)                   : DEL required
+note         / note.stage               / sequence (integer)            : DEL
+note         / note.stage               / user_id (many2one)            : DEL relation: res.users, required
+note         / note.tag                 / color (integer)               : DEL
+note         / note.tag                 / name (char)                   : DEL required
+---XML records in module 'note'---
+DEL ir.actions.act_window: note.action_note_note
+DEL ir.actions.act_window: note.action_note_stage
+DEL ir.actions.act_window: note.note_tag_action
+DEL ir.model.access: note.access_note_note
+DEL ir.model.access: note.access_note_stage
+DEL ir.model.access: note.access_note_tag
+DEL ir.model.constraint: note.constraint_note_tag_name_uniq
+DEL ir.rule: note.ir_rule_note_note_multi_company (noupdate)
+DEL ir.rule: note.note_note_create_unlink_global (noupdate)
+DEL ir.rule: note.note_note_rule_global (noupdate)
+DEL ir.rule: note.note_stage_rule_global (noupdate)
+DEL ir.ui.menu: note.menu_note_configuration
+DEL ir.ui.menu: note.menu_note_notes
+DEL ir.ui.menu: note.menu_notes_stage
+DEL ir.ui.menu: note.notes_tag_menu
+DEL ir.ui.view: note.note_tag_view_form
+DEL ir.ui.view: note.note_tag_view_tree
+DEL ir.ui.view: note.view_note_note_filter
+DEL ir.ui.view: note.view_note_note_form
+DEL ir.ui.view: note.view_note_note_kanban
+DEL ir.ui.view: note.view_note_note_tree
+DEL ir.ui.view: note.view_note_stage_form
+DEL ir.ui.view: note.view_note_stage_tree
+DEL mail.activity.type: note.mail_activity_data_reminder [renamed to project_todo module] (noupdate)
+DEL note.stage: note.note_stage_00
+DEL note.stage: note.note_stage_01
+DEL note.stage: note.note_stage_02
+DEL note.stage: note.note_stage_03
+ERROR: module not in list of installed modules:
+---Models in module 'pos_cache'---
+obsolete model pos.cache
+---Fields in module 'pos_cache'---
+pos_cache    / pos.cache                / cache (binary)                : DEL attachment: True
+pos_cache    / pos.cache                / compute_user_id (many2one)    : DEL relation: res.users, required
+pos_cache    / pos.cache                / config_id (many2one)          : DEL relation: pos.config, required
+pos_cache    / pos.cache                / product_domain (text)         : DEL required
+pos_cache    / pos.cache                / product_fields (text)         : DEL required
+pos_cache    / pos.config               / cache_ids (one2many)          : DEL relation: pos.cache
+---XML records in module 'pos_cache'---
+DEL ir.cron: pos_cache.refresh_pos_cache_cron
+DEL ir.model.access: pos_cache.access_pos_cache
+DEL ir.ui.view: pos_cache.view_pos_config_kanban
+ERROR: module not in list of installed modules:
+---Models in module 'pos_daily_sales_reports'---
+model pos.daily.sales.reports.wizard (moved to point_of_sale) [column['model_type']]
+---Fields in module 'pos_daily_sales_reports'---
+pos_daily_sales_reports / pos.session              / closing_notes (text)          : module is now 'point_of_sale' ('pos_daily_sales_reports')
+---XML records in module 'pos_daily_sales_reports'---
+DEL ir.actions.act_window: pos_daily_sales_reports.action_report_pos_daily_sales_reports [renamed to point_of_sale module]
+DEL ir.model.access: pos_daily_sales_reports.access_pos_daily_sales_reports_wizard [renamed to point_of_sale module]
+DEL ir.ui.menu: pos_daily_sales_reports.menu_report_daily_details [renamed to point_of_sale module]
+DEL ir.ui.view: pos_daily_sales_reports.pos_daily_report
+DEL ir.ui.view: pos_daily_sales_reports.view_pos_daily_sales_reports_wizard
+ERROR: module not in list of installed modules:
+---Models in module 'pos_epson_printer_restaurant'---
+---Fields in module 'pos_epson_printer_restaurant'---
+pos_epson_printer_restaurant / restaurant.printer       / epson_printer_ip (char)       : DEL
+pos_epson_printer_restaurant / restaurant.printer       / printer_type (False)          : DEL selection_keys: ['epson_epos', 'iot'], mode: modify
+---XML records in module 'pos_epson_printer_restaurant'---
+DEL ir.ui.view: pos_epson_printer_restaurant.view_restaurant_printer_iot_form
+ERROR: module not in list of installed modules:
+---Models in module 'purchase_price_diff'---
+---Fields in module 'purchase_price_diff'---
+purchase_price_diff / product.category         / property_account_creditor_price_difference_categ (many2one): module is now 'purchase_stock' ('purchase_price_diff')
+purchase_price_diff / product.product          / property_account_creditor_price_difference (many2one): module is now 'purchase_stock' ('purchase_price_diff')
+purchase_price_diff / product.template         / property_account_creditor_price_difference (many2one): module is now 'purchase_stock' ('purchase_price_diff')
+---XML records in module 'purchase_price_diff'---
+DEL ir.ui.view: purchase_price_diff.product_template_form_view
+DEL ir.ui.view: purchase_price_diff.view_category_property_form
+ERROR: module not in list of installed modules:
 ---Models in module 'sale_quotation_builder'---
 ---Fields in module 'sale_quotation_builder'---
 sale_quotation_builder / product.template         / quotation_only_description (html): DEL
 sale_quotation_builder / sale.order               / website_description (html)    : DEL
 sale_quotation_builder / sale.order.line          / website_description (html)    : DEL
 sale_quotation_builder / sale.order.option        / website_description (html)    : DEL
 sale_quotation_builder / sale.order.template      / website_description (html)    : DEL
@@ -701,15 +4576,15 @@
 DEL ir.actions.act_window: website_event_questions.action_event_registration_report [renamed to website_event module]
 DEL ir.model.access: website_event_questions.access_event_question
 DEL ir.model.access: website_event_questions.access_event_question_answer
 DEL ir.model.access: website_event_questions.access_event_question_answer_registration [renamed to website_event module]
 DEL ir.model.access: website_event_questions.access_event_question_answer_user [renamed to website_event module]
 DEL ir.model.access: website_event_questions.access_event_question_user [renamed to website_event module]
 DEL ir.model.access: website_event_questions.access_event_registration_answer_registration
-DEL ir.model.constraint: website_event_questions.constraint_event_registration_answer_value_check
+DEL ir.model.constraint: website_event_questions.constraint_event_registration_answer_value_check [renamed to website_event module]
 DEL ir.rule: website_event_questions.ir_rule_event_question_answer_event_user [renamed to website_event module] (noupdate)
 DEL ir.rule: website_event_questions.ir_rule_event_question_answer_published [renamed to website_event module] (noupdate)
 DEL ir.rule: website_event_questions.ir_rule_event_question_event_user [renamed to website_event module] (noupdate)
 DEL ir.rule: website_event_questions.ir_rule_event_question_published [renamed to website_event module] (noupdate)
 DEL ir.ui.view: website_event_questions.event_event_view_form
 DEL ir.ui.view: website_event_questions.event_question_view_form
 DEL ir.ui.view: website_event_questions.event_registration_answer_view_graph
@@ -718,14 +4593,49 @@
 DEL ir.ui.view: website_event_questions.event_registration_answer_view_tree
 DEL ir.ui.view: website_event_questions.event_registration_view_form_inherit_question
 DEL ir.ui.view: website_event_questions.event_registration_view_tree
 DEL ir.ui.view: website_event_questions.event_type_view_form_inherit_question
 DEL ir.ui.view: website_event_questions.registration_attendee_details_questions
 DEL ir.ui.view: website_event_questions.registration_event_question
 ERROR: module not in list of installed modules:
+---Models in module 'website_sale_delivery'---
+---Fields in module 'website_sale_delivery'---
+website_sale_delivery / delivery.carrier         / can_publish (boolean)         : module is now 'website_sale' ('website_sale_delivery')
+website_sale_delivery / delivery.carrier         / is_published (boolean)        : module is now 'website_sale' ('website_sale_delivery')
+website_sale_delivery / delivery.carrier         / website_description (text)    : module is now 'website_sale' ('website_sale_delivery')
+website_sale_delivery / delivery.carrier         / website_id (many2one)         : module is now 'website_sale' ('website_sale_delivery')
+website_sale_delivery / delivery.carrier         / website_published (boolean)   : module is now 'website_sale' ('website_sale_delivery')
+website_sale_delivery / delivery.carrier         / website_url (char)            : module is now 'website_sale' ('website_sale_delivery')
+website_sale_delivery / sale.order               / amount_delivery (float)       : module is now 'website_sale' ('website_sale_delivery')
+website_sale_delivery / sale.order               / amount_delivery (float)       : not stored anymore
+---XML records in module 'website_sale_delivery'---
+DEL ir.ui.menu: website_sale_delivery.menu_ecommerce_delivery [renamed to website_sale module]
+DEL ir.ui.view: website_sale_delivery.cart_delivery
+DEL ir.ui.view: website_sale_delivery.payment_delivery
+DEL ir.ui.view: website_sale_delivery.payment_delivery_methods
+DEL ir.ui.view: website_sale_delivery.payment_delivery_shipping_method
+DEL ir.ui.view: website_sale_delivery.res_config_settings_view_form
+DEL ir.ui.view: website_sale_delivery.view_delivery_carrier_form_website_delivery
+DEL ir.ui.view: website_sale_delivery.view_delivery_carrier_search_inherit_website_sale_delivery
+DEL ir.ui.view: website_sale_delivery.view_delivery_carrier_tree_inherit_website_sale_delivery
+ERROR: module not in list of installed modules:
+---Models in module 'website_sale_delivery_mondialrelay'---
+---Fields in module 'website_sale_delivery_mondialrelay'---
+---XML records in module 'website_sale_delivery_mondialrelay'---
+DEL ir.ui.view: website_sale_delivery_mondialrelay.delivery_carrier_view_search_inherit_website_sale_delivery_mondialrelay
+DEL ir.ui.view: website_sale_delivery_mondialrelay.res_config_settings_view_form_inherit_website_sale_delivery_mondial_relay
+DEL ir.ui.view: website_sale_delivery_mondialrelay.website_sale_delivery_mondialrelay_address_kanban
+DEL ir.ui.view: website_sale_delivery_mondialrelay.website_sale_delivery_mondialrelay_address_on_payment
+DEL ir.ui.view: website_sale_delivery_mondialrelay.website_sale_delivery_mondialrelay_checkout
+ERROR: module not in list of installed modules:
 ---Models in module 'website_sale_digital'---
 ---Fields in module 'website_sale_digital'---
 website_sale_digital / ir.attachment            / product_downloadable (boolean): DEL
 ---XML records in module 'website_sale_digital'---
 DEL ir.ui.view: website_sale_digital.product_product_view_form_inherit_digital
 DEL ir.ui.view: website_sale_digital.product_template_view_form_inherit_digital
 DEL ir.ui.view: website_sale_digital.sale_order_portal_content_inherit_website_sale_digital
+ERROR: module not in list of installed modules:
+---Models in module 'website_sale_stock_product_configurator'---
+---Fields in module 'website_sale_stock_product_configurator'---
+---XML records in module 'website_sale_stock_product_configurator'---
+DEL ir.ui.view: website_sale_stock_product_configurator.website_sale_stock_modal
```

## odoo/addons/openupgrade_scripts/scripts/calendar/17.0.1.1/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/calendar/17.0.1.1/noupdate_changes.xml

```diff
@@ -1,162 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
-  <record id="calendar_template_meeting_changedate" model="mail.template">
-    <field name="body_html" type="html">
-      <div>
-        <t t-set="colors" t-value="{'needsAction': 'grey', 'accepted': 'green', 'tentative': '#FFFF00', 'declined': 'red'}"/>
-        <t t-set="is_online" t-value="'appointment_type_id' in object.event_id and object.event_id.appointment_type_id"/>
-        <t t-set="customer" t-value="object.event_id.find_partner_customer()"/>
-        <t t-set="target_responsible" t-value="object.partner_id == object.event_id.partner_id"/>
-        <t t-set="target_customer" t-value="object.partner_id == customer"/>
-        <t t-set="recurrent" t-value="object.recurrence_id and not ctx.get('calendar_template_ignore_recurrence')"/>
-        <p>
-          Hello
-          <t t-out="object.common_name or ''">Ready Mat</t>
-          ,
-          <br/>
-          <br/>
-          <t t-if="is_online and target_responsible">
-            <t t-if="customer">
-              The date of your appointment with
-              <t t-out="customer.name or ''">Jesse Brown</t>
-              has been updated.
-            </t>
-            <t t-else="">Your appointment has been updated.</t>
-            The appointment
-            <strong t-out="object.event_id.appointment_type_id.name or ''">Schedule a Demo</strong>
-            is now scheduled for
-            <t t-out="object.event_id.get_display_time_tz(tz=object.partner_id.tz) or ''">05/04/2021 at (11:00:00 To 11:30:00) (Europe/Brussels)</t>
-          </t>
-          <t t-elif="is_online and target_customer">
-            The date of your appointment with
-            <t t-out="object.event_id.user_id.partner_id.name or ''">Colleen Diaz</t>
-            has been updated.
-            The appointment
-            <strong t-out="object.event_id.appointment_type_id.name or ''"/>
-            is now scheduled for
-            <t t-out="object.event_id.get_display_time_tz(tz=object.partner_id.tz) or ''">05/04/2021 at (11:00:00 To 11:30:00) (Europe/Brussels)</t>
-            .
-          </t>
-          <t t-else="">
-            The date of the meeting has been updated.
-            The meeting
-            <strong t-out="object.event_id.name or ''">Follow-up for Project proposal</strong>
-            created by
-            <t t-out="object.event_id.user_id.partner_id.name or ''">Colleen Diaz</t>
-            is now scheduled for
-            <t t-out="object.event_id.get_display_time_tz(tz=object.partner_id.tz) or ''">05/04/2021 at (11:00:00 To 11:30:00) (Europe/Brussels)</t>
-            .
-          </t>
-        </p>
-        <div style="text-align: center; padding: 16px 0px 16px 0px;">
-          <a t-attf-href="/calendar/meeting/accept?token={{ object.access_token }}&amp;id={{ object.event_id.id }}" style="padding: 5px 10px; color: #FFFFFF; text-decoration: none; background-color: #875A7B; border: 1px solid #875A7B; border-radius: 3px">Accept</a>
-          <a t-attf-href="/calendar/meeting/decline?token={{ object.access_token }}&amp;id={{ object.event_id.id }}" style="padding: 5px 10px; color: #FFFFFF; text-decoration: none; background-color: #875A7B; border: 1px solid #875A7B; border-radius: 3px">Decline</a>
-          <a t-attf-href="/calendar/meeting/view?token={{ object.access_token }}&amp;id={{ object.event_id.id }}" style="padding: 5px 10px; color: #FFFFFF; text-decoration: none; background-color: #875A7B; border: 1px solid #875A7B; border-radius: 3px">View</a>
-        </div>
-        <table border="0" cellpadding="0" cellspacing="0">
-          <tr>
-            <td width="130px;" style="min-width: 130px;">
-              <div style="border-top-start-radius: 3px; border-top-end-radius: 3px; font-size: 12px; border-collapse: separate; text-align: center; font-weight: bold; color: #ffffff; min-height: 18px; background-color: #875A7B; border: 1px solid #875A7B;">
-                <t t-out="format_datetime(dt=object.event_id.start, tz=object.mail_tz if not object.event_id.allday else None, dt_format=&quot;EEEE&quot;, lang_code=object.env.lang) or &quot;&quot;">Tuesday</t>
-              </div>
-              <div style="font-size: 48px; min-height: auto; font-weight: bold; text-align: center; color: #5F5F5F; background-color: #F8F8F8; border: 1px solid #875A7B;">
-                <t t-out="format_datetime(dt=object.event_id.start, tz=object.mail_tz if not object.event_id.allday else None, dt_format='d', lang_code=object.env.lang) or ''">4</t>
-              </div>
-              <div style="font-size: 12px; text-align: center; font-weight: bold; color: #ffffff; background-color: #875A7B;">
-                <t t-out="format_datetime(dt=object.event_id.start, tz=object.mail_tz if not object.event_id.allday else None, dt_format=&quot;MMMM y&quot;, lang_code=object.env.lang) or &quot;&quot;">May 2021</t>
-              </div>
-              <div style="border-collapse: separate; color: #5F5F5F; text-align: center; font-size: 12px; border-bottom-end-radius: 3px; font-weight: bold; border: 1px solid #875A7B; border-bottom-start-radius: 3px;">
-                <t t-if="not object.event_id.allday">
-                  <div>
-                    <t t-out="format_time(time=object.event_id.start, tz=object.mail_tz, time_format=&quot;short&quot;, lang_code=object.env.lang) or &quot;&quot;">11:00 AM</t>
-                  </div>
-                  <t t-if="object.mail_tz">
-                    <div style="font-size: 10px; font-weight: normal">
-                      (
-                      <t t-out="object.mail_tz or ''">Europe/Brussels</t>
-                      )
-                    </div>
-                  </t>
-                </t>
-              </div>
-            </td>
-            <td width="20px;"/>
-            <td style="padding-top: 5px;">
-              <p>
-                <strong>Details of the event</strong>
-              </p>
-              <ul>
-                <t t-if="object.event_id.location">
-                  <li>
-                    Location:
-                    <t t-out="object.event_id.location or ''">Bruxelles</t>
-                    (
-                    <a target="_blank" t-attf-href="http://maps.google.com/maps?oi=map&amp;q={{ object.event_id.location }}">View Map</a>
-                    )
-                  </li>
-                </t>
-                <t t-if="recurrent">
-                  <li>
-                    When:
-                    <t t-out="object.recurrence_id.name or ''">Every 1 Weeks, for 3 events</t>
-                  </li>
-                </t>
-                <t t-if="not object.event_id.allday and object.event_id.duration">
-                  <li>
-                    Duration:
-                    <t t-out="('%dH%02d' % (object.event_id.duration,round(object.event_id.duration*60)%60)) or ''">0H30</t>
-                  </li>
-                </t>
-                <li>
-                  Attendees
-                  <ul>
-                    <li t-foreach="object.event_id.attendee_ids" t-as="attendee">
-                      <div t-attf-style="display: inline-block; border-radius: 50%; width: 10px; height: 10px; background: {{ colors.get(attendee.state) or 'white' }};"/>
-                      <t t-if="attendee.common_name != object.common_name">
-                        <span style="margin-left:5px" t-out="attendee.common_name or ''">Mitchell Admin</span>
-                      </t>
-                      <t t-else="">
-                        <span style="margin-left:5px">You</span>
-                      </t>
-                    </li>
-                  </ul>
-                </li>
-                <t t-if="object.event_id.videocall_location">
-                  <li>
-                    How to Join:
-                    <t t-if="object.get_base_url() in object.event_id.videocall_location">Join with Odoo Discuss</t>
-                    <t t-else="">Join at</t>
-                    <br/>
-                    <a t-att-href="object.event_id.videocall_location" target="_blank" t-out="object.event_id.videocall_location or ''">www.mycompany.com/calendar/join_videocall/xyz</a>
-                  </li>
-                </t>
-                <t t-if="not is_html_empty(object.event_id.description)">
-                  <li>
-                    Description of the event:
-                    <t t-out="object.event_id.description">Internal meeting for discussion for new pricing for product and services.</t>
-                  </li>
-                </t>
-              </ul>
-            </td>
-          </tr>
-        </table>
-        <br/>
-        Thank you,
-        <t t-if="object.event_id.user_id.signature">
-          <br/>
-          <t t-out="object.event_id.user_id.signature or ''">
-            --
-            <br/>
-            Mitchell Admin
-          </t>
-        </t>
-      </div>
-    </field>
-  </record>
   <record id="calendar_template_meeting_invitation" model="mail.template">
     <field name="body_html" type="html">
       <div>
         <t t-set="colors" t-value="{'needsAction': 'grey', 'accepted': 'green', 'tentative': '#FFFF00', 'declined': 'red'}"/>
         <t t-set="customer" t-value=" object.event_id.find_partner_customer()"/>
         <t t-set="target_responsible" t-value="object.partner_id == object.event_id.partner_id"/>
         <t t-set="target_customer" t-value="object.partner_id == customer"/>
@@ -225,15 +72,15 @@
                     <a target="_blank" t-attf-href="http://maps.google.com/maps?oi=map&amp;q={{object.event_id.location}}">View Map</a>
                     )
                   </li>
                 </t>
                 <t t-if="recurrent">
                   <li>
                     When:
-                    <t t-out="object.recurrence_id.name or ''">Every 1 Weeks, for 3 events</t>
+                    <t t-out="object.recurrence_id.get_recurrence_name()">Every 1 Weeks, for 3 events</t>
                   </li>
                 </t>
                 <t t-if="not object.event_id.allday and object.event_id.duration">
                   <li>
                     Duration:
                     <t t-out="('%dH%02d' % (object.event_id.duration,round(object.event_id.duration*60)%60)) or ''">0H30</t>
                   </li>
@@ -344,15 +191,15 @@
                     <a target="_blank" t-attf-href="http://maps.google.com/maps?oi=map&amp;q={{ object.event_id.location }}">View Map</a>
                     )
                   </li>
                 </t>
                 <t t-if="recurrent">
                   <li>
                     When:
-                    <t t-out="object.recurrence_id.name or ''">Every 1 Weeks, for 3 events</t>
+                    <t t-out="object.recurrence_id.get_recurrence_name()">Every 1 Weeks, for 3 events</t>
                   </li>
                 </t>
                 <t t-if="not object.event_id.allday and object.event_id.duration">
                   <li>
                     Duration:
                     <t t-out="('%dH%02d' % (object.event_id.duration,round(object.event_id.duration*60)%60)) or ''">0H30</t>
                   </li>
@@ -469,15 +316,15 @@
                       <a target="_blank" t-attf-href="http://maps.google.com/maps?oi=map&amp;q={{object.location}}">View Map</a>
                       )
                     </li>
                   </t>
                   <t t-if="recurrent">
                     <li>
                       When:
-                      <t t-out="object.recurrence_id.name or ''">Every 1 Weeks, for 3 events</t>
+                      <t t-out="object.recurrence_id.get_recurrence_name()">Every 1 Weeks, for 3 events</t>
                     </li>
                   </t>
                   <t t-if="not object.allday and object.duration">
                     <li>
                       Duration:
                       <t t-out="('%dH%02d' % (object.duration,round(object.duration*60)%60))">0H30</t>
                     </li>
```

## odoo/addons/openupgrade_scripts/scripts/crm/17.0.1.8/upgrade_analysis.txt

```diff
@@ -10,14 +10,12 @@
 crm          / crm.lead                 / recurring_revenue_prorated (float): NEW isfunction: function, stored
 ---XML records in module 'crm'---
 NEW ir.actions.act_window: crm.mail_activity_plan_action_lead
 DEL ir.actions.server: crm.action_mark_as_lost
 NEW ir.model.access: crm.access_crm_activity_report_salesman
 NEW ir.model.access: crm.access_mail_activity_plan_sale_manager
 NEW ir.model.access: crm.access_mail_activity_plan_template_sale_manager
-DEL ir.model.constraint: crm.constraint_crm_lead_check_probability
-DEL ir.model.constraint: crm.constraint_crm_recurring_plan_check_number_of_months
 NEW ir.rule: crm.mail_plan_rule_group_sale_manager_lead (noupdate)
 NEW ir.rule: crm.mail_plan_templates_rule_group_sale_manager_lead (noupdate)
 NEW ir.ui.menu: crm.mail_activity_plan_menu_config_lead
 NEW ir.ui.view: crm.crm_lead_view_tree_opportunity_reporting
 NEW ir.ui.view: crm.res_partner_view_form_simple_form
```

## odoo/addons/openupgrade_scripts/scripts/crm_iap_enrich/17.0.1.1/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/crm_iap_enrich/17.0.1.1/noupdate_changes.xml

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <template id="mail_message_lead_enrich_no_email">
     <p>Lead Enrichment (based on email address)</p>
-    <div style="background-color:#ffffff;padding:15px;padding-left:0px;">
+    <div style="padding:15px;padding-left:0px;">
       <span>Enrichment could not be done because the email address does not look valid.</span>
     </div>
   </template>
   <template id="mail_message_lead_enrich_notfound">
     <p>Lead Enrichment (based on email address)</p>
-    <div style="background-color:#ffffff;padding:15px;padding-left:0px;">
+    <div style="padding:15px;padding-left:0px;">
       <span>No company data found based on the email address or email address is one of an email provider. No credit was consumed.</span>
     </div>
   </template>
 </odoo>
```

## odoo/addons/openupgrade_scripts/scripts/crm_iap_mine/17.0.1.2/upgrade_analysis.txt

```diff
@@ -1,8 +1,5 @@
 ---Models in module 'crm_iap_mine'---
 ---Fields in module 'crm_iap_mine'---
 ---XML records in module 'crm_iap_mine'---
-DEL ir.model.constraint: crm_iap_mine.constraint_crm_iap_lead_industry_name_uniq
-DEL ir.model.constraint: crm_iap_mine.constraint_crm_iap_lead_role_name_uniq
-DEL ir.model.constraint: crm_iap_mine.constraint_crm_iap_lead_seniority_name_uniq
 NEW ir.ui.view: crm_iap_mine.crm_case_kanban_view_leads
 NEW ir.ui.view: crm_iap_mine.view_crm_lead_kanban
```

## odoo/addons/openupgrade_scripts/scripts/data_recycle/17.0.1.3/upgrade_analysis.txt

```diff
@@ -1,4 +1,4 @@
 ---Models in module 'data_recycle'---
 ---Fields in module 'data_recycle'---
 ---XML records in module 'data_recycle'---
-DEL ir.model.constraint: data_recycle.constraint_data_recycle_model_check_notif_freq
+---nothing has changed in this module--
```

## odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/noupdate_changes.xml

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <record id="delivery_carrier_comp_rule" model="ir.rule">
-    <field name="domain_force">['|', ('company_id', 'in', company_ids), ('company_id', '=', False)]</field>
+    <field name="domain_force">[('company_id', 'in', company_ids + [False])]</field>
   </record>
   <record id="free_delivery_carrier" model="delivery.carrier">
     <field name="amount"/>
     <field name="free_over"/>
     <field name="name">Standard delivery</field>
   </record>
   <record id="product_product_delivery" model="product.product">
```

## odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/upgrade_analysis.txt

```diff
@@ -40,17 +40,15 @@
 NEW ir.model.access: delivery.access_delivery_zip_prefix_sale_manager
 DEL ir.model.access: delivery.access_choose_delivery_carrier_salesman
 DEL ir.model.access: delivery.access_choose_delivery_package [renamed to stock_delivery module]
 DEL ir.model.access: delivery.access_delivery_carrier_stock_manager [renamed to stock_delivery module]
 DEL ir.model.access: delivery.access_delivery_carrier_stock_user [renamed to stock_delivery module]
 DEL ir.model.access: delivery.access_delivery_price_rule_stock_manager [renamed to stock_delivery module]
 DEL ir.model.access: delivery.access_delivery_zip_prefix_stock_manager [renamed to stock_delivery module]
-DEL ir.model.constraint: delivery.constraint_delivery_carrier_margin_not_under_100_percent
-DEL ir.model.constraint: delivery.constraint_delivery_carrier_shipping_insurance_is_percentage
-DEL ir.model.constraint: delivery.constraint_delivery_zip_prefix_name_uniq
+ir.model.constraint: delivery.constraint_delivery_carrier_margin_not_under_100_percent (changed definition: is now 'check(margin >= -1)' ('check(margin >= -100)'))
 DEL ir.ui.menu: delivery.menu_action_delivery_carrier_form [renamed to stock_delivery module]
 DEL ir.ui.menu: delivery.menu_delivery_zip_prefix [renamed to stock_delivery module]
 DEL ir.ui.view: delivery.choose_delivery_package_view_form
 DEL ir.ui.view: delivery.delivery_stock_report_delivery_no_package_section_line
 DEL ir.ui.view: delivery.delivery_tracking_url_warning_form
 DEL ir.ui.view: delivery.label_package_template_view_delivery
 DEL ir.ui.view: delivery.product_template_hs_code
```

## odoo/addons/openupgrade_scripts/scripts/digest/17.0.1.1/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/digest/17.0.1.1/noupdate_changes.xml

```diff
@@ -5,173 +5,166 @@
     <html xmlns="http://www.w3.org/1999/xhtml">
       <head>
         <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
         <meta name="format-detection" content="telephone=no"/>
         <meta name="viewport" content="width=device-width; initial-scale=1.0; maximum-scale=1.0; user-scalable=no;"/>
         <meta http-equiv="X-UA-Compatible" content="IE=9; IE=8; IE=7; IE=EDGE"/>
         <style type="text/css">
-          <t t-set="color_company" t-value="company.email_secondary_color or '#875a7b'"/>
+          <t t-set="color_company" t-value="company.email_secondary_color or '#714B67'"/>
           /* Remove space around the email design. */
             html,
             body {
                 margin: 0 auto !important;
                 padding: 0 !important;
                 height: 100% !important;
                 width: 100% !important;
                 font-family: Arial, Helvetica, Verdana, sans-serif;
             }
             /* Prevent Windows 10 Mail from underlining links. Styles for underlined links should be inline. */
             a {
                 text-decoration: none;
             }
             #header_background {
-                background-color:
-          <t t-out="color_company"/>
-          ;
-                padding-top:70px;
+                padding-top:20px;
             }
             #header {
-                border-start: 1px solid
-          <t t-out="color_company"/>
-          ;
-                border-end: 1px solid
-          <t t-out="color_company"/>
-          ;
+                border-top: 1px solid #d8dadd;
             }
             .global_layout {
                 width: 588px;
                 margin: 0 auto;
                 background-color: #ffffff;
+                border-left: 1px solid #d8dadd;
+                border-right: 1px solid #d8dadd;
             }
             .company_name {
                 display: inline;
                 vertical-align: middle;
+                color: #878d97;
                 font-weight: bold;
-                color: #8f8f8f;
-                font-size: 25px;
+                font-size: 24px;
             }
             .header_title {
-                font-weight: bold;
-                color: #282f33;
+                color: #374151;
+                font-size: 18px;
                 word-break: break-all;
             }
-            .button {
-                color: #ffffff;
-            }
             .td_button {
+                border-radius: 3px;
+                white-space: nowrap;
+            }
+            .td_button_connect {
                 background-color:
           <t t-out="color_company"/>
           ;
-                border-radius: 5px;
-                white-space: nowrap;
             }
             #button_connect {
-                font-size: 15px;
+                color: #ffffff;
+                font-size: 16px;
+            }
+            #button_open_report {
+                color: #007e84;
+                font-size: 14px;
             }
             .header_date {
-                color: #8f8f8f;
-                font-size: 12px;
+                color: #878d97;
+                font-size: 14px;
             }
             .tip_title {
                 margin-top: 0;
                 font-weight: bold;
                 font-size: 20px;
             }
             .tip_content {
                 margin: 0 auto;
-                color: #333333;
+                color: #374151;
                 text-align: justify;
                 text-justify: inter-word;
                 margin: 15px auto 0 auto;
-                font-size: 15px;
+                font-size: 16px;
                 line-height: 25px;
             }
             .tip_button {
                 background-color:
           <t t-out="color_company"/>
           ;
-                border-radius: 5px;
+                border-radius: 3px;
                 padding: 10px;
                 text-decoration: none;
             }
             .tip_button_text {
                 color: #ffffff;
             }
             .illustration_border {
                 width: 100%;
-                border: 1px solid #808080;
+                border: 1px solid #d8dadd;
                 margin-top: 20px;
             }
             .kpi_row_footer {
                 padding-bottom: 20px;
             }
             .kpi_header {
-                font-size: 15px;
+                font-size: 14px;
                 font-weight: bold;
-                color: #282f33;
-            }
-            #button_open_report {
-                font-size: 12px;
-                font-weight: normal;
+                color: #374151;
             }
             .kpi_cell {
                 width: 33%;
                 text-align: center;
-                padding-top: 2px;
+                padding-top: 10px;
                 padding: 0;
             }
             .kpi_value {
-                color: #282f33;
+                color: #374151;
                 font-weight: bold;
                 text-decoration: none;
-                font-size: 30px;
+                font-size: 28px;
             }
             .kpi_border_col {
-                color: #00A09D;
+                color: #374151;
             }
             .kpi_value_label {
                 display: inline-block;
                 margin-bottom: 10px;
-                color: #888888;
-                font-size: 12px;
-                text-transform: uppercase;
+                color: #878d97;
+                font-size: 14px;
             }
             .kpi_margin_margin {
                 margin-bottom: 10px;
             }
             .download_app {
                 margin-bottom: 5px;
                 display: inline-block;
             }
             .preference {
                 margin-bottom: 15px;
-                color: #6b6d70;
-                font-size: 15px;
+                color: #374151;
+                font-size: 14px;
             }
             .by_odoo {
-                color: #8f8f8f;
+                color: #878d97;
                 font-size: 12px;
             }
             .odoo_link_text {
                 font-weight: bold;
                 color:
           <t t-out="color_company"/>
           ;
             }
             .run_business {
-                color: #2d2a26;
+                color: #374151;
                 margin: 15px auto;
                 font-size: 18px;
             }
             #footer {
-                background-color: #eeeeee;
-                color: #8f8f8f;
+                background-color: #F9FAFB;
+                color: #878d97;
                 text-align: center;
                 font-size: 20px;
-                border: 1px solid #eeeeee;
+                border: 1px solid #F9FAFB;
                 border-top: 0;
             }
             #stock_tip {
                 overflow: auto;
                 margin-top: 20px;
             }
             #stock_div_img {
@@ -188,15 +181,15 @@
                     display: block !important;
                 }
                 #header_background {
                     padding-top: 0px;
                 }
                 #header {
                     padding: 15px 20px;
-                    border: 1px solid #eeeeee;
+                    border: 1px solid #F9FAFB;
                 }
                 .company_name {
                     font-size: 15px;
                 }
                 .header_title {
                     margin: 5px auto;
                 }
@@ -273,25 +266,25 @@
       </head>
       <body>
         <t t-out="body"/>
       </body>
     </html>
   </template>
   <template id="digest_mail_main">
-    <table cellspacing="0" cellpadding="0" style="width: 100%;border: 1px solid #eeeeee;border-bottom: 0;" align="center">
+    <table cellspacing="0" cellpadding="0" style="width: 100%;background-color: #F9FAFB;" align="center">
       <tbody>
         <tr>
           <td id="header_background" align="center">
             <table cellspacing="0" cellpadding="0" border="0" id="header" class="global_layout">
               <tbody>
                 <tr>
-                  <td style="padding: 20px 20px 0px 20px;" class="p0">
+                  <td style="padding: 20px 20px 5px 20px;" class="p0">
                     <p t-field="company.name" class="company_name"/>
                   </td>
-                  <td align="right" style="padding: 20px 20px 0px 0px;" class="p0">
+                  <td align="right" style="padding: 20px 20px 5px 0px;" class="p0">
                     <table>
                       <tbody>
                         <tr>
                           <td class="td_button td_button_connect" style="height: 29px;padding: 3px 10px;">
                             <a t-att-href="top_button_url" target="_blank">
                               <span t-esc="top_button_label" class="button" id="button_connect"/>
                             </a>
@@ -306,32 +299,32 @@
                     <div class="header_title">
                       <p t-esc="title"/>
                       <p t-if="sub_title" t-esc="sub_title"/>
                     </div>
                   </td>
                 </tr>
                 <tr>
-                  <td style="padding: 0px 0px 20px 20px;" class="p0" colspan="2">
+                  <td style="padding: 10px 0px 20px 20px;" class="p0" colspan="2">
                     <span t-esc="formatted_date" class="header_date"/>
                   </td>
                 </tr>
               </tbody>
             </table>
           </td>
         </tr>
       </tbody>
     </table>
-    <table cellspacing="0" cellpadding="0" border="0" style="width: 100%;background-color: #eeeeee;">
+    <table cellspacing="0" cellpadding="0" border="0" style="width: 100%;background-color: #F9FAFB;">
       <tbody>
         <tr>
           <td align="center">
             <table cellspacing="0" cellpadding="0" border="0" class="global_layout">
               <tbody>
                 <tr t-if="tips" t-foreach="tips" t-as="tip">
-                  <td colspan="3" style="width: 100%;padding: 20px;border: 1px solid #eeeeee;">
+                  <td colspan="3" style="width: 100%;padding: 20px;border: 1px solid #F9FAFB;">
                     <table>
                       <tbody>
                         <tr>
                           <td t-out="tip"/>
                         </tr>
                       </tbody>
                     </table>
@@ -340,47 +333,47 @@
                 <tr t-if="kpi_data">
                   <td style="padding: 20px 20px 0px 20px;" class="global_td">
                     <table t-foreach="kpi_data" t-as="kpi_info" style="width: 100%;" cellspacing="0" cellpadding="0">
                       <tr>
                         <td style="padding-bottom: 20px;">
                           <table t-if="kpi_info.get('kpi_col1') or kpi_info.get('kpi_col2') or kpi_info.get('kpi_col3')" t-att-data-field="kpi_info['kpi_name']" cellspacing="0" cellpadding="10" style="width: 100%;margin-bottom: 5px;">
                             <tr class="kpi_header">
-                              <td colspan="2" style="padding: 0px 0px 10px 0px;">
-                                <span t-esc="kpi_info['kpi_fullname']"/>
+                              <td colspan="2" style="padding: 0px 0px 5px 0px;">
+                                <span style="text-transform: uppercase;" t-esc="kpi_info['kpi_fullname']"/>
                               </td>
-                              <td t-if="kpi_info['kpi_action']" align="right" style="padding: 0px 0px 10px 0px;">
+                              <td t-if="kpi_info['kpi_action']" align="right" style="padding: 0px 0px 5px 0px;">
                                 <table>
                                   <tbody>
                                     <tr>
-                                      <td class="td_button td_button_open_report" style="padding: 1px 10px;height: 24px;">
+                                      <td class="td_button td_button_open_report" style="padding: 1px 5px;height: 24px;">
                                         <a t-att-href="'/web#action=%s' % kpi_info['kpi_action']">
-                                          <span class="button" id="button_open_report">Open Report</span>
+                                          <span class="button" id="button_open_report">➔ Open Report</span>
                                         </a>
                                       </td>
                                     </tr>
                                   </tbody>
                                 </table>
                               </td>
                             </tr>
                             <tr style="vertical-align: top;">
-                              <td t-if="kpi_info.get('kpi_col1')" class="kpi_cell" style="border-top: 2px solid #00A09D;">
+                              <td t-if="kpi_info.get('kpi_col1')" class="kpi_cell" style="padding-top: 10px; border-top: 1px solid #e6e6e6;">
                                 <div t-call="digest.digest_tool_kpi">
                                   <t t-set="kpi_value" t-value="kpi_info['kpi_col1']['value']"/>
                                   <t t-set="kpi_margin" t-value="kpi_info['kpi_col1'].get('margin')"/>
                                   <t t-set="kpi_subtitle" t-value="kpi_info['kpi_col1']['col_subtitle']"/>
                                 </div>
                               </td>
-                              <td t-if="kpi_info.get('kpi_col2')" class="kpi_cell" t-att-style="'border-top: 2px solid ' + (company.email_secondary_color or '#875a7b')">
+                              <td t-if="kpi_info.get('kpi_col2')" class="kpi_cell" style="padding-top: 10px; border-top: 1px solid #e6e6e6;">
                                 <div t-call="digest.digest_tool_kpi">
                                   <t t-set="kpi_value" t-value="kpi_info['kpi_col2']['value']"/>
                                   <t t-set="kpi_margin" t-value="kpi_info['kpi_col2'].get('margin')"/>
                                   <t t-set="kpi_subtitle" t-value="kpi_info['kpi_col2']['col_subtitle']"/>
                                 </div>
                               </td>
-                              <td t-if="kpi_info.get('kpi_col3')" class="kpi_cell" style="border-top: 2px solid #00A09D;">
+                              <td t-if="kpi_info.get('kpi_col3')" class="kpi_cell" style="padding-top: 10px; border-top: 1px solid #e6e6e6;">
                                 <div t-call="digest.digest_tool_kpi">
                                   <t t-set="kpi_value" t-value="kpi_info['kpi_col3']['value']"/>
                                   <t t-set="kpi_margin" t-value="kpi_info['kpi_col3'].get('margin')"/>
                                   <t t-set="kpi_subtitle" t-value="kpi_info['kpi_col3']['col_subtitle']"/>
                                 </div>
                               </td>
                             </tr>
@@ -394,37 +387,37 @@
                   <td style="padding: 20px 20px 0px 20px;" class="global_td">
                     <t t-out="body"/>
                   </td>
                 </tr>
               </tbody>
               <tfoot>
                 <tr>
-                  <td style="padding: 20px;border: 1px solid #eeeeee;">
+                  <td style="padding: 20px; border-bottom: 1px solid #d8dadd;">
                     <table border="0" width="100%">
                       <tbody>
-                        <tr style="background-color: #eeeeee;">
+                        <tr style="background-color: #F9FAFB;">
                           <td align="center" colspan="3" valign="center" style="padding: 15px;">
                             <div t-if="preferences" t-foreach="preferences" t-as="preference" class="preference">
                               <t t-out="preference"/>
                             </div>
                             <div class="by_odoo" style="margin-bottom: 15px;">
                               Sent by
                               <a href="https://www.odoo.com" target="_blank">
                                 <span class="odoo_link_text">Odoo</span>
                               </a>
                               <t t-if="unsubscribe_token">
                                 –
                                 <a t-attf-href="/digest/#{object.id}/unsubscribe?token=#{unsubscribe_token}&amp;user_id=#{user.id}" target="_blank" style="text-decoration: none;">
-                                  <span style="color: #8f8f8f;">Unsubscribe</span>
+                                  <span style="color: #878d97;">Unsubscribe</span>
                                 </a>
                               </t>
                               <t t-elif="object and object._name == 'digest.digest'">
                                 –
                                 <a t-att-href="'/web#view_type=form&amp;model=digest.digest&amp;id=%s' % object.id" target="_blank" style="text-decoration: none;">
-                                  <span style="color: #8f8f8f;">Unsubscribe</span>
+                                  <span style="color: #878d97;">Unsubscribe</span>
                                 </a>
                               </t>
                             </div>
                           </td>
                         </tr>
                       </tbody>
                     </table>
@@ -456,22 +449,22 @@
             </table>
           </td>
         </tr>
       </tfoot>
     </table>
   </template>
   <template id="digest_section_mobile">
-    <td colspan="3" style="padding: 20px;width:100%">
+    <td colspan="3" style="padding: 20px;width:100%; border-bottom: 1px solid #d8dadd;">
       <table>
         <tbody>
           <tr>
-            <td align="right" style="width: 50%;">
-              <img src="https://www.odoo.com/web/image/24717933/odoo-mobile.png" alt="Odoo Mobile"/>
+            <td align="right" style="width: 33%;">
+              <img src="https://www.odoo.com/web/image/38874595-16ef5349/odoo-mobile.png" alt="Odoo Mobile"/>
             </td>
-            <td align="left" style="width: 50%;">
+            <td align="left" style="width: 66%;">
               <table>
                 <tbody>
                   <tr>
                     <td>
                       <p class="run_business">
                         Run your business from anywhere with
                         <b>Odoo Mobile</b>
@@ -498,26 +491,26 @@
             </td>
           </tr>
         </tbody>
       </table>
     </td>
   </template>
   <template id="digest_tool_kpi">
-    <span t-esc="kpi_value" style="color: #00A09D;font-weight: bold;text-decoration: none;" class="kpi_value kpi_border_col"/>
+    <span t-esc="kpi_value" style="color: #374151;text-decoration: none;" class="kpi_value kpi_border_col"/>
     <br/>
     <span t-esc="kpi_subtitle" class="kpi_value_label"/>
     <table t-if="kpi_margin" class="kpi_margin_margin" align="center" border="0" cellspacing="0" cellpadding="0">
       <tr>
-        <td t-if="kpi_margin &gt; 0.0" class="kpi_margin positive_kpi_margin" style="padding: 5px 10px;font-size: 12px;text-decoration: none;border-radius: 5px;border: 1px solid #c4ecd7;border-radius: 5px; background-color: #c4ecd7;color: #17613a;">
-          ▲
+        <td t-if="kpi_margin &gt; 0.0" class="kpi_margin positive_kpi_margin" style="padding: 3px 10px;font-size: 12px;text-decoration: none;border-radius: 50px;border: 1px solid #c4ecd7;border-radius: 5px; background-color: #c4ecd7;color: #17613a;">
+          ⬆
           <t t-esc="'%.2f' % kpi_margin"/>
           %
         </td>
-        <td t-elif="kpi_margin &lt; 0.0" class="kpi_margin negative_kpi_margin" style="padding: 5px 10px;font-size: 12px;text-decoration: none;border-radius: 5px;border: 1px solid #f4cfce;background-color: #f7dddc;color: #712b29;">
-          ▼
+        <td t-elif="kpi_margin &lt; 0.0" class="kpi_margin negative_kpi_margin" style="padding: 3px 10px;font-size: 12px;text-decoration: none;border-radius: 50px;border: 1px solid #f4cfce;background-color: #f7dddc;color: #712b29;">
+          ⬇
           <t t-esc="'%.2f' % kpi_margin"/>
           %
         </td>
       </tr>
     </table>
   </template>
 </odoo>
```

## odoo/addons/openupgrade_scripts/scripts/event/17.0.1.8/upgrade_analysis.txt

```diff
@@ -31,14 +31,15 @@
 NEW ir.actions.report: event.action_report_event_event_attendee_list
 NEW ir.actions.report: event.action_report_event_event_badge
 NEW ir.actions.report: event.action_report_event_registration_attendee_list
 NEW ir.actions.report: event.action_report_event_registration_badge
 NEW ir.actions.report: event.action_report_event_registration_responsive_html_ticket
 DEL ir.actions.report: event.action_report_event_event_foldable_badge
 DEL ir.actions.report: event.action_report_event_registration_foldable_badge
+NEW ir.model.constraint: event.constraint_event_registration_barcode_event_uniq
 NEW ir.ui.menu: event.menu_event_registration_desk
 NEW ir.ui.view: event.attendee_list
 NEW ir.ui.view: event.event_event_attendee_list
 NEW ir.ui.view: event.event_event_report_template_badge
 NEW ir.ui.view: event.event_event_view_activity
 NEW ir.ui.view: event.event_registration_attendee_list
 NEW ir.ui.view: event.event_registration_report_template_badge
```

## odoo/addons/openupgrade_scripts/scripts/event_booth_sale/17.0.1.2/upgrade_analysis.txt

```diff
@@ -1,7 +1,6 @@
 ---Models in module 'event_booth_sale'---
 ---Fields in module 'event_booth_sale'---
 event_booth_sale / event.booth.category     / price_incl (float)            : NEW hasdefault: compute
 event_booth_sale / event.booth.registration / contact_mobile (char)         : DEL
 event_booth_sale / product.template         / detailed_type (False)         : selection_keys is now '['combo', 'consu', 'event', 'event_booth', 'product', 'service']' ('['consu', 'course', 'event', 'event_booth', 'product', 'service']')
 ---XML records in module 'event_booth_sale'---
-DEL ir.model.constraint: event_booth_sale.constraint_event_booth_registration_unique_registration
```

## odoo/addons/openupgrade_scripts/scripts/fleet/17.0.0.1/upgrade_analysis.txt

```diff
@@ -22,11 +22,8 @@
 fleet        / fleet.vehicle.model      / image_256 (binary)            : NEW attachment: True, isrelated: related, stored
 fleet        / fleet.vehicle.model      / image_512 (binary)            : NEW attachment: True, isrelated: related, stored
 fleet        / fleet.vehicle.model      / vehicle_properties_definition (properties_definition): NEW
 fleet        / fleet.vehicle.model.brand / active (boolean)              : NEW hasdefault: default
 ---XML records in module 'fleet'---
 NEW fleet.service.type: fleet.type_contract_leasing (noupdate)
 NEW fleet.service.type: fleet.type_contract_omnium (noupdate)
-DEL ir.model.constraint: fleet.constraint_fleet_vehicle_model_category_name_uniq
-DEL ir.model.constraint: fleet.constraint_fleet_vehicle_state_fleet_state_name_unique
-DEL ir.model.constraint: fleet.constraint_fleet_vehicle_tag_name_uniq
 NEW ir.ui.view: fleet.fleet_vechicle_costs_report_view_form
```

## odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/noupdate_changes.xml

```diff
@@ -175,16 +175,48 @@
               </td>
             </tr>
           </tbody>
         </table>
       </div>
     </field>
   </record>
+  <record id="rank_bachelor" model="gamification.karma.rank">
+    <field name="description_motivational" type="html">
+      <div class="d-flex align-items-center">
+        <div class="flex-grow-1">Reach the next rank to improve your status!</div>
+        <img class="ms-3 img img-fluid" style="max-height: 72px;" src="/gamification/static/img/rank_bachelor_badge.svg" alt=""/>
+      </div>
+    </field>
+  </record>
+  <record id="rank_doctor" model="gamification.karma.rank">
+    <field name="description_motivational" type="html">
+      <div class="d-flex align-items-center">
+        <div class="flex-grow-1">Reach the next rank and become a powerful user!</div>
+        <img class="ms-3 img img-fluid" style="max-height: 72px;" src="/gamification/static/img/rank_doctor_badge.svg" alt=""/>
+      </div>
+    </field>
+  </record>
+  <record id="rank_master" model="gamification.karma.rank">
+    <field name="description_motivational" type="html">
+      <div class="d-flex align-items-center">
+        <div class="flex-grow-1">Reach the next rank and become a Master!</div>
+        <img class="ms-3 img img-fluid" style="max-height: 72px;" src="/gamification/static/img/rank_master_badge.svg" alt=""/>
+      </div>
+    </field>
+  </record>
   <record id="rank_newbie" model="gamification.karma.rank">
     <field name="description_motivational" type="html">
       <div class="d-flex align-items-center">
         <div class="flex-grow-1">Earn your first points and join the adventure!</div>
-        <img class="ms-3 img img-fluid" style="max-height: 72px;" src="/gamification/static/img/rank_newbie_badge.svg"/>
+        <img class="ms-3 img img-fluid" style="max-height: 72px;" src="/gamification/static/img/rank_newbie_badge.svg" alt=""/>
+      </div>
+    </field>
+  </record>
+  <record id="rank_student" model="gamification.karma.rank">
+    <field name="description_motivational" type="html">
+      <div class="d-flex align-items-center">
+        <div class="flex-grow-1">Reach the next rank to show the rest of the world you exist.</div>
+        <img class="ms-3 img img-fluid" style="max-height: 72px;" src="/gamification/static/img/rank_student_badge.svg" alt=""/>
       </div>
     </field>
   </record>
 </odoo>
```

## odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/upgrade_analysis.txt

```diff
@@ -14,8 +14,7 @@
 NEW gamification.karma.tracking: gamification.karma_tracking_user_root (noupdate)
 NEW ir.cron: gamification.ir_cron_consolidate (noupdate)
 DEL ir.cron: gamification.ir_cron_consolidate_last_month (noupdate)
 NEW ir.model.access: gamification.gamification_karma_rank_access_employee
 NEW ir.model.access: gamification.gamification_karma_rank_access_portal
 NEW ir.model.access: gamification.gamification_karma_rank_access_public
 DEL ir.model.access: gamification.gamification_karma_rank_access_all
-DEL ir.model.constraint: gamification.constraint_gamification_karma_rank_karma_min_check
```

## odoo/addons/openupgrade_scripts/scripts/google_calendar/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,6 +1,5 @@
 ---Models in module 'google_calendar'---
 ---Fields in module 'google_calendar'---
 google_calendar / calendar.event           / guests_readonly (boolean)     : NEW hasdefault: default
 google_calendar / calendar.event           / videocall_source (False)      : NEW selection_keys: ['custom', 'discuss', 'google_meet'], mode: modify
 ---XML records in module 'google_calendar'---
-DEL ir.model.constraint: google_calendar.constraint_res_users_google_token_uniq
```

## odoo/addons/openupgrade_scripts/scripts/hr/17.0.1.1/upgrade_analysis.txt

```diff
@@ -72,19 +72,14 @@
 NEW ir.model.access: hr.access_mail_activity_plan_hr_manager
 NEW ir.model.access: hr.access_mail_activity_plan_template_hr_manager
 DEL ir.model.access: hr.access_hr_plan_activity_type_employee
 DEL ir.model.access: hr.access_hr_plan_activity_type_hr_user
 DEL ir.model.access: hr.access_hr_plan_employee
 DEL ir.model.access: hr.access_hr_plan_hr_user
 DEL ir.model.access: hr.access_hr_plan_wizard
-DEL ir.model.constraint: hr.constraint_hr_employee_barcode_uniq
-DEL ir.model.constraint: hr.constraint_hr_employee_category_name_uniq
-DEL ir.model.constraint: hr.constraint_hr_employee_user_uniq
-DEL ir.model.constraint: hr.constraint_hr_job_name_company_uniq
-DEL ir.model.constraint: hr.constraint_hr_job_no_of_recruitment_positive
 NEW ir.rule: hr.ir_rule_hr_contract_type_multi_company (noupdate)
 NEW ir.rule: hr.ir_rule_res_partner_bank_employees (noupdate)
 NEW ir.rule: hr.ir_rule_res_partner_bank_internal_users (noupdate)
 NEW ir.rule: hr.mail_plan_rule_group_hr_manager (noupdate)
 NEW ir.rule: hr.mail_plan_templates_rule_group_hr_manager (noupdate)
 DEL ir.rule: hr.hr_plan_activity_type_company_rule (noupdate)
 DEL ir.rule: hr.hr_plan_company_rule (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/hr_expense/17.0.2.0/upgrade_analysis.txt

```diff
@@ -40,12 +40,11 @@
 hr_expense   / hr.expense.sheet         / total_tax_amount (float)      : NEW isfunction: function, stored
 hr_expense   / res.company              / company_expense_allowed_payment_method_line_ids (many2many): NEW relation: account.payment.method.line
 hr_expense   / res.company              / company_expense_journal_id (many2one): DEL relation: account.journal
 hr_expense   / res.company              / expense_product_id (many2one) : NEW relation: product.product
 ---XML records in module 'hr_expense'---
 ir.actions.act_window: hr_expense.action_hr_expense_sheet_my_all (deleted domain)
 NEW ir.actions.report: hr_expense.action_report_expense_sheet_img
-DEL ir.model.constraint: hr_expense.constraint_hr_expense_sheet_journal_id_required_posted
 NEW ir.ui.view: hr_expense.product_product_expense_kanban_view
 NEW ir.ui.view: hr_expense.report_expense_sheet_img
 NEW mail.message.subtype: hr_expense.mt_expense_entry_delete (noupdate)
 NEW mail.message.subtype: hr_expense.mt_expense_reset (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/hr_holidays/17.0.1.6/upgrade_analysis.txt

```diff
@@ -14,15 +14,14 @@
 hr_holidays  / hr.leave                 / mode_company_id (many2one)    : not a function anymore
 hr_holidays  / hr.leave                 / number_of_days (float)        : now a function
 hr_holidays  / hr.leave                 / number_of_hours (float)       : NEW isfunction: function, stored
 hr_holidays  / hr.leave                 / rating_ids (one2many)         : NEW relation: rating.rating
 hr_holidays  / hr.leave                 / resource_calendar_id (many2one): NEW relation: resource.calendar, hasdefault: compute
 hr_holidays  / hr.leave                 / website_message_ids (one2many): previously in module portal
 hr_holidays  / hr.leave.accrual.level   / action_with_unused_accruals (selection): selection_keys is now '['all', 'lost', 'maximum']' ('['lost', 'postponed']')
-hr_holidays  / hr.leave.accrual.level   / added_value_type (selection)  : now a function
 hr_holidays  / hr.leave.accrual.level   / added_value_type (selection)  : selection_keys is now '['day', 'hour']' ('['days', 'hours']')
 hr_holidays  / hr.leave.accrual.level   / cap_accrued_time (boolean)    : NEW hasdefault: default
 hr_holidays  / hr.leave.accrual.level   / frequency (selection)         : selection_keys is now '['bimonthly', 'biyearly', 'daily', 'hourly', 'monthly', 'weekly', 'yearly']' ('['bimonthly', 'biyearly', 'daily', 'monthly', 'weekly', 'yearly']')
 hr_holidays  / hr.leave.accrual.level   / is_based_on_worked_time (boolean): DEL
 hr_holidays  / hr.leave.accrual.level   / parent_id (many2one)          : DEL relation: hr.leave.accrual.level
 hr_holidays  / hr.leave.accrual.plan    / accrued_gain_time (selection) : NEW required, selection_keys: ['end', 'start'], hasdefault: default
 hr_holidays  / hr.leave.accrual.plan    / active (boolean)              : NEW hasdefault: default
@@ -73,23 +72,19 @@
 DEL ir.actions.report: hr_holidays.action_report_holidayssummary2
 DEL ir.actions.server: hr_holidays.act_hr_employee_holiday_request
 NEW ir.cron: hr_holidays.hr_leave_cron_cancel_invalid
 NEW ir.model.access: hr_holidays.access_hr_leave_mandatory_day_manager
 NEW ir.model.access: hr_holidays.access_hr_leave_mandatory_day_user
 DEL ir.model.access: hr_holidays.access_hr_leave_stress_day_manager
 DEL ir.model.access: hr_holidays.access_hr_leave_stress_day_user
-DEL ir.model.constraint: hr_holidays.constraint_hr_leave_accrual_level_added_value_greater_than_zero
-DEL ir.model.constraint: hr_holidays.constraint_hr_leave_accrual_level_check_dates
-DEL ir.model.constraint: hr_holidays.constraint_hr_leave_accrual_level_start_count_check
-DEL ir.model.constraint: hr_holidays.constraint_hr_leave_allocation_duration_check
-DEL ir.model.constraint: hr_holidays.constraint_hr_leave_allocation_type_value
-DEL ir.model.constraint: hr_holidays.constraint_hr_leave_date_check2
-DEL ir.model.constraint: hr_holidays.constraint_hr_leave_duration_check
+ir.model.constraint: hr_holidays.constraint_hr_leave_accrual_level_check_dates (changed definition: is now 'check((frequency in('daily','hourly')) or(week_day is not null and frequency = 'weekly') or(first_day > 0 and second_day > first_day and first_day <= 31 and second_day <= 31 and frequency = 'bimonthly') or(first_day > 0 and first_day <= 31 and frequency = 'monthly')or(first_month_day > 0 and first_month_day <= 31 and second_month_day > 0 and second_month_day <= 31 and frequency = 'biyearly') or(yearly_day > 0 and yearly_day <= 31 and frequency = 'yearly'))' ('check((frequency = 'daily') or(week_day is not null and frequency = 'weekly') or(first_day > 0 and second_day > first_day and first_day <= 31 and second_day <= 31 and frequency = 'bimonthly') or(first_day > 0 and first_day <= 31 and frequency = 'monthly')or(first_month_day > 0 and first_month_day <= 31 and second_month_day > 0 and second_month_day <= 31 and frequency = 'biyearly') or(yearly_day > 0 and yearly_day <= 31 and frequency = 'yearly'))'))
+NEW ir.model.constraint: hr_holidays.constraint_hr_leave_date_check3
+NEW ir.model.constraint: hr_holidays.constraint_hr_leave_mandatory_day_date_from_after_day_to
+NEW ir.model.constraint: hr_holidays.constraint_hr_leave_type_check_negative
 DEL ir.model.constraint: hr_holidays.constraint_hr_leave_stress_day_date_from_after_day_to
-DEL ir.model.constraint: hr_holidays.constraint_hr_leave_type_value
 NEW ir.rule: hr_holidays.hr_leave_accrual_plan_rule_multi_company (noupdate)
 NEW ir.rule: hr_holidays.hr_leave_mandatory_day_rule_multi_company (noupdate)
 DEL ir.rule: hr_holidays.hr_leave_stress_day_rule_multi_company (noupdate)
 NEW ir.ui.menu: hr_holidays.hr_holidays_mandatory_day_menu_configuration
 NEW ir.ui.menu: hr_holidays.menu_hr_holidays_management
 DEL ir.ui.menu: hr_holidays.hr_holidays_stress_day_menu_configuration
 DEL ir.ui.menu: hr_holidays.menu_hr_holidays_approvals
```

## odoo/addons/openupgrade_scripts/scripts/hr_homeworking/17.0.1.0/upgrade_analysis.txt

```diff
@@ -15,14 +15,15 @@
 hr_homeworking / hr.employee.location     / employee_id (many2one)        : NEW relation: hr.employee, required, hasdefault: default
 hr_homeworking / hr.employee.location     / work_location_id (many2one)   : NEW relation: hr.work.location, required
 ---XML records in module 'hr_homeworking'---
 NEW ir.actions.act_window: hr_homeworking.set_location_wizard_action
 NEW ir.model.access: hr_homeworking.access_homework_location_wizard
 NEW ir.model.access: hr_homeworking.access_hr_employee_location
 NEW ir.model.access: hr_homeworking.access_user_employee_location
+NEW ir.model.constraint: hr_homeworking.constraint_hr_employee_location_uniq_exceptional_per_day
 NEW ir.rule: hr_homeworking.homeworking_admin_rule (noupdate)
 NEW ir.rule: hr_homeworking.homeworking_location_wizard_admin_rule (noupdate)
 NEW ir.rule: hr_homeworking.homeworking_location_wizard_own_rule (noupdate)
 NEW ir.rule: hr_homeworking.homeworking_own_rule (noupdate)
 NEW ir.ui.view: hr_homeworking.homework_location_wizard_view_form
 NEW ir.ui.view: hr_homeworking.res_useurs_view_form_profile
 NEW ir.ui.view: hr_homeworking.view_employee_filter
```

## odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/noupdate_changes.xml

```diff
@@ -3,15 +3,15 @@
   <template id="applicant_hired_template">
     Employee created:
     <a href="#" t-att-data-oe-id="applicant.emp_id.id" data-oe-model="hr.employee">
       <t t-esc="applicant.emp_id.name"/>
     </a>
   </template>
   <record id="base.module_category_human_resources_recruitment" model="ir.module.category">
-    <field name="description">Interviewer right will give access to all job position/applications where the employee is defined. It will allow to refuse, plan meetings. Chatter content will not be available.</field>
+    <field name="description">Interviewer right will give access to all job position/applications where the employee is defined. It will allow to refuse, plan meetings.</field>
   </record>
   <record id="group_hr_recruitment_interviewer" model="res.groups">
     <field name="category_id" ref="base.module_category_human_resources_recruitment"/>
     <field name="name">Interviewer</field>
   </record>
   <record id="group_hr_recruitment_manager" model="res.groups">
     <field name="implied_ids" eval="[(4, ref('group_hr_recruitment_user')), (4, ref('mail.group_mail_template_editor'))]"/>
```

## odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/upgrade_analysis.txt

```diff
@@ -2,33 +2,29 @@
 ---Fields in module 'hr_recruitment'---
 hr_recruitment / hr.applicant             / activity_user_id (many2one)   : not related anymore
 hr_recruitment / hr.applicant             / activity_user_id (many2one)   : now a function
 hr_recruitment / hr.applicant             / applicant_properties (properties): NEW hasdefault: compute
 hr_recruitment / hr.applicant             / application_status (selection): selection_keys is now '['archived', 'hired', 'ongoing', 'refused']' ('['hired', 'ongoing', 'refused']')
 hr_recruitment / hr.applicant             / email_normalized (char)       : NEW isfunction: function, stored
 hr_recruitment / hr.applicant             / message_bounce (integer)      : NEW hasdefault: default
-hr_recruitment / hr.applicant             / partner_mobile (char)         : not a function anymore
 hr_recruitment / hr.applicant             / partner_mobile_sanitized (char): NEW isfunction: function, stored
-hr_recruitment / hr.applicant             / partner_phone (char)          : not a function anymore
 hr_recruitment / hr.applicant             / partner_phone_sanitized (char): NEW isfunction: function, stored
 hr_recruitment / hr.applicant             / phone_mobile_search (char)    : NEW
 hr_recruitment / hr.applicant             / phone_sanitized (char)        : NEW isfunction: function, stored
 hr_recruitment / hr.applicant             / rating_ids (one2many)         : NEW relation: rating.rating
 hr_recruitment / hr.applicant.refuse.reason / _order                        : _order is now 'sequence' ('id')
 hr_recruitment / hr.applicant.refuse.reason / sequence (integer)            : NEW hasdefault: default
 hr_recruitment / hr.job                   / applicant_properties_definition (properties_definition): NEW
 hr_recruitment / hr.job                   / hr_responsible_id (many2one)  : DEL relation: res.users
 ---XML records in module 'hr_recruitment'---
 NEW hr.recruitment.stage: hr_recruitment.stage_job0 (noupdate)
 NEW ir.actions.act_window: hr_recruitment.action_hr_applicant_mass_sms
 DEL ir.actions.act_window: hr_recruitment.hr_employee_action_from_department
 NEW ir.actions.server: hr_recruitment.ir_actions_server_refuse_applicant
 NEW ir.config_parameter: hr_recruitment.hr_recruitment_blacklisted_emails (noupdate)
-DEL ir.model.constraint: hr_recruitment.constraint_hr_applicant_category_name_uniq
-DEL ir.model.constraint: hr_recruitment.constraint_hr_recruitment_degree_name_uniq
 NEW ir.rule: hr_recruitment.hr_applicant_user_rule (noupdate)
 NEW ir.rule: hr_recruitment.hr_job_user_rule (noupdate)
 NEW ir.rule: hr_recruitment.mail_message_user_rule (noupdate)
 DEL ir.rule: hr_recruitment.mail_message_interviewer_rule (noupdate)
 NEW ir.ui.view: hr_recruitment.mail_notification_light_without_background (noupdate)
 DEL ir.ui.view: hr_recruitment.hr_employee_view_search
 DEL mail.alias: hr_recruitment.mail_alias_jobs (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/hr_recruitment_skills/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,7 +1,6 @@
 ---Models in module 'hr_recruitment_skills'---
 ---Fields in module 'hr_recruitment_skills'---
 ---XML records in module 'hr_recruitment_skills'---
 DEL ir.model.access: hr_recruitment_skills.access_hr_applicant_skill
-DEL ir.model.constraint: hr_recruitment_skills.constraint_hr_applicant_skill__unique_skill
 NEW ir.rule: hr_recruitment_skills.hr_applicant_skill_officer_rule (noupdate)
 NEW ir.ui.menu: hr_recruitment_skills.hr_recruitment_skill_type_menu
```

## odoo/addons/openupgrade_scripts/scripts/hr_skills/17.0.1.0/upgrade_analysis.txt

```diff
@@ -5,17 +5,13 @@
 ---XML records in module 'hr_skills'---
 NEW hr.skill.type: hr_skills.hr_skill_type_lang (noupdate)
 NEW ir.actions.act_window: hr_skills.action_hr_employee_cv_wizard
 NEW ir.actions.report: hr_skills.action_report_employee_cv
 NEW ir.actions.server: hr_skills.action_print_employees_cv
 DEL ir.actions.server: hr_skills.action_open_skills_log_employee
 NEW ir.model.access: hr_skills.access_hr_employee_cv_wizard
-DEL ir.model.constraint: hr_skills.constraint_hr_employee_skill__unique_skill
-DEL ir.model.constraint: hr_skills.constraint_hr_employee_skill_log__unique_skill_log
-DEL ir.model.constraint: hr_skills.constraint_hr_resume_line_date_check
-DEL ir.model.constraint: hr_skills.constraint_hr_skill_level_check_level_progress
 NEW ir.ui.view: hr_skills.hr_employee_cv_wizard_view_form
 NEW ir.ui.view: hr_skills.report_employee_cv
 NEW ir.ui.view: hr_skills.report_employee_cv_company
 NEW ir.ui.view: hr_skills.report_employee_cv_main_panel
 NEW ir.ui.view: hr_skills.report_employee_cv_sidepanel
 NEW report.paperformat: hr_skills.paperformat_resume
```

## odoo/addons/openupgrade_scripts/scripts/hr_timesheet/17.0.1.0/upgrade_analysis.txt

```diff
@@ -10,17 +10,20 @@
 hr_timesheet / project.update           / uom_id (many2one)             : NEW relation: uom.uom
 ---XML records in module 'hr_timesheet'---
 DEL ir.actions.act_window.view: hr_timesheet.timesheet_action_view_from_employee_list
 NEW ir.actions.server: hr_timesheet.unlink_employee_action
 NEW ir.model.access: hr_timesheet.access_hr_employee_delete_wizard
 DEL ir.model.access: hr_timesheet.access_project_task
 NEW ir.ui.view: hr_timesheet.hr_employee_delete_wizard_form
+NEW ir.ui.view: hr_timesheet.hr_timesheet_line_portal_tree
 NEW ir.ui.view: hr_timesheet.portal_my_task_allocated_hours_template
 NEW ir.ui.view: hr_timesheet.project_update_view_kanban_inherit
+NEW ir.ui.view: hr_timesheet.timesheet_view_form_portal_user
 NEW ir.ui.view: hr_timesheet.view_employee_tree_inherit_timesheet
+NEW ir.ui.view: hr_timesheet.view_kanban_account_analytic_line_portal_user
 DEL ir.ui.view: hr_timesheet.portal_my_task_planned_hours_template
 DEL ir.ui.view: hr_timesheet.project_sharing_inherit_project_task_view_tree
 DEL ir.ui.view: hr_timesheet.project_sharing_project_task_view_search_inherit_timesheet
 DEL ir.ui.view: hr_timesheet.rating_rating_view_search_project_inherited
 DEL ir.ui.view: hr_timesheet.report_project_task_user_view_search
 DEL ir.ui.view: hr_timesheet.report_project_task_user_view_tree
 DEL ir.ui.view: hr_timesheet.view_task_search_form_hr_extended
```

## odoo/addons/openupgrade_scripts/scripts/hr_work_entry/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,10 +1,5 @@
 ---Models in module 'hr_work_entry'---
 ---Fields in module 'hr_work_entry'---
 hr_work_entry / hr.work.entry.type       / external_code (char)          : NEW
 ---XML records in module 'hr_work_entry'---
 NEW hr.work.entry.type: hr_work_entry.overtime_work_entry_type
-DEL ir.model.constraint: hr_work_entry.constraint_hr_user_work_entry_employee_user_id_employee_id_unique
-DEL ir.model.constraint: hr_work_entry.constraint_hr_work_entry__work_entries_no_validated_conflict
-DEL ir.model.constraint: hr_work_entry.constraint_hr_work_entry__work_entry_has_end
-DEL ir.model.constraint: hr_work_entry.constraint_hr_work_entry__work_entry_start_before_end
-DEL ir.model.constraint: hr_work_entry.constraint_hr_work_entry_type_unique_work_entry_code
```

## odoo/addons/openupgrade_scripts/scripts/im_livechat/17.0.1.0/upgrade_analysis.txt

```diff
@@ -48,15 +48,15 @@
 NEW ir.model.access: im_livechat.access_livechat_channel_rule_portal
 NEW ir.model.access: im_livechat.access_livechat_channel_rule_public
 DEL ir.model.access: im_livechat.access_chatbot_message_all
 DEL ir.model.access: im_livechat.access_chatbot_script
 DEL ir.model.access: im_livechat.access_chatbot_script_step
 DEL ir.model.access: im_livechat.access_livechat_channel
 DEL ir.model.access: im_livechat.access_livechat_channel_rule
-DEL ir.model.constraint: im_livechat.constraint_chatbot_message__unique_mail_message_id
+NEW ir.model.constraint: im_livechat.constraint_discuss_channel_livechat_operator_id
 DEL ir.model.constraint: im_livechat.constraint_mail_channel_livechat_operator_id
 NEW ir.rule: im_livechat.ir_rule_discuss_channel_group_im_livechat_group_manager (noupdate)
 NEW ir.rule: im_livechat.ir_rule_discuss_channel_member_group_im_livechat_group_manager (noupdate)
 DEL ir.rule: im_livechat.im_livechat_rule_manager_read_all_mail_channel (noupdate)
 NEW ir.ui.view: im_livechat.discuss_channel_view_form
 NEW ir.ui.view: im_livechat.discuss_channel_view_search
 NEW ir.ui.view: im_livechat.discuss_channel_view_tree
```

## odoo/addons/openupgrade_scripts/scripts/l10n_ar/17.0.3.5/upgrade_analysis.txt

```diff
@@ -496,10 +496,8 @@
 DEL account.tax.template: l10n_ar.ri_tax_vat_exento_ventas
 DEL account.tax.template: l10n_ar.ri_tax_vat_no_corresponde_compras
 DEL account.tax.template: l10n_ar.ri_tax_vat_no_corresponde_ventas
 DEL account.tax.template: l10n_ar.ri_tax_vat_no_gravado_compras
 DEL account.tax.template: l10n_ar.ri_tax_vat_no_gravado_ventas
 NEW ir.model.access: l10n_ar.access_l10n_ar_afip_responsibility_type_portal
 NEW ir.model.access: l10n_ar.access_l10n_ar_afip_responsibility_type_public
-DEL ir.model.constraint: l10n_ar.constraint_l10n_ar_afip_responsibility_type_code
-DEL ir.model.constraint: l10n_ar.constraint_l10n_ar_afip_responsibility_type_name
 DEL ir.ui.view: l10n_ar.report_invoice_with_payments
```

## odoo/addons/openupgrade_scripts/scripts/l10n_ar_withholding/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,11 +1,11 @@
 ---Models in module 'l10n_ar_withholding'---
 new model l10n_ar.payment.register.withholding [transient]
 ---Fields in module 'l10n_ar_withholding'---
-l10n_ar_withholding / account.tax              / l10n_ar_withholding_payment_type (selection): NEW selection_keys: ['customer', 'supplier']
+l10n_ar_withholding / account.tax              / l10n_ar_withholding_payment_type (selection): NEW selection_keys: ['customer', 'supplier'], hasdefault: compute
 l10n_ar_withholding / account.tax              / l10n_ar_withholding_sequence_id (many2one): NEW relation: ir.sequence
 l10n_ar_withholding / res.company              / l10n_ar_tax_base_account_id (many2one): NEW relation: account.account
 ---XML records in module 'l10n_ar_withholding'---
 NEW ir.model.access: l10n_ar_withholding.access_l10n_ar_payment_register_withholding
 NEW ir.ui.view: l10n_ar_withholding.report_payment_receipt_document
 NEW ir.ui.view: l10n_ar_withholding.res_config_settings_view_form
 NEW ir.ui.view: l10n_ar_withholding.view_account_payment_form
```

## odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/upgrade_analysis.txt

```diff
@@ -131,14 +131,15 @@
 DEL account.account.template: l10n_cl.account_290110
 DEL account.account.template: l10n_cl.account_290210
 DEL account.account.template: l10n_cl.account_290220
 DEL account.account.template: l10n_cl.account_290230
 DEL account.account.template: l10n_cl.account_310110
 DEL account.account.template: l10n_cl.account_310115
 DEL account.account.template: l10n_cl.account_310120
+DEL account.account.template: l10n_cl.account_310122
 DEL account.account.template: l10n_cl.account_310125
 DEL account.account.template: l10n_cl.account_310130
 DEL account.account.template: l10n_cl.account_320210
 DEL account.account.template: l10n_cl.account_320220
 DEL account.account.template: l10n_cl.account_320225
 DEL account.account.template: l10n_cl.account_320230
 DEL account.account.template: l10n_cl.account_320235
```

## odoo/addons/openupgrade_scripts/scripts/l10n_de/17.0.2.0/upgrade_analysis.txt

```diff
@@ -1,2704 +1,4 @@
 ---Models in module 'l10n_de'---
 ---Fields in module 'l10n_de'---
 l10n_de      / account.tax.template     / l10n_de_datev_code (char)     : DEL
 ---XML records in module 'l10n_de'---
-DEL account.account.template: l10n_de_skr03.account_0005
-DEL account.account.template: l10n_de_skr03.account_0010
-DEL account.account.template: l10n_de_skr03.account_0015
-DEL account.account.template: l10n_de_skr03.account_0020
-DEL account.account.template: l10n_de_skr03.account_0025
-DEL account.account.template: l10n_de_skr03.account_0027
-DEL account.account.template: l10n_de_skr03.account_0030
-DEL account.account.template: l10n_de_skr03.account_0035
-DEL account.account.template: l10n_de_skr03.account_0038
-DEL account.account.template: l10n_de_skr03.account_0039
-DEL account.account.template: l10n_de_skr03.account_0040
-DEL account.account.template: l10n_de_skr03.account_0043
-DEL account.account.template: l10n_de_skr03.account_0045
-DEL account.account.template: l10n_de_skr03.account_0046
-DEL account.account.template: l10n_de_skr03.account_0047
-DEL account.account.template: l10n_de_skr03.account_0048
-DEL account.account.template: l10n_de_skr03.account_0050
-DEL account.account.template: l10n_de_skr03.account_0059
-DEL account.account.template: l10n_de_skr03.account_0060
-DEL account.account.template: l10n_de_skr03.account_0065
-DEL account.account.template: l10n_de_skr03.account_0070
-DEL account.account.template: l10n_de_skr03.account_0075
-DEL account.account.template: l10n_de_skr03.account_0079
-DEL account.account.template: l10n_de_skr03.account_0080
-DEL account.account.template: l10n_de_skr03.account_0085
-DEL account.account.template: l10n_de_skr03.account_0090
-DEL account.account.template: l10n_de_skr03.account_0100
-DEL account.account.template: l10n_de_skr03.account_0110
-DEL account.account.template: l10n_de_skr03.account_0111
-DEL account.account.template: l10n_de_skr03.account_0112
-DEL account.account.template: l10n_de_skr03.account_0113
-DEL account.account.template: l10n_de_skr03.account_0115
-DEL account.account.template: l10n_de_skr03.account_0120
-DEL account.account.template: l10n_de_skr03.account_0129
-DEL account.account.template: l10n_de_skr03.account_0140
-DEL account.account.template: l10n_de_skr03.account_0145
-DEL account.account.template: l10n_de_skr03.account_0146
-DEL account.account.template: l10n_de_skr03.account_0147
-DEL account.account.template: l10n_de_skr03.account_0148
-DEL account.account.template: l10n_de_skr03.account_0149
-DEL account.account.template: l10n_de_skr03.account_0150
-DEL account.account.template: l10n_de_skr03.account_0159
-DEL account.account.template: l10n_de_skr03.account_0160
-DEL account.account.template: l10n_de_skr03.account_0165
-DEL account.account.template: l10n_de_skr03.account_0170
-DEL account.account.template: l10n_de_skr03.account_0175
-DEL account.account.template: l10n_de_skr03.account_0176
-DEL account.account.template: l10n_de_skr03.account_0177
-DEL account.account.template: l10n_de_skr03.account_0178
-DEL account.account.template: l10n_de_skr03.account_0179
-DEL account.account.template: l10n_de_skr03.account_0180
-DEL account.account.template: l10n_de_skr03.account_0189
-DEL account.account.template: l10n_de_skr03.account_0190
-DEL account.account.template: l10n_de_skr03.account_0191
-DEL account.account.template: l10n_de_skr03.account_0192
-DEL account.account.template: l10n_de_skr03.account_0193
-DEL account.account.template: l10n_de_skr03.account_0194
-DEL account.account.template: l10n_de_skr03.account_0195
-DEL account.account.template: l10n_de_skr03.account_0199
-DEL account.account.template: l10n_de_skr03.account_0200
-DEL account.account.template: l10n_de_skr03.account_0210
-DEL account.account.template: l10n_de_skr03.account_0220
-DEL account.account.template: l10n_de_skr03.account_0240
-DEL account.account.template: l10n_de_skr03.account_0260
-DEL account.account.template: l10n_de_skr03.account_0280
-DEL account.account.template: l10n_de_skr03.account_0290
-DEL account.account.template: l10n_de_skr03.account_0299
-DEL account.account.template: l10n_de_skr03.account_0300
-DEL account.account.template: l10n_de_skr03.account_0310
-DEL account.account.template: l10n_de_skr03.account_0320
-DEL account.account.template: l10n_de_skr03.account_0350
-DEL account.account.template: l10n_de_skr03.account_0380
-DEL account.account.template: l10n_de_skr03.account_0400
-DEL account.account.template: l10n_de_skr03.account_0410
-DEL account.account.template: l10n_de_skr03.account_0420
-DEL account.account.template: l10n_de_skr03.account_0430
-DEL account.account.template: l10n_de_skr03.account_0440
-DEL account.account.template: l10n_de_skr03.account_0450
-DEL account.account.template: l10n_de_skr03.account_0460
-DEL account.account.template: l10n_de_skr03.account_0480
-DEL account.account.template: l10n_de_skr03.account_0485
-DEL account.account.template: l10n_de_skr03.account_0490
-DEL account.account.template: l10n_de_skr03.account_0498
-DEL account.account.template: l10n_de_skr03.account_0499
-DEL account.account.template: l10n_de_skr03.account_0500
-DEL account.account.template: l10n_de_skr03.account_0501
-DEL account.account.template: l10n_de_skr03.account_0502
-DEL account.account.template: l10n_de_skr03.account_0503
-DEL account.account.template: l10n_de_skr03.account_0504
-DEL account.account.template: l10n_de_skr03.account_0505
-DEL account.account.template: l10n_de_skr03.account_0506
-DEL account.account.template: l10n_de_skr03.account_0507
-DEL account.account.template: l10n_de_skr03.account_0508
-DEL account.account.template: l10n_de_skr03.account_0509
-DEL account.account.template: l10n_de_skr03.account_0510
-DEL account.account.template: l10n_de_skr03.account_0513
-DEL account.account.template: l10n_de_skr03.account_0516
-DEL account.account.template: l10n_de_skr03.account_0517
-DEL account.account.template: l10n_de_skr03.account_0518
-DEL account.account.template: l10n_de_skr03.account_0519
-DEL account.account.template: l10n_de_skr03.account_0520
-DEL account.account.template: l10n_de_skr03.account_0523
-DEL account.account.template: l10n_de_skr03.account_0524
-DEL account.account.template: l10n_de_skr03.account_0525
-DEL account.account.template: l10n_de_skr03.account_0530
-DEL account.account.template: l10n_de_skr03.account_0535
-DEL account.account.template: l10n_de_skr03.account_0540
-DEL account.account.template: l10n_de_skr03.account_0550
-DEL account.account.template: l10n_de_skr03.account_0570
-DEL account.account.template: l10n_de_skr03.account_0580
-DEL account.account.template: l10n_de_skr03.account_0582
-DEL account.account.template: l10n_de_skr03.account_0584
-DEL account.account.template: l10n_de_skr03.account_0586
-DEL account.account.template: l10n_de_skr03.account_0590
-DEL account.account.template: l10n_de_skr03.account_0595
-DEL account.account.template: l10n_de_skr03.account_0600
-DEL account.account.template: l10n_de_skr03.account_0601
-DEL account.account.template: l10n_de_skr03.account_0605
-DEL account.account.template: l10n_de_skr03.account_0610
-DEL account.account.template: l10n_de_skr03.account_0615
-DEL account.account.template: l10n_de_skr03.account_0616
-DEL account.account.template: l10n_de_skr03.account_0620
-DEL account.account.template: l10n_de_skr03.account_0625
-DEL account.account.template: l10n_de_skr03.account_0630
-DEL account.account.template: l10n_de_skr03.account_0631
-DEL account.account.template: l10n_de_skr03.account_0640
-DEL account.account.template: l10n_de_skr03.account_0650
-DEL account.account.template: l10n_de_skr03.account_0660
-DEL account.account.template: l10n_de_skr03.account_0661
-DEL account.account.template: l10n_de_skr03.account_0670
-DEL account.account.template: l10n_de_skr03.account_0680
-DEL account.account.template: l10n_de_skr03.account_0699
-DEL account.account.template: l10n_de_skr03.account_0700
-DEL account.account.template: l10n_de_skr03.account_0701
-DEL account.account.template: l10n_de_skr03.account_0705
-DEL account.account.template: l10n_de_skr03.account_0710
-DEL account.account.template: l10n_de_skr03.account_0715
-DEL account.account.template: l10n_de_skr03.account_0716
-DEL account.account.template: l10n_de_skr03.account_0720
-DEL account.account.template: l10n_de_skr03.account_0725
-DEL account.account.template: l10n_de_skr03.account_0730
-DEL account.account.template: l10n_de_skr03.account_0731
-DEL account.account.template: l10n_de_skr03.account_0740
-DEL account.account.template: l10n_de_skr03.account_0750
-DEL account.account.template: l10n_de_skr03.account_0755
-DEL account.account.template: l10n_de_skr03.account_0760
-DEL account.account.template: l10n_de_skr03.account_0761
-DEL account.account.template: l10n_de_skr03.account_0764
-DEL account.account.template: l10n_de_skr03.account_0767
-DEL account.account.template: l10n_de_skr03.account_0770
-DEL account.account.template: l10n_de_skr03.account_0771
-DEL account.account.template: l10n_de_skr03.account_0774
-DEL account.account.template: l10n_de_skr03.account_0777
-DEL account.account.template: l10n_de_skr03.account_0780
-DEL account.account.template: l10n_de_skr03.account_0781
-DEL account.account.template: l10n_de_skr03.account_0784
-DEL account.account.template: l10n_de_skr03.account_0787
-DEL account.account.template: l10n_de_skr03.account_0799
-DEL account.account.template: l10n_de_skr03.account_0809
-DEL account.account.template: l10n_de_skr03.account_0810
-DEL account.account.template: l10n_de_skr03.account_0811
-DEL account.account.template: l10n_de_skr03.account_0812
-DEL account.account.template: l10n_de_skr03.account_0813
-DEL account.account.template: l10n_de_skr03.account_0815
-DEL account.account.template: l10n_de_skr03.account_0819
-DEL account.account.template: l10n_de_skr03.account_0839
-DEL account.account.template: l10n_de_skr03.account_0845
-DEL account.account.template: l10n_de_skr03.account_0848
-DEL account.account.template: l10n_de_skr03.account_0849
-DEL account.account.template: l10n_de_skr03.account_0852
-DEL account.account.template: l10n_de_skr03.account_0853
-DEL account.account.template: l10n_de_skr03.account_0854
-DEL account.account.template: l10n_de_skr03.account_0857
-DEL account.account.template: l10n_de_skr03.account_0858
-DEL account.account.template: l10n_de_skr03.account_0859
-DEL account.account.template: l10n_de_skr03.account_0865
-DEL account.account.template: l10n_de_skr03.account_0867
-DEL account.account.template: l10n_de_skr03.account_0870
-DEL account.account.template: l10n_de_skr03.account_0880
-DEL account.account.template: l10n_de_skr03.account_0890
-DEL account.account.template: l10n_de_skr03.account_0900
-DEL account.account.template: l10n_de_skr03.account_0910
-DEL account.account.template: l10n_de_skr03.account_0920
-DEL account.account.template: l10n_de_skr03.account_0950
-DEL account.account.template: l10n_de_skr03.account_0951
-DEL account.account.template: l10n_de_skr03.account_0952
-DEL account.account.template: l10n_de_skr03.account_0953
-DEL account.account.template: l10n_de_skr03.account_0954
-DEL account.account.template: l10n_de_skr03.account_0955
-DEL account.account.template: l10n_de_skr03.account_0956
-DEL account.account.template: l10n_de_skr03.account_0957
-DEL account.account.template: l10n_de_skr03.account_0961
-DEL account.account.template: l10n_de_skr03.account_0962
-DEL account.account.template: l10n_de_skr03.account_0963
-DEL account.account.template: l10n_de_skr03.account_0964
-DEL account.account.template: l10n_de_skr03.account_0965
-DEL account.account.template: l10n_de_skr03.account_0966
-DEL account.account.template: l10n_de_skr03.account_0967
-DEL account.account.template: l10n_de_skr03.account_0968
-DEL account.account.template: l10n_de_skr03.account_0969
-DEL account.account.template: l10n_de_skr03.account_0970
-DEL account.account.template: l10n_de_skr03.account_0971
-DEL account.account.template: l10n_de_skr03.account_0973
-DEL account.account.template: l10n_de_skr03.account_0974
-DEL account.account.template: l10n_de_skr03.account_0976
-DEL account.account.template: l10n_de_skr03.account_0977
-DEL account.account.template: l10n_de_skr03.account_0978
-DEL account.account.template: l10n_de_skr03.account_0979
-DEL account.account.template: l10n_de_skr03.account_0980
-DEL account.account.template: l10n_de_skr03.account_0983
-DEL account.account.template: l10n_de_skr03.account_0984
-DEL account.account.template: l10n_de_skr03.account_0985
-DEL account.account.template: l10n_de_skr03.account_0986
-DEL account.account.template: l10n_de_skr03.account_0987
-DEL account.account.template: l10n_de_skr03.account_0988
-DEL account.account.template: l10n_de_skr03.account_0989
-DEL account.account.template: l10n_de_skr03.account_0990
-DEL account.account.template: l10n_de_skr03.account_0996
-DEL account.account.template: l10n_de_skr03.account_0997
-DEL account.account.template: l10n_de_skr03.account_0998
-DEL account.account.template: l10n_de_skr03.account_0999
-DEL account.account.template: l10n_de_skr03.account_1010
-DEL account.account.template: l10n_de_skr03.account_1020
-DEL account.account.template: l10n_de_skr03.account_1100
-DEL account.account.template: l10n_de_skr03.account_1110
-DEL account.account.template: l10n_de_skr03.account_1120
-DEL account.account.template: l10n_de_skr03.account_1130
-DEL account.account.template: l10n_de_skr03.account_1190
-DEL account.account.template: l10n_de_skr03.account_1195
-DEL account.account.template: l10n_de_skr03.account_1210
-DEL account.account.template: l10n_de_skr03.account_1220
-DEL account.account.template: l10n_de_skr03.account_1230
-DEL account.account.template: l10n_de_skr03.account_1240
-DEL account.account.template: l10n_de_skr03.account_1250
-DEL account.account.template: l10n_de_skr03.account_1290
-DEL account.account.template: l10n_de_skr03.account_1295
-DEL account.account.template: l10n_de_skr03.account_1300
-DEL account.account.template: l10n_de_skr03.account_1301
-DEL account.account.template: l10n_de_skr03.account_1302
-DEL account.account.template: l10n_de_skr03.account_1305
-DEL account.account.template: l10n_de_skr03.account_1310
-DEL account.account.template: l10n_de_skr03.account_1311
-DEL account.account.template: l10n_de_skr03.account_1312
-DEL account.account.template: l10n_de_skr03.account_1315
-DEL account.account.template: l10n_de_skr03.account_1320
-DEL account.account.template: l10n_de_skr03.account_1321
-DEL account.account.template: l10n_de_skr03.account_1322
-DEL account.account.template: l10n_de_skr03.account_1325
-DEL account.account.template: l10n_de_skr03.account_1327
-DEL account.account.template: l10n_de_skr03.account_1329
-DEL account.account.template: l10n_de_skr03.account_1330
-DEL account.account.template: l10n_de_skr03.account_1340
-DEL account.account.template: l10n_de_skr03.account_1344
-DEL account.account.template: l10n_de_skr03.account_1348
-DEL account.account.template: l10n_de_skr03.account_1349
-DEL account.account.template: l10n_de_skr03.account_1350
-DEL account.account.template: l10n_de_skr03.account_1352
-DEL account.account.template: l10n_de_skr03.account_1353
-DEL account.account.template: l10n_de_skr03.account_1354
-DEL account.account.template: l10n_de_skr03.account_1355
-DEL account.account.template: l10n_de_skr03.account_1356
-DEL account.account.template: l10n_de_skr03.account_1357
-DEL account.account.template: l10n_de_skr03.account_1370
-DEL account.account.template: l10n_de_skr03.account_1371
-DEL account.account.template: l10n_de_skr03.account_1372
-DEL account.account.template: l10n_de_skr03.account_1373
-DEL account.account.template: l10n_de_skr03.account_1374
-DEL account.account.template: l10n_de_skr03.account_1375
-DEL account.account.template: l10n_de_skr03.account_1376
-DEL account.account.template: l10n_de_skr03.account_1377
-DEL account.account.template: l10n_de_skr03.account_1378
-DEL account.account.template: l10n_de_skr03.account_1380
-DEL account.account.template: l10n_de_skr03.account_1381
-DEL account.account.template: l10n_de_skr03.account_1382
-DEL account.account.template: l10n_de_skr03.account_1383
-DEL account.account.template: l10n_de_skr03.account_1385
-DEL account.account.template: l10n_de_skr03.account_1386
-DEL account.account.template: l10n_de_skr03.account_1387
-DEL account.account.template: l10n_de_skr03.account_1389
-DEL account.account.template: l10n_de_skr03.account_1390
-DEL account.account.template: l10n_de_skr03.account_1400
-DEL account.account.template: l10n_de_skr03.account_1401
-DEL account.account.template: l10n_de_skr03.account_1410
-DEL account.account.template: l10n_de_skr03.account_1411
-DEL account.account.template: l10n_de_skr03.account_1445
-DEL account.account.template: l10n_de_skr03.account_1446
-DEL account.account.template: l10n_de_skr03.account_1447
-DEL account.account.template: l10n_de_skr03.account_1448
-DEL account.account.template: l10n_de_skr03.account_1449
-DEL account.account.template: l10n_de_skr03.account_1450
-DEL account.account.template: l10n_de_skr03.account_1451
-DEL account.account.template: l10n_de_skr03.account_1455
-DEL account.account.template: l10n_de_skr03.account_1460
-DEL account.account.template: l10n_de_skr03.account_1461
-DEL account.account.template: l10n_de_skr03.account_1465
-DEL account.account.template: l10n_de_skr03.account_1470
-DEL account.account.template: l10n_de_skr03.account_1471
-DEL account.account.template: l10n_de_skr03.account_1475
-DEL account.account.template: l10n_de_skr03.account_1478
-DEL account.account.template: l10n_de_skr03.account_1479
-DEL account.account.template: l10n_de_skr03.account_1480
-DEL account.account.template: l10n_de_skr03.account_1481
-DEL account.account.template: l10n_de_skr03.account_1485
-DEL account.account.template: l10n_de_skr03.account_1488
-DEL account.account.template: l10n_de_skr03.account_1489
-DEL account.account.template: l10n_de_skr03.account_1490
-DEL account.account.template: l10n_de_skr03.account_1491
-DEL account.account.template: l10n_de_skr03.account_1495
-DEL account.account.template: l10n_de_skr03.account_1498
-DEL account.account.template: l10n_de_skr03.account_1499
-DEL account.account.template: l10n_de_skr03.account_1500
-DEL account.account.template: l10n_de_skr03.account_1501
-DEL account.account.template: l10n_de_skr03.account_1502
-DEL account.account.template: l10n_de_skr03.account_1503
-DEL account.account.template: l10n_de_skr03.account_1504
-DEL account.account.template: l10n_de_skr03.account_1505
-DEL account.account.template: l10n_de_skr03.account_1506
-DEL account.account.template: l10n_de_skr03.account_1507
-DEL account.account.template: l10n_de_skr03.account_1508
-DEL account.account.template: l10n_de_skr03.account_1510
-DEL account.account.template: l10n_de_skr03.account_1511
-DEL account.account.template: l10n_de_skr03.account_1518
-DEL account.account.template: l10n_de_skr03.account_1519
-DEL account.account.template: l10n_de_skr03.account_1520
-DEL account.account.template: l10n_de_skr03.account_1521
-DEL account.account.template: l10n_de_skr03.account_1522
-DEL account.account.template: l10n_de_skr03.account_1524
-DEL account.account.template: l10n_de_skr03.account_1525
-DEL account.account.template: l10n_de_skr03.account_1526
-DEL account.account.template: l10n_de_skr03.account_1527
-DEL account.account.template: l10n_de_skr03.account_1528
-DEL account.account.template: l10n_de_skr03.account_1529
-DEL account.account.template: l10n_de_skr03.account_1530
-DEL account.account.template: l10n_de_skr03.account_1531
-DEL account.account.template: l10n_de_skr03.account_1537
-DEL account.account.template: l10n_de_skr03.account_1538
-DEL account.account.template: l10n_de_skr03.account_1539
-DEL account.account.template: l10n_de_skr03.account_1540
-DEL account.account.template: l10n_de_skr03.account_1542
-DEL account.account.template: l10n_de_skr03.account_1543
-DEL account.account.template: l10n_de_skr03.account_1544
-DEL account.account.template: l10n_de_skr03.account_1545
-DEL account.account.template: l10n_de_skr03.account_1547
-DEL account.account.template: l10n_de_skr03.account_1548
-DEL account.account.template: l10n_de_skr03.account_1549
-DEL account.account.template: l10n_de_skr03.account_1550
-DEL account.account.template: l10n_de_skr03.account_1551
-DEL account.account.template: l10n_de_skr03.account_1555
-DEL account.account.template: l10n_de_skr03.account_1556
-DEL account.account.template: l10n_de_skr03.account_1557
-DEL account.account.template: l10n_de_skr03.account_1558
-DEL account.account.template: l10n_de_skr03.account_1559
-DEL account.account.template: l10n_de_skr03.account_1560
-DEL account.account.template: l10n_de_skr03.account_1561
-DEL account.account.template: l10n_de_skr03.account_1562
-DEL account.account.template: l10n_de_skr03.account_1563
-DEL account.account.template: l10n_de_skr03.account_1566
-DEL account.account.template: l10n_de_skr03.account_1567
-DEL account.account.template: l10n_de_skr03.account_1569
-DEL account.account.template: l10n_de_skr03.account_1570
-DEL account.account.template: l10n_de_skr03.account_1571
-DEL account.account.template: l10n_de_skr03.account_1572
-DEL account.account.template: l10n_de_skr03.account_1574
-DEL account.account.template: l10n_de_skr03.account_1576
-DEL account.account.template: l10n_de_skr03.account_1577
-DEL account.account.template: l10n_de_skr03.account_1578
-DEL account.account.template: l10n_de_skr03.account_1580
-DEL account.account.template: l10n_de_skr03.account_1581
-DEL account.account.template: l10n_de_skr03.account_1582
-DEL account.account.template: l10n_de_skr03.account_1583
-DEL account.account.template: l10n_de_skr03.account_1584
-DEL account.account.template: l10n_de_skr03.account_1585
-DEL account.account.template: l10n_de_skr03.account_1587
-DEL account.account.template: l10n_de_skr03.account_1588
-DEL account.account.template: l10n_de_skr03.account_1590
-DEL account.account.template: l10n_de_skr03.account_1592
-DEL account.account.template: l10n_de_skr03.account_1593
-DEL account.account.template: l10n_de_skr03.account_1594
-DEL account.account.template: l10n_de_skr03.account_1595
-DEL account.account.template: l10n_de_skr03.account_1596
-DEL account.account.template: l10n_de_skr03.account_1597
-DEL account.account.template: l10n_de_skr03.account_1598
-DEL account.account.template: l10n_de_skr03.account_1599
-DEL account.account.template: l10n_de_skr03.account_1600
-DEL account.account.template: l10n_de_skr03.account_1601
-DEL account.account.template: l10n_de_skr03.account_1605
-DEL account.account.template: l10n_de_skr03.account_1606
-DEL account.account.template: l10n_de_skr03.account_1607
-DEL account.account.template: l10n_de_skr03.account_1609
-DEL account.account.template: l10n_de_skr03.account_1610
-DEL account.account.template: l10n_de_skr03.account_1624
-DEL account.account.template: l10n_de_skr03.account_1625
-DEL account.account.template: l10n_de_skr03.account_1626
-DEL account.account.template: l10n_de_skr03.account_1628
-DEL account.account.template: l10n_de_skr03.account_1630
-DEL account.account.template: l10n_de_skr03.account_1631
-DEL account.account.template: l10n_de_skr03.account_1635
-DEL account.account.template: l10n_de_skr03.account_1638
-DEL account.account.template: l10n_de_skr03.account_1640
-DEL account.account.template: l10n_de_skr03.account_1641
-DEL account.account.template: l10n_de_skr03.account_1645
-DEL account.account.template: l10n_de_skr03.account_1648
-DEL account.account.template: l10n_de_skr03.account_1650
-DEL account.account.template: l10n_de_skr03.account_1651
-DEL account.account.template: l10n_de_skr03.account_1655
-DEL account.account.template: l10n_de_skr03.account_1658
-DEL account.account.template: l10n_de_skr03.account_1659
-DEL account.account.template: l10n_de_skr03.account_1660
-DEL account.account.template: l10n_de_skr03.account_1661
-DEL account.account.template: l10n_de_skr03.account_1662
-DEL account.account.template: l10n_de_skr03.account_1663
-DEL account.account.template: l10n_de_skr03.account_1665
-DEL account.account.template: l10n_de_skr03.account_1666
-DEL account.account.template: l10n_de_skr03.account_1667
-DEL account.account.template: l10n_de_skr03.account_1668
-DEL account.account.template: l10n_de_skr03.account_1670
-DEL account.account.template: l10n_de_skr03.account_1671
-DEL account.account.template: l10n_de_skr03.account_1672
-DEL account.account.template: l10n_de_skr03.account_1673
-DEL account.account.template: l10n_de_skr03.account_1675
-DEL account.account.template: l10n_de_skr03.account_1676
-DEL account.account.template: l10n_de_skr03.account_1677
-DEL account.account.template: l10n_de_skr03.account_1678
-DEL account.account.template: l10n_de_skr03.account_1691
-DEL account.account.template: l10n_de_skr03.account_1695
-DEL account.account.template: l10n_de_skr03.account_1696
-DEL account.account.template: l10n_de_skr03.account_1697
-DEL account.account.template: l10n_de_skr03.account_1698
-DEL account.account.template: l10n_de_skr03.account_1700
-DEL account.account.template: l10n_de_skr03.account_1701
-DEL account.account.template: l10n_de_skr03.account_1702
-DEL account.account.template: l10n_de_skr03.account_1703
-DEL account.account.template: l10n_de_skr03.account_1704
-DEL account.account.template: l10n_de_skr03.account_1705
-DEL account.account.template: l10n_de_skr03.account_1706
-DEL account.account.template: l10n_de_skr03.account_1707
-DEL account.account.template: l10n_de_skr03.account_1708
-DEL account.account.template: l10n_de_skr03.account_1709
-DEL account.account.template: l10n_de_skr03.account_1710
-DEL account.account.template: l10n_de_skr03.account_1711
-DEL account.account.template: l10n_de_skr03.account_1716
-DEL account.account.template: l10n_de_skr03.account_1718
-DEL account.account.template: l10n_de_skr03.account_1719
-DEL account.account.template: l10n_de_skr03.account_1720
-DEL account.account.template: l10n_de_skr03.account_1721
-DEL account.account.template: l10n_de_skr03.account_1722
-DEL account.account.template: l10n_de_skr03.account_1725
-DEL account.account.template: l10n_de_skr03.account_1728
-DEL account.account.template: l10n_de_skr03.account_1729
-DEL account.account.template: l10n_de_skr03.account_1730
-DEL account.account.template: l10n_de_skr03.account_1731
-DEL account.account.template: l10n_de_skr03.account_1732
-DEL account.account.template: l10n_de_skr03.account_1733
-DEL account.account.template: l10n_de_skr03.account_1734
-DEL account.account.template: l10n_de_skr03.account_1735
-DEL account.account.template: l10n_de_skr03.account_1736
-DEL account.account.template: l10n_de_skr03.account_1737
-DEL account.account.template: l10n_de_skr03.account_1738
-DEL account.account.template: l10n_de_skr03.account_1739
-DEL account.account.template: l10n_de_skr03.account_1740
-DEL account.account.template: l10n_de_skr03.account_1741
-DEL account.account.template: l10n_de_skr03.account_1742
-DEL account.account.template: l10n_de_skr03.account_1743
-DEL account.account.template: l10n_de_skr03.account_1744
-DEL account.account.template: l10n_de_skr03.account_1745
-DEL account.account.template: l10n_de_skr03.account_1746
-DEL account.account.template: l10n_de_skr03.account_1747
-DEL account.account.template: l10n_de_skr03.account_1748
-DEL account.account.template: l10n_de_skr03.account_1749
-DEL account.account.template: l10n_de_skr03.account_1750
-DEL account.account.template: l10n_de_skr03.account_1751
-DEL account.account.template: l10n_de_skr03.account_1752
-DEL account.account.template: l10n_de_skr03.account_1753
-DEL account.account.template: l10n_de_skr03.account_1754
-DEL account.account.template: l10n_de_skr03.account_1755
-DEL account.account.template: l10n_de_skr03.account_1756
-DEL account.account.template: l10n_de_skr03.account_1758
-DEL account.account.template: l10n_de_skr03.account_1759
-DEL account.account.template: l10n_de_skr03.account_1760
-DEL account.account.template: l10n_de_skr03.account_1761
-DEL account.account.template: l10n_de_skr03.account_1762
-DEL account.account.template: l10n_de_skr03.account_1764
-DEL account.account.template: l10n_de_skr03.account_1766
-DEL account.account.template: l10n_de_skr03.account_1767
-DEL account.account.template: l10n_de_skr03.account_1768
-DEL account.account.template: l10n_de_skr03.account_1769
-DEL account.account.template: l10n_de_skr03.account_1770
-DEL account.account.template: l10n_de_skr03.account_1771
-DEL account.account.template: l10n_de_skr03.account_1772
-DEL account.account.template: l10n_de_skr03.account_1774
-DEL account.account.template: l10n_de_skr03.account_1776
-DEL account.account.template: l10n_de_skr03.account_1777
-DEL account.account.template: l10n_de_skr03.account_1778
-DEL account.account.template: l10n_de_skr03.account_1779
-DEL account.account.template: l10n_de_skr03.account_1780
-DEL account.account.template: l10n_de_skr03.account_1781
-DEL account.account.template: l10n_de_skr03.account_1782
-DEL account.account.template: l10n_de_skr03.account_1783
-DEL account.account.template: l10n_de_skr03.account_1784
-DEL account.account.template: l10n_de_skr03.account_1785
-DEL account.account.template: l10n_de_skr03.account_1787
-DEL account.account.template: l10n_de_skr03.account_1788
-DEL account.account.template: l10n_de_skr03.account_1789
-DEL account.account.template: l10n_de_skr03.account_1790
-DEL account.account.template: l10n_de_skr03.account_1791
-DEL account.account.template: l10n_de_skr03.account_1792
-DEL account.account.template: l10n_de_skr03.account_1793
-DEL account.account.template: l10n_de_skr03.account_1794
-DEL account.account.template: l10n_de_skr03.account_1795
-DEL account.account.template: l10n_de_skr03.account_1796
-DEL account.account.template: l10n_de_skr03.account_1797
-DEL account.account.template: l10n_de_skr03.account_1800
-DEL account.account.template: l10n_de_skr03.account_1810
-DEL account.account.template: l10n_de_skr03.account_1820
-DEL account.account.template: l10n_de_skr03.account_1830
-DEL account.account.template: l10n_de_skr03.account_1840
-DEL account.account.template: l10n_de_skr03.account_1850
-DEL account.account.template: l10n_de_skr03.account_1860
-DEL account.account.template: l10n_de_skr03.account_1869
-DEL account.account.template: l10n_de_skr03.account_1870
-DEL account.account.template: l10n_de_skr03.account_1879
-DEL account.account.template: l10n_de_skr03.account_1880
-DEL account.account.template: l10n_de_skr03.account_1890
-DEL account.account.template: l10n_de_skr03.account_1900
-DEL account.account.template: l10n_de_skr03.account_1910
-DEL account.account.template: l10n_de_skr03.account_1920
-DEL account.account.template: l10n_de_skr03.account_1930
-DEL account.account.template: l10n_de_skr03.account_1940
-DEL account.account.template: l10n_de_skr03.account_1950
-DEL account.account.template: l10n_de_skr03.account_1960
-DEL account.account.template: l10n_de_skr03.account_1970
-DEL account.account.template: l10n_de_skr03.account_1980
-DEL account.account.template: l10n_de_skr03.account_1990
-DEL account.account.template: l10n_de_skr03.account_2000
-DEL account.account.template: l10n_de_skr03.account_2001
-DEL account.account.template: l10n_de_skr03.account_2004
-DEL account.account.template: l10n_de_skr03.account_2005
-DEL account.account.template: l10n_de_skr03.account_2006
-DEL account.account.template: l10n_de_skr03.account_2007
-DEL account.account.template: l10n_de_skr03.account_2008
-DEL account.account.template: l10n_de_skr03.account_2010
-DEL account.account.template: l10n_de_skr03.account_2020
-DEL account.account.template: l10n_de_skr03.account_2090
-DEL account.account.template: l10n_de_skr03.account_2091
-DEL account.account.template: l10n_de_skr03.account_2092
-DEL account.account.template: l10n_de_skr03.account_2094
-DEL account.account.template: l10n_de_skr03.account_2100
-DEL account.account.template: l10n_de_skr03.account_2102
-DEL account.account.template: l10n_de_skr03.account_2103
-DEL account.account.template: l10n_de_skr03.account_2104
-DEL account.account.template: l10n_de_skr03.account_2105
-DEL account.account.template: l10n_de_skr03.account_2106
-DEL account.account.template: l10n_de_skr03.account_2107
-DEL account.account.template: l10n_de_skr03.account_2108
-DEL account.account.template: l10n_de_skr03.account_2109
-DEL account.account.template: l10n_de_skr03.account_2110
-DEL account.account.template: l10n_de_skr03.account_2113
-DEL account.account.template: l10n_de_skr03.account_2114
-DEL account.account.template: l10n_de_skr03.account_2115
-DEL account.account.template: l10n_de_skr03.account_2116
-DEL account.account.template: l10n_de_skr03.account_2117
-DEL account.account.template: l10n_de_skr03.account_2118
-DEL account.account.template: l10n_de_skr03.account_2119
-DEL account.account.template: l10n_de_skr03.account_2120
-DEL account.account.template: l10n_de_skr03.account_2123
-DEL account.account.template: l10n_de_skr03.account_2124
-DEL account.account.template: l10n_de_skr03.account_2125
-DEL account.account.template: l10n_de_skr03.account_2126
-DEL account.account.template: l10n_de_skr03.account_2127
-DEL account.account.template: l10n_de_skr03.account_2128
-DEL account.account.template: l10n_de_skr03.account_2129
-DEL account.account.template: l10n_de_skr03.account_2130
-DEL account.account.template: l10n_de_skr03.account_2139
-DEL account.account.template: l10n_de_skr03.account_2140
-DEL account.account.template: l10n_de_skr03.account_2141
-DEL account.account.template: l10n_de_skr03.account_2142
-DEL account.account.template: l10n_de_skr03.account_2143
-DEL account.account.template: l10n_de_skr03.account_2144
-DEL account.account.template: l10n_de_skr03.account_2145
-DEL account.account.template: l10n_de_skr03.account_2146
-DEL account.account.template: l10n_de_skr03.account_2147
-DEL account.account.template: l10n_de_skr03.account_2148
-DEL account.account.template: l10n_de_skr03.account_2149
-DEL account.account.template: l10n_de_skr03.account_2150
-DEL account.account.template: l10n_de_skr03.account_2151
-DEL account.account.template: l10n_de_skr03.account_2166
-DEL account.account.template: l10n_de_skr03.account_2170
-DEL account.account.template: l10n_de_skr03.account_2171
-DEL account.account.template: l10n_de_skr03.account_2176
-DEL account.account.template: l10n_de_skr03.account_2200
-DEL account.account.template: l10n_de_skr03.account_2203
-DEL account.account.template: l10n_de_skr03.account_2204
-DEL account.account.template: l10n_de_skr03.account_2208
-DEL account.account.template: l10n_de_skr03.account_2209
-DEL account.account.template: l10n_de_skr03.account_2210
-DEL account.account.template: l10n_de_skr03.account_2213
-DEL account.account.template: l10n_de_skr03.account_2216
-DEL account.account.template: l10n_de_skr03.account_2219
-DEL account.account.template: l10n_de_skr03.account_2250
-DEL account.account.template: l10n_de_skr03.account_2255
-DEL account.account.template: l10n_de_skr03.account_2260
-DEL account.account.template: l10n_de_skr03.account_2265
-DEL account.account.template: l10n_de_skr03.account_2280
-DEL account.account.template: l10n_de_skr03.account_2281
-DEL account.account.template: l10n_de_skr03.account_2282
-DEL account.account.template: l10n_de_skr03.account_2283
-DEL account.account.template: l10n_de_skr03.account_2284
-DEL account.account.template: l10n_de_skr03.account_2285
-DEL account.account.template: l10n_de_skr03.account_2287
-DEL account.account.template: l10n_de_skr03.account_2289
-DEL account.account.template: l10n_de_skr03.account_2300
-DEL account.account.template: l10n_de_skr03.account_2307
-DEL account.account.template: l10n_de_skr03.account_2308
-DEL account.account.template: l10n_de_skr03.account_2309
-DEL account.account.template: l10n_de_skr03.account_2310
-DEL account.account.template: l10n_de_skr03.account_2311
-DEL account.account.template: l10n_de_skr03.account_2312
-DEL account.account.template: l10n_de_skr03.account_2313
-DEL account.account.template: l10n_de_skr03.account_2315
-DEL account.account.template: l10n_de_skr03.account_2316
-DEL account.account.template: l10n_de_skr03.account_2317
-DEL account.account.template: l10n_de_skr03.account_2318
-DEL account.account.template: l10n_de_skr03.account_2320
-DEL account.account.template: l10n_de_skr03.account_2323
-DEL account.account.template: l10n_de_skr03.account_2325
-DEL account.account.template: l10n_de_skr03.account_2326
-DEL account.account.template: l10n_de_skr03.account_2327
-DEL account.account.template: l10n_de_skr03.account_2328
-DEL account.account.template: l10n_de_skr03.account_2339
-DEL account.account.template: l10n_de_skr03.account_2340
-DEL account.account.template: l10n_de_skr03.account_2341
-DEL account.account.template: l10n_de_skr03.account_2342
-DEL account.account.template: l10n_de_skr03.account_2344
-DEL account.account.template: l10n_de_skr03.account_2345
-DEL account.account.template: l10n_de_skr03.account_2347
-DEL account.account.template: l10n_de_skr03.account_2350
-DEL account.account.template: l10n_de_skr03.account_2375
-DEL account.account.template: l10n_de_skr03.account_2380
-DEL account.account.template: l10n_de_skr03.account_2381
-DEL account.account.template: l10n_de_skr03.account_2382
-DEL account.account.template: l10n_de_skr03.account_2383
-DEL account.account.template: l10n_de_skr03.account_2384
-DEL account.account.template: l10n_de_skr03.account_2385
-DEL account.account.template: l10n_de_skr03.account_2386
-DEL account.account.template: l10n_de_skr03.account_2387
-DEL account.account.template: l10n_de_skr03.account_2388
-DEL account.account.template: l10n_de_skr03.account_2389
-DEL account.account.template: l10n_de_skr03.account_2390
-DEL account.account.template: l10n_de_skr03.account_2400
-DEL account.account.template: l10n_de_skr03.account_2401
-DEL account.account.template: l10n_de_skr03.account_2402
-DEL account.account.template: l10n_de_skr03.account_2403
-DEL account.account.template: l10n_de_skr03.account_2406
-DEL account.account.template: l10n_de_skr03.account_2408
-DEL account.account.template: l10n_de_skr03.account_2430
-DEL account.account.template: l10n_de_skr03.account_2431
-DEL account.account.template: l10n_de_skr03.account_2436
-DEL account.account.template: l10n_de_skr03.account_2440
-DEL account.account.template: l10n_de_skr03.account_2441
-DEL account.account.template: l10n_de_skr03.account_2450
-DEL account.account.template: l10n_de_skr03.account_2451
-DEL account.account.template: l10n_de_skr03.account_2480
-DEL account.account.template: l10n_de_skr03.account_2481
-DEL account.account.template: l10n_de_skr03.account_2485
-DEL account.account.template: l10n_de_skr03.account_2490
-DEL account.account.template: l10n_de_skr03.account_2492
-DEL account.account.template: l10n_de_skr03.account_2493
-DEL account.account.template: l10n_de_skr03.account_2494
-DEL account.account.template: l10n_de_skr03.account_2498
-DEL account.account.template: l10n_de_skr03.account_2500
-DEL account.account.template: l10n_de_skr03.account_2501
-DEL account.account.template: l10n_de_skr03.account_2504
-DEL account.account.template: l10n_de_skr03.account_2505
-DEL account.account.template: l10n_de_skr03.account_2506
-DEL account.account.template: l10n_de_skr03.account_2507
-DEL account.account.template: l10n_de_skr03.account_2508
-DEL account.account.template: l10n_de_skr03.account_2510
-DEL account.account.template: l10n_de_skr03.account_2520
-DEL account.account.template: l10n_de_skr03.account_2590
-DEL account.account.template: l10n_de_skr03.account_2591
-DEL account.account.template: l10n_de_skr03.account_2592
-DEL account.account.template: l10n_de_skr03.account_2593
-DEL account.account.template: l10n_de_skr03.account_2594
-DEL account.account.template: l10n_de_skr03.account_2600
-DEL account.account.template: l10n_de_skr03.account_2603
-DEL account.account.template: l10n_de_skr03.account_2615
-DEL account.account.template: l10n_de_skr03.account_2616
-DEL account.account.template: l10n_de_skr03.account_2617
-DEL account.account.template: l10n_de_skr03.account_2618
-DEL account.account.template: l10n_de_skr03.account_2619
-DEL account.account.template: l10n_de_skr03.account_2620
-DEL account.account.template: l10n_de_skr03.account_2621
-DEL account.account.template: l10n_de_skr03.account_2622
-DEL account.account.template: l10n_de_skr03.account_2623
-DEL account.account.template: l10n_de_skr03.account_2625
-DEL account.account.template: l10n_de_skr03.account_2626
-DEL account.account.template: l10n_de_skr03.account_2640
-DEL account.account.template: l10n_de_skr03.account_2641
-DEL account.account.template: l10n_de_skr03.account_2646
-DEL account.account.template: l10n_de_skr03.account_2647
-DEL account.account.template: l10n_de_skr03.account_2648
-DEL account.account.template: l10n_de_skr03.account_2649
-DEL account.account.template: l10n_de_skr03.account_2650
-DEL account.account.template: l10n_de_skr03.account_2652
-DEL account.account.template: l10n_de_skr03.account_2653
-DEL account.account.template: l10n_de_skr03.account_2654
-DEL account.account.template: l10n_de_skr03.account_2655
-DEL account.account.template: l10n_de_skr03.account_2656
-DEL account.account.template: l10n_de_skr03.account_2657
-DEL account.account.template: l10n_de_skr03.account_2658
-DEL account.account.template: l10n_de_skr03.account_2659
-DEL account.account.template: l10n_de_skr03.account_2660
-DEL account.account.template: l10n_de_skr03.account_2661
-DEL account.account.template: l10n_de_skr03.account_2666
-DEL account.account.template: l10n_de_skr03.account_2670
-DEL account.account.template: l10n_de_skr03.account_2679
-DEL account.account.template: l10n_de_skr03.account_2680
-DEL account.account.template: l10n_de_skr03.account_2682
-DEL account.account.template: l10n_de_skr03.account_2683
-DEL account.account.template: l10n_de_skr03.account_2684
-DEL account.account.template: l10n_de_skr03.account_2685
-DEL account.account.template: l10n_de_skr03.account_2686
-DEL account.account.template: l10n_de_skr03.account_2687
-DEL account.account.template: l10n_de_skr03.account_2688
-DEL account.account.template: l10n_de_skr03.account_2689
-DEL account.account.template: l10n_de_skr03.account_2700
-DEL account.account.template: l10n_de_skr03.account_2705
-DEL account.account.template: l10n_de_skr03.account_2707
-DEL account.account.template: l10n_de_skr03.account_2709
-DEL account.account.template: l10n_de_skr03.account_2710
-DEL account.account.template: l10n_de_skr03.account_2711
-DEL account.account.template: l10n_de_skr03.account_2712
-DEL account.account.template: l10n_de_skr03.account_2713
-DEL account.account.template: l10n_de_skr03.account_2714
-DEL account.account.template: l10n_de_skr03.account_2715
-DEL account.account.template: l10n_de_skr03.account_2716
-DEL account.account.template: l10n_de_skr03.account_2720
-DEL account.account.template: l10n_de_skr03.account_2723
-DEL account.account.template: l10n_de_skr03.account_2725
-DEL account.account.template: l10n_de_skr03.account_2726
-DEL account.account.template: l10n_de_skr03.account_2727
-DEL account.account.template: l10n_de_skr03.account_2728
-DEL account.account.template: l10n_de_skr03.account_2729
-DEL account.account.template: l10n_de_skr03.account_2730
-DEL account.account.template: l10n_de_skr03.account_2731
-DEL account.account.template: l10n_de_skr03.account_2732
-DEL account.account.template: l10n_de_skr03.account_2733
-DEL account.account.template: l10n_de_skr03.account_2734
-DEL account.account.template: l10n_de_skr03.account_2735
-DEL account.account.template: l10n_de_skr03.account_2736
-DEL account.account.template: l10n_de_skr03.account_2738
-DEL account.account.template: l10n_de_skr03.account_2739
-DEL account.account.template: l10n_de_skr03.account_2740
-DEL account.account.template: l10n_de_skr03.account_2741
-DEL account.account.template: l10n_de_skr03.account_2742
-DEL account.account.template: l10n_de_skr03.account_2743
-DEL account.account.template: l10n_de_skr03.account_2744
-DEL account.account.template: l10n_de_skr03.account_2746
-DEL account.account.template: l10n_de_skr03.account_2747
-DEL account.account.template: l10n_de_skr03.account_2749
-DEL account.account.template: l10n_de_skr03.account_2750
-DEL account.account.template: l10n_de_skr03.account_2751
-DEL account.account.template: l10n_de_skr03.account_2752
-DEL account.account.template: l10n_de_skr03.account_2760
-DEL account.account.template: l10n_de_skr03.account_2762
-DEL account.account.template: l10n_de_skr03.account_2764
-DEL account.account.template: l10n_de_skr03.account_2790
-DEL account.account.template: l10n_de_skr03.account_2792
-DEL account.account.template: l10n_de_skr03.account_2794
-DEL account.account.template: l10n_de_skr03.account_2798
-DEL account.account.template: l10n_de_skr03.account_2840
-DEL account.account.template: l10n_de_skr03.account_2841
-DEL account.account.template: l10n_de_skr03.account_2850
-DEL account.account.template: l10n_de_skr03.account_2865
-DEL account.account.template: l10n_de_skr03.account_2867
-DEL account.account.template: l10n_de_skr03.account_2870
-DEL account.account.template: l10n_de_skr03.account_2890
-DEL account.account.template: l10n_de_skr03.account_2891
-DEL account.account.template: l10n_de_skr03.account_2892
-DEL account.account.template: l10n_de_skr03.account_2893
-DEL account.account.template: l10n_de_skr03.account_2894
-DEL account.account.template: l10n_de_skr03.account_2895
-DEL account.account.template: l10n_de_skr03.account_2990
-DEL account.account.template: l10n_de_skr03.account_3000
-DEL account.account.template: l10n_de_skr03.account_3010
-DEL account.account.template: l10n_de_skr03.account_3030
-DEL account.account.template: l10n_de_skr03.account_3060
-DEL account.account.template: l10n_de_skr03.account_3062
-DEL account.account.template: l10n_de_skr03.account_3066
-DEL account.account.template: l10n_de_skr03.account_3067
-DEL account.account.template: l10n_de_skr03.account_3070
-DEL account.account.template: l10n_de_skr03.account_3071
-DEL account.account.template: l10n_de_skr03.account_3075
-DEL account.account.template: l10n_de_skr03.account_3076
-DEL account.account.template: l10n_de_skr03.account_3089
-DEL account.account.template: l10n_de_skr03.account_3090
-DEL account.account.template: l10n_de_skr03.account_3091
-DEL account.account.template: l10n_de_skr03.account_3092
-DEL account.account.template: l10n_de_skr03.account_3100
-DEL account.account.template: l10n_de_skr03.account_3106
-DEL account.account.template: l10n_de_skr03.account_3108
-DEL account.account.template: l10n_de_skr03.account_3109
-DEL account.account.template: l10n_de_skr03.account_3110
-DEL account.account.template: l10n_de_skr03.account_3113
-DEL account.account.template: l10n_de_skr03.account_3115
-DEL account.account.template: l10n_de_skr03.account_3120
-DEL account.account.template: l10n_de_skr03.account_3123
-DEL account.account.template: l10n_de_skr03.account_3125
-DEL account.account.template: l10n_de_skr03.account_3130
-DEL account.account.template: l10n_de_skr03.account_3133
-DEL account.account.template: l10n_de_skr03.account_3135
-DEL account.account.template: l10n_de_skr03.account_3140
-DEL account.account.template: l10n_de_skr03.account_3143
-DEL account.account.template: l10n_de_skr03.account_3145
-DEL account.account.template: l10n_de_skr03.account_3150
-DEL account.account.template: l10n_de_skr03.account_3151
-DEL account.account.template: l10n_de_skr03.account_3153
-DEL account.account.template: l10n_de_skr03.account_3154
-DEL account.account.template: l10n_de_skr03.account_3160
-DEL account.account.template: l10n_de_skr03.account_3165
-DEL account.account.template: l10n_de_skr03.account_3170
-DEL account.account.template: l10n_de_skr03.account_3175
-DEL account.account.template: l10n_de_skr03.account_3180
-DEL account.account.template: l10n_de_skr03.account_3185
-DEL account.account.template: l10n_de_skr03.account_3200
-DEL account.account.template: l10n_de_skr03.account_3300
-DEL account.account.template: l10n_de_skr03.account_3349
-DEL account.account.template: l10n_de_skr03.account_3400
-DEL account.account.template: l10n_de_skr03.account_3420
-DEL account.account.template: l10n_de_skr03.account_3425
-DEL account.account.template: l10n_de_skr03.account_3430
-DEL account.account.template: l10n_de_skr03.account_3435
-DEL account.account.template: l10n_de_skr03.account_3440
-DEL account.account.template: l10n_de_skr03.account_3505
-DEL account.account.template: l10n_de_skr03.account_3540
-DEL account.account.template: l10n_de_skr03.account_3550
-DEL account.account.template: l10n_de_skr03.account_3551
-DEL account.account.template: l10n_de_skr03.account_3552
-DEL account.account.template: l10n_de_skr03.account_3553
-DEL account.account.template: l10n_de_skr03.account_3557
-DEL account.account.template: l10n_de_skr03.account_3558
-DEL account.account.template: l10n_de_skr03.account_3559
-DEL account.account.template: l10n_de_skr03.account_3560
-DEL account.account.template: l10n_de_skr03.account_3565
-DEL account.account.template: l10n_de_skr03.account_3600
-DEL account.account.template: l10n_de_skr03.account_3610
-DEL account.account.template: l10n_de_skr03.account_3660
-DEL account.account.template: l10n_de_skr03.account_3700
-DEL account.account.template: l10n_de_skr03.account_3701
-DEL account.account.template: l10n_de_skr03.account_3710
-DEL account.account.template: l10n_de_skr03.account_3714
-DEL account.account.template: l10n_de_skr03.account_3715
-DEL account.account.template: l10n_de_skr03.account_3717
-DEL account.account.template: l10n_de_skr03.account_3718
-DEL account.account.template: l10n_de_skr03.account_3720
-DEL account.account.template: l10n_de_skr03.account_3724
-DEL account.account.template: l10n_de_skr03.account_3725
-DEL account.account.template: l10n_de_skr03.account_3730
-DEL account.account.template: l10n_de_skr03.account_3731
-DEL account.account.template: l10n_de_skr03.account_3733
-DEL account.account.template: l10n_de_skr03.account_3734
-DEL account.account.template: l10n_de_skr03.account_3736
-DEL account.account.template: l10n_de_skr03.account_3738
-DEL account.account.template: l10n_de_skr03.account_3741
-DEL account.account.template: l10n_de_skr03.account_3743
-DEL account.account.template: l10n_de_skr03.account_3744
-DEL account.account.template: l10n_de_skr03.account_3745
-DEL account.account.template: l10n_de_skr03.account_3746
-DEL account.account.template: l10n_de_skr03.account_3748
-DEL account.account.template: l10n_de_skr03.account_3750
-DEL account.account.template: l10n_de_skr03.account_3753
-DEL account.account.template: l10n_de_skr03.account_3754
-DEL account.account.template: l10n_de_skr03.account_3755
-DEL account.account.template: l10n_de_skr03.account_3760
-DEL account.account.template: l10n_de_skr03.account_3769
-DEL account.account.template: l10n_de_skr03.account_3770
-DEL account.account.template: l10n_de_skr03.account_3780
-DEL account.account.template: l10n_de_skr03.account_3783
-DEL account.account.template: l10n_de_skr03.account_3784
-DEL account.account.template: l10n_de_skr03.account_3785
-DEL account.account.template: l10n_de_skr03.account_3788
-DEL account.account.template: l10n_de_skr03.account_3790
-DEL account.account.template: l10n_de_skr03.account_3792
-DEL account.account.template: l10n_de_skr03.account_3793
-DEL account.account.template: l10n_de_skr03.account_3794
-DEL account.account.template: l10n_de_skr03.account_3796
-DEL account.account.template: l10n_de_skr03.account_3798
-DEL account.account.template: l10n_de_skr03.account_3800
-DEL account.account.template: l10n_de_skr03.account_3830
-DEL account.account.template: l10n_de_skr03.account_3850
-DEL account.account.template: l10n_de_skr03.account_3950
-DEL account.account.template: l10n_de_skr03.account_3955
-DEL account.account.template: l10n_de_skr03.account_3960
-DEL account.account.template: l10n_de_skr03.account_3970
-DEL account.account.template: l10n_de_skr03.account_3980
-DEL account.account.template: l10n_de_skr03.account_4100
-DEL account.account.template: l10n_de_skr03.account_4110
-DEL account.account.template: l10n_de_skr03.account_4120
-DEL account.account.template: l10n_de_skr03.account_4124
-DEL account.account.template: l10n_de_skr03.account_4125
-DEL account.account.template: l10n_de_skr03.account_4126
-DEL account.account.template: l10n_de_skr03.account_4127
-DEL account.account.template: l10n_de_skr03.account_4128
-DEL account.account.template: l10n_de_skr03.account_4129
-DEL account.account.template: l10n_de_skr03.account_4130
-DEL account.account.template: l10n_de_skr03.account_4137
-DEL account.account.template: l10n_de_skr03.account_4138
-DEL account.account.template: l10n_de_skr03.account_4139
-DEL account.account.template: l10n_de_skr03.account_4140
-DEL account.account.template: l10n_de_skr03.account_4141
-DEL account.account.template: l10n_de_skr03.account_4144
-DEL account.account.template: l10n_de_skr03.account_4145
-DEL account.account.template: l10n_de_skr03.account_4146
-DEL account.account.template: l10n_de_skr03.account_4147
-DEL account.account.template: l10n_de_skr03.account_4148
-DEL account.account.template: l10n_de_skr03.account_4149
-DEL account.account.template: l10n_de_skr03.account_4150
-DEL account.account.template: l10n_de_skr03.account_4151
-DEL account.account.template: l10n_de_skr03.account_4152
-DEL account.account.template: l10n_de_skr03.account_4153
-DEL account.account.template: l10n_de_skr03.account_4154
-DEL account.account.template: l10n_de_skr03.account_4155
-DEL account.account.template: l10n_de_skr03.account_4156
-DEL account.account.template: l10n_de_skr03.account_4157
-DEL account.account.template: l10n_de_skr03.account_4158
-DEL account.account.template: l10n_de_skr03.account_4159
-DEL account.account.template: l10n_de_skr03.account_4160
-DEL account.account.template: l10n_de_skr03.account_4165
-DEL account.account.template: l10n_de_skr03.account_4166
-DEL account.account.template: l10n_de_skr03.account_4167
-DEL account.account.template: l10n_de_skr03.account_4168
-DEL account.account.template: l10n_de_skr03.account_4169
-DEL account.account.template: l10n_de_skr03.account_4170
-DEL account.account.template: l10n_de_skr03.account_4175
-DEL account.account.template: l10n_de_skr03.account_4180
-DEL account.account.template: l10n_de_skr03.account_4190
-DEL account.account.template: l10n_de_skr03.account_4194
-DEL account.account.template: l10n_de_skr03.account_4195
-DEL account.account.template: l10n_de_skr03.account_4196
-DEL account.account.template: l10n_de_skr03.account_4197
-DEL account.account.template: l10n_de_skr03.account_4198
-DEL account.account.template: l10n_de_skr03.account_4199
-DEL account.account.template: l10n_de_skr03.account_4200
-DEL account.account.template: l10n_de_skr03.account_4210
-DEL account.account.template: l10n_de_skr03.account_4211
-DEL account.account.template: l10n_de_skr03.account_4212
-DEL account.account.template: l10n_de_skr03.account_4215
-DEL account.account.template: l10n_de_skr03.account_4219
-DEL account.account.template: l10n_de_skr03.account_4220
-DEL account.account.template: l10n_de_skr03.account_4222
-DEL account.account.template: l10n_de_skr03.account_4228
-DEL account.account.template: l10n_de_skr03.account_4229
-DEL account.account.template: l10n_de_skr03.account_4230
-DEL account.account.template: l10n_de_skr03.account_4240
-DEL account.account.template: l10n_de_skr03.account_4250
-DEL account.account.template: l10n_de_skr03.account_4260
-DEL account.account.template: l10n_de_skr03.account_4270
-DEL account.account.template: l10n_de_skr03.account_4280
-DEL account.account.template: l10n_de_skr03.account_4288
-DEL account.account.template: l10n_de_skr03.account_4289
-DEL account.account.template: l10n_de_skr03.account_4290
-DEL account.account.template: l10n_de_skr03.account_4300
-DEL account.account.template: l10n_de_skr03.account_4301
-DEL account.account.template: l10n_de_skr03.account_4306
-DEL account.account.template: l10n_de_skr03.account_4320
-DEL account.account.template: l10n_de_skr03.account_4340
-DEL account.account.template: l10n_de_skr03.account_4350
-DEL account.account.template: l10n_de_skr03.account_4355
-DEL account.account.template: l10n_de_skr03.account_4360
-DEL account.account.template: l10n_de_skr03.account_4366
-DEL account.account.template: l10n_de_skr03.account_4370
-DEL account.account.template: l10n_de_skr03.account_4380
-DEL account.account.template: l10n_de_skr03.account_4390
-DEL account.account.template: l10n_de_skr03.account_4396
-DEL account.account.template: l10n_de_skr03.account_4397
-DEL account.account.template: l10n_de_skr03.account_4500
-DEL account.account.template: l10n_de_skr03.account_4510
-DEL account.account.template: l10n_de_skr03.account_4520
-DEL account.account.template: l10n_de_skr03.account_4530
-DEL account.account.template: l10n_de_skr03.account_4540
-DEL account.account.template: l10n_de_skr03.account_4550
-DEL account.account.template: l10n_de_skr03.account_4560
-DEL account.account.template: l10n_de_skr03.account_4570
-DEL account.account.template: l10n_de_skr03.account_4580
-DEL account.account.template: l10n_de_skr03.account_4590
-DEL account.account.template: l10n_de_skr03.account_4595
-DEL account.account.template: l10n_de_skr03.account_4600
-DEL account.account.template: l10n_de_skr03.account_4605
-DEL account.account.template: l10n_de_skr03.account_4630
-DEL account.account.template: l10n_de_skr03.account_4631
-DEL account.account.template: l10n_de_skr03.account_4632
-DEL account.account.template: l10n_de_skr03.account_4633
-DEL account.account.template: l10n_de_skr03.account_4635
-DEL account.account.template: l10n_de_skr03.account_4636
-DEL account.account.template: l10n_de_skr03.account_4637
-DEL account.account.template: l10n_de_skr03.account_4638
-DEL account.account.template: l10n_de_skr03.account_4639
-DEL account.account.template: l10n_de_skr03.account_4640
-DEL account.account.template: l10n_de_skr03.account_4650
-DEL account.account.template: l10n_de_skr03.account_4651
-DEL account.account.template: l10n_de_skr03.account_4652
-DEL account.account.template: l10n_de_skr03.account_4653
-DEL account.account.template: l10n_de_skr03.account_4654
-DEL account.account.template: l10n_de_skr03.account_4655
-DEL account.account.template: l10n_de_skr03.account_4660
-DEL account.account.template: l10n_de_skr03.account_4663
-DEL account.account.template: l10n_de_skr03.account_4664
-DEL account.account.template: l10n_de_skr03.account_4666
-DEL account.account.template: l10n_de_skr03.account_4668
-DEL account.account.template: l10n_de_skr03.account_4670
-DEL account.account.template: l10n_de_skr03.account_4672
-DEL account.account.template: l10n_de_skr03.account_4673
-DEL account.account.template: l10n_de_skr03.account_4674
-DEL account.account.template: l10n_de_skr03.account_4676
-DEL account.account.template: l10n_de_skr03.account_4678
-DEL account.account.template: l10n_de_skr03.account_4679
-DEL account.account.template: l10n_de_skr03.account_4680
-DEL account.account.template: l10n_de_skr03.account_4681
-DEL account.account.template: l10n_de_skr03.account_4700
-DEL account.account.template: l10n_de_skr03.account_4710
-DEL account.account.template: l10n_de_skr03.account_4730
-DEL account.account.template: l10n_de_skr03.account_4750
-DEL account.account.template: l10n_de_skr03.account_4760
-DEL account.account.template: l10n_de_skr03.account_4780
-DEL account.account.template: l10n_de_skr03.account_4790
-DEL account.account.template: l10n_de_skr03.account_4800
-DEL account.account.template: l10n_de_skr03.account_4801
-DEL account.account.template: l10n_de_skr03.account_4805
-DEL account.account.template: l10n_de_skr03.account_4806
-DEL account.account.template: l10n_de_skr03.account_4808
-DEL account.account.template: l10n_de_skr03.account_4809
-DEL account.account.template: l10n_de_skr03.account_4810
-DEL account.account.template: l10n_de_skr03.account_4815
-DEL account.account.template: l10n_de_skr03.account_4820
-DEL account.account.template: l10n_de_skr03.account_4822
-DEL account.account.template: l10n_de_skr03.account_4823
-DEL account.account.template: l10n_de_skr03.account_4824
-DEL account.account.template: l10n_de_skr03.account_4825
-DEL account.account.template: l10n_de_skr03.account_4826
-DEL account.account.template: l10n_de_skr03.account_4827
-DEL account.account.template: l10n_de_skr03.account_4830
-DEL account.account.template: l10n_de_skr03.account_4831
-DEL account.account.template: l10n_de_skr03.account_4832
-DEL account.account.template: l10n_de_skr03.account_4833
-DEL account.account.template: l10n_de_skr03.account_4840
-DEL account.account.template: l10n_de_skr03.account_4841
-DEL account.account.template: l10n_de_skr03.account_4842
-DEL account.account.template: l10n_de_skr03.account_4843
-DEL account.account.template: l10n_de_skr03.account_4850
-DEL account.account.template: l10n_de_skr03.account_4851
-DEL account.account.template: l10n_de_skr03.account_4852
-DEL account.account.template: l10n_de_skr03.account_4853
-DEL account.account.template: l10n_de_skr03.account_4854
-DEL account.account.template: l10n_de_skr03.account_4855
-DEL account.account.template: l10n_de_skr03.account_4860
-DEL account.account.template: l10n_de_skr03.account_4862
-DEL account.account.template: l10n_de_skr03.account_4865
-DEL account.account.template: l10n_de_skr03.account_4866
-DEL account.account.template: l10n_de_skr03.account_4870
-DEL account.account.template: l10n_de_skr03.account_4871
-DEL account.account.template: l10n_de_skr03.account_4872
-DEL account.account.template: l10n_de_skr03.account_4873
-DEL account.account.template: l10n_de_skr03.account_4874
-DEL account.account.template: l10n_de_skr03.account_4875
-DEL account.account.template: l10n_de_skr03.account_4876
-DEL account.account.template: l10n_de_skr03.account_4877
-DEL account.account.template: l10n_de_skr03.account_4878
-DEL account.account.template: l10n_de_skr03.account_4880
-DEL account.account.template: l10n_de_skr03.account_4882
-DEL account.account.template: l10n_de_skr03.account_4886
-DEL account.account.template: l10n_de_skr03.account_4887
-DEL account.account.template: l10n_de_skr03.account_4892
-DEL account.account.template: l10n_de_skr03.account_4893
-DEL account.account.template: l10n_de_skr03.account_4900
-DEL account.account.template: l10n_de_skr03.account_4902
-DEL account.account.template: l10n_de_skr03.account_4905
-DEL account.account.template: l10n_de_skr03.account_4909
-DEL account.account.template: l10n_de_skr03.account_4910
-DEL account.account.template: l10n_de_skr03.account_4920
-DEL account.account.template: l10n_de_skr03.account_4925
-DEL account.account.template: l10n_de_skr03.account_4930
-DEL account.account.template: l10n_de_skr03.account_4940
-DEL account.account.template: l10n_de_skr03.account_4945
-DEL account.account.template: l10n_de_skr03.account_4946
-DEL account.account.template: l10n_de_skr03.account_4948
-DEL account.account.template: l10n_de_skr03.account_4949
-DEL account.account.template: l10n_de_skr03.account_4950
-DEL account.account.template: l10n_de_skr03.account_4955
-DEL account.account.template: l10n_de_skr03.account_4957
-DEL account.account.template: l10n_de_skr03.account_4958
-DEL account.account.template: l10n_de_skr03.account_4959
-DEL account.account.template: l10n_de_skr03.account_4960
-DEL account.account.template: l10n_de_skr03.account_4961
-DEL account.account.template: l10n_de_skr03.account_4963
-DEL account.account.template: l10n_de_skr03.account_4964
-DEL account.account.template: l10n_de_skr03.account_4965
-DEL account.account.template: l10n_de_skr03.account_4969
-DEL account.account.template: l10n_de_skr03.account_4970
-DEL account.account.template: l10n_de_skr03.account_4975
-DEL account.account.template: l10n_de_skr03.account_4976
-DEL account.account.template: l10n_de_skr03.account_4980
-DEL account.account.template: l10n_de_skr03.account_4984
-DEL account.account.template: l10n_de_skr03.account_4985
-DEL account.account.template: l10n_de_skr03.account_4990
-DEL account.account.template: l10n_de_skr03.account_4991
-DEL account.account.template: l10n_de_skr03.account_4992
-DEL account.account.template: l10n_de_skr03.account_4993
-DEL account.account.template: l10n_de_skr03.account_4994
-DEL account.account.template: l10n_de_skr03.account_4995
-DEL account.account.template: l10n_de_skr03.account_4996
-DEL account.account.template: l10n_de_skr03.account_4997
-DEL account.account.template: l10n_de_skr03.account_4998
-DEL account.account.template: l10n_de_skr03.account_4999
-DEL account.account.template: l10n_de_skr03.account_7000
-DEL account.account.template: l10n_de_skr03.account_7050
-DEL account.account.template: l10n_de_skr03.account_7080
-DEL account.account.template: l10n_de_skr03.account_7090
-DEL account.account.template: l10n_de_skr03.account_7095
-DEL account.account.template: l10n_de_skr03.account_7100
-DEL account.account.template: l10n_de_skr03.account_7110
-DEL account.account.template: l10n_de_skr03.account_7140
-DEL account.account.template: l10n_de_skr03.account_7200
-DEL account.account.template: l10n_de_skr03.account_8100
-DEL account.account.template: l10n_de_skr03.account_8105
-DEL account.account.template: l10n_de_skr03.account_8110
-DEL account.account.template: l10n_de_skr03.account_8120
-DEL account.account.template: l10n_de_skr03.account_8125
-DEL account.account.template: l10n_de_skr03.account_8130
-DEL account.account.template: l10n_de_skr03.account_8135
-DEL account.account.template: l10n_de_skr03.account_8140
-DEL account.account.template: l10n_de_skr03.account_8150
-DEL account.account.template: l10n_de_skr03.account_8160
-DEL account.account.template: l10n_de_skr03.account_8165
-DEL account.account.template: l10n_de_skr03.account_8190
-DEL account.account.template: l10n_de_skr03.account_8191
-DEL account.account.template: l10n_de_skr03.account_8193
-DEL account.account.template: l10n_de_skr03.account_8194
-DEL account.account.template: l10n_de_skr03.account_8195
-DEL account.account.template: l10n_de_skr03.account_8196
-DEL account.account.template: l10n_de_skr03.account_8200
-DEL account.account.template: l10n_de_skr03.account_8300
-DEL account.account.template: l10n_de_skr03.account_8310
-DEL account.account.template: l10n_de_skr03.account_8315
-DEL account.account.template: l10n_de_skr03.account_8320
-DEL account.account.template: l10n_de_skr03.account_8331
-DEL account.account.template: l10n_de_skr03.account_8335
-DEL account.account.template: l10n_de_skr03.account_8336
-DEL account.account.template: l10n_de_skr03.account_8337
-DEL account.account.template: l10n_de_skr03.account_8338
-DEL account.account.template: l10n_de_skr03.account_8339
-DEL account.account.template: l10n_de_skr03.account_8400
-DEL account.account.template: l10n_de_skr03.account_8410
-DEL account.account.template: l10n_de_skr03.account_8499
-DEL account.account.template: l10n_de_skr03.account_8500
-DEL account.account.template: l10n_de_skr03.account_8501
-DEL account.account.template: l10n_de_skr03.account_8502
-DEL account.account.template: l10n_de_skr03.account_8503
-DEL account.account.template: l10n_de_skr03.account_8504
-DEL account.account.template: l10n_de_skr03.account_8505
-DEL account.account.template: l10n_de_skr03.account_8510
-DEL account.account.template: l10n_de_skr03.account_8514
-DEL account.account.template: l10n_de_skr03.account_8515
-DEL account.account.template: l10n_de_skr03.account_8516
-DEL account.account.template: l10n_de_skr03.account_8519
-DEL account.account.template: l10n_de_skr03.account_8520
-DEL account.account.template: l10n_de_skr03.account_8540
-DEL account.account.template: l10n_de_skr03.account_8570
-DEL account.account.template: l10n_de_skr03.account_8574
-DEL account.account.template: l10n_de_skr03.account_8575
-DEL account.account.template: l10n_de_skr03.account_8576
-DEL account.account.template: l10n_de_skr03.account_8579
-DEL account.account.template: l10n_de_skr03.account_8589
-DEL account.account.template: l10n_de_skr03.account_8590
-DEL account.account.template: l10n_de_skr03.account_8591
-DEL account.account.template: l10n_de_skr03.account_8595
-DEL account.account.template: l10n_de_skr03.account_8600
-DEL account.account.template: l10n_de_skr03.account_8603
-DEL account.account.template: l10n_de_skr03.account_8604
-DEL account.account.template: l10n_de_skr03.account_8605
-DEL account.account.template: l10n_de_skr03.account_8606
-DEL account.account.template: l10n_de_skr03.account_8607
-DEL account.account.template: l10n_de_skr03.account_8609
-DEL account.account.template: l10n_de_skr03.account_8610
-DEL account.account.template: l10n_de_skr03.account_8611
-DEL account.account.template: l10n_de_skr03.account_8613
-DEL account.account.template: l10n_de_skr03.account_8614
-DEL account.account.template: l10n_de_skr03.account_8625
-DEL account.account.template: l10n_de_skr03.account_8630
-DEL account.account.template: l10n_de_skr03.account_8640
-DEL account.account.template: l10n_de_skr03.account_8650
-DEL account.account.template: l10n_de_skr03.account_8660
-DEL account.account.template: l10n_de_skr03.account_8700
-DEL account.account.template: l10n_de_skr03.account_8701
-DEL account.account.template: l10n_de_skr03.account_8702
-DEL account.account.template: l10n_de_skr03.account_8703
-DEL account.account.template: l10n_de_skr03.account_8704
-DEL account.account.template: l10n_de_skr03.account_8705
-DEL account.account.template: l10n_de_skr03.account_8710
-DEL account.account.template: l10n_de_skr03.account_8720
-DEL account.account.template: l10n_de_skr03.account_8724
-DEL account.account.template: l10n_de_skr03.account_8725
-DEL account.account.template: l10n_de_skr03.account_8726
-DEL account.account.template: l10n_de_skr03.account_8727
-DEL account.account.template: l10n_de_skr03.account_8730
-DEL account.account.template: l10n_de_skr03.account_8731
-DEL account.account.template: l10n_de_skr03.account_8736
-DEL account.account.template: l10n_de_skr03.account_8738
-DEL account.account.template: l10n_de_skr03.account_8741
-DEL account.account.template: l10n_de_skr03.account_8742
-DEL account.account.template: l10n_de_skr03.account_8743
-DEL account.account.template: l10n_de_skr03.account_8745
-DEL account.account.template: l10n_de_skr03.account_8746
-DEL account.account.template: l10n_de_skr03.account_8748
-DEL account.account.template: l10n_de_skr03.account_8750
-DEL account.account.template: l10n_de_skr03.account_8760
-DEL account.account.template: l10n_de_skr03.account_8769
-DEL account.account.template: l10n_de_skr03.account_8770
-DEL account.account.template: l10n_de_skr03.account_8780
-DEL account.account.template: l10n_de_skr03.account_8790
-DEL account.account.template: l10n_de_skr03.account_8800
-DEL account.account.template: l10n_de_skr03.account_8801
-DEL account.account.template: l10n_de_skr03.account_8807
-DEL account.account.template: l10n_de_skr03.account_8808
-DEL account.account.template: l10n_de_skr03.account_8817
-DEL account.account.template: l10n_de_skr03.account_8818
-DEL account.account.template: l10n_de_skr03.account_8819
-DEL account.account.template: l10n_de_skr03.account_8820
-DEL account.account.template: l10n_de_skr03.account_8827
-DEL account.account.template: l10n_de_skr03.account_8828
-DEL account.account.template: l10n_de_skr03.account_8829
-DEL account.account.template: l10n_de_skr03.account_8837
-DEL account.account.template: l10n_de_skr03.account_8838
-DEL account.account.template: l10n_de_skr03.account_8839
-DEL account.account.template: l10n_de_skr03.account_8850
-DEL account.account.template: l10n_de_skr03.account_8851
-DEL account.account.template: l10n_de_skr03.account_8852
-DEL account.account.template: l10n_de_skr03.account_8853
-DEL account.account.template: l10n_de_skr03.account_8900
-DEL account.account.template: l10n_de_skr03.account_8905
-DEL account.account.template: l10n_de_skr03.account_8906
-DEL account.account.template: l10n_de_skr03.account_8910
-DEL account.account.template: l10n_de_skr03.account_8915
-DEL account.account.template: l10n_de_skr03.account_8918
-DEL account.account.template: l10n_de_skr03.account_8919
-DEL account.account.template: l10n_de_skr03.account_8920
-DEL account.account.template: l10n_de_skr03.account_8921
-DEL account.account.template: l10n_de_skr03.account_8922
-DEL account.account.template: l10n_de_skr03.account_8924
-DEL account.account.template: l10n_de_skr03.account_8925
-DEL account.account.template: l10n_de_skr03.account_8929
-DEL account.account.template: l10n_de_skr03.account_8930
-DEL account.account.template: l10n_de_skr03.account_8932
-DEL account.account.template: l10n_de_skr03.account_8935
-DEL account.account.template: l10n_de_skr03.account_8939
-DEL account.account.template: l10n_de_skr03.account_8940
-DEL account.account.template: l10n_de_skr03.account_8945
-DEL account.account.template: l10n_de_skr03.account_8949
-DEL account.account.template: l10n_de_skr03.account_8950
-DEL account.account.template: l10n_de_skr03.account_8955
-DEL account.account.template: l10n_de_skr03.account_8959
-DEL account.account.template: l10n_de_skr03.account_8960
-DEL account.account.template: l10n_de_skr03.account_8970
-DEL account.account.template: l10n_de_skr03.account_8975
-DEL account.account.template: l10n_de_skr03.account_8977
-DEL account.account.template: l10n_de_skr03.account_8980
-DEL account.account.template: l10n_de_skr03.account_8990
-DEL account.account.template: l10n_de_skr03.account_8994
-DEL account.account.template: l10n_de_skr03.account_8995
-DEL account.account.template: l10n_de_skr03.account_9000
-DEL account.account.template: l10n_de_skr03.account_9001
-DEL account.account.template: l10n_de_skr03.account_9008
-DEL account.account.template: l10n_de_skr03.account_9009
-DEL account.account.template: l10n_de_skr03.account_9089
-DEL account.account.template: l10n_de_skr03.account_9090
-DEL account.account.template: l10n_de_skr04.chart_skr04_100
-DEL account.account.template: l10n_de_skr04.chart_skr04_1000
-DEL account.account.template: l10n_de_skr04.chart_skr04_1040
-DEL account.account.template: l10n_de_skr04.chart_skr04_1050
-DEL account.account.template: l10n_de_skr04.chart_skr04_1080
-DEL account.account.template: l10n_de_skr04.chart_skr04_1090
-DEL account.account.template: l10n_de_skr04.chart_skr04_1095
-DEL account.account.template: l10n_de_skr04.chart_skr04_110
-DEL account.account.template: l10n_de_skr04.chart_skr04_1100
-DEL account.account.template: l10n_de_skr04.chart_skr04_1110
-DEL account.account.template: l10n_de_skr04.chart_skr04_1140
-DEL account.account.template: l10n_de_skr04.chart_skr04_1180
-DEL account.account.template: l10n_de_skr04.chart_skr04_1181
-DEL account.account.template: l10n_de_skr04.chart_skr04_1186
-DEL account.account.template: l10n_de_skr04.chart_skr04_1190
-DEL account.account.template: l10n_de_skr04.chart_skr04_120
-DEL account.account.template: l10n_de_skr04.chart_skr04_1200
-DEL account.account.template: l10n_de_skr04.chart_skr04_1205
-DEL account.account.template: l10n_de_skr04.chart_skr04_1206
-DEL account.account.template: l10n_de_skr04.chart_skr04_1210
-DEL account.account.template: l10n_de_skr04.chart_skr04_1215
-DEL account.account.template: l10n_de_skr04.chart_skr04_1216
-DEL account.account.template: l10n_de_skr04.chart_skr04_1217
-DEL account.account.template: l10n_de_skr04.chart_skr04_1218
-DEL account.account.template: l10n_de_skr04.chart_skr04_1219
-DEL account.account.template: l10n_de_skr04.chart_skr04_1220
-DEL account.account.template: l10n_de_skr04.chart_skr04_1221
-DEL account.account.template: l10n_de_skr04.chart_skr04_1225
-DEL account.account.template: l10n_de_skr04.chart_skr04_1230
-DEL account.account.template: l10n_de_skr04.chart_skr04_1231
-DEL account.account.template: l10n_de_skr04.chart_skr04_1232
-DEL account.account.template: l10n_de_skr04.chart_skr04_1235
-DEL account.account.template: l10n_de_skr04.chart_skr04_1240
-DEL account.account.template: l10n_de_skr04.chart_skr04_1241
-DEL account.account.template: l10n_de_skr04.chart_skr04_1245
-DEL account.account.template: l10n_de_skr04.chart_skr04_1246
-DEL account.account.template: l10n_de_skr04.chart_skr04_1247
-DEL account.account.template: l10n_de_skr04.chart_skr04_1248
-DEL account.account.template: l10n_de_skr04.chart_skr04_1249
-DEL account.account.template: l10n_de_skr04.chart_skr04_1250
-DEL account.account.template: l10n_de_skr04.chart_skr04_1251
-DEL account.account.template: l10n_de_skr04.chart_skr04_1255
-DEL account.account.template: l10n_de_skr04.chart_skr04_1260
-DEL account.account.template: l10n_de_skr04.chart_skr04_1261
-DEL account.account.template: l10n_de_skr04.chart_skr04_1265
-DEL account.account.template: l10n_de_skr04.chart_skr04_1266
-DEL account.account.template: l10n_de_skr04.chart_skr04_1267
-DEL account.account.template: l10n_de_skr04.chart_skr04_1268
-DEL account.account.template: l10n_de_skr04.chart_skr04_1269
-DEL account.account.template: l10n_de_skr04.chart_skr04_1270
-DEL account.account.template: l10n_de_skr04.chart_skr04_1271
-DEL account.account.template: l10n_de_skr04.chart_skr04_1275
-DEL account.account.template: l10n_de_skr04.chart_skr04_1276
-DEL account.account.template: l10n_de_skr04.chart_skr04_1277
-DEL account.account.template: l10n_de_skr04.chart_skr04_1280
-DEL account.account.template: l10n_de_skr04.chart_skr04_1281
-DEL account.account.template: l10n_de_skr04.chart_skr04_1285
-DEL account.account.template: l10n_de_skr04.chart_skr04_1286
-DEL account.account.template: l10n_de_skr04.chart_skr04_1287
-DEL account.account.template: l10n_de_skr04.chart_skr04_1288
-DEL account.account.template: l10n_de_skr04.chart_skr04_1289
-DEL account.account.template: l10n_de_skr04.chart_skr04_1290
-DEL account.account.template: l10n_de_skr04.chart_skr04_1291
-DEL account.account.template: l10n_de_skr04.chart_skr04_1295
-DEL account.account.template: l10n_de_skr04.chart_skr04_1296
-DEL account.account.template: l10n_de_skr04.chart_skr04_1297
-DEL account.account.template: l10n_de_skr04.chart_skr04_1298
-DEL account.account.template: l10n_de_skr04.chart_skr04_1299
-DEL account.account.template: l10n_de_skr04.chart_skr04_130
-DEL account.account.template: l10n_de_skr04.chart_skr04_1300
-DEL account.account.template: l10n_de_skr04.chart_skr04_1301
-DEL account.account.template: l10n_de_skr04.chart_skr04_1305
-DEL account.account.template: l10n_de_skr04.chart_skr04_1307
-DEL account.account.template: l10n_de_skr04.chart_skr04_1308
-DEL account.account.template: l10n_de_skr04.chart_skr04_1309
-DEL account.account.template: l10n_de_skr04.chart_skr04_1310
-DEL account.account.template: l10n_de_skr04.chart_skr04_1311
-DEL account.account.template: l10n_de_skr04.chart_skr04_1315
-DEL account.account.template: l10n_de_skr04.chart_skr04_1317
-DEL account.account.template: l10n_de_skr04.chart_skr04_1318
-DEL account.account.template: l10n_de_skr04.chart_skr04_1319
-DEL account.account.template: l10n_de_skr04.chart_skr04_1320
-DEL account.account.template: l10n_de_skr04.chart_skr04_1321
-DEL account.account.template: l10n_de_skr04.chart_skr04_1325
-DEL account.account.template: l10n_de_skr04.chart_skr04_1327
-DEL account.account.template: l10n_de_skr04.chart_skr04_1328
-DEL account.account.template: l10n_de_skr04.chart_skr04_1329
-DEL account.account.template: l10n_de_skr04.chart_skr04_1330
-DEL account.account.template: l10n_de_skr04.chart_skr04_1331
-DEL account.account.template: l10n_de_skr04.chart_skr04_1335
-DEL account.account.template: l10n_de_skr04.chart_skr04_1337
-DEL account.account.template: l10n_de_skr04.chart_skr04_1338
-DEL account.account.template: l10n_de_skr04.chart_skr04_1339
-DEL account.account.template: l10n_de_skr04.chart_skr04_1340
-DEL account.account.template: l10n_de_skr04.chart_skr04_1341
-DEL account.account.template: l10n_de_skr04.chart_skr04_1345
-DEL account.account.template: l10n_de_skr04.chart_skr04_135
-DEL account.account.template: l10n_de_skr04.chart_skr04_1350
-DEL account.account.template: l10n_de_skr04.chart_skr04_1351
-DEL account.account.template: l10n_de_skr04.chart_skr04_1355
-DEL account.account.template: l10n_de_skr04.chart_skr04_1360
-DEL account.account.template: l10n_de_skr04.chart_skr04_1361
-DEL account.account.template: l10n_de_skr04.chart_skr04_1365
-DEL account.account.template: l10n_de_skr04.chart_skr04_1369
-DEL account.account.template: l10n_de_skr04.chart_skr04_1370
-DEL account.account.template: l10n_de_skr04.chart_skr04_1374
-DEL account.account.template: l10n_de_skr04.chart_skr04_1375
-DEL account.account.template: l10n_de_skr04.chart_skr04_1378
-DEL account.account.template: l10n_de_skr04.chart_skr04_1380
-DEL account.account.template: l10n_de_skr04.chart_skr04_1381
-DEL account.account.template: l10n_de_skr04.chart_skr04_1382
-DEL account.account.template: l10n_de_skr04.chart_skr04_1383
-DEL account.account.template: l10n_de_skr04.chart_skr04_1390
-DEL account.account.template: l10n_de_skr04.chart_skr04_1391
-DEL account.account.template: l10n_de_skr04.chart_skr04_1393
-DEL account.account.template: l10n_de_skr04.chart_skr04_1394
-DEL account.account.template: l10n_de_skr04.chart_skr04_1395
-DEL account.account.template: l10n_de_skr04.chart_skr04_1396
-DEL account.account.template: l10n_de_skr04.chart_skr04_1397
-DEL account.account.template: l10n_de_skr04.chart_skr04_1398
-DEL account.account.template: l10n_de_skr04.chart_skr04_1399
-DEL account.account.template: l10n_de_skr04.chart_skr04_140
-DEL account.account.template: l10n_de_skr04.chart_skr04_1400
-DEL account.account.template: l10n_de_skr04.chart_skr04_1401
-DEL account.account.template: l10n_de_skr04.chart_skr04_1402
-DEL account.account.template: l10n_de_skr04.chart_skr04_1404
-DEL account.account.template: l10n_de_skr04.chart_skr04_1406
-DEL account.account.template: l10n_de_skr04.chart_skr04_1407
-DEL account.account.template: l10n_de_skr04.chart_skr04_1408
-DEL account.account.template: l10n_de_skr04.chart_skr04_1410
-DEL account.account.template: l10n_de_skr04.chart_skr04_1411
-DEL account.account.template: l10n_de_skr04.chart_skr04_1412
-DEL account.account.template: l10n_de_skr04.chart_skr04_1413
-DEL account.account.template: l10n_de_skr04.chart_skr04_1416
-DEL account.account.template: l10n_de_skr04.chart_skr04_1417
-DEL account.account.template: l10n_de_skr04.chart_skr04_1419
-DEL account.account.template: l10n_de_skr04.chart_skr04_1420
-DEL account.account.template: l10n_de_skr04.chart_skr04_1421
-DEL account.account.template: l10n_de_skr04.chart_skr04_1422
-DEL account.account.template: l10n_de_skr04.chart_skr04_1425
-DEL account.account.template: l10n_de_skr04.chart_skr04_1427
-DEL account.account.template: l10n_de_skr04.chart_skr04_143
-DEL account.account.template: l10n_de_skr04.chart_skr04_1431
-DEL account.account.template: l10n_de_skr04.chart_skr04_1432
-DEL account.account.template: l10n_de_skr04.chart_skr04_1433
-DEL account.account.template: l10n_de_skr04.chart_skr04_1434
-DEL account.account.template: l10n_de_skr04.chart_skr04_1435
-DEL account.account.template: l10n_de_skr04.chart_skr04_1436
-DEL account.account.template: l10n_de_skr04.chart_skr04_144
-DEL account.account.template: l10n_de_skr04.chart_skr04_1440
-DEL account.account.template: l10n_de_skr04.chart_skr04_145
-DEL account.account.template: l10n_de_skr04.chart_skr04_1450
-DEL account.account.template: l10n_de_skr04.chart_skr04_1456
-DEL account.account.template: l10n_de_skr04.chart_skr04_1457
-DEL account.account.template: l10n_de_skr04.chart_skr04_146
-DEL account.account.template: l10n_de_skr04.chart_skr04_147
-DEL account.account.template: l10n_de_skr04.chart_skr04_148
-DEL account.account.template: l10n_de_skr04.chart_skr04_1480
-DEL account.account.template: l10n_de_skr04.chart_skr04_1481
-DEL account.account.template: l10n_de_skr04.chart_skr04_1482
-DEL account.account.template: l10n_de_skr04.chart_skr04_1483
-DEL account.account.template: l10n_de_skr04.chart_skr04_1485
-DEL account.account.template: l10n_de_skr04.chart_skr04_1486
-DEL account.account.template: l10n_de_skr04.chart_skr04_1490
-DEL account.account.template: l10n_de_skr04.chart_skr04_1495
-DEL account.account.template: l10n_de_skr04.chart_skr04_1498
-DEL account.account.template: l10n_de_skr04.chart_skr04_150
-DEL account.account.template: l10n_de_skr04.chart_skr04_1500
-DEL account.account.template: l10n_de_skr04.chart_skr04_1504
-DEL account.account.template: l10n_de_skr04.chart_skr04_1510
-DEL account.account.template: l10n_de_skr04.chart_skr04_1520
-DEL account.account.template: l10n_de_skr04.chart_skr04_1525
-DEL account.account.template: l10n_de_skr04.chart_skr04_1530
-DEL account.account.template: l10n_de_skr04.chart_skr04_1550
-DEL account.account.template: l10n_de_skr04.chart_skr04_1610
-DEL account.account.template: l10n_de_skr04.chart_skr04_1620
-DEL account.account.template: l10n_de_skr04.chart_skr04_170
-DEL account.account.template: l10n_de_skr04.chart_skr04_1700
-DEL account.account.template: l10n_de_skr04.chart_skr04_1710
-DEL account.account.template: l10n_de_skr04.chart_skr04_1720
-DEL account.account.template: l10n_de_skr04.chart_skr04_1730
-DEL account.account.template: l10n_de_skr04.chart_skr04_1780
-DEL account.account.template: l10n_de_skr04.chart_skr04_179
-DEL account.account.template: l10n_de_skr04.chart_skr04_1790
-DEL account.account.template: l10n_de_skr04.chart_skr04_1810
-DEL account.account.template: l10n_de_skr04.chart_skr04_1820
-DEL account.account.template: l10n_de_skr04.chart_skr04_1830
-DEL account.account.template: l10n_de_skr04.chart_skr04_1840
-DEL account.account.template: l10n_de_skr04.chart_skr04_1850
-DEL account.account.template: l10n_de_skr04.chart_skr04_1890
-DEL account.account.template: l10n_de_skr04.chart_skr04_1900
-DEL account.account.template: l10n_de_skr04.chart_skr04_1920
-DEL account.account.template: l10n_de_skr04.chart_skr04_1930
-DEL account.account.template: l10n_de_skr04.chart_skr04_1940
-DEL account.account.template: l10n_de_skr04.chart_skr04_1950
-DEL account.account.template: l10n_de_skr04.chart_skr04_200
-DEL account.account.template: l10n_de_skr04.chart_skr04_2000
-DEL account.account.template: l10n_de_skr04.chart_skr04_2010
-DEL account.account.template: l10n_de_skr04.chart_skr04_2020
-DEL account.account.template: l10n_de_skr04.chart_skr04_2050
-DEL account.account.template: l10n_de_skr04.chart_skr04_2060
-DEL account.account.template: l10n_de_skr04.chart_skr04_2070
-DEL account.account.template: l10n_de_skr04.chart_skr04_210
-DEL account.account.template: l10n_de_skr04.chart_skr04_2100
-DEL account.account.template: l10n_de_skr04.chart_skr04_2130
-DEL account.account.template: l10n_de_skr04.chart_skr04_215
-DEL account.account.template: l10n_de_skr04.chart_skr04_2150
-DEL account.account.template: l10n_de_skr04.chart_skr04_2180
-DEL account.account.template: l10n_de_skr04.chart_skr04_220
-DEL account.account.template: l10n_de_skr04.chart_skr04_2200
-DEL account.account.template: l10n_de_skr04.chart_skr04_2230
-DEL account.account.template: l10n_de_skr04.chart_skr04_225
-DEL account.account.template: l10n_de_skr04.chart_skr04_2250
-DEL account.account.template: l10n_de_skr04.chart_skr04_2280
-DEL account.account.template: l10n_de_skr04.chart_skr04_230
-DEL account.account.template: l10n_de_skr04.chart_skr04_2300
-DEL account.account.template: l10n_de_skr04.chart_skr04_2349
-DEL account.account.template: l10n_de_skr04.chart_skr04_235
-DEL account.account.template: l10n_de_skr04.chart_skr04_2350
-DEL account.account.template: l10n_de_skr04.chart_skr04_2399
-DEL account.account.template: l10n_de_skr04.chart_skr04_240
-DEL account.account.template: l10n_de_skr04.chart_skr04_250
-DEL account.account.template: l10n_de_skr04.chart_skr04_2500
-DEL account.account.template: l10n_de_skr04.chart_skr04_2530
-DEL account.account.template: l10n_de_skr04.chart_skr04_2550
-DEL account.account.template: l10n_de_skr04.chart_skr04_2580
-DEL account.account.template: l10n_de_skr04.chart_skr04_260
-DEL account.account.template: l10n_de_skr04.chart_skr04_2600
-DEL account.account.template: l10n_de_skr04.chart_skr04_2630
-DEL account.account.template: l10n_de_skr04.chart_skr04_2650
-DEL account.account.template: l10n_de_skr04.chart_skr04_2680
-DEL account.account.template: l10n_de_skr04.chart_skr04_270
-DEL account.account.template: l10n_de_skr04.chart_skr04_2700
-DEL account.account.template: l10n_de_skr04.chart_skr04_2750
-DEL account.account.template: l10n_de_skr04.chart_skr04_280
-DEL account.account.template: l10n_de_skr04.chart_skr04_285
-DEL account.account.template: l10n_de_skr04.chart_skr04_290
-DEL account.account.template: l10n_de_skr04.chart_skr04_2900
-DEL account.account.template: l10n_de_skr04.chart_skr04_2901
-DEL account.account.template: l10n_de_skr04.chart_skr04_2902
-DEL account.account.template: l10n_de_skr04.chart_skr04_2903
-DEL account.account.template: l10n_de_skr04.chart_skr04_2906
-DEL account.account.template: l10n_de_skr04.chart_skr04_2907
-DEL account.account.template: l10n_de_skr04.chart_skr04_2908
-DEL account.account.template: l10n_de_skr04.chart_skr04_2909
-DEL account.account.template: l10n_de_skr04.chart_skr04_2910
-DEL account.account.template: l10n_de_skr04.chart_skr04_2920
-DEL account.account.template: l10n_de_skr04.chart_skr04_2925
-DEL account.account.template: l10n_de_skr04.chart_skr04_2926
-DEL account.account.template: l10n_de_skr04.chart_skr04_2927
-DEL account.account.template: l10n_de_skr04.chart_skr04_2928
-DEL account.account.template: l10n_de_skr04.chart_skr04_2929
-DEL account.account.template: l10n_de_skr04.chart_skr04_2930
-DEL account.account.template: l10n_de_skr04.chart_skr04_2935
-DEL account.account.template: l10n_de_skr04.chart_skr04_2937
-DEL account.account.template: l10n_de_skr04.chart_skr04_2950
-DEL account.account.template: l10n_de_skr04.chart_skr04_2959
-DEL account.account.template: l10n_de_skr04.chart_skr04_2960
-DEL account.account.template: l10n_de_skr04.chart_skr04_2961
-DEL account.account.template: l10n_de_skr04.chart_skr04_2962
-DEL account.account.template: l10n_de_skr04.chart_skr04_2963
-DEL account.account.template: l10n_de_skr04.chart_skr04_2964
-DEL account.account.template: l10n_de_skr04.chart_skr04_2965
-DEL account.account.template: l10n_de_skr04.chart_skr04_2966
-DEL account.account.template: l10n_de_skr04.chart_skr04_2967
-DEL account.account.template: l10n_de_skr04.chart_skr04_2968
-DEL account.account.template: l10n_de_skr04.chart_skr04_2969
-DEL account.account.template: l10n_de_skr04.chart_skr04_2970
-DEL account.account.template: l10n_de_skr04.chart_skr04_2975
-DEL account.account.template: l10n_de_skr04.chart_skr04_2977
-DEL account.account.template: l10n_de_skr04.chart_skr04_2978
-DEL account.account.template: l10n_de_skr04.chart_skr04_2979
-DEL account.account.template: l10n_de_skr04.chart_skr04_300
-DEL account.account.template: l10n_de_skr04.chart_skr04_3000
-DEL account.account.template: l10n_de_skr04.chart_skr04_3005
-DEL account.account.template: l10n_de_skr04.chart_skr04_3009
-DEL account.account.template: l10n_de_skr04.chart_skr04_3010
-DEL account.account.template: l10n_de_skr04.chart_skr04_3011
-DEL account.account.template: l10n_de_skr04.chart_skr04_3015
-DEL account.account.template: l10n_de_skr04.chart_skr04_3020
-DEL account.account.template: l10n_de_skr04.chart_skr04_3030
-DEL account.account.template: l10n_de_skr04.chart_skr04_3035
-DEL account.account.template: l10n_de_skr04.chart_skr04_3040
-DEL account.account.template: l10n_de_skr04.chart_skr04_305
-DEL account.account.template: l10n_de_skr04.chart_skr04_3050
-DEL account.account.template: l10n_de_skr04.chart_skr04_3060
-DEL account.account.template: l10n_de_skr04.chart_skr04_3065
-DEL account.account.template: l10n_de_skr04.chart_skr04_3070
-DEL account.account.template: l10n_de_skr04.chart_skr04_3075
-DEL account.account.template: l10n_de_skr04.chart_skr04_3076
-DEL account.account.template: l10n_de_skr04.chart_skr04_3077
-DEL account.account.template: l10n_de_skr04.chart_skr04_3079
-DEL account.account.template: l10n_de_skr04.chart_skr04_3085
-DEL account.account.template: l10n_de_skr04.chart_skr04_3090
-DEL account.account.template: l10n_de_skr04.chart_skr04_3092
-DEL account.account.template: l10n_de_skr04.chart_skr04_3095
-DEL account.account.template: l10n_de_skr04.chart_skr04_3098
-DEL account.account.template: l10n_de_skr04.chart_skr04_3099
-DEL account.account.template: l10n_de_skr04.chart_skr04_310
-DEL account.account.template: l10n_de_skr04.chart_skr04_3100
-DEL account.account.template: l10n_de_skr04.chart_skr04_3101
-DEL account.account.template: l10n_de_skr04.chart_skr04_3105
-DEL account.account.template: l10n_de_skr04.chart_skr04_3110
-DEL account.account.template: l10n_de_skr04.chart_skr04_3120
-DEL account.account.template: l10n_de_skr04.chart_skr04_3121
-DEL account.account.template: l10n_de_skr04.chart_skr04_3125
-DEL account.account.template: l10n_de_skr04.chart_skr04_3130
-DEL account.account.template: l10n_de_skr04.chart_skr04_315
-DEL account.account.template: l10n_de_skr04.chart_skr04_3150
-DEL account.account.template: l10n_de_skr04.chart_skr04_3151
-DEL account.account.template: l10n_de_skr04.chart_skr04_3160
-DEL account.account.template: l10n_de_skr04.chart_skr04_3170
-DEL account.account.template: l10n_de_skr04.chart_skr04_3180
-DEL account.account.template: l10n_de_skr04.chart_skr04_3181
-DEL account.account.template: l10n_de_skr04.chart_skr04_3190
-DEL account.account.template: l10n_de_skr04.chart_skr04_320
-DEL account.account.template: l10n_de_skr04.chart_skr04_3200
-DEL account.account.template: l10n_de_skr04.chart_skr04_3250
-DEL account.account.template: l10n_de_skr04.chart_skr04_3260
-DEL account.account.template: l10n_de_skr04.chart_skr04_3272
-DEL account.account.template: l10n_de_skr04.chart_skr04_3280
-DEL account.account.template: l10n_de_skr04.chart_skr04_3284
-DEL account.account.template: l10n_de_skr04.chart_skr04_3285
-DEL account.account.template: l10n_de_skr04.chart_skr04_329
-DEL account.account.template: l10n_de_skr04.chart_skr04_330
-DEL account.account.template: l10n_de_skr04.chart_skr04_3300
-DEL account.account.template: l10n_de_skr04.chart_skr04_3301
-DEL account.account.template: l10n_de_skr04.chart_skr04_3305
-DEL account.account.template: l10n_de_skr04.chart_skr04_3306
-DEL account.account.template: l10n_de_skr04.chart_skr04_3307
-DEL account.account.template: l10n_de_skr04.chart_skr04_3309
-DEL account.account.template: l10n_de_skr04.chart_skr04_3310
-DEL account.account.template: l10n_de_skr04.chart_skr04_3334
-DEL account.account.template: l10n_de_skr04.chart_skr04_3335
-DEL account.account.template: l10n_de_skr04.chart_skr04_3337
-DEL account.account.template: l10n_de_skr04.chart_skr04_3338
-DEL account.account.template: l10n_de_skr04.chart_skr04_3340
-DEL account.account.template: l10n_de_skr04.chart_skr04_3341
-DEL account.account.template: l10n_de_skr04.chart_skr04_3345
-DEL account.account.template: l10n_de_skr04.chart_skr04_3348
-DEL account.account.template: l10n_de_skr04.chart_skr04_3350
-DEL account.account.template: l10n_de_skr04.chart_skr04_3351
-DEL account.account.template: l10n_de_skr04.chart_skr04_3380
-DEL account.account.template: l10n_de_skr04.chart_skr04_3390
-DEL account.account.template: l10n_de_skr04.chart_skr04_340
-DEL account.account.template: l10n_de_skr04.chart_skr04_3400
-DEL account.account.template: l10n_de_skr04.chart_skr04_3401
-DEL account.account.template: l10n_de_skr04.chart_skr04_3405
-DEL account.account.template: l10n_de_skr04.chart_skr04_3410
-DEL account.account.template: l10n_de_skr04.chart_skr04_3420
-DEL account.account.template: l10n_de_skr04.chart_skr04_3421
-DEL account.account.template: l10n_de_skr04.chart_skr04_3425
-DEL account.account.template: l10n_de_skr04.chart_skr04_3430
-DEL account.account.template: l10n_de_skr04.chart_skr04_3450
-DEL account.account.template: l10n_de_skr04.chart_skr04_3451
-DEL account.account.template: l10n_de_skr04.chart_skr04_3455
-DEL account.account.template: l10n_de_skr04.chart_skr04_3460
-DEL account.account.template: l10n_de_skr04.chart_skr04_3470
-DEL account.account.template: l10n_de_skr04.chart_skr04_3471
-DEL account.account.template: l10n_de_skr04.chart_skr04_3475
-DEL account.account.template: l10n_de_skr04.chart_skr04_3480
-DEL account.account.template: l10n_de_skr04.chart_skr04_350
-DEL account.account.template: l10n_de_skr04.chart_skr04_3500
-DEL account.account.template: l10n_de_skr04.chart_skr04_3501
-DEL account.account.template: l10n_de_skr04.chart_skr04_3504
-DEL account.account.template: l10n_de_skr04.chart_skr04_3507
-DEL account.account.template: l10n_de_skr04.chart_skr04_3509
-DEL account.account.template: l10n_de_skr04.chart_skr04_3510
-DEL account.account.template: l10n_de_skr04.chart_skr04_3511
-DEL account.account.template: l10n_de_skr04.chart_skr04_3514
-DEL account.account.template: l10n_de_skr04.chart_skr04_3517
-DEL account.account.template: l10n_de_skr04.chart_skr04_3519
-DEL account.account.template: l10n_de_skr04.chart_skr04_3520
-DEL account.account.template: l10n_de_skr04.chart_skr04_3521
-DEL account.account.template: l10n_de_skr04.chart_skr04_3524
-DEL account.account.template: l10n_de_skr04.chart_skr04_3527
-DEL account.account.template: l10n_de_skr04.chart_skr04_3530
-DEL account.account.template: l10n_de_skr04.chart_skr04_3531
-DEL account.account.template: l10n_de_skr04.chart_skr04_3534
-DEL account.account.template: l10n_de_skr04.chart_skr04_3537
-DEL account.account.template: l10n_de_skr04.chart_skr04_3540
-DEL account.account.template: l10n_de_skr04.chart_skr04_3541
-DEL account.account.template: l10n_de_skr04.chart_skr04_3544
-DEL account.account.template: l10n_de_skr04.chart_skr04_3547
-DEL account.account.template: l10n_de_skr04.chart_skr04_3550
-DEL account.account.template: l10n_de_skr04.chart_skr04_3551
-DEL account.account.template: l10n_de_skr04.chart_skr04_3554
-DEL account.account.template: l10n_de_skr04.chart_skr04_3557
-DEL account.account.template: l10n_de_skr04.chart_skr04_3560
-DEL account.account.template: l10n_de_skr04.chart_skr04_3561
-DEL account.account.template: l10n_de_skr04.chart_skr04_3564
-DEL account.account.template: l10n_de_skr04.chart_skr04_3567
-DEL account.account.template: l10n_de_skr04.chart_skr04_360
-DEL account.account.template: l10n_de_skr04.chart_skr04_3600
-DEL account.account.template: l10n_de_skr04.chart_skr04_3610
-DEL account.account.template: l10n_de_skr04.chart_skr04_3611
-DEL account.account.template: l10n_de_skr04.chart_skr04_3620
-DEL account.account.template: l10n_de_skr04.chart_skr04_3630
-DEL account.account.template: l10n_de_skr04.chart_skr04_3635
-DEL account.account.template: l10n_de_skr04.chart_skr04_3640
-DEL account.account.template: l10n_de_skr04.chart_skr04_3641
-DEL account.account.template: l10n_de_skr04.chart_skr04_3642
-DEL account.account.template: l10n_de_skr04.chart_skr04_3643
-DEL account.account.template: l10n_de_skr04.chart_skr04_3645
-DEL account.account.template: l10n_de_skr04.chart_skr04_3646
-DEL account.account.template: l10n_de_skr04.chart_skr04_3647
-DEL account.account.template: l10n_de_skr04.chart_skr04_3648
-DEL account.account.template: l10n_de_skr04.chart_skr04_3650
-DEL account.account.template: l10n_de_skr04.chart_skr04_3651
-DEL account.account.template: l10n_de_skr04.chart_skr04_3652
-DEL account.account.template: l10n_de_skr04.chart_skr04_3653
-DEL account.account.template: l10n_de_skr04.chart_skr04_3655
-DEL account.account.template: l10n_de_skr04.chart_skr04_3656
-DEL account.account.template: l10n_de_skr04.chart_skr04_3657
-DEL account.account.template: l10n_de_skr04.chart_skr04_3658
-DEL account.account.template: l10n_de_skr04.chart_skr04_3695
-DEL account.account.template: l10n_de_skr04.chart_skr04_370
-DEL account.account.template: l10n_de_skr04.chart_skr04_3700
-DEL account.account.template: l10n_de_skr04.chart_skr04_3701
-DEL account.account.template: l10n_de_skr04.chart_skr04_3710
-DEL account.account.template: l10n_de_skr04.chart_skr04_3715
-DEL account.account.template: l10n_de_skr04.chart_skr04_3720
-DEL account.account.template: l10n_de_skr04.chart_skr04_3725
-DEL account.account.template: l10n_de_skr04.chart_skr04_3726
-DEL account.account.template: l10n_de_skr04.chart_skr04_3730
-DEL account.account.template: l10n_de_skr04.chart_skr04_3740
-DEL account.account.template: l10n_de_skr04.chart_skr04_3741
-DEL account.account.template: l10n_de_skr04.chart_skr04_3750
-DEL account.account.template: l10n_de_skr04.chart_skr04_3755
-DEL account.account.template: l10n_de_skr04.chart_skr04_3759
-DEL account.account.template: l10n_de_skr04.chart_skr04_3760
-DEL account.account.template: l10n_de_skr04.chart_skr04_3761
-DEL account.account.template: l10n_de_skr04.chart_skr04_3770
-DEL account.account.template: l10n_de_skr04.chart_skr04_3771
-DEL account.account.template: l10n_de_skr04.chart_skr04_3780
-DEL account.account.template: l10n_de_skr04.chart_skr04_3785
-DEL account.account.template: l10n_de_skr04.chart_skr04_3786
-DEL account.account.template: l10n_de_skr04.chart_skr04_3790
-DEL account.account.template: l10n_de_skr04.chart_skr04_3796
-DEL account.account.template: l10n_de_skr04.chart_skr04_3798
-DEL account.account.template: l10n_de_skr04.chart_skr04_3799
-DEL account.account.template: l10n_de_skr04.chart_skr04_380
-DEL account.account.template: l10n_de_skr04.chart_skr04_3800
-DEL account.account.template: l10n_de_skr04.chart_skr04_3801
-DEL account.account.template: l10n_de_skr04.chart_skr04_3802
-DEL account.account.template: l10n_de_skr04.chart_skr04_3804
-DEL account.account.template: l10n_de_skr04.chart_skr04_3806
-DEL account.account.template: l10n_de_skr04.chart_skr04_3807
-DEL account.account.template: l10n_de_skr04.chart_skr04_3808
-DEL account.account.template: l10n_de_skr04.chart_skr04_3809
-DEL account.account.template: l10n_de_skr04.chart_skr04_3810
-DEL account.account.template: l10n_de_skr04.chart_skr04_3811
-DEL account.account.template: l10n_de_skr04.chart_skr04_3812
-DEL account.account.template: l10n_de_skr04.chart_skr04_3814
-DEL account.account.template: l10n_de_skr04.chart_skr04_3816
-DEL account.account.template: l10n_de_skr04.chart_skr04_3817
-DEL account.account.template: l10n_de_skr04.chart_skr04_3818
-DEL account.account.template: l10n_de_skr04.chart_skr04_3819
-DEL account.account.template: l10n_de_skr04.chart_skr04_3820
-DEL account.account.template: l10n_de_skr04.chart_skr04_3830
-DEL account.account.template: l10n_de_skr04.chart_skr04_3832
-DEL account.account.template: l10n_de_skr04.chart_skr04_3834
-DEL account.account.template: l10n_de_skr04.chart_skr04_3835
-DEL account.account.template: l10n_de_skr04.chart_skr04_3837
-DEL account.account.template: l10n_de_skr04.chart_skr04_3840
-DEL account.account.template: l10n_de_skr04.chart_skr04_3841
-DEL account.account.template: l10n_de_skr04.chart_skr04_3845
-DEL account.account.template: l10n_de_skr04.chart_skr04_3850
-DEL account.account.template: l10n_de_skr04.chart_skr04_3851
-DEL account.account.template: l10n_de_skr04.chart_skr04_3854
-DEL account.account.template: l10n_de_skr04.chart_skr04_3860
-DEL account.account.template: l10n_de_skr04.chart_skr04_3865
-DEL account.account.template: l10n_de_skr04.chart_skr04_390
-DEL account.account.template: l10n_de_skr04.chart_skr04_3900
-DEL account.account.template: l10n_de_skr04.chart_skr04_395
-DEL account.account.template: l10n_de_skr04.chart_skr04_3950
-DEL account.account.template: l10n_de_skr04.chart_skr04_398
-DEL account.account.template: l10n_de_skr04.chart_skr04_400
-DEL account.account.template: l10n_de_skr04.chart_skr04_4000
-DEL account.account.template: l10n_de_skr04.chart_skr04_4100
-DEL account.account.template: l10n_de_skr04.chart_skr04_4110
-DEL account.account.template: l10n_de_skr04.chart_skr04_4120
-DEL account.account.template: l10n_de_skr04.chart_skr04_4125
-DEL account.account.template: l10n_de_skr04.chart_skr04_4130
-DEL account.account.template: l10n_de_skr04.chart_skr04_4135
-DEL account.account.template: l10n_de_skr04.chart_skr04_4136
-DEL account.account.template: l10n_de_skr04.chart_skr04_4138
-DEL account.account.template: l10n_de_skr04.chart_skr04_4139
-DEL account.account.template: l10n_de_skr04.chart_skr04_4140
-DEL account.account.template: l10n_de_skr04.chart_skr04_4150
-DEL account.account.template: l10n_de_skr04.chart_skr04_4160
-DEL account.account.template: l10n_de_skr04.chart_skr04_4165
-DEL account.account.template: l10n_de_skr04.chart_skr04_4180
-DEL account.account.template: l10n_de_skr04.chart_skr04_4185
-DEL account.account.template: l10n_de_skr04.chart_skr04_4186
-DEL account.account.template: l10n_de_skr04.chart_skr04_420
-DEL account.account.template: l10n_de_skr04.chart_skr04_4200
-DEL account.account.template: l10n_de_skr04.chart_skr04_4300
-DEL account.account.template: l10n_de_skr04.chart_skr04_4310
-DEL account.account.template: l10n_de_skr04.chart_skr04_4315
-DEL account.account.template: l10n_de_skr04.chart_skr04_4320
-DEL account.account.template: l10n_de_skr04.chart_skr04_4331
-DEL account.account.template: l10n_de_skr04.chart_skr04_4335
-DEL account.account.template: l10n_de_skr04.chart_skr04_4336
-DEL account.account.template: l10n_de_skr04.chart_skr04_4337
-DEL account.account.template: l10n_de_skr04.chart_skr04_4338
-DEL account.account.template: l10n_de_skr04.chart_skr04_4339
-DEL account.account.template: l10n_de_skr04.chart_skr04_440
-DEL account.account.template: l10n_de_skr04.chart_skr04_4400
-DEL account.account.template: l10n_de_skr04.chart_skr04_4499
-DEL account.account.template: l10n_de_skr04.chart_skr04_450
-DEL account.account.template: l10n_de_skr04.chart_skr04_4510
-DEL account.account.template: l10n_de_skr04.chart_skr04_4520
-DEL account.account.template: l10n_de_skr04.chart_skr04_4560
-DEL account.account.template: l10n_de_skr04.chart_skr04_4564
-DEL account.account.template: l10n_de_skr04.chart_skr04_4566
-DEL account.account.template: l10n_de_skr04.chart_skr04_4569
-DEL account.account.template: l10n_de_skr04.chart_skr04_4570
-DEL account.account.template: l10n_de_skr04.chart_skr04_4574
-DEL account.account.template: l10n_de_skr04.chart_skr04_4575
-DEL account.account.template: l10n_de_skr04.chart_skr04_4576
-DEL account.account.template: l10n_de_skr04.chart_skr04_4579
-DEL account.account.template: l10n_de_skr04.chart_skr04_460
-DEL account.account.template: l10n_de_skr04.chart_skr04_4600
-DEL account.account.template: l10n_de_skr04.chart_skr04_4605
-DEL account.account.template: l10n_de_skr04.chart_skr04_4610
-DEL account.account.template: l10n_de_skr04.chart_skr04_4616
-DEL account.account.template: l10n_de_skr04.chart_skr04_4619
-DEL account.account.template: l10n_de_skr04.chart_skr04_4620
-DEL account.account.template: l10n_de_skr04.chart_skr04_4630
-DEL account.account.template: l10n_de_skr04.chart_skr04_4639
-DEL account.account.template: l10n_de_skr04.chart_skr04_4640
-DEL account.account.template: l10n_de_skr04.chart_skr04_4645
-DEL account.account.template: l10n_de_skr04.chart_skr04_4646
-DEL account.account.template: l10n_de_skr04.chart_skr04_4650
-DEL account.account.template: l10n_de_skr04.chart_skr04_4659
-DEL account.account.template: l10n_de_skr04.chart_skr04_4660
-DEL account.account.template: l10n_de_skr04.chart_skr04_4670
-DEL account.account.template: l10n_de_skr04.chart_skr04_4679
-DEL account.account.template: l10n_de_skr04.chart_skr04_4680
-DEL account.account.template: l10n_de_skr04.chart_skr04_4686
-DEL account.account.template: l10n_de_skr04.chart_skr04_4689
-DEL account.account.template: l10n_de_skr04.chart_skr04_4690
-DEL account.account.template: l10n_de_skr04.chart_skr04_4695
-DEL account.account.template: l10n_de_skr04.chart_skr04_4699
-DEL account.account.template: l10n_de_skr04.chart_skr04_470
-DEL account.account.template: l10n_de_skr04.chart_skr04_4700
-DEL account.account.template: l10n_de_skr04.chart_skr04_4701
-DEL account.account.template: l10n_de_skr04.chart_skr04_4702
-DEL account.account.template: l10n_de_skr04.chart_skr04_4703
-DEL account.account.template: l10n_de_skr04.chart_skr04_4704
-DEL account.account.template: l10n_de_skr04.chart_skr04_4705
-DEL account.account.template: l10n_de_skr04.chart_skr04_4710
-DEL account.account.template: l10n_de_skr04.chart_skr04_4720
-DEL account.account.template: l10n_de_skr04.chart_skr04_4724
-DEL account.account.template: l10n_de_skr04.chart_skr04_4725
-DEL account.account.template: l10n_de_skr04.chart_skr04_4726
-DEL account.account.template: l10n_de_skr04.chart_skr04_4727
-DEL account.account.template: l10n_de_skr04.chart_skr04_4730
-DEL account.account.template: l10n_de_skr04.chart_skr04_4731
-DEL account.account.template: l10n_de_skr04.chart_skr04_4736
-DEL account.account.template: l10n_de_skr04.chart_skr04_4738
-DEL account.account.template: l10n_de_skr04.chart_skr04_4741
-DEL account.account.template: l10n_de_skr04.chart_skr04_4742
-DEL account.account.template: l10n_de_skr04.chart_skr04_4743
-DEL account.account.template: l10n_de_skr04.chart_skr04_4745
-DEL account.account.template: l10n_de_skr04.chart_skr04_4746
-DEL account.account.template: l10n_de_skr04.chart_skr04_4748
-DEL account.account.template: l10n_de_skr04.chart_skr04_4750
-DEL account.account.template: l10n_de_skr04.chart_skr04_4760
-DEL account.account.template: l10n_de_skr04.chart_skr04_4770
-DEL account.account.template: l10n_de_skr04.chart_skr04_4780
-DEL account.account.template: l10n_de_skr04.chart_skr04_4790
-DEL account.account.template: l10n_de_skr04.chart_skr04_4800
-DEL account.account.template: l10n_de_skr04.chart_skr04_4810
-DEL account.account.template: l10n_de_skr04.chart_skr04_4815
-DEL account.account.template: l10n_de_skr04.chart_skr04_4816
-DEL account.account.template: l10n_de_skr04.chart_skr04_4818
-DEL account.account.template: l10n_de_skr04.chart_skr04_4820
-DEL account.account.template: l10n_de_skr04.chart_skr04_4824
-DEL account.account.template: l10n_de_skr04.chart_skr04_4825
-DEL account.account.template: l10n_de_skr04.chart_skr04_4830
-DEL account.account.template: l10n_de_skr04.chart_skr04_4832
-DEL account.account.template: l10n_de_skr04.chart_skr04_4833
-DEL account.account.template: l10n_de_skr04.chart_skr04_4835
-DEL account.account.template: l10n_de_skr04.chart_skr04_4836
-DEL account.account.template: l10n_de_skr04.chart_skr04_4837
-DEL account.account.template: l10n_de_skr04.chart_skr04_4838
-DEL account.account.template: l10n_de_skr04.chart_skr04_4839
-DEL account.account.template: l10n_de_skr04.chart_skr04_4840
-DEL account.account.template: l10n_de_skr04.chart_skr04_4841
-DEL account.account.template: l10n_de_skr04.chart_skr04_4842
-DEL account.account.template: l10n_de_skr04.chart_skr04_4843
-DEL account.account.template: l10n_de_skr04.chart_skr04_4844
-DEL account.account.template: l10n_de_skr04.chart_skr04_4845
-DEL account.account.template: l10n_de_skr04.chart_skr04_4847
-DEL account.account.template: l10n_de_skr04.chart_skr04_4848
-DEL account.account.template: l10n_de_skr04.chart_skr04_4849
-DEL account.account.template: l10n_de_skr04.chart_skr04_4850
-DEL account.account.template: l10n_de_skr04.chart_skr04_4851
-DEL account.account.template: l10n_de_skr04.chart_skr04_4852
-DEL account.account.template: l10n_de_skr04.chart_skr04_4855
-DEL account.account.template: l10n_de_skr04.chart_skr04_4856
-DEL account.account.template: l10n_de_skr04.chart_skr04_4857
-DEL account.account.template: l10n_de_skr04.chart_skr04_4858
-DEL account.account.template: l10n_de_skr04.chart_skr04_4860
-DEL account.account.template: l10n_de_skr04.chart_skr04_4861
-DEL account.account.template: l10n_de_skr04.chart_skr04_4862
-DEL account.account.template: l10n_de_skr04.chart_skr04_4900
-DEL account.account.template: l10n_de_skr04.chart_skr04_4901
-DEL account.account.template: l10n_de_skr04.chart_skr04_4905
-DEL account.account.template: l10n_de_skr04.chart_skr04_4906
-DEL account.account.template: l10n_de_skr04.chart_skr04_4910
-DEL account.account.template: l10n_de_skr04.chart_skr04_4911
-DEL account.account.template: l10n_de_skr04.chart_skr04_4912
-DEL account.account.template: l10n_de_skr04.chart_skr04_4913
-DEL account.account.template: l10n_de_skr04.chart_skr04_4914
-DEL account.account.template: l10n_de_skr04.chart_skr04_4915
-DEL account.account.template: l10n_de_skr04.chart_skr04_4916
-DEL account.account.template: l10n_de_skr04.chart_skr04_4920
-DEL account.account.template: l10n_de_skr04.chart_skr04_4923
-DEL account.account.template: l10n_de_skr04.chart_skr04_4925
-DEL account.account.template: l10n_de_skr04.chart_skr04_4927
-DEL account.account.template: l10n_de_skr04.chart_skr04_4928
-DEL account.account.template: l10n_de_skr04.chart_skr04_4929
-DEL account.account.template: l10n_de_skr04.chart_skr04_4930
-DEL account.account.template: l10n_de_skr04.chart_skr04_4932
-DEL account.account.template: l10n_de_skr04.chart_skr04_4934
-DEL account.account.template: l10n_de_skr04.chart_skr04_4935
-DEL account.account.template: l10n_de_skr04.chart_skr04_4936
-DEL account.account.template: l10n_de_skr04.chart_skr04_4937
-DEL account.account.template: l10n_de_skr04.chart_skr04_4938
-DEL account.account.template: l10n_de_skr04.chart_skr04_4939
-DEL account.account.template: l10n_de_skr04.chart_skr04_4940
-DEL account.account.template: l10n_de_skr04.chart_skr04_4941
-DEL account.account.template: l10n_de_skr04.chart_skr04_4945
-DEL account.account.template: l10n_de_skr04.chart_skr04_4947
-DEL account.account.template: l10n_de_skr04.chart_skr04_4948
-DEL account.account.template: l10n_de_skr04.chart_skr04_4949
-DEL account.account.template: l10n_de_skr04.chart_skr04_4960
-DEL account.account.template: l10n_de_skr04.chart_skr04_4970
-DEL account.account.template: l10n_de_skr04.chart_skr04_4972
-DEL account.account.template: l10n_de_skr04.chart_skr04_4975
-DEL account.account.template: l10n_de_skr04.chart_skr04_4980
-DEL account.account.template: l10n_de_skr04.chart_skr04_4981
-DEL account.account.template: l10n_de_skr04.chart_skr04_4982
-DEL account.account.template: l10n_de_skr04.chart_skr04_4987
-DEL account.account.template: l10n_de_skr04.chart_skr04_4989
-DEL account.account.template: l10n_de_skr04.chart_skr04_4992
-DEL account.account.template: l10n_de_skr04.chart_skr04_50
-DEL account.account.template: l10n_de_skr04.chart_skr04_500
-DEL account.account.template: l10n_de_skr04.chart_skr04_5000
-DEL account.account.template: l10n_de_skr04.chart_skr04_510
-DEL account.account.template: l10n_de_skr04.chart_skr04_5100
-DEL account.account.template: l10n_de_skr04.chart_skr04_5110
-DEL account.account.template: l10n_de_skr04.chart_skr04_5130
-DEL account.account.template: l10n_de_skr04.chart_skr04_5160
-DEL account.account.template: l10n_de_skr04.chart_skr04_5162
-DEL account.account.template: l10n_de_skr04.chart_skr04_5166
-DEL account.account.template: l10n_de_skr04.chart_skr04_5167
-DEL account.account.template: l10n_de_skr04.chart_skr04_5189
-DEL account.account.template: l10n_de_skr04.chart_skr04_5190
-DEL account.account.template: l10n_de_skr04.chart_skr04_5191
-DEL account.account.template: l10n_de_skr04.chart_skr04_5192
-DEL account.account.template: l10n_de_skr04.chart_skr04_520
-DEL account.account.template: l10n_de_skr04.chart_skr04_5200
-DEL account.account.template: l10n_de_skr04.chart_skr04_5300
-DEL account.account.template: l10n_de_skr04.chart_skr04_5349
-DEL account.account.template: l10n_de_skr04.chart_skr04_540
-DEL account.account.template: l10n_de_skr04.chart_skr04_5400
-DEL account.account.template: l10n_de_skr04.chart_skr04_5420
-DEL account.account.template: l10n_de_skr04.chart_skr04_5425
-DEL account.account.template: l10n_de_skr04.chart_skr04_5430
-DEL account.account.template: l10n_de_skr04.chart_skr04_5435
-DEL account.account.template: l10n_de_skr04.chart_skr04_5440
-DEL account.account.template: l10n_de_skr04.chart_skr04_5550
-DEL account.account.template: l10n_de_skr04.chart_skr04_5551
-DEL account.account.template: l10n_de_skr04.chart_skr04_5552
-DEL account.account.template: l10n_de_skr04.chart_skr04_5553
-DEL account.account.template: l10n_de_skr04.chart_skr04_5557
-DEL account.account.template: l10n_de_skr04.chart_skr04_5559
-DEL account.account.template: l10n_de_skr04.chart_skr04_560
-DEL account.account.template: l10n_de_skr04.chart_skr04_5600
-DEL account.account.template: l10n_de_skr04.chart_skr04_5610
-DEL account.account.template: l10n_de_skr04.chart_skr04_5660
-DEL account.account.template: l10n_de_skr04.chart_skr04_5700
-DEL account.account.template: l10n_de_skr04.chart_skr04_5701
-DEL account.account.template: l10n_de_skr04.chart_skr04_5710
-DEL account.account.template: l10n_de_skr04.chart_skr04_5714
-DEL account.account.template: l10n_de_skr04.chart_skr04_5715
-DEL account.account.template: l10n_de_skr04.chart_skr04_5717
-DEL account.account.template: l10n_de_skr04.chart_skr04_5718
-DEL account.account.template: l10n_de_skr04.chart_skr04_5720
-DEL account.account.template: l10n_de_skr04.chart_skr04_5724
-DEL account.account.template: l10n_de_skr04.chart_skr04_5725
-DEL account.account.template: l10n_de_skr04.chart_skr04_5730
-DEL account.account.template: l10n_de_skr04.chart_skr04_5731
-DEL account.account.template: l10n_de_skr04.chart_skr04_5733
-DEL account.account.template: l10n_de_skr04.chart_skr04_5734
-DEL account.account.template: l10n_de_skr04.chart_skr04_5736
-DEL account.account.template: l10n_de_skr04.chart_skr04_5738
-DEL account.account.template: l10n_de_skr04.chart_skr04_5741
-DEL account.account.template: l10n_de_skr04.chart_skr04_5743
-DEL account.account.template: l10n_de_skr04.chart_skr04_5744
-DEL account.account.template: l10n_de_skr04.chart_skr04_5750
-DEL account.account.template: l10n_de_skr04.chart_skr04_5753
-DEL account.account.template: l10n_de_skr04.chart_skr04_5754
-DEL account.account.template: l10n_de_skr04.chart_skr04_5755
-DEL account.account.template: l10n_de_skr04.chart_skr04_5760
-DEL account.account.template: l10n_de_skr04.chart_skr04_5770
-DEL account.account.template: l10n_de_skr04.chart_skr04_5780
-DEL account.account.template: l10n_de_skr04.chart_skr04_5783
-DEL account.account.template: l10n_de_skr04.chart_skr04_5784
-DEL account.account.template: l10n_de_skr04.chart_skr04_5785
-DEL account.account.template: l10n_de_skr04.chart_skr04_5788
-DEL account.account.template: l10n_de_skr04.chart_skr04_5790
-DEL account.account.template: l10n_de_skr04.chart_skr04_5792
-DEL account.account.template: l10n_de_skr04.chart_skr04_5793
-DEL account.account.template: l10n_de_skr04.chart_skr04_5794
-DEL account.account.template: l10n_de_skr04.chart_skr04_5796
-DEL account.account.template: l10n_de_skr04.chart_skr04_5798
-DEL account.account.template: l10n_de_skr04.chart_skr04_5800
-DEL account.account.template: l10n_de_skr04.chart_skr04_5820
-DEL account.account.template: l10n_de_skr04.chart_skr04_5840
-DEL account.account.template: l10n_de_skr04.chart_skr04_5880
-DEL account.account.template: l10n_de_skr04.chart_skr04_5881
-DEL account.account.template: l10n_de_skr04.chart_skr04_5885
-DEL account.account.template: l10n_de_skr04.chart_skr04_5900
-DEL account.account.template: l10n_de_skr04.chart_skr04_5906
-DEL account.account.template: l10n_de_skr04.chart_skr04_5908
-DEL account.account.template: l10n_de_skr04.chart_skr04_5909
-DEL account.account.template: l10n_de_skr04.chart_skr04_5910
-DEL account.account.template: l10n_de_skr04.chart_skr04_5913
-DEL account.account.template: l10n_de_skr04.chart_skr04_5915
-DEL account.account.template: l10n_de_skr04.chart_skr04_5920
-DEL account.account.template: l10n_de_skr04.chart_skr04_5923
-DEL account.account.template: l10n_de_skr04.chart_skr04_5925
-DEL account.account.template: l10n_de_skr04.chart_skr04_5950
-DEL account.account.template: l10n_de_skr04.chart_skr04_5951
-DEL account.account.template: l10n_de_skr04.chart_skr04_5970
-DEL account.account.template: l10n_de_skr04.chart_skr04_5975
-DEL account.account.template: l10n_de_skr04.chart_skr04_5980
-DEL account.account.template: l10n_de_skr04.chart_skr04_5985
-DEL account.account.template: l10n_de_skr04.chart_skr04_60
-DEL account.account.template: l10n_de_skr04.chart_skr04_6000
-DEL account.account.template: l10n_de_skr04.chart_skr04_6010
-DEL account.account.template: l10n_de_skr04.chart_skr04_6020
-DEL account.account.template: l10n_de_skr04.chart_skr04_6024
-DEL account.account.template: l10n_de_skr04.chart_skr04_6026
-DEL account.account.template: l10n_de_skr04.chart_skr04_6027
-DEL account.account.template: l10n_de_skr04.chart_skr04_6028
-DEL account.account.template: l10n_de_skr04.chart_skr04_6029
-DEL account.account.template: l10n_de_skr04.chart_skr04_6030
-DEL account.account.template: l10n_de_skr04.chart_skr04_6035
-DEL account.account.template: l10n_de_skr04.chart_skr04_6036
-DEL account.account.template: l10n_de_skr04.chart_skr04_6037
-DEL account.account.template: l10n_de_skr04.chart_skr04_6038
-DEL account.account.template: l10n_de_skr04.chart_skr04_6039
-DEL account.account.template: l10n_de_skr04.chart_skr04_6040
-DEL account.account.template: l10n_de_skr04.chart_skr04_6045
-DEL account.account.template: l10n_de_skr04.chart_skr04_6050
-DEL account.account.template: l10n_de_skr04.chart_skr04_6060
-DEL account.account.template: l10n_de_skr04.chart_skr04_6066
-DEL account.account.template: l10n_de_skr04.chart_skr04_6067
-DEL account.account.template: l10n_de_skr04.chart_skr04_6068
-DEL account.account.template: l10n_de_skr04.chart_skr04_6069
-DEL account.account.template: l10n_de_skr04.chart_skr04_6070
-DEL account.account.template: l10n_de_skr04.chart_skr04_6071
-DEL account.account.template: l10n_de_skr04.chart_skr04_6072
-DEL account.account.template: l10n_de_skr04.chart_skr04_6073
-DEL account.account.template: l10n_de_skr04.chart_skr04_6074
-DEL account.account.template: l10n_de_skr04.chart_skr04_6075
-DEL account.account.template: l10n_de_skr04.chart_skr04_6076
-DEL account.account.template: l10n_de_skr04.chart_skr04_6077
-DEL account.account.template: l10n_de_skr04.chart_skr04_6078
-DEL account.account.template: l10n_de_skr04.chart_skr04_6079
-DEL account.account.template: l10n_de_skr04.chart_skr04_6080
-DEL account.account.template: l10n_de_skr04.chart_skr04_6090
-DEL account.account.template: l10n_de_skr04.chart_skr04_6100
-DEL account.account.template: l10n_de_skr04.chart_skr04_6110
-DEL account.account.template: l10n_de_skr04.chart_skr04_6118
-DEL account.account.template: l10n_de_skr04.chart_skr04_6120
-DEL account.account.template: l10n_de_skr04.chart_skr04_6130
-DEL account.account.template: l10n_de_skr04.chart_skr04_6140
-DEL account.account.template: l10n_de_skr04.chart_skr04_6147
-DEL account.account.template: l10n_de_skr04.chart_skr04_6148
-DEL account.account.template: l10n_de_skr04.chart_skr04_6149
-DEL account.account.template: l10n_de_skr04.chart_skr04_6150
-DEL account.account.template: l10n_de_skr04.chart_skr04_6160
-DEL account.account.template: l10n_de_skr04.chart_skr04_6170
-DEL account.account.template: l10n_de_skr04.chart_skr04_6171
-DEL account.account.template: l10n_de_skr04.chart_skr04_620
-DEL account.account.template: l10n_de_skr04.chart_skr04_6200
-DEL account.account.template: l10n_de_skr04.chart_skr04_6201
-DEL account.account.template: l10n_de_skr04.chart_skr04_6205
-DEL account.account.template: l10n_de_skr04.chart_skr04_6209
-DEL account.account.template: l10n_de_skr04.chart_skr04_6210
-DEL account.account.template: l10n_de_skr04.chart_skr04_6211
-DEL account.account.template: l10n_de_skr04.chart_skr04_6220
-DEL account.account.template: l10n_de_skr04.chart_skr04_6221
-DEL account.account.template: l10n_de_skr04.chart_skr04_6222
-DEL account.account.template: l10n_de_skr04.chart_skr04_6223
-DEL account.account.template: l10n_de_skr04.chart_skr04_6230
-DEL account.account.template: l10n_de_skr04.chart_skr04_6231
-DEL account.account.template: l10n_de_skr04.chart_skr04_6232
-DEL account.account.template: l10n_de_skr04.chart_skr04_6233
-DEL account.account.template: l10n_de_skr04.chart_skr04_6240
-DEL account.account.template: l10n_de_skr04.chart_skr04_6241
-DEL account.account.template: l10n_de_skr04.chart_skr04_6242
-DEL account.account.template: l10n_de_skr04.chart_skr04_6243
-DEL account.account.template: l10n_de_skr04.chart_skr04_6244
-DEL account.account.template: l10n_de_skr04.chart_skr04_6250
-DEL account.account.template: l10n_de_skr04.chart_skr04_6260
-DEL account.account.template: l10n_de_skr04.chart_skr04_6262
-DEL account.account.template: l10n_de_skr04.chart_skr04_6264
-DEL account.account.template: l10n_de_skr04.chart_skr04_6266
-DEL account.account.template: l10n_de_skr04.chart_skr04_6268
-DEL account.account.template: l10n_de_skr04.chart_skr04_6270
-DEL account.account.template: l10n_de_skr04.chart_skr04_6272
-DEL account.account.template: l10n_de_skr04.chart_skr04_6278
-DEL account.account.template: l10n_de_skr04.chart_skr04_6279
-DEL account.account.template: l10n_de_skr04.chart_skr04_6280
-DEL account.account.template: l10n_de_skr04.chart_skr04_6281
-DEL account.account.template: l10n_de_skr04.chart_skr04_6286
-DEL account.account.template: l10n_de_skr04.chart_skr04_6290
-DEL account.account.template: l10n_de_skr04.chart_skr04_6291
-DEL account.account.template: l10n_de_skr04.chart_skr04_630
-DEL account.account.template: l10n_de_skr04.chart_skr04_6300
-DEL account.account.template: l10n_de_skr04.chart_skr04_6302
-DEL account.account.template: l10n_de_skr04.chart_skr04_6303
-DEL account.account.template: l10n_de_skr04.chart_skr04_6304
-DEL account.account.template: l10n_de_skr04.chart_skr04_6305
-DEL account.account.template: l10n_de_skr04.chart_skr04_6310
-DEL account.account.template: l10n_de_skr04.chart_skr04_6312
-DEL account.account.template: l10n_de_skr04.chart_skr04_6313
-DEL account.account.template: l10n_de_skr04.chart_skr04_6314
-DEL account.account.template: l10n_de_skr04.chart_skr04_6315
-DEL account.account.template: l10n_de_skr04.chart_skr04_6316
-DEL account.account.template: l10n_de_skr04.chart_skr04_6317
-DEL account.account.template: l10n_de_skr04.chart_skr04_6319
-DEL account.account.template: l10n_de_skr04.chart_skr04_6320
-DEL account.account.template: l10n_de_skr04.chart_skr04_6325
-DEL account.account.template: l10n_de_skr04.chart_skr04_6330
-DEL account.account.template: l10n_de_skr04.chart_skr04_6335
-DEL account.account.template: l10n_de_skr04.chart_skr04_6340
-DEL account.account.template: l10n_de_skr04.chart_skr04_6345
-DEL account.account.template: l10n_de_skr04.chart_skr04_6348
-DEL account.account.template: l10n_de_skr04.chart_skr04_6349
-DEL account.account.template: l10n_de_skr04.chart_skr04_635
-DEL account.account.template: l10n_de_skr04.chart_skr04_6350
-DEL account.account.template: l10n_de_skr04.chart_skr04_6390
-DEL account.account.template: l10n_de_skr04.chart_skr04_6391
-DEL account.account.template: l10n_de_skr04.chart_skr04_6392
-DEL account.account.template: l10n_de_skr04.chart_skr04_6393
-DEL account.account.template: l10n_de_skr04.chart_skr04_6394
-DEL account.account.template: l10n_de_skr04.chart_skr04_6395
-DEL account.account.template: l10n_de_skr04.chart_skr04_6396
-DEL account.account.template: l10n_de_skr04.chart_skr04_6397
-DEL account.account.template: l10n_de_skr04.chart_skr04_6398
-DEL account.account.template: l10n_de_skr04.chart_skr04_640
-DEL account.account.template: l10n_de_skr04.chart_skr04_6400
-DEL account.account.template: l10n_de_skr04.chart_skr04_6405
-DEL account.account.template: l10n_de_skr04.chart_skr04_6410
-DEL account.account.template: l10n_de_skr04.chart_skr04_6420
-DEL account.account.template: l10n_de_skr04.chart_skr04_6430
-DEL account.account.template: l10n_de_skr04.chart_skr04_6436
-DEL account.account.template: l10n_de_skr04.chart_skr04_6437
-DEL account.account.template: l10n_de_skr04.chart_skr04_6440
-DEL account.account.template: l10n_de_skr04.chart_skr04_6450
-DEL account.account.template: l10n_de_skr04.chart_skr04_6460
-DEL account.account.template: l10n_de_skr04.chart_skr04_6470
-DEL account.account.template: l10n_de_skr04.chart_skr04_6475
-DEL account.account.template: l10n_de_skr04.chart_skr04_6485
-DEL account.account.template: l10n_de_skr04.chart_skr04_6490
-DEL account.account.template: l10n_de_skr04.chart_skr04_6495
-DEL account.account.template: l10n_de_skr04.chart_skr04_6498
-DEL account.account.template: l10n_de_skr04.chart_skr04_650
-DEL account.account.template: l10n_de_skr04.chart_skr04_6500
-DEL account.account.template: l10n_de_skr04.chart_skr04_6520
-DEL account.account.template: l10n_de_skr04.chart_skr04_6530
-DEL account.account.template: l10n_de_skr04.chart_skr04_6540
-DEL account.account.template: l10n_de_skr04.chart_skr04_6550
-DEL account.account.template: l10n_de_skr04.chart_skr04_6560
-DEL account.account.template: l10n_de_skr04.chart_skr04_6570
-DEL account.account.template: l10n_de_skr04.chart_skr04_6580
-DEL account.account.template: l10n_de_skr04.chart_skr04_6590
-DEL account.account.template: l10n_de_skr04.chart_skr04_6595
-DEL account.account.template: l10n_de_skr04.chart_skr04_660
-DEL account.account.template: l10n_de_skr04.chart_skr04_6600
-DEL account.account.template: l10n_de_skr04.chart_skr04_6605
-DEL account.account.template: l10n_de_skr04.chart_skr04_6610
-DEL account.account.template: l10n_de_skr04.chart_skr04_6611
-DEL account.account.template: l10n_de_skr04.chart_skr04_6612
-DEL account.account.template: l10n_de_skr04.chart_skr04_6620
-DEL account.account.template: l10n_de_skr04.chart_skr04_6621
-DEL account.account.template: l10n_de_skr04.chart_skr04_6625
-DEL account.account.template: l10n_de_skr04.chart_skr04_6629
-DEL account.account.template: l10n_de_skr04.chart_skr04_6630
-DEL account.account.template: l10n_de_skr04.chart_skr04_6640
-DEL account.account.template: l10n_de_skr04.chart_skr04_6641
-DEL account.account.template: l10n_de_skr04.chart_skr04_6642
-DEL account.account.template: l10n_de_skr04.chart_skr04_6643
-DEL account.account.template: l10n_de_skr04.chart_skr04_6644
-DEL account.account.template: l10n_de_skr04.chart_skr04_6645
-DEL account.account.template: l10n_de_skr04.chart_skr04_6650
-DEL account.account.template: l10n_de_skr04.chart_skr04_6660
-DEL account.account.template: l10n_de_skr04.chart_skr04_6663
-DEL account.account.template: l10n_de_skr04.chart_skr04_6664
-DEL account.account.template: l10n_de_skr04.chart_skr04_6668
-DEL account.account.template: l10n_de_skr04.chart_skr04_6670
-DEL account.account.template: l10n_de_skr04.chart_skr04_6673
-DEL account.account.template: l10n_de_skr04.chart_skr04_6674
-DEL account.account.template: l10n_de_skr04.chart_skr04_6680
-DEL account.account.template: l10n_de_skr04.chart_skr04_6688
-DEL account.account.template: l10n_de_skr04.chart_skr04_6689
-DEL account.account.template: l10n_de_skr04.chart_skr04_6690
-DEL account.account.template: l10n_de_skr04.chart_skr04_6691
-DEL account.account.template: l10n_de_skr04.chart_skr04_670
-DEL account.account.template: l10n_de_skr04.chart_skr04_6700
-DEL account.account.template: l10n_de_skr04.chart_skr04_6710
-DEL account.account.template: l10n_de_skr04.chart_skr04_6740
-DEL account.account.template: l10n_de_skr04.chart_skr04_675
-DEL account.account.template: l10n_de_skr04.chart_skr04_6760
-DEL account.account.template: l10n_de_skr04.chart_skr04_6770
-DEL account.account.template: l10n_de_skr04.chart_skr04_6780
-DEL account.account.template: l10n_de_skr04.chart_skr04_6790
-DEL account.account.template: l10n_de_skr04.chart_skr04_680
-DEL account.account.template: l10n_de_skr04.chart_skr04_6800
-DEL account.account.template: l10n_de_skr04.chart_skr04_6805
-DEL account.account.template: l10n_de_skr04.chart_skr04_6810
-DEL account.account.template: l10n_de_skr04.chart_skr04_6815
-DEL account.account.template: l10n_de_skr04.chart_skr04_6820
-DEL account.account.template: l10n_de_skr04.chart_skr04_6821
-DEL account.account.template: l10n_de_skr04.chart_skr04_6822
-DEL account.account.template: l10n_de_skr04.chart_skr04_6823
-DEL account.account.template: l10n_de_skr04.chart_skr04_6824
-DEL account.account.template: l10n_de_skr04.chart_skr04_6825
-DEL account.account.template: l10n_de_skr04.chart_skr04_6827
-DEL account.account.template: l10n_de_skr04.chart_skr04_6830
-DEL account.account.template: l10n_de_skr04.chart_skr04_6833
-DEL account.account.template: l10n_de_skr04.chart_skr04_6834
-DEL account.account.template: l10n_de_skr04.chart_skr04_6835
-DEL account.account.template: l10n_de_skr04.chart_skr04_6837
-DEL account.account.template: l10n_de_skr04.chart_skr04_6838
-DEL account.account.template: l10n_de_skr04.chart_skr04_6840
-DEL account.account.template: l10n_de_skr04.chart_skr04_6845
-DEL account.account.template: l10n_de_skr04.chart_skr04_6850
-DEL account.account.template: l10n_de_skr04.chart_skr04_6854
-DEL account.account.template: l10n_de_skr04.chart_skr04_6855
-DEL account.account.template: l10n_de_skr04.chart_skr04_6856
-DEL account.account.template: l10n_de_skr04.chart_skr04_6857
-DEL account.account.template: l10n_de_skr04.chart_skr04_6859
-DEL account.account.template: l10n_de_skr04.chart_skr04_6860
-DEL account.account.template: l10n_de_skr04.chart_skr04_6865
-DEL account.account.template: l10n_de_skr04.chart_skr04_6871
-DEL account.account.template: l10n_de_skr04.chart_skr04_6875
-DEL account.account.template: l10n_de_skr04.chart_skr04_6876
-DEL account.account.template: l10n_de_skr04.chart_skr04_6880
-DEL account.account.template: l10n_de_skr04.chart_skr04_6881
-DEL account.account.template: l10n_de_skr04.chart_skr04_6883
-DEL account.account.template: l10n_de_skr04.chart_skr04_6884
-DEL account.account.template: l10n_de_skr04.chart_skr04_6885
-DEL account.account.template: l10n_de_skr04.chart_skr04_6888
-DEL account.account.template: l10n_de_skr04.chart_skr04_6889
-DEL account.account.template: l10n_de_skr04.chart_skr04_6890
-DEL account.account.template: l10n_de_skr04.chart_skr04_6891
-DEL account.account.template: l10n_de_skr04.chart_skr04_6892
-DEL account.account.template: l10n_de_skr04.chart_skr04_6895
-DEL account.account.template: l10n_de_skr04.chart_skr04_6896
-DEL account.account.template: l10n_de_skr04.chart_skr04_6897
-DEL account.account.template: l10n_de_skr04.chart_skr04_6898
-DEL account.account.template: l10n_de_skr04.chart_skr04_690
-DEL account.account.template: l10n_de_skr04.chart_skr04_6900
-DEL account.account.template: l10n_de_skr04.chart_skr04_6903
-DEL account.account.template: l10n_de_skr04.chart_skr04_6905
-DEL account.account.template: l10n_de_skr04.chart_skr04_6906
-DEL account.account.template: l10n_de_skr04.chart_skr04_6910
-DEL account.account.template: l10n_de_skr04.chart_skr04_6912
-DEL account.account.template: l10n_de_skr04.chart_skr04_6918
-DEL account.account.template: l10n_de_skr04.chart_skr04_6920
-DEL account.account.template: l10n_de_skr04.chart_skr04_6922
-DEL account.account.template: l10n_de_skr04.chart_skr04_6923
-DEL account.account.template: l10n_de_skr04.chart_skr04_6924
-DEL account.account.template: l10n_de_skr04.chart_skr04_6927
-DEL account.account.template: l10n_de_skr04.chart_skr04_6928
-DEL account.account.template: l10n_de_skr04.chart_skr04_6929
-DEL account.account.template: l10n_de_skr04.chart_skr04_6930
-DEL account.account.template: l10n_de_skr04.chart_skr04_6931
-DEL account.account.template: l10n_de_skr04.chart_skr04_6932
-DEL account.account.template: l10n_de_skr04.chart_skr04_6933
-DEL account.account.template: l10n_de_skr04.chart_skr04_6936
-DEL account.account.template: l10n_de_skr04.chart_skr04_6938
-DEL account.account.template: l10n_de_skr04.chart_skr04_6960
-DEL account.account.template: l10n_de_skr04.chart_skr04_6967
-DEL account.account.template: l10n_de_skr04.chart_skr04_6968
-DEL account.account.template: l10n_de_skr04.chart_skr04_6969
-DEL account.account.template: l10n_de_skr04.chart_skr04_70
-DEL account.account.template: l10n_de_skr04.chart_skr04_700
-DEL account.account.template: l10n_de_skr04.chart_skr04_7000
-DEL account.account.template: l10n_de_skr04.chart_skr04_7004
-DEL account.account.template: l10n_de_skr04.chart_skr04_7005
-DEL account.account.template: l10n_de_skr04.chart_skr04_7006
-DEL account.account.template: l10n_de_skr04.chart_skr04_7008
-DEL account.account.template: l10n_de_skr04.chart_skr04_7009
-DEL account.account.template: l10n_de_skr04.chart_skr04_7010
-DEL account.account.template: l10n_de_skr04.chart_skr04_7011
-DEL account.account.template: l10n_de_skr04.chart_skr04_7012
-DEL account.account.template: l10n_de_skr04.chart_skr04_7013
-DEL account.account.template: l10n_de_skr04.chart_skr04_7014
-DEL account.account.template: l10n_de_skr04.chart_skr04_7015
-DEL account.account.template: l10n_de_skr04.chart_skr04_7016
-DEL account.account.template: l10n_de_skr04.chart_skr04_7017
-DEL account.account.template: l10n_de_skr04.chart_skr04_7018
-DEL account.account.template: l10n_de_skr04.chart_skr04_7019
-DEL account.account.template: l10n_de_skr04.chart_skr04_7020
-DEL account.account.template: l10n_de_skr04.chart_skr04_7030
-DEL account.account.template: l10n_de_skr04.chart_skr04_705
-DEL account.account.template: l10n_de_skr04.chart_skr04_710
-DEL account.account.template: l10n_de_skr04.chart_skr04_7100
-DEL account.account.template: l10n_de_skr04.chart_skr04_7103
-DEL account.account.template: l10n_de_skr04.chart_skr04_7104
-DEL account.account.template: l10n_de_skr04.chart_skr04_7105
-DEL account.account.template: l10n_de_skr04.chart_skr04_7106
-DEL account.account.template: l10n_de_skr04.chart_skr04_7107
-DEL account.account.template: l10n_de_skr04.chart_skr04_7109
-DEL account.account.template: l10n_de_skr04.chart_skr04_7110
-DEL account.account.template: l10n_de_skr04.chart_skr04_7119
-DEL account.account.template: l10n_de_skr04.chart_skr04_7120
-DEL account.account.template: l10n_de_skr04.chart_skr04_7129
-DEL account.account.template: l10n_de_skr04.chart_skr04_7130
-DEL account.account.template: l10n_de_skr04.chart_skr04_7139
-DEL account.account.template: l10n_de_skr04.chart_skr04_7140
-DEL account.account.template: l10n_de_skr04.chart_skr04_7141
-DEL account.account.template: l10n_de_skr04.chart_skr04_7142
-DEL account.account.template: l10n_de_skr04.chart_skr04_7143
-DEL account.account.template: l10n_de_skr04.chart_skr04_7144
-DEL account.account.template: l10n_de_skr04.chart_skr04_7145
-DEL account.account.template: l10n_de_skr04.chart_skr04_7190
-DEL account.account.template: l10n_de_skr04.chart_skr04_7192
-DEL account.account.template: l10n_de_skr04.chart_skr04_7194
-DEL account.account.template: l10n_de_skr04.chart_skr04_720
-DEL account.account.template: l10n_de_skr04.chart_skr04_7200
-DEL account.account.template: l10n_de_skr04.chart_skr04_7201
-DEL account.account.template: l10n_de_skr04.chart_skr04_7204
-DEL account.account.template: l10n_de_skr04.chart_skr04_7207
-DEL account.account.template: l10n_de_skr04.chart_skr04_7208
-DEL account.account.template: l10n_de_skr04.chart_skr04_7210
-DEL account.account.template: l10n_de_skr04.chart_skr04_7214
-DEL account.account.template: l10n_de_skr04.chart_skr04_7217
-DEL account.account.template: l10n_de_skr04.chart_skr04_725
-DEL account.account.template: l10n_de_skr04.chart_skr04_7250
-DEL account.account.template: l10n_de_skr04.chart_skr04_7255
-DEL account.account.template: l10n_de_skr04.chart_skr04_7300
-DEL account.account.template: l10n_de_skr04.chart_skr04_7302
-DEL account.account.template: l10n_de_skr04.chart_skr04_7303
-DEL account.account.template: l10n_de_skr04.chart_skr04_7304
-DEL account.account.template: l10n_de_skr04.chart_skr04_7305
-DEL account.account.template: l10n_de_skr04.chart_skr04_7306
-DEL account.account.template: l10n_de_skr04.chart_skr04_7309
-DEL account.account.template: l10n_de_skr04.chart_skr04_7310
-DEL account.account.template: l10n_de_skr04.chart_skr04_7313
-DEL account.account.template: l10n_de_skr04.chart_skr04_7316
-DEL account.account.template: l10n_de_skr04.chart_skr04_7317
-DEL account.account.template: l10n_de_skr04.chart_skr04_7319
-DEL account.account.template: l10n_de_skr04.chart_skr04_7320
-DEL account.account.template: l10n_de_skr04.chart_skr04_7323
-DEL account.account.template: l10n_de_skr04.chart_skr04_7324
-DEL account.account.template: l10n_de_skr04.chart_skr04_7325
-DEL account.account.template: l10n_de_skr04.chart_skr04_7326
-DEL account.account.template: l10n_de_skr04.chart_skr04_7327
-DEL account.account.template: l10n_de_skr04.chart_skr04_7328
-DEL account.account.template: l10n_de_skr04.chart_skr04_7329
-DEL account.account.template: l10n_de_skr04.chart_skr04_7330
-DEL account.account.template: l10n_de_skr04.chart_skr04_7339
-DEL account.account.template: l10n_de_skr04.chart_skr04_7340
-DEL account.account.template: l10n_de_skr04.chart_skr04_7349
-DEL account.account.template: l10n_de_skr04.chart_skr04_735
-DEL account.account.template: l10n_de_skr04.chart_skr04_7350
-DEL account.account.template: l10n_de_skr04.chart_skr04_7351
-DEL account.account.template: l10n_de_skr04.chart_skr04_7355
-DEL account.account.template: l10n_de_skr04.chart_skr04_7360
-DEL account.account.template: l10n_de_skr04.chart_skr04_7361
-DEL account.account.template: l10n_de_skr04.chart_skr04_7362
-DEL account.account.template: l10n_de_skr04.chart_skr04_7363
-DEL account.account.template: l10n_de_skr04.chart_skr04_7364
-DEL account.account.template: l10n_de_skr04.chart_skr04_7365
-DEL account.account.template: l10n_de_skr04.chart_skr04_7366
-DEL account.account.template: l10n_de_skr04.chart_skr04_7390
-DEL account.account.template: l10n_de_skr04.chart_skr04_7392
-DEL account.account.template: l10n_de_skr04.chart_skr04_7394
-DEL account.account.template: l10n_de_skr04.chart_skr04_7399
-DEL account.account.template: l10n_de_skr04.chart_skr04_740
-DEL account.account.template: l10n_de_skr04.chart_skr04_7400
-DEL account.account.template: l10n_de_skr04.chart_skr04_7401
-DEL account.account.template: l10n_de_skr04.chart_skr04_7450
-DEL account.account.template: l10n_de_skr04.chart_skr04_7451
-DEL account.account.template: l10n_de_skr04.chart_skr04_7452
-DEL account.account.template: l10n_de_skr04.chart_skr04_7453
-DEL account.account.template: l10n_de_skr04.chart_skr04_7454
-DEL account.account.template: l10n_de_skr04.chart_skr04_7460
-DEL account.account.template: l10n_de_skr04.chart_skr04_7461
-DEL account.account.template: l10n_de_skr04.chart_skr04_7462
-DEL account.account.template: l10n_de_skr04.chart_skr04_7463
-DEL account.account.template: l10n_de_skr04.chart_skr04_7464
-DEL account.account.template: l10n_de_skr04.chart_skr04_7500
-DEL account.account.template: l10n_de_skr04.chart_skr04_7501
-DEL account.account.template: l10n_de_skr04.chart_skr04_755
-DEL account.account.template: l10n_de_skr04.chart_skr04_7550
-DEL account.account.template: l10n_de_skr04.chart_skr04_7551
-DEL account.account.template: l10n_de_skr04.chart_skr04_7552
-DEL account.account.template: l10n_de_skr04.chart_skr04_7553
-DEL account.account.template: l10n_de_skr04.chart_skr04_7554
-DEL account.account.template: l10n_de_skr04.chart_skr04_7560
-DEL account.account.template: l10n_de_skr04.chart_skr04_7561
-DEL account.account.template: l10n_de_skr04.chart_skr04_7562
-DEL account.account.template: l10n_de_skr04.chart_skr04_7563
-DEL account.account.template: l10n_de_skr04.chart_skr04_7600
-DEL account.account.template: l10n_de_skr04.chart_skr04_7603
-DEL account.account.template: l10n_de_skr04.chart_skr04_7604
-DEL account.account.template: l10n_de_skr04.chart_skr04_7607
-DEL account.account.template: l10n_de_skr04.chart_skr04_7608
-DEL account.account.template: l10n_de_skr04.chart_skr04_7609
-DEL account.account.template: l10n_de_skr04.chart_skr04_7610
-DEL account.account.template: l10n_de_skr04.chart_skr04_7630
-DEL account.account.template: l10n_de_skr04.chart_skr04_7633
-DEL account.account.template: l10n_de_skr04.chart_skr04_7639
-DEL account.account.template: l10n_de_skr04.chart_skr04_7640
-DEL account.account.template: l10n_de_skr04.chart_skr04_7641
-DEL account.account.template: l10n_de_skr04.chart_skr04_7642
-DEL account.account.template: l10n_de_skr04.chart_skr04_7643
-DEL account.account.template: l10n_de_skr04.chart_skr04_7644
-DEL account.account.template: l10n_de_skr04.chart_skr04_7646
-DEL account.account.template: l10n_de_skr04.chart_skr04_7648
-DEL account.account.template: l10n_de_skr04.chart_skr04_7649
-DEL account.account.template: l10n_de_skr04.chart_skr04_765
-DEL account.account.template: l10n_de_skr04.chart_skr04_7650
-DEL account.account.template: l10n_de_skr04.chart_skr04_7675
-DEL account.account.template: l10n_de_skr04.chart_skr04_7678
-DEL account.account.template: l10n_de_skr04.chart_skr04_7680
-DEL account.account.template: l10n_de_skr04.chart_skr04_7685
-DEL account.account.template: l10n_de_skr04.chart_skr04_7690
-DEL account.account.template: l10n_de_skr04.chart_skr04_7692
-DEL account.account.template: l10n_de_skr04.chart_skr04_7694
-DEL account.account.template: l10n_de_skr04.chart_skr04_770
-DEL account.account.template: l10n_de_skr04.chart_skr04_7705
-DEL account.account.template: l10n_de_skr04.chart_skr04_7725
-DEL account.account.template: l10n_de_skr04.chart_skr04_7744
-DEL account.account.template: l10n_de_skr04.chart_skr04_7751
-DEL account.account.template: l10n_de_skr04.chart_skr04_7781
-DEL account.account.template: l10n_de_skr04.chart_skr04_7785
-DEL account.account.template: l10n_de_skr04.chart_skr04_780
-DEL account.account.template: l10n_de_skr04.chart_skr04_785
-DEL account.account.template: l10n_de_skr04.chart_skr04_795
-DEL account.account.template: l10n_de_skr04.chart_skr04_80
-DEL account.account.template: l10n_de_skr04.chart_skr04_800
-DEL account.account.template: l10n_de_skr04.chart_skr04_803
-DEL account.account.template: l10n_de_skr04.chart_skr04_804
-DEL account.account.template: l10n_de_skr04.chart_skr04_805
-DEL account.account.template: l10n_de_skr04.chart_skr04_808
-DEL account.account.template: l10n_de_skr04.chart_skr04_809
-DEL account.account.template: l10n_de_skr04.chart_skr04_810
-DEL account.account.template: l10n_de_skr04.chart_skr04_813
-DEL account.account.template: l10n_de_skr04.chart_skr04_814
-DEL account.account.template: l10n_de_skr04.chart_skr04_815
-DEL account.account.template: l10n_de_skr04.chart_skr04_820
-DEL account.account.template: l10n_de_skr04.chart_skr04_829
-DEL account.account.template: l10n_de_skr04.chart_skr04_830
-DEL account.account.template: l10n_de_skr04.chart_skr04_840
-DEL account.account.template: l10n_de_skr04.chart_skr04_850
-DEL account.account.template: l10n_de_skr04.chart_skr04_860
-DEL account.account.template: l10n_de_skr04.chart_skr04_880
-DEL account.account.template: l10n_de_skr04.chart_skr04_883
-DEL account.account.template: l10n_de_skr04.chart_skr04_885
-DEL account.account.template: l10n_de_skr04.chart_skr04_90
-DEL account.account.template: l10n_de_skr04.chart_skr04_900
-DEL account.account.template: l10n_de_skr04.chart_skr04_9000
-DEL account.account.template: l10n_de_skr04.chart_skr04_9008
-DEL account.account.template: l10n_de_skr04.chart_skr04_9009
-DEL account.account.template: l10n_de_skr04.chart_skr04_9090
-DEL account.account.template: l10n_de_skr04.chart_skr04_910
-DEL account.account.template: l10n_de_skr04.chart_skr04_920
-DEL account.account.template: l10n_de_skr04.chart_skr04_930
-DEL account.account.template: l10n_de_skr04.chart_skr04_940
-DEL account.account.template: l10n_de_skr04.chart_skr04_960
-DEL account.account.template: l10n_de_skr04.chart_skr04_961
-DEL account.account.template: l10n_de_skr04.chart_skr04_962
-DEL account.account.template: l10n_de_skr04.chart_skr04_963
-DEL account.account.template: l10n_de_skr04.chart_skr04_964
-DEL account.account.template: l10n_de_skr04.chart_skr04_970
-DEL account.account.template: l10n_de_skr04.chart_skr04_980
-DEL account.account.template: l10n_de_skr04.chart_skr04_9991
-DEL account.account.template: l10n_de_skr04.chart_skr04_9994
-DEL account.chart.template: l10n_de_skr03.l10n_de_chart_template
-DEL account.chart.template: l10n_de_skr04.l10n_chart_de_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_no_id_partner_19a_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_no_id_partner_19b_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_no_id_partner_7b_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_no_id_partner_afa7a_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_partner_19b_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_partner_afa19a_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_partner_afa7a_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_partner_afa7b_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_purchase_service_19_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_eu_vat_id_purchase_service_7_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_acc_non_eu_purchase_services_19_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_no_id_purchase_19_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_no_id_sale_19_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_vat_id_purchase_19_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_vat_id_purchase_7_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_vat_id_sale_19_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_eu_vat_id_sale_7_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_no_id_purchase_7_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_no_id_sale_7_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_purchase_19_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_purchase_7_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_sale_19_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_sale_7_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr03.account_fiscal_position_account_non_eu_sale_services_19_skr03
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_no_id_partner_19a_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_no_id_partner_19b_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_no_id_partner_7b_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_no_id_partner_afa7a_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_partner_19b_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_partner_afa19a_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_partner_afa7a_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_partner_afa7b_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_purchase_service_19_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_eu_vat_id_purchase_service_7_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_acc_non_eu_purchase_services_19_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_no_id_purchase_19_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_no_id_sale_19_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_vat_id_purchase_19_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_vat_id_purchase_7_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_vat_id_sale_19_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_eu_vat_id_sale_7_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_no_id_purchase_7_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_no_id_sale_7_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_purchase_19_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_purchase_7_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_sale_19_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_sale_7_skr04
-DEL account.fiscal.position.account.template: l10n_de_skr04.chart_skr04_fiscal_position_account_non_eu_sale_services_19_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_no_id_purchase_19_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_no_id_purchase_7_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_no_id_sale_19_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_purchase_19_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_purchase_7_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_purchase_services_19_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_purchase_services_7_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_sale_19_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_eu_vat_id_sale_7_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_purchase_19_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_purchase_7_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_purchase_services_19_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_sale_19_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_sale_7_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr03.account_fiscal_position_tax_non_eu_sale_services_19_skr03
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_no_id_purchase_19_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_no_id_purchase_7_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_no_id_sale_19_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_purchase_19_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_purchase_7_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_purchase_services_19_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_purchase_services_7_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_sale_19_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_eu_vat_id_sale_7_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_purchase_19_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_purchase_7_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_purchase_services_19_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_sale_19_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_sale_7_skr04
-DEL account.fiscal.position.tax.template: l10n_de_skr04.chart_skr04_fiscal_position_tax_non_eu_sale_services_19_skr04
-DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_domestic_skr03
-DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_eu_no_id_partner_skr03
-DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_eu_vat_id_partner_service_skr03
-DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_eu_vat_id_partner_skr03
-DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_non_eu_partner_service_skr03
-DEL account.fiscal.position.template: l10n_de_skr03.fiscal_position_non_eu_partner_skr03
-DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_domestic_skr04
-DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_eu_no_id_partner_skr04
-DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_eu_vat_id_partner_service_skr04
-DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_eu_vat_id_partner_skr04
-DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_non_eu_partner_service_skr04
-DEL account.fiscal.position.template: l10n_de_skr04.fiscal_position_non_eu_partner_skr04
-DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_2401_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_2406_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_3731_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_3736_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_8731_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr03.reconcile_8736_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_4731_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_4736_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_5731_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_5736_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_6931_line (noupdate)
-DEL account.reconcile.model.line.template: l10n_de_skr04.reconcile_6936_line (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr03.reconcile_2401 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr03.reconcile_2406 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr03.reconcile_3731 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr03.reconcile_3736 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr03.reconcile_8731 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr03.reconcile_8736 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr04.reconcile_4731 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr04.reconcile_4736 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr04.reconcile_5731 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr04.reconcile_5736 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr04.reconcile_6931 (noupdate)
-DEL account.reconcile.model.template: l10n_de_skr04.reconcile_6936 (noupdate)
-DEL account.tax.group: l10n_de_skr03.tax_group_0 (noupdate)
-DEL account.tax.group: l10n_de_skr03.tax_group_107 (noupdate)
-DEL account.tax.group: l10n_de_skr03.tax_group_19 (noupdate)
-DEL account.tax.group: l10n_de_skr03.tax_group_55 (noupdate)
-DEL account.tax.group: l10n_de_skr03.tax_group_7 (noupdate)
-DEL account.tax.group: l10n_de_skr03.tax_group_x (noupdate)
-DEL account.tax.group: l10n_de_skr04.tax_group_0 (noupdate)
-DEL account.tax.group: l10n_de_skr04.tax_group_107 (noupdate)
-DEL account.tax.group: l10n_de_skr04.tax_group_19 (noupdate)
-DEL account.tax.group: l10n_de_skr04.tax_group_55 (noupdate)
-DEL account.tax.group: l10n_de_skr04.tax_group_7 (noupdate)
-DEL account.tax.group: l10n_de_skr04.tax_group_x (noupdate)
-DEL account.tax.template: l10n_de_skr03.tax_eu_19_purchase_goods_skr03
-DEL account.tax.template: l10n_de_skr03.tax_eu_19_purchase_no_vst_skr03
-DEL account.tax.template: l10n_de_skr03.tax_eu_19_purchase_skr03
-DEL account.tax.template: l10n_de_skr03.tax_eu_7_purchase_goods_skr03
-DEL account.tax.template: l10n_de_skr03.tax_eu_7_purchase_no_vst_skr03
-DEL account.tax.template: l10n_de_skr03.tax_eu_7_purchase_skr03
-DEL account.tax.template: l10n_de_skr03.tax_eu_car_purchase_skr03
-DEL account.tax.template: l10n_de_skr03.tax_eu_purchase_tax_free_skr03
-DEL account.tax.template: l10n_de_skr03.tax_eu_sale_skr03
-DEL account.tax.template: l10n_de_skr03.tax_export_skr03
-DEL account.tax.template: l10n_de_skr03.tax_free_eu_skr03
-DEL account.tax.template: l10n_de_skr03.tax_free_newcar_skr03
-DEL account.tax.template: l10n_de_skr03.tax_free_skr03_mit_vst
-DEL account.tax.template: l10n_de_skr03.tax_free_skr03_ohne_vst
-DEL account.tax.template: l10n_de_skr03.tax_free_third_country_skr03
-DEL account.tax.template: l10n_de_skr03.tax_import_19_and_payable_skr03
-DEL account.tax.template: l10n_de_skr03.tax_import_7_and_payable_skr03
-DEL account.tax.template: l10n_de_skr03.tax_not_taxable_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_107_farmer_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_19_13b_ausland_ohne_vst_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_19_13b_bau_ohne_vst_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_19_13b_eu_ohne_vst_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_19_3eck_first_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_19_eu_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_19_farmer_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_19_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_19_taxinclusive_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_55_farmer_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_7_13b_ausland_ohne_vst_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_7_13b_bau_ohne_vst_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_7_13b_eu_ohne_vst_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_7_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_7_taxinclusive_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_eu_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_free_bau_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_free_mobil_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_no_ustpflicht_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_vst_19_purchase_13b_bau_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_vst_7_purchase_13b_bau_skr03
-DEL account.tax.template: l10n_de_skr03.tax_ust_x_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_107_farmer_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_19_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_19_taxinclusive_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_55_farmer_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_7_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_7_taxinclusive_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_no_ustpflicht_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_ust_19_purchase_13a_auslagerung_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_ust_19_purchase_13b_mobil_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_ust_19_purchase_13b_werk_ausland_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_ust_19_purchase_3eck_last_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_ust_7_purchase_13a_auslagerung_skr03
-DEL account.tax.template: l10n_de_skr03.tax_vst_ust_7_purchase_13b_werk_ausland_skr03
-DEL account.tax.template: l10n_de_skr04.tax_eu_19_purchase_goods_skr04
-DEL account.tax.template: l10n_de_skr04.tax_eu_19_purchase_no_vst_skr04
-DEL account.tax.template: l10n_de_skr04.tax_eu_19_purchase_skr04
-DEL account.tax.template: l10n_de_skr04.tax_eu_7_purchase_goods_skr04
-DEL account.tax.template: l10n_de_skr04.tax_eu_7_purchase_no_vst_skr04
-DEL account.tax.template: l10n_de_skr04.tax_eu_7_purchase_skr04
-DEL account.tax.template: l10n_de_skr04.tax_eu_car_purchase_skr04
-DEL account.tax.template: l10n_de_skr04.tax_eu_purchase_tax_free_skr04
-DEL account.tax.template: l10n_de_skr04.tax_eu_sale_skr04
-DEL account.tax.template: l10n_de_skr04.tax_export_skr04
-DEL account.tax.template: l10n_de_skr04.tax_free_eu_skr04
-DEL account.tax.template: l10n_de_skr04.tax_free_newcar_skr04
-DEL account.tax.template: l10n_de_skr04.tax_free_skr04_mit_vst
-DEL account.tax.template: l10n_de_skr04.tax_free_skr04_ohne_vst
-DEL account.tax.template: l10n_de_skr04.tax_free_third_country_skr04
-DEL account.tax.template: l10n_de_skr04.tax_import_19_and_payable_skr04
-DEL account.tax.template: l10n_de_skr04.tax_import_7_and_payable_skr04
-DEL account.tax.template: l10n_de_skr04.tax_not_taxable_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_107_farmer_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_19_13b_ausland_ohne_vst_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_19_13b_bau_ohne_vst_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_19_13b_eu_ohne_vst_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_19_3eck_first_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_19_eu_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_19_farmer_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_19_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_19_taxinclusive_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_55_farmer_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_7_13b_ausland_ohne_vst_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_7_13b_bau_ohne_vst_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_7_13b_eu_ohne_vst_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_7_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_7_taxinclusive_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_eu_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_free_bau_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_free_mobil_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_no_ustpflicht_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_vst_19_purchase_13b_bau_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_vst_7_purchase_13b_bau_skr04
-DEL account.tax.template: l10n_de_skr04.tax_ust_x_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_107_farmer_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_19_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_19_taxinclusive_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_55_farmer_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_7_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_7_taxinclusive_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_no_ustpflicht_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_ust_19_purchase_13a_auslagerung_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_ust_19_purchase_13b_mobil_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_ust_19_purchase_13b_werk_ausland_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_ust_19_purchase_3eck_last_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_ust_7_purchase_13a_auslagerung_skr04
-DEL account.tax.template: l10n_de_skr04.tax_vst_ust_7_purchase_13b_werk_ausland_skr04
```

## odoo/addons/openupgrade_scripts/scripts/l10n_dk_oioubl/17.0.0.1/upgrade_analysis.txt

```diff
@@ -1,6 +1,6 @@
 ---Models in module 'l10n_dk_oioubl'---
 new model account.edi.xml.oioubl_201 [abstract]
 ---Fields in module 'l10n_dk_oioubl'---
-l10n_dk_oioubl / res.partner              / ubl_cii_format (False)        : NEW selection_keys: ['facturx', 'nlcius', 'oioubl_201', 'pint_jp', 'ubl_a_nz', 'ubl_bis3', 'ubl_sg', 'xrechnung'], mode: modify
+l10n_dk_oioubl / res.partner              / ubl_cii_format (False)        : NEW selection_keys: ['facturx', 'nlcius', 'oioubl_201', 'pint_jp', 'pint_my', 'ubl_a_nz', 'ubl_bis3', 'ubl_sg', 'xrechnung'], mode: modify
 ---XML records in module 'l10n_dk_oioubl'---
 NEW ir.ui.view: l10n_dk_oioubl.oioubl_PaymentTermsType
```

## odoo/addons/openupgrade_scripts/scripts/l10n_dz/17.0.1.0/upgrade_analysis.txt

```diff
@@ -902,15 +902,15 @@
 DEL account.fiscal.position.tax.template: l10n_dz.fp_tax_ve_template_exo_normale19
 DEL account.fiscal.position.tax.template: l10n_dz.fp_tax_ve_template_exo_specifique9
 DEL account.fiscal.position.tax.template: l10n_dz.fp_tax_ve_template_imp_exp_normale19
 DEL account.fiscal.position.tax.template: l10n_dz.fp_tax_ve_template_imp_exp_specifique9
 DEL account.fiscal.position.template: l10n_dz.fiscal_position_template_exo
 DEL account.fiscal.position.template: l10n_dz.fiscal_position_template_import_export
 DEL account.fiscal.position.template: l10n_dz.fiscal_position_template_national
-NEW account.report: l10n_dz.tax_report [renamed from l10n_pt module]
+NEW account.report: l10n_dz.tax_report
 NEW account.report.column: l10n_dz.tax_report_balance [renamed from l10n_ma module]
 NEW account.report.column: l10n_dz.tax_report_exempt_turnover
 NEW account.report.column: l10n_dz.tax_report_taxable_turnover
 NEW account.report.column: l10n_dz.tax_report_total_turnover
 NEW account.report.expression: l10n_dz.l10n_dz_tax_report_E3B11_balance_tag
 NEW account.report.expression: l10n_dz.l10n_dz_tax_report_E3B11_exempt_turnover_tag
 NEW account.report.expression: l10n_dz.l10n_dz_tax_report_E3B11_taxable_turnover_tag
```

## odoo/addons/openupgrade_scripts/scripts/l10n_eg_edi_eta/17.0.0.2/upgrade_analysis.txt

```diff
@@ -1,4 +1,4 @@
 ---Models in module 'l10n_eg_edi_eta'---
 ---Fields in module 'l10n_eg_edi_eta'---
 ---XML records in module 'l10n_eg_edi_eta'---
-DEL ir.model.constraint: l10n_eg_edi_eta.constraint_l10n_eg_edi_thumb_drive_user_drive_uniq
+---nothing has changed in this module--
```

## odoo/addons/openupgrade_scripts/scripts/l10n_hr/17.0.13.0/upgrade_analysis.txt

```diff
@@ -1671,698 +1671,30 @@
 DEL account.account.template: l10n_hr.kp_rrif9983
 DEL account.account.template: l10n_hr.kp_rrif9987
 DEL account.account.template: l10n_hr.kp_rrif9990
 DEL account.account.template: l10n_hr.kp_rrif9991
 DEL account.account.template: l10n_hr.kp_rrif9992
 DEL account.account.template: l10n_hr.kp_rrif9993
 DEL account.account.template: l10n_hr.kp_rrif9994
-DEL account.account.template: l10n_hr_euro.hr_000000
-DEL account.account.template: l10n_hr_euro.hr_001000
-DEL account.account.template: l10n_hr_euro.hr_002000
-DEL account.account.template: l10n_hr_euro.hr_003000
-DEL account.account.template: l10n_hr_euro.hr_004000
-DEL account.account.template: l10n_hr_euro.hr_010000
-DEL account.account.template: l10n_hr_euro.hr_011000
-DEL account.account.template: l10n_hr_euro.hr_012000
-DEL account.account.template: l10n_hr_euro.hr_013000
-DEL account.account.template: l10n_hr_euro.hr_014000
-DEL account.account.template: l10n_hr_euro.hr_015000
-DEL account.account.template: l10n_hr_euro.hr_016000
-DEL account.account.template: l10n_hr_euro.hr_017000
-DEL account.account.template: l10n_hr_euro.hr_018000
-DEL account.account.template: l10n_hr_euro.hr_019000
-DEL account.account.template: l10n_hr_euro.hr_020000
-DEL account.account.template: l10n_hr_euro.hr_021000
-DEL account.account.template: l10n_hr_euro.hr_023000
-DEL account.account.template: l10n_hr_euro.hr_024000
-DEL account.account.template: l10n_hr_euro.hr_026000
-DEL account.account.template: l10n_hr_euro.hr_027000
-DEL account.account.template: l10n_hr_euro.hr_028000
-DEL account.account.template: l10n_hr_euro.hr_029000
-DEL account.account.template: l10n_hr_euro.hr_030000
-DEL account.account.template: l10n_hr_euro.hr_031000
-DEL account.account.template: l10n_hr_euro.hr_032000
-DEL account.account.template: l10n_hr_euro.hr_033000
-DEL account.account.template: l10n_hr_euro.hr_034000
-DEL account.account.template: l10n_hr_euro.hr_035000
-DEL account.account.template: l10n_hr_euro.hr_036000
-DEL account.account.template: l10n_hr_euro.hr_037000
-DEL account.account.template: l10n_hr_euro.hr_038000
-DEL account.account.template: l10n_hr_euro.hr_039000
-DEL account.account.template: l10n_hr_euro.hr_040000
-DEL account.account.template: l10n_hr_euro.hr_041000
-DEL account.account.template: l10n_hr_euro.hr_046000
-DEL account.account.template: l10n_hr_euro.hr_047000
-DEL account.account.template: l10n_hr_euro.hr_048000
-DEL account.account.template: l10n_hr_euro.hr_049000
-DEL account.account.template: l10n_hr_euro.hr_050000
-DEL account.account.template: l10n_hr_euro.hr_051000
-DEL account.account.template: l10n_hr_euro.hr_056000
-DEL account.account.template: l10n_hr_euro.hr_057000
-DEL account.account.template: l10n_hr_euro.hr_058000
-DEL account.account.template: l10n_hr_euro.hr_059000
-DEL account.account.template: l10n_hr_euro.hr_060000
-DEL account.account.template: l10n_hr_euro.hr_060100
-DEL account.account.template: l10n_hr_euro.hr_061000
-DEL account.account.template: l10n_hr_euro.hr_062000
-DEL account.account.template: l10n_hr_euro.hr_062100
-DEL account.account.template: l10n_hr_euro.hr_063000
-DEL account.account.template: l10n_hr_euro.hr_064000
-DEL account.account.template: l10n_hr_euro.hr_065000
-DEL account.account.template: l10n_hr_euro.hr_066000
-DEL account.account.template: l10n_hr_euro.hr_067000
-DEL account.account.template: l10n_hr_euro.hr_068000
-DEL account.account.template: l10n_hr_euro.hr_069000
-DEL account.account.template: l10n_hr_euro.hr_070000
-DEL account.account.template: l10n_hr_euro.hr_071000
-DEL account.account.template: l10n_hr_euro.hr_072000
-DEL account.account.template: l10n_hr_euro.hr_073000
-DEL account.account.template: l10n_hr_euro.hr_074000
-DEL account.account.template: l10n_hr_euro.hr_075000
-DEL account.account.template: l10n_hr_euro.hr_076000
-DEL account.account.template: l10n_hr_euro.hr_077000
-DEL account.account.template: l10n_hr_euro.hr_078000
-DEL account.account.template: l10n_hr_euro.hr_079000
-DEL account.account.template: l10n_hr_euro.hr_080000
-DEL account.account.template: l10n_hr_euro.hr_081000
-DEL account.account.template: l10n_hr_euro.hr_100000
-DEL account.account.template: l10n_hr_euro.hr_101000
-DEL account.account.template: l10n_hr_euro.hr_102000
-DEL account.account.template: l10n_hr_euro.hr_103000
-DEL account.account.template: l10n_hr_euro.hr_104000
-DEL account.account.template: l10n_hr_euro.hr_105000
-DEL account.account.template: l10n_hr_euro.hr_106000
-DEL account.account.template: l10n_hr_euro.hr_108000
-DEL account.account.template: l10n_hr_euro.hr_109000
-DEL account.account.template: l10n_hr_euro.hr_110000
-DEL account.account.template: l10n_hr_euro.hr_110100
-DEL account.account.template: l10n_hr_euro.hr_111000
-DEL account.account.template: l10n_hr_euro.hr_112000
-DEL account.account.template: l10n_hr_euro.hr_112100
-DEL account.account.template: l10n_hr_euro.hr_113000
-DEL account.account.template: l10n_hr_euro.hr_114000
-DEL account.account.template: l10n_hr_euro.hr_115000
-DEL account.account.template: l10n_hr_euro.hr_116000
-DEL account.account.template: l10n_hr_euro.hr_117000
-DEL account.account.template: l10n_hr_euro.hr_118000
-DEL account.account.template: l10n_hr_euro.hr_119000
-DEL account.account.template: l10n_hr_euro.hr_120000
-DEL account.account.template: l10n_hr_euro.hr_120100
-DEL account.account.template: l10n_hr_euro.hr_121000
-DEL account.account.template: l10n_hr_euro.hr_122000
-DEL account.account.template: l10n_hr_euro.hr_123000
-DEL account.account.template: l10n_hr_euro.hr_124000
-DEL account.account.template: l10n_hr_euro.hr_125000
-DEL account.account.template: l10n_hr_euro.hr_126000
-DEL account.account.template: l10n_hr_euro.hr_127000
-DEL account.account.template: l10n_hr_euro.hr_128000
-DEL account.account.template: l10n_hr_euro.hr_129000
-DEL account.account.template: l10n_hr_euro.hr_130000
-DEL account.account.template: l10n_hr_euro.hr_131000
-DEL account.account.template: l10n_hr_euro.hr_133000
-DEL account.account.template: l10n_hr_euro.hr_134000
-DEL account.account.template: l10n_hr_euro.hr_135000
-DEL account.account.template: l10n_hr_euro.hr_136000
-DEL account.account.template: l10n_hr_euro.hr_137000
-DEL account.account.template: l10n_hr_euro.hr_138000
-DEL account.account.template: l10n_hr_euro.hr_139000
-DEL account.account.template: l10n_hr_euro.hr_140000
-DEL account.account.template: l10n_hr_euro.hr_140010
-DEL account.account.template: l10n_hr_euro.hr_140011
-DEL account.account.template: l10n_hr_euro.hr_140012
-DEL account.account.template: l10n_hr_euro.hr_140020
-DEL account.account.template: l10n_hr_euro.hr_140021
-DEL account.account.template: l10n_hr_euro.hr_140022
-DEL account.account.template: l10n_hr_euro.hr_140030
-DEL account.account.template: l10n_hr_euro.hr_140031
-DEL account.account.template: l10n_hr_euro.hr_140032
-DEL account.account.template: l10n_hr_euro.hr_140100
-DEL account.account.template: l10n_hr_euro.hr_140200
-DEL account.account.template: l10n_hr_euro.hr_140210
-DEL account.account.template: l10n_hr_euro.hr_140220
-DEL account.account.template: l10n_hr_euro.hr_140300
-DEL account.account.template: l10n_hr_euro.hr_140310
-DEL account.account.template: l10n_hr_euro.hr_140320
-DEL account.account.template: l10n_hr_euro.hr_140400
-DEL account.account.template: l10n_hr_euro.hr_140410
-DEL account.account.template: l10n_hr_euro.hr_140420
-DEL account.account.template: l10n_hr_euro.hr_140500
-DEL account.account.template: l10n_hr_euro.hr_140700
-DEL account.account.template: l10n_hr_euro.hr_140800
-DEL account.account.template: l10n_hr_euro.hr_141000
-DEL account.account.template: l10n_hr_euro.hr_142000
-DEL account.account.template: l10n_hr_euro.hr_143000
-DEL account.account.template: l10n_hr_euro.hr_144000
-DEL account.account.template: l10n_hr_euro.hr_145000
-DEL account.account.template: l10n_hr_euro.hr_146000
-DEL account.account.template: l10n_hr_euro.hr_147000
-DEL account.account.template: l10n_hr_euro.hr_148000
-DEL account.account.template: l10n_hr_euro.hr_149000
-DEL account.account.template: l10n_hr_euro.hr_150000
-DEL account.account.template: l10n_hr_euro.hr_151000
-DEL account.account.template: l10n_hr_euro.hr_152000
-DEL account.account.template: l10n_hr_euro.hr_153000
-DEL account.account.template: l10n_hr_euro.hr_154000
-DEL account.account.template: l10n_hr_euro.hr_155000
-DEL account.account.template: l10n_hr_euro.hr_156000
-DEL account.account.template: l10n_hr_euro.hr_159000
-DEL account.account.template: l10n_hr_euro.hr_190000
-DEL account.account.template: l10n_hr_euro.hr_191000
-DEL account.account.template: l10n_hr_euro.hr_192000
-DEL account.account.template: l10n_hr_euro.hr_193000
-DEL account.account.template: l10n_hr_euro.hr_194000
-DEL account.account.template: l10n_hr_euro.hr_195000
-DEL account.account.template: l10n_hr_euro.hr_196000
-DEL account.account.template: l10n_hr_euro.hr_197000
-DEL account.account.template: l10n_hr_euro.hr_199000
-DEL account.account.template: l10n_hr_euro.hr_200000
-DEL account.account.template: l10n_hr_euro.hr_200100
-DEL account.account.template: l10n_hr_euro.hr_201000
-DEL account.account.template: l10n_hr_euro.hr_210000
-DEL account.account.template: l10n_hr_euro.hr_211000
-DEL account.account.template: l10n_hr_euro.hr_212000
-DEL account.account.template: l10n_hr_euro.hr_213000
-DEL account.account.template: l10n_hr_euro.hr_213100
-DEL account.account.template: l10n_hr_euro.hr_214000
-DEL account.account.template: l10n_hr_euro.hr_215000
-DEL account.account.template: l10n_hr_euro.hr_216000
-DEL account.account.template: l10n_hr_euro.hr_217000
-DEL account.account.template: l10n_hr_euro.hr_218000
-DEL account.account.template: l10n_hr_euro.hr_220000
-DEL account.account.template: l10n_hr_euro.hr_221000
-DEL account.account.template: l10n_hr_euro.hr_222000
-DEL account.account.template: l10n_hr_euro.hr_223000
-DEL account.account.template: l10n_hr_euro.hr_224000
-DEL account.account.template: l10n_hr_euro.hr_225000
-DEL account.account.template: l10n_hr_euro.hr_230000
-DEL account.account.template: l10n_hr_euro.hr_231000
-DEL account.account.template: l10n_hr_euro.hr_232000
-DEL account.account.template: l10n_hr_euro.hr_233000
-DEL account.account.template: l10n_hr_euro.hr_234000
-DEL account.account.template: l10n_hr_euro.hr_235000
-DEL account.account.template: l10n_hr_euro.hr_236000
-DEL account.account.template: l10n_hr_euro.hr_237000
-DEL account.account.template: l10n_hr_euro.hr_238000
-DEL account.account.template: l10n_hr_euro.hr_239000
-DEL account.account.template: l10n_hr_euro.hr_240000
-DEL account.account.template: l10n_hr_euro.hr_240010
-DEL account.account.template: l10n_hr_euro.hr_240011
-DEL account.account.template: l10n_hr_euro.hr_240012
-DEL account.account.template: l10n_hr_euro.hr_240020
-DEL account.account.template: l10n_hr_euro.hr_240021
-DEL account.account.template: l10n_hr_euro.hr_240022
-DEL account.account.template: l10n_hr_euro.hr_240030
-DEL account.account.template: l10n_hr_euro.hr_240031
-DEL account.account.template: l10n_hr_euro.hr_240032
-DEL account.account.template: l10n_hr_euro.hr_240040
-DEL account.account.template: l10n_hr_euro.hr_240050
-DEL account.account.template: l10n_hr_euro.hr_240100
-DEL account.account.template: l10n_hr_euro.hr_240200
-DEL account.account.template: l10n_hr_euro.hr_240210
-DEL account.account.template: l10n_hr_euro.hr_240220
-DEL account.account.template: l10n_hr_euro.hr_240300
-DEL account.account.template: l10n_hr_euro.hr_240310
-DEL account.account.template: l10n_hr_euro.hr_240320
-DEL account.account.template: l10n_hr_euro.hr_240400
-DEL account.account.template: l10n_hr_euro.hr_240410
-DEL account.account.template: l10n_hr_euro.hr_240420
-DEL account.account.template: l10n_hr_euro.hr_240500
-DEL account.account.template: l10n_hr_euro.hr_240700
-DEL account.account.template: l10n_hr_euro.hr_240800
-DEL account.account.template: l10n_hr_euro.hr_241000
-DEL account.account.template: l10n_hr_euro.hr_242000
-DEL account.account.template: l10n_hr_euro.hr_243000
-DEL account.account.template: l10n_hr_euro.hr_244000
-DEL account.account.template: l10n_hr_euro.hr_245000
-DEL account.account.template: l10n_hr_euro.hr_246000
-DEL account.account.template: l10n_hr_euro.hr_247000
-DEL account.account.template: l10n_hr_euro.hr_248000
-DEL account.account.template: l10n_hr_euro.hr_249000
-DEL account.account.template: l10n_hr_euro.hr_250000
-DEL account.account.template: l10n_hr_euro.hr_250100
-DEL account.account.template: l10n_hr_euro.hr_251000
-DEL account.account.template: l10n_hr_euro.hr_251100
-DEL account.account.template: l10n_hr_euro.hr_252000
-DEL account.account.template: l10n_hr_euro.hr_253000
-DEL account.account.template: l10n_hr_euro.hr_254000
-DEL account.account.template: l10n_hr_euro.hr_255000
-DEL account.account.template: l10n_hr_euro.hr_256000
-DEL account.account.template: l10n_hr_euro.hr_257000
-DEL account.account.template: l10n_hr_euro.hr_258000
-DEL account.account.template: l10n_hr_euro.hr_259000
-DEL account.account.template: l10n_hr_euro.hr_260000
-DEL account.account.template: l10n_hr_euro.hr_280000
-DEL account.account.template: l10n_hr_euro.hr_281000
-DEL account.account.template: l10n_hr_euro.hr_282000
-DEL account.account.template: l10n_hr_euro.hr_283000
-DEL account.account.template: l10n_hr_euro.hr_284000
-DEL account.account.template: l10n_hr_euro.hr_285000
-DEL account.account.template: l10n_hr_euro.hr_290000
-DEL account.account.template: l10n_hr_euro.hr_291000
-DEL account.account.template: l10n_hr_euro.hr_292000
-DEL account.account.template: l10n_hr_euro.hr_293000
-DEL account.account.template: l10n_hr_euro.hr_294000
-DEL account.account.template: l10n_hr_euro.hr_295000
-DEL account.account.template: l10n_hr_euro.hr_296000
-DEL account.account.template: l10n_hr_euro.hr_297000
-DEL account.account.template: l10n_hr_euro.hr_298000
-DEL account.account.template: l10n_hr_euro.hr_299000
-DEL account.account.template: l10n_hr_euro.hr_300000
-DEL account.account.template: l10n_hr_euro.hr_301000
-DEL account.account.template: l10n_hr_euro.hr_302000
-DEL account.account.template: l10n_hr_euro.hr_303000
-DEL account.account.template: l10n_hr_euro.hr_309000
-DEL account.account.template: l10n_hr_euro.hr_310000
-DEL account.account.template: l10n_hr_euro.hr_311000
-DEL account.account.template: l10n_hr_euro.hr_312000
-DEL account.account.template: l10n_hr_euro.hr_313000
-DEL account.account.template: l10n_hr_euro.hr_318000
-DEL account.account.template: l10n_hr_euro.hr_319000
-DEL account.account.template: l10n_hr_euro.hr_320000
-DEL account.account.template: l10n_hr_euro.hr_328000
-DEL account.account.template: l10n_hr_euro.hr_329000
-DEL account.account.template: l10n_hr_euro.hr_350000
-DEL account.account.template: l10n_hr_euro.hr_351000
-DEL account.account.template: l10n_hr_euro.hr_352000
-DEL account.account.template: l10n_hr_euro.hr_358000
-DEL account.account.template: l10n_hr_euro.hr_359000
-DEL account.account.template: l10n_hr_euro.hr_360000
-DEL account.account.template: l10n_hr_euro.hr_361000
-DEL account.account.template: l10n_hr_euro.hr_362000
-DEL account.account.template: l10n_hr_euro.hr_363000
-DEL account.account.template: l10n_hr_euro.hr_364000
-DEL account.account.template: l10n_hr_euro.hr_365000
-DEL account.account.template: l10n_hr_euro.hr_369000
-DEL account.account.template: l10n_hr_euro.hr_370000
-DEL account.account.template: l10n_hr_euro.hr_371000
-DEL account.account.template: l10n_hr_euro.hr_372000
-DEL account.account.template: l10n_hr_euro.hr_373000
-DEL account.account.template: l10n_hr_euro.hr_374000
-DEL account.account.template: l10n_hr_euro.hr_379000
-DEL account.account.template: l10n_hr_euro.hr_400000
-DEL account.account.template: l10n_hr_euro.hr_401000
-DEL account.account.template: l10n_hr_euro.hr_402000
-DEL account.account.template: l10n_hr_euro.hr_403000
-DEL account.account.template: l10n_hr_euro.hr_404000
-DEL account.account.template: l10n_hr_euro.hr_405000
-DEL account.account.template: l10n_hr_euro.hr_406000
-DEL account.account.template: l10n_hr_euro.hr_407000
-DEL account.account.template: l10n_hr_euro.hr_408000
-DEL account.account.template: l10n_hr_euro.hr_409000
-DEL account.account.template: l10n_hr_euro.hr_410000
-DEL account.account.template: l10n_hr_euro.hr_411000
-DEL account.account.template: l10n_hr_euro.hr_412000
-DEL account.account.template: l10n_hr_euro.hr_413000
-DEL account.account.template: l10n_hr_euro.hr_414000
-DEL account.account.template: l10n_hr_euro.hr_415000
-DEL account.account.template: l10n_hr_euro.hr_416000
-DEL account.account.template: l10n_hr_euro.hr_417000
-DEL account.account.template: l10n_hr_euro.hr_418000
-DEL account.account.template: l10n_hr_euro.hr_419000
-DEL account.account.template: l10n_hr_euro.hr_420000
-DEL account.account.template: l10n_hr_euro.hr_421000
-DEL account.account.template: l10n_hr_euro.hr_422000
-DEL account.account.template: l10n_hr_euro.hr_423000
-DEL account.account.template: l10n_hr_euro.hr_424000
-DEL account.account.template: l10n_hr_euro.hr_430000
-DEL account.account.template: l10n_hr_euro.hr_431000
-DEL account.account.template: l10n_hr_euro.hr_432000
-DEL account.account.template: l10n_hr_euro.hr_433000
-DEL account.account.template: l10n_hr_euro.hr_434000
-DEL account.account.template: l10n_hr_euro.hr_435000
-DEL account.account.template: l10n_hr_euro.hr_436000
-DEL account.account.template: l10n_hr_euro.hr_440000
-DEL account.account.template: l10n_hr_euro.hr_441000
-DEL account.account.template: l10n_hr_euro.hr_442000
-DEL account.account.template: l10n_hr_euro.hr_444000
-DEL account.account.template: l10n_hr_euro.hr_445000
-DEL account.account.template: l10n_hr_euro.hr_446000
-DEL account.account.template: l10n_hr_euro.hr_447000
-DEL account.account.template: l10n_hr_euro.hr_448000
-DEL account.account.template: l10n_hr_euro.hr_449000
-DEL account.account.template: l10n_hr_euro.hr_450000
-DEL account.account.template: l10n_hr_euro.hr_451000
-DEL account.account.template: l10n_hr_euro.hr_452000
-DEL account.account.template: l10n_hr_euro.hr_453000
-DEL account.account.template: l10n_hr_euro.hr_454000
-DEL account.account.template: l10n_hr_euro.hr_455000
-DEL account.account.template: l10n_hr_euro.hr_456000
-DEL account.account.template: l10n_hr_euro.hr_457000
-DEL account.account.template: l10n_hr_euro.hr_460000
-DEL account.account.template: l10n_hr_euro.hr_461000
-DEL account.account.template: l10n_hr_euro.hr_462000
-DEL account.account.template: l10n_hr_euro.hr_463000
-DEL account.account.template: l10n_hr_euro.hr_464000
-DEL account.account.template: l10n_hr_euro.hr_465000
-DEL account.account.template: l10n_hr_euro.hr_466000
-DEL account.account.template: l10n_hr_euro.hr_467000
-DEL account.account.template: l10n_hr_euro.hr_468000
-DEL account.account.template: l10n_hr_euro.hr_469000
-DEL account.account.template: l10n_hr_euro.hr_470000
-DEL account.account.template: l10n_hr_euro.hr_471000
-DEL account.account.template: l10n_hr_euro.hr_472000
-DEL account.account.template: l10n_hr_euro.hr_473000
-DEL account.account.template: l10n_hr_euro.hr_474000
-DEL account.account.template: l10n_hr_euro.hr_475000
-DEL account.account.template: l10n_hr_euro.hr_476000
-DEL account.account.template: l10n_hr_euro.hr_477000
-DEL account.account.template: l10n_hr_euro.hr_478000
-DEL account.account.template: l10n_hr_euro.hr_478200
-DEL account.account.template: l10n_hr_euro.hr_479000
-DEL account.account.template: l10n_hr_euro.hr_480000
-DEL account.account.template: l10n_hr_euro.hr_481000
-DEL account.account.template: l10n_hr_euro.hr_482000
-DEL account.account.template: l10n_hr_euro.hr_483000
-DEL account.account.template: l10n_hr_euro.hr_484000
-DEL account.account.template: l10n_hr_euro.hr_485000
-DEL account.account.template: l10n_hr_euro.hr_486000
-DEL account.account.template: l10n_hr_euro.hr_487000
-DEL account.account.template: l10n_hr_euro.hr_488000
-DEL account.account.template: l10n_hr_euro.hr_489000
-DEL account.account.template: l10n_hr_euro.hr_490000
-DEL account.account.template: l10n_hr_euro.hr_491000
-DEL account.account.template: l10n_hr_euro.hr_500000
-DEL account.account.template: l10n_hr_euro.hr_501000
-DEL account.account.template: l10n_hr_euro.hr_502000
-DEL account.account.template: l10n_hr_euro.hr_505000
-DEL account.account.template: l10n_hr_euro.hr_510000
-DEL account.account.template: l10n_hr_euro.hr_511000
-DEL account.account.template: l10n_hr_euro.hr_512000
-DEL account.account.template: l10n_hr_euro.hr_513000
-DEL account.account.template: l10n_hr_euro.hr_515000
-DEL account.account.template: l10n_hr_euro.hr_590000
-DEL account.account.template: l10n_hr_euro.hr_591000
-DEL account.account.template: l10n_hr_euro.hr_600000
-DEL account.account.template: l10n_hr_euro.hr_601000
-DEL account.account.template: l10n_hr_euro.hr_602000
-DEL account.account.template: l10n_hr_euro.hr_605000
-DEL account.account.template: l10n_hr_euro.hr_606000
-DEL account.account.template: l10n_hr_euro.hr_607000
-DEL account.account.template: l10n_hr_euro.hr_608000
-DEL account.account.template: l10n_hr_euro.hr_609000
-DEL account.account.template: l10n_hr_euro.hr_610000
-DEL account.account.template: l10n_hr_euro.hr_611000
-DEL account.account.template: l10n_hr_euro.hr_619000
-DEL account.account.template: l10n_hr_euro.hr_620000
-DEL account.account.template: l10n_hr_euro.hr_621000
-DEL account.account.template: l10n_hr_euro.hr_629000
-DEL account.account.template: l10n_hr_euro.hr_630000
-DEL account.account.template: l10n_hr_euro.hr_631000
-DEL account.account.template: l10n_hr_euro.hr_632000
-DEL account.account.template: l10n_hr_euro.hr_633000
-DEL account.account.template: l10n_hr_euro.hr_634000
-DEL account.account.template: l10n_hr_euro.hr_635000
-DEL account.account.template: l10n_hr_euro.hr_636000
-DEL account.account.template: l10n_hr_euro.hr_637000
-DEL account.account.template: l10n_hr_euro.hr_638000
-DEL account.account.template: l10n_hr_euro.hr_639000
-DEL account.account.template: l10n_hr_euro.hr_640000
-DEL account.account.template: l10n_hr_euro.hr_641000
-DEL account.account.template: l10n_hr_euro.hr_648000
-DEL account.account.template: l10n_hr_euro.hr_649000
-DEL account.account.template: l10n_hr_euro.hr_660000
-DEL account.account.template: l10n_hr_euro.hr_661000
-DEL account.account.template: l10n_hr_euro.hr_662000
-DEL account.account.template: l10n_hr_euro.hr_663000
-DEL account.account.template: l10n_hr_euro.hr_664000
-DEL account.account.template: l10n_hr_euro.hr_665000
-DEL account.account.template: l10n_hr_euro.hr_666000
-DEL account.account.template: l10n_hr_euro.hr_667000
-DEL account.account.template: l10n_hr_euro.hr_668000
-DEL account.account.template: l10n_hr_euro.hr_669000
-DEL account.account.template: l10n_hr_euro.hr_670000
-DEL account.account.template: l10n_hr_euro.hr_671000
-DEL account.account.template: l10n_hr_euro.hr_672000
-DEL account.account.template: l10n_hr_euro.hr_673000
-DEL account.account.template: l10n_hr_euro.hr_679000
-DEL account.account.template: l10n_hr_euro.hr_680000
-DEL account.account.template: l10n_hr_euro.hr_681000
-DEL account.account.template: l10n_hr_euro.hr_682000
-DEL account.account.template: l10n_hr_euro.hr_683000
-DEL account.account.template: l10n_hr_euro.hr_684000
-DEL account.account.template: l10n_hr_euro.hr_685000
-DEL account.account.template: l10n_hr_euro.hr_687000
-DEL account.account.template: l10n_hr_euro.hr_688000
-DEL account.account.template: l10n_hr_euro.hr_689000
-DEL account.account.template: l10n_hr_euro.hr_690000
-DEL account.account.template: l10n_hr_euro.hr_691000
-DEL account.account.template: l10n_hr_euro.hr_699000
-DEL account.account.template: l10n_hr_euro.hr_700000
-DEL account.account.template: l10n_hr_euro.hr_701000
-DEL account.account.template: l10n_hr_euro.hr_702000
-DEL account.account.template: l10n_hr_euro.hr_703000
-DEL account.account.template: l10n_hr_euro.hr_704000
-DEL account.account.template: l10n_hr_euro.hr_705000
-DEL account.account.template: l10n_hr_euro.hr_706000
-DEL account.account.template: l10n_hr_euro.hr_707000
-DEL account.account.template: l10n_hr_euro.hr_708000
-DEL account.account.template: l10n_hr_euro.hr_710000
-DEL account.account.template: l10n_hr_euro.hr_711000
-DEL account.account.template: l10n_hr_euro.hr_712000
-DEL account.account.template: l10n_hr_euro.hr_713000
-DEL account.account.template: l10n_hr_euro.hr_714000
-DEL account.account.template: l10n_hr_euro.hr_715000
-DEL account.account.template: l10n_hr_euro.hr_718000
-DEL account.account.template: l10n_hr_euro.hr_719000
-DEL account.account.template: l10n_hr_euro.hr_720000
-DEL account.account.template: l10n_hr_euro.hr_721000
-DEL account.account.template: l10n_hr_euro.hr_730000
-DEL account.account.template: l10n_hr_euro.hr_731000
-DEL account.account.template: l10n_hr_euro.hr_732000
-DEL account.account.template: l10n_hr_euro.hr_733000
-DEL account.account.template: l10n_hr_euro.hr_734000
-DEL account.account.template: l10n_hr_euro.hr_735000
-DEL account.account.template: l10n_hr_euro.hr_736000
-DEL account.account.template: l10n_hr_euro.hr_737000
-DEL account.account.template: l10n_hr_euro.hr_738000
-DEL account.account.template: l10n_hr_euro.hr_740000
-DEL account.account.template: l10n_hr_euro.hr_740100
-DEL account.account.template: l10n_hr_euro.hr_745000
-DEL account.account.template: l10n_hr_euro.hr_745100
-DEL account.account.template: l10n_hr_euro.hr_750000
-DEL account.account.template: l10n_hr_euro.hr_751000
-DEL account.account.template: l10n_hr_euro.hr_752000
-DEL account.account.template: l10n_hr_euro.hr_753000
-DEL account.account.template: l10n_hr_euro.hr_754000
-DEL account.account.template: l10n_hr_euro.hr_755000
-DEL account.account.template: l10n_hr_euro.hr_756000
-DEL account.account.template: l10n_hr_euro.hr_757000
-DEL account.account.template: l10n_hr_euro.hr_758000
-DEL account.account.template: l10n_hr_euro.hr_759000
-DEL account.account.template: l10n_hr_euro.hr_760000
-DEL account.account.template: l10n_hr_euro.hr_761000
-DEL account.account.template: l10n_hr_euro.hr_762000
-DEL account.account.template: l10n_hr_euro.hr_763000
-DEL account.account.template: l10n_hr_euro.hr_764000
-DEL account.account.template: l10n_hr_euro.hr_765000
-DEL account.account.template: l10n_hr_euro.hr_766000
-DEL account.account.template: l10n_hr_euro.hr_767000
-DEL account.account.template: l10n_hr_euro.hr_768000
-DEL account.account.template: l10n_hr_euro.hr_769000
-DEL account.account.template: l10n_hr_euro.hr_770000
-DEL account.account.template: l10n_hr_euro.hr_770100
-DEL account.account.template: l10n_hr_euro.hr_770200
-DEL account.account.template: l10n_hr_euro.hr_770300
-DEL account.account.template: l10n_hr_euro.hr_771000
-DEL account.account.template: l10n_hr_euro.hr_772000
-DEL account.account.template: l10n_hr_euro.hr_773000
-DEL account.account.template: l10n_hr_euro.hr_774000
-DEL account.account.template: l10n_hr_euro.hr_775000
-DEL account.account.template: l10n_hr_euro.hr_776000
-DEL account.account.template: l10n_hr_euro.hr_777000
-DEL account.account.template: l10n_hr_euro.hr_778000
-DEL account.account.template: l10n_hr_euro.hr_779000
-DEL account.account.template: l10n_hr_euro.hr_780000
-DEL account.account.template: l10n_hr_euro.hr_780900
-DEL account.account.template: l10n_hr_euro.hr_781000
-DEL account.account.template: l10n_hr_euro.hr_782000
-DEL account.account.template: l10n_hr_euro.hr_783000
-DEL account.account.template: l10n_hr_euro.hr_783900
-DEL account.account.template: l10n_hr_euro.hr_784000
-DEL account.account.template: l10n_hr_euro.hr_785000
-DEL account.account.template: l10n_hr_euro.hr_786000
-DEL account.account.template: l10n_hr_euro.hr_787000
-DEL account.account.template: l10n_hr_euro.hr_788000
-DEL account.account.template: l10n_hr_euro.hr_789000
-DEL account.account.template: l10n_hr_euro.hr_803000
-DEL account.account.template: l10n_hr_euro.hr_900000
-DEL account.account.template: l10n_hr_euro.hr_901000
-DEL account.account.template: l10n_hr_euro.hr_902000
-DEL account.account.template: l10n_hr_euro.hr_903000
-DEL account.account.template: l10n_hr_euro.hr_904000
-DEL account.account.template: l10n_hr_euro.hr_905000
-DEL account.account.template: l10n_hr_euro.hr_906000
-DEL account.account.template: l10n_hr_euro.hr_910000
-DEL account.account.template: l10n_hr_euro.hr_911000
-DEL account.account.template: l10n_hr_euro.hr_912000
-DEL account.account.template: l10n_hr_euro.hr_913000
-DEL account.account.template: l10n_hr_euro.hr_914000
-DEL account.account.template: l10n_hr_euro.hr_915000
-DEL account.account.template: l10n_hr_euro.hr_916000
-DEL account.account.template: l10n_hr_euro.hr_917000
-DEL account.account.template: l10n_hr_euro.hr_918000
-DEL account.account.template: l10n_hr_euro.hr_919000
-DEL account.account.template: l10n_hr_euro.hr_920000
-DEL account.account.template: l10n_hr_euro.hr_921000
-DEL account.account.template: l10n_hr_euro.hr_922000
-DEL account.account.template: l10n_hr_euro.hr_923000
-DEL account.account.template: l10n_hr_euro.hr_924000
-DEL account.account.template: l10n_hr_euro.hr_930000
-DEL account.account.template: l10n_hr_euro.hr_931000
-DEL account.account.template: l10n_hr_euro.hr_931200
-DEL account.account.template: l10n_hr_euro.hr_931300
-DEL account.account.template: l10n_hr_euro.hr_932000
-DEL account.account.template: l10n_hr_euro.hr_933000
-DEL account.account.template: l10n_hr_euro.hr_934000
-DEL account.account.template: l10n_hr_euro.hr_935000
-DEL account.account.template: l10n_hr_euro.hr_940000
-DEL account.account.template: l10n_hr_euro.hr_941000
-DEL account.account.template: l10n_hr_euro.hr_960000
-DEL account.account.template: l10n_hr_euro.hr_990000
-DEL account.account.template: l10n_hr_euro.hr_991000
-DEL account.account.template: l10n_hr_euro.hr_992000
-DEL account.account.template: l10n_hr_euro.hr_993000
-DEL account.account.template: l10n_hr_euro.hr_994000
-DEL account.account.template: l10n_hr_euro.hr_995000
-DEL account.account.template: l10n_hr_euro.hr_996000
-DEL account.account.template: l10n_hr_euro.hr_997000
-DEL account.account.template: l10n_hr_euro.hr_998000
-DEL account.account.template: l10n_hr_euro.hr_999000
 DEL account.chart.template: l10n_hr.l10n_hr_chart_template_rrif
-DEL account.chart.template: l10n_hr_euro.l10n_hr_euro_chart_template
 DEL account.fiscal.position.account.template: l10n_hr.account_fiscal_position_account_template_rrif_1
 DEL account.fiscal.position.account.template: l10n_hr.account_fiscal_position_account_template_rrif_2
 DEL account.fiscal.position.account.template: l10n_hr.account_fiscal_position_account_template_rrif_3
 DEL account.fiscal.position.tax.template: l10n_hr.account_fiscal_position_tax_template_rrif_3
 DEL account.fiscal.position.tax.template: l10n_hr.account_fiscal_position_tax_template_rrif_4
 DEL account.fiscal.position.tax.template: l10n_hr.account_fiscal_position_tax_template_rrif_5
 DEL account.fiscal.position.tax.template: l10n_hr.account_fiscal_position_tax_template_rrif_6
 DEL account.fiscal.position.tax.template: l10n_hr.account_fiscal_position_tax_template_rrif_7
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_P_G_hr_eu_1
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_P_G_hr_eu_2
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_P_G_hr_eu_3
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_S_G_hr_eu_1
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_S_G_hr_eu_2
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_S_G_hr_eu_3
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_exempt_tax_1
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_exempt_tax_2
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_exempt_tax_3
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_out_eu_1
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_out_eu_2
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_P_out_eu_3
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_exempt_tax_1
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_exempt_tax_2
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_exempt_tax_3
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_out_eu_1
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_out_eu_2
-DEL account.fiscal.position.tax.template: l10n_hr_euro.fiscal_position_hr_S_out_eu_3
 DEL account.fiscal.position.template: l10n_hr.account_fiscal_position_template_rrif_2
 DEL account.fiscal.position.template: l10n_hr.account_fiscal_position_template_rrif_3
 DEL account.fiscal.position.template: l10n_hr.account_fiscal_position_template_rrif_4
 DEL account.fiscal.position.template: l10n_hr.account_fiscal_position_template_rrif_domairpartneri0
-DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_eu (noupdate)
-DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_eu_out (noupdate)
-DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_exempt (noupdate)
-DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_national (noupdate)
-DEL account.fiscal.position.template: l10n_hr_euro.fiscal_position_hr_person_private (noupdate)
-DEL account.group.template: l10n_hr_euro.hr_group_0
-DEL account.group.template: l10n_hr_euro.hr_group_00
-DEL account.group.template: l10n_hr_euro.hr_group_01
-DEL account.group.template: l10n_hr_euro.hr_group_02
-DEL account.group.template: l10n_hr_euro.hr_group_03
-DEL account.group.template: l10n_hr_euro.hr_group_04
-DEL account.group.template: l10n_hr_euro.hr_group_05
-DEL account.group.template: l10n_hr_euro.hr_group_06
-DEL account.group.template: l10n_hr_euro.hr_group_07
-DEL account.group.template: l10n_hr_euro.hr_group_08
-DEL account.group.template: l10n_hr_euro.hr_group_1
-DEL account.group.template: l10n_hr_euro.hr_group_10
-DEL account.group.template: l10n_hr_euro.hr_group_11
-DEL account.group.template: l10n_hr_euro.hr_group_12
-DEL account.group.template: l10n_hr_euro.hr_group_13
-DEL account.group.template: l10n_hr_euro.hr_group_14
-DEL account.group.template: l10n_hr_euro.hr_group_15
-DEL account.group.template: l10n_hr_euro.hr_group_19
-DEL account.group.template: l10n_hr_euro.hr_group_2
-DEL account.group.template: l10n_hr_euro.hr_group_20
-DEL account.group.template: l10n_hr_euro.hr_group_21
-DEL account.group.template: l10n_hr_euro.hr_group_22
-DEL account.group.template: l10n_hr_euro.hr_group_23
-DEL account.group.template: l10n_hr_euro.hr_group_24
-DEL account.group.template: l10n_hr_euro.hr_group_25
-DEL account.group.template: l10n_hr_euro.hr_group_26
-DEL account.group.template: l10n_hr_euro.hr_group_28
-DEL account.group.template: l10n_hr_euro.hr_group_29
-DEL account.group.template: l10n_hr_euro.hr_group_3
-DEL account.group.template: l10n_hr_euro.hr_group_30
-DEL account.group.template: l10n_hr_euro.hr_group_31
-DEL account.group.template: l10n_hr_euro.hr_group_32
-DEL account.group.template: l10n_hr_euro.hr_group_35
-DEL account.group.template: l10n_hr_euro.hr_group_36
-DEL account.group.template: l10n_hr_euro.hr_group_37
-DEL account.group.template: l10n_hr_euro.hr_group_4
-DEL account.group.template: l10n_hr_euro.hr_group_40
-DEL account.group.template: l10n_hr_euro.hr_group_41
-DEL account.group.template: l10n_hr_euro.hr_group_42
-DEL account.group.template: l10n_hr_euro.hr_group_43
-DEL account.group.template: l10n_hr_euro.hr_group_44
-DEL account.group.template: l10n_hr_euro.hr_group_45
-DEL account.group.template: l10n_hr_euro.hr_group_46
-DEL account.group.template: l10n_hr_euro.hr_group_47
-DEL account.group.template: l10n_hr_euro.hr_group_48
-DEL account.group.template: l10n_hr_euro.hr_group_49
-DEL account.group.template: l10n_hr_euro.hr_group_5
-DEL account.group.template: l10n_hr_euro.hr_group_50
-DEL account.group.template: l10n_hr_euro.hr_group_51
-DEL account.group.template: l10n_hr_euro.hr_group_52
-DEL account.group.template: l10n_hr_euro.hr_group_53
-DEL account.group.template: l10n_hr_euro.hr_group_54
-DEL account.group.template: l10n_hr_euro.hr_group_59
-DEL account.group.template: l10n_hr_euro.hr_group_6
-DEL account.group.template: l10n_hr_euro.hr_group_60
-DEL account.group.template: l10n_hr_euro.hr_group_61
-DEL account.group.template: l10n_hr_euro.hr_group_62
-DEL account.group.template: l10n_hr_euro.hr_group_63
-DEL account.group.template: l10n_hr_euro.hr_group_64
-DEL account.group.template: l10n_hr_euro.hr_group_65
-DEL account.group.template: l10n_hr_euro.hr_group_66
-DEL account.group.template: l10n_hr_euro.hr_group_67
-DEL account.group.template: l10n_hr_euro.hr_group_68
-DEL account.group.template: l10n_hr_euro.hr_group_69
-DEL account.group.template: l10n_hr_euro.hr_group_7
-DEL account.group.template: l10n_hr_euro.hr_group_70
-DEL account.group.template: l10n_hr_euro.hr_group_71
-DEL account.group.template: l10n_hr_euro.hr_group_72
-DEL account.group.template: l10n_hr_euro.hr_group_73
-DEL account.group.template: l10n_hr_euro.hr_group_74
-DEL account.group.template: l10n_hr_euro.hr_group_75
-DEL account.group.template: l10n_hr_euro.hr_group_76
-DEL account.group.template: l10n_hr_euro.hr_group_77
-DEL account.group.template: l10n_hr_euro.hr_group_78
-DEL account.group.template: l10n_hr_euro.hr_group_79
-DEL account.group.template: l10n_hr_euro.hr_group_8
-DEL account.group.template: l10n_hr_euro.hr_group_80
-DEL account.group.template: l10n_hr_euro.hr_group_81
-DEL account.group.template: l10n_hr_euro.hr_group_82
-DEL account.group.template: l10n_hr_euro.hr_group_83
-DEL account.group.template: l10n_hr_euro.hr_group_9
-DEL account.group.template: l10n_hr_euro.hr_group_90
-DEL account.group.template: l10n_hr_euro.hr_group_91
-DEL account.group.template: l10n_hr_euro.hr_group_92
-DEL account.group.template: l10n_hr_euro.hr_group_93
-DEL account.group.template: l10n_hr_euro.hr_group_94
-DEL account.group.template: l10n_hr_euro.hr_group_95
-DEL account.group.template: l10n_hr_euro.hr_group_96
-DEL account.group.template: l10n_hr_euro.hr_group_99
-DEL account.report: l10n_hr_euro.tax_report [renamed to l10n_tn module]
 NEW account.report.column: l10n_hr.tax_report_tax_amount [renamed from l10n_hr_euro module]
 NEW account.report.column: l10n_hr.tax_report_tax_base [renamed from l10n_hr_euro module]
 DEL account.report.column: l10n_hr.tax_report_balance [renamed to l10n_hr_kuna module]
-DEL account.report.column: l10n_hr_euro.tax_report_tax_amount [renamed to l10n_hr module]
-DEL account.report.column: l10n_hr_euro.tax_report_tax_base [renamed to l10n_hr module]
 NEW account.report.expression: l10n_hr.tax_report_line_0_0_tag_column1 [renamed from l10n_hr_euro module]
 NEW account.report.expression: l10n_hr.tax_report_line_0_0_tag_column2 [renamed from l10n_hr_euro module]
 NEW account.report.expression: l10n_hr.tax_report_line_III_0_tag_column1 [renamed from l10n_hr_euro module]
 NEW account.report.expression: l10n_hr.tax_report_line_III_0_tag_column2 [renamed from l10n_hr_euro module]
 NEW account.report.expression: l10n_hr.tax_report_line_III_10_tag_column1 [renamed from l10n_hr_euro module]
 NEW account.report.expression: l10n_hr.tax_report_line_III_10_tag_column2 [renamed from l10n_hr_euro module]
 NEW account.report.expression: l10n_hr.tax_report_line_III_11_tag_column1 [renamed from l10n_hr_euro module]
@@ -2498,99 +1830,14 @@
 DEL account.report.expression: l10n_hr.account_tax_report_line_pretporez_koji_neplaceni_usluge_25_tag [renamed to l10n_hr_kuna module]
 DEL account.report.expression: l10n_hr.account_tax_report_line_pretporez_koji_tag [renamed to l10n_hr_kuna module]
 DEL account.report.expression: l10n_hr.account_tax_report_line_prodaja_dugotrajne_formula [renamed to l10n_hr_kuna module]
 DEL account.report.expression: l10n_hr.account_tax_report_line_prodaja_formula [renamed to l10n_hr_kuna module]
 DEL account.report.expression: l10n_hr.account_tax_report_line_prodaja_osobnih_formula [renamed to l10n_hr_kuna module]
 DEL account.report.expression: l10n_hr.account_tax_report_line_tuzemne_tag [renamed to l10n_hr_kuna module]
 DEL account.report.expression: l10n_hr.account_tax_report_line_uplaceno_formula [renamed to l10n_hr_kuna module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_0_0_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_0_0_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_0_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_0_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_10_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_10_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_11_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_11_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_12_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_12_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_13_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_13_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_14_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_14_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_15_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_1_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_1_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_2_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_2_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_3_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_3_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_4_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_4_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_5_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_5_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_6_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_6_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_7_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_7_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_8_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_8_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_9_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_III_9_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_0_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_0_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_10_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_10_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_11_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_11_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_12_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_12_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_13_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_13_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_14_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_14_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_15_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_15_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_1_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_1_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_2_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_2_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_3_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_3_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_4_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_4_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_5_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_5_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_6_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_6_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_7_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_7_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_8_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_8_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_9_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_II_9_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_IV_0_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_IV_1_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_IV_2_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_0_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_10_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_1_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_2_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_3_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_4_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_5_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_6_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_7_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_8_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_I_9_tag_column1 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_VI_0_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_VI_1_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_VI_2_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_V_0_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_V_1_tag_column2 [renamed to l10n_hr module]
-DEL account.report.expression: l10n_hr_euro.tax_report_line_V_2_tag_column2 [renamed to l10n_hr module]
 NEW account.report.line: l10n_hr.tax_report_line_III_1 [renamed from l10n_hr_euro module]
 NEW account.report.line: l10n_hr.tax_report_line_III_10 [renamed from l10n_hr_euro module]
 NEW account.report.line: l10n_hr.tax_report_line_III_11 [renamed from l10n_hr_euro module]
 NEW account.report.line: l10n_hr.tax_report_line_III_12 [renamed from l10n_hr_euro module]
 NEW account.report.line: l10n_hr.tax_report_line_III_13 [renamed from l10n_hr_euro module]
 NEW account.report.line: l10n_hr.tax_report_line_III_14 [renamed from l10n_hr_euro module]
 NEW account.report.line: l10n_hr.tax_report_line_III_15 [renamed from l10n_hr_euro module]
@@ -2718,77 +1965,19 @@
 DEL account.report.line: l10n_hr.account_tax_report_line_pretporez_koji_neplaceni_usluge_25 [renamed to l10n_hr_kuna module]
 DEL account.report.line: l10n_hr.account_tax_report_line_pretporez_koji_ukupno [renamed to l10n_hr_kuna module]
 DEL account.report.line: l10n_hr.account_tax_report_line_prodaja [renamed to l10n_hr_kuna module]
 DEL account.report.line: l10n_hr.account_tax_report_line_prodaja_dugotrajne [renamed to l10n_hr_kuna module]
 DEL account.report.line: l10n_hr.account_tax_report_line_prodaja_osobnih [renamed to l10n_hr_kuna module]
 DEL account.report.line: l10n_hr.account_tax_report_line_tuzemne [renamed to l10n_hr_kuna module]
 DEL account.report.line: l10n_hr.account_tax_report_line_uplaceno [renamed to l10n_hr_kuna module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_1 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_10 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_11 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_12 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_13 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_14 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_15 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_2 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_3 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_4 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_5 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_6 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_7 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_8 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_III_9 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_1 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_10 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_11 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_12 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_13 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_14 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_15 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_2 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_3 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_4 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_5 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_6 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_7 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_8 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_II_9 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_IV_1 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_IV_2 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_1 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_10 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_2 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_3 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_4 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_5 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_6 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_7 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_8 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_I_9 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_VI_1 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_VI_2 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_V_1 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_line_V_2 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_title_annual_deductible [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_title_calculed_vat [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_title_prev_calculation [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_title_total_dif [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_title_transactions0 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_title_transactions1 [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_title_vat_calculation [renamed to l10n_hr module]
-DEL account.report.line: l10n_hr_euro.tax_report_title_vat_liab [renamed to l10n_hr module]
 DEL account.tax.group: l10n_hr.tax_group_0
 DEL account.tax.group: l10n_hr.tax_group_10
 DEL account.tax.group: l10n_hr.tax_group_25
 DEL account.tax.group: l10n_hr.tax_group_30
 DEL account.tax.group: l10n_hr.tax_group_70
-DEL account.tax.group: l10n_hr_euro.tax_group_pdv_0
-DEL account.tax.group: l10n_hr_euro.tax_group_pdv_13
-DEL account.tax.group: l10n_hr_euro.tax_group_pdv_25
-DEL account.tax.group: l10n_hr_euro.tax_group_pdv_5
 DEL account.tax.template: l10n_hr.rrif_pdv_0
 DEL account.tax.template: l10n_hr.rrif_pdv_10
 DEL account.tax.template: l10n_hr.rrif_pdv_25
 DEL account.tax.template: l10n_hr.rrif_pdv_25usl
 DEL account.tax.template: l10n_hr.rrif_pdv_avans_0
 DEL account.tax.template: l10n_hr.rrif_pdv_avans_10
 DEL account.tax.template: l10n_hr.rrif_pdv_avans_25
@@ -2814,38 +2003,8 @@
 DEL account.tax.template: l10n_hr.rrif_pp_uvoz_samopdv_25
 DEL account.tax.template: l10n_hr.rrif_pp_uvoz_samopdv_25usl
 DEL account.tax.template: l10n_hr.rrif_ppdnp1_3070_1
 DEL account.tax.template: l10n_hr.rrif_ppdnp1_3070_1_r2
 DEL account.tax.template: l10n_hr.rrif_ppdnp1_7030_1
 DEL account.tax.template: l10n_hr.rrif_ppdnp1_7030_1_r2
 DEL account.tax.template: l10n_hr.rrif_ppr2_25
-DEL account.tax.template: l10n_hr_euro.VAT_P_G_IN_EU_13
-DEL account.tax.template: l10n_hr_euro.VAT_P_G_IN_EU_25
-DEL account.tax.template: l10n_hr_euro.VAT_P_G_IN_EU_5
-DEL account.tax.template: l10n_hr_euro.VAT_P_IN_ROC_13
-DEL account.tax.template: l10n_hr_euro.VAT_P_IN_ROC_25
-DEL account.tax.template: l10n_hr_euro.VAT_P_IN_ROC_5
-DEL account.tax.template: l10n_hr_euro.VAT_P_NOT_IN_EU_13
-DEL account.tax.template: l10n_hr_euro.VAT_P_NOT_IN_EU_25
-DEL account.tax.template: l10n_hr_euro.VAT_P_NOT_IN_EU_5
-DEL account.tax.template: l10n_hr_euro.VAT_P_O
-DEL account.tax.template: l10n_hr_euro.VAT_P_S_IN_EU_13
-DEL account.tax.template: l10n_hr_euro.VAT_P_S_IN_EU_25
-DEL account.tax.template: l10n_hr_euro.VAT_P_S_IN_EU_5
-DEL account.tax.template: l10n_hr_euro.VAT_P_install_assemb_goods_O
-DEL account.tax.template: l10n_hr_euro.VAT_P_reverse_charge
-DEL account.tax.template: l10n_hr_euro.VAT_S_EU_G
-DEL account.tax.template: l10n_hr_euro.VAT_S_EU_S
-DEL account.tax.template: l10n_hr_euro.VAT_S_EX_O
-DEL account.tax.template: l10n_hr_euro.VAT_S_IN_ROC_13
-DEL account.tax.template: l10n_hr_euro.VAT_S_IN_ROC_25
-DEL account.tax.template: l10n_hr_euro.VAT_S_IN_ROC_5
-DEL account.tax.template: l10n_hr_euro.VAT_S_TAX_PERSON_13%
-DEL account.tax.template: l10n_hr_euro.VAT_S_TAX_PERSON_25%
-DEL account.tax.template: l10n_hr_euro.VAT_S_TAX_PERSON_5%
-DEL account.tax.template: l10n_hr_euro.VAT_S_carried_other_state_O
-DEL account.tax.template: l10n_hr_euro.VAT_S_new_transport_other_state_O
-DEL account.tax.template: l10n_hr_euro.VAT_S_other_exempt_O
-DEL account.tax.template: l10n_hr_euro.VAT_S_person_not_in_ROC_O
-DEL account.tax.template: l10n_hr_euro.VAT_S_reverse_O
 NEW ir.ui.menu: l10n_hr.account_reports_hr_statements_menu [renamed from l10n_hr_euro module]
-DEL ir.ui.menu: l10n_hr_euro.account_reports_hr_statements_menu [renamed to l10n_hr module]
```

## odoo/addons/openupgrade_scripts/scripts/l10n_in/17.0.2.0/upgrade_analysis.txt

```diff
@@ -1,11 +1,14 @@
 ---Models in module 'l10n_in'---
 ---Fields in module 'l10n_in'---
 l10n_in      / account.journal          / l10n_in_gstin_partner_id (many2one): DEL relation: res.partner
 l10n_in      / account.tax.template     / l10n_in_reverse_charge (boolean): DEL
+l10n_in      / res.company              / l10n_in_upi_id (char)         : previously in module l10n_in_upi
+l10n_in      / res.partner              / l10n_in_pan (char)            : previously in module l10n_in_tcs_tds
+l10n_in      / res.users                / l10n_in_pan (char)            : previously in module l10n_in_tcs_tds
 ---XML records in module 'l10n_in'---
 DEL account.account.template: l10n_in.2012
 DEL account.account.template: l10n_in.p10031
 DEL account.account.template: l10n_in.p10040
 DEL account.account.template: l10n_in.p10041
 DEL account.account.template: l10n_in.p10051
 DEL account.account.template: l10n_in.p10052
@@ -71,16 +74,14 @@
 DEL account.account.template: l10n_in.p21182
 DEL account.account.template: l10n_in.p21183
 DEL account.account.template: l10n_in.p2121
 DEL account.account.template: l10n_in.p2122
 DEL account.account.template: l10n_in.p2123
 DEL account.account.template: l10n_in.p2131
 DEL account.account.template: l10n_in.p2132
-DEL account.account.template: l10n_in_tcs_tds.p11244
-DEL account.account.template: l10n_in_tcs_tds.p11245
 DEL account.chart.template: l10n_in.indian_chart_template_standard
 DEL account.fiscal.position.tax.template: l10n_in.account_fiscal_position_tax_in_purchase_12_exp
 DEL account.fiscal.position.tax.template: l10n_in.account_fiscal_position_tax_in_purchase_12_inter
 DEL account.fiscal.position.tax.template: l10n_in.account_fiscal_position_tax_in_purchase_12_intra_rc
 DEL account.fiscal.position.tax.template: l10n_in.account_fiscal_position_tax_in_purchase_12_rc_inter_rc
 DEL account.fiscal.position.tax.template: l10n_in.account_fiscal_position_tax_in_purchase_18_exp
 DEL account.fiscal.position.tax.template: l10n_in.account_fiscal_position_tax_in_purchase_18_inter
@@ -116,20 +117,16 @@
 DEL account.fiscal.position.tax.template: l10n_in.account_fiscal_position_tax_in_sale_5_inter
 DEL account.fiscal.position.template: l10n_in.fiscal_position_in_export
 DEL account.fiscal.position.template: l10n_in.fiscal_position_in_inter_state
 DEL account.fiscal.position.template: l10n_in.fiscal_position_in_reverse_charge_inter
 DEL account.fiscal.position.template: l10n_in.fiscal_position_in_reverse_charge_intra
 NEW account.report: l10n_in.tcs_report [renamed from l10n_in_tcs_tds module]
 NEW account.report: l10n_in.tds_report [renamed from l10n_in_tcs_tds module]
-DEL account.report: l10n_in_tcs_tds.tcs_report [renamed to l10n_in module]
-DEL account.report: l10n_in_tcs_tds.tds_report [renamed to l10n_in module]
 NEW account.report.column: l10n_in.tcs_report_balance [renamed from l10n_in_tcs_tds module]
 NEW account.report.column: l10n_in.tds_report_balance [renamed from l10n_in_tcs_tds module]
-DEL account.report.column: l10n_in_tcs_tds.tcs_report_balance [renamed to l10n_in module]
-DEL account.report.column: l10n_in_tcs_tds.tds_report_balance [renamed to l10n_in module]
 NEW account.report.expression: l10n_in.tcs_report_line_section_206c_1_alfhc_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tcs_report_line_section_206c_1_aofpnbtotl_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tcs_report_line_section_206c_1_mbcoloio_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tcs_report_line_section_206c_1_s_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tcs_report_line_section_206c_1_tl_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tcs_report_line_section_206c_1_tobaotuafl_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tcs_report_line_section_206c_1_touafl_tag [renamed from l10n_in_tcs_tds module]
@@ -167,59 +164,14 @@
 NEW account.report.expression: l10n_in.tds_report_line_section_194lbb_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tds_report_line_section_194lbc_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tds_report_line_section_194m_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tds_report_line_section_194n_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tds_report_line_section_194o_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tds_report_line_section_194q_tag [renamed from l10n_in_tcs_tds module]
 NEW account.report.expression: l10n_in.tds_report_line_section_195_tag [renamed from l10n_in_tcs_tds module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_alfhc_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_aofpnbtotl_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_mbcoloio_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_s_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_tl_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_tobaotuafl_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1_touafl_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_maq_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_pl_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_tp_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1f_mv_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1g_soaotpp_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1g_som_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tcs_report_line_section_206c_1h_sog_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_192_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_192a_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_193_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194a_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194b_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194bb_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194c_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194d_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194da_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194e_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194ee_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194f_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194g_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194h_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194i_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194ia_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194ib_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194ic_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194j_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194k_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194la_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194lb_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194lba_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194lbb_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194lbc_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194m_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194n_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194o_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_194q_tag [renamed to l10n_in module]
-DEL account.report.expression: l10n_in_tcs_tds.tds_report_line_section_195_tag [renamed to l10n_in module]
 NEW account.report.line: l10n_in.tcs_report_line_section_206c_1_alfhc [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tcs_report_line_section_206c_1_aofpnbtotl [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tcs_report_line_section_206c_1_mbcoloio [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tcs_report_line_section_206c_1_s [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tcs_report_line_section_206c_1_tl [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tcs_report_line_section_206c_1_tobaotuafl [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tcs_report_line_section_206c_1_touafl [renamed from l10n_in_tcs_tds module]
@@ -257,69 +209,22 @@
 NEW account.report.line: l10n_in.tds_report_line_section_194lbb [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tds_report_line_section_194lbc [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tds_report_line_section_194m [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tds_report_line_section_194n [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tds_report_line_section_194o [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tds_report_line_section_194q [renamed from l10n_in_tcs_tds module]
 NEW account.report.line: l10n_in.tds_report_line_section_195 [renamed from l10n_in_tcs_tds module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_alfhc [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_aofpnbtotl [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_mbcoloio [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_s [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_tl [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_tobaotuafl [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1_touafl [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_maq [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_pl [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1c_tp [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1f_mv [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1g_soaotpp [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1g_som [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tcs_report_line_section_206c_1h_sog [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_192 [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_192a [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_193 [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194 [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194a [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194b [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194bb [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194c [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194d [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194da [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194e [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194ee [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194f [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194g [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194h [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194i [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194ia [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194ib [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194ic [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194j [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194k [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194la [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194lb [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194lba [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194lbb [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194lbc [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194m [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194n [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194o [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_194q [renamed to l10n_in module]
-DEL account.report.line: l10n_in_tcs_tds.tds_report_line_section_195 [renamed to l10n_in module]
 DEL account.tax.group: l10n_in.cess_group (noupdate)
 DEL account.tax.group: l10n_in.cgst_group (noupdate)
 DEL account.tax.group: l10n_in.exempt_group (noupdate)
 DEL account.tax.group: l10n_in.gst_group (noupdate)
 DEL account.tax.group: l10n_in.igst_group (noupdate)
 DEL account.tax.group: l10n_in.nil_rated_group (noupdate)
 DEL account.tax.group: l10n_in.non_gst_supplies_group (noupdate)
 DEL account.tax.group: l10n_in.sgst_group (noupdate)
-DEL account.tax.group: l10n_in_tcs_tds.tcs_group (noupdate)
-DEL account.tax.group: l10n_in_tcs_tds.tds_group (noupdate)
 DEL account.tax.template: l10n_in.cess_21_4170_higer_purchase
 DEL account.tax.template: l10n_in.cess_21_4170_higer_purchase_rc
 DEL account.tax.template: l10n_in.cess_21_4170_higer_sale
 DEL account.tax.template: l10n_in.cess_5_plus_1591_purchase
 DEL account.tax.template: l10n_in.cess_5_plus_1591_purchase_rc
 DEL account.tax.template: l10n_in.cess_5_plus_1591_sale
 DEL account.tax.template: l10n_in.cess_purchase_1591
@@ -403,100 +308,10 @@
 DEL account.tax.template: l10n_in.sgst_sale_1_2
 DEL account.tax.template: l10n_in.sgst_sale_2
 DEL account.tax.template: l10n_in.sgst_sale_28
 DEL account.tax.template: l10n_in.sgst_sale_2_5
 DEL account.tax.template: l10n_in.sgst_sale_5
 DEL account.tax.template: l10n_in.sgst_sale_6
 DEL account.tax.template: l10n_in.sgst_sale_9
-DEL account.tax.template: l10n_in_tcs_tds.tcs_0_1_us_206c_1h_sog
-DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1_alfhc
-DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1_mbcoloio
-DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1_s
-DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1f_mv
-DEL account.tax.template: l10n_in_tcs_tds.tcs_1_us_206c_1h_sog
-DEL account.tax.template: l10n_in_tcs_tds.tcs_2_5_us_206c_1_aofpnbtotl
-DEL account.tax.template: l10n_in_tcs_tds.tcs_2_5_us_206c_1_tobamotuafl
-DEL account.tax.template: l10n_in_tcs_tds.tcs_2_5_us_206c_1_touafl
-DEL account.tax.template: l10n_in_tcs_tds.tcs_2_us_206c_1c_maq
-DEL account.tax.template: l10n_in_tcs_tds.tcs_2_us_206c_1c_pl
-DEL account.tax.template: l10n_in_tcs_tds.tcs_2_us_206c_1c_tp
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_alfhc
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_aofpnbtotl
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_mbcoloio
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_s
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_tl
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_tobamotuafl
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1_touafl
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1c_maq
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1c_pl
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1c_tp
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1f_mv
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1g_soaotpp
-DEL account.tax.template: l10n_in_tcs_tds.tcs_5_us_206c_1g_som
-DEL account.tax.template: l10n_in_tcs_tds.tds_01_us_194q
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_4_us_195
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_192a
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_193
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194a
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194d
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194ee
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194i
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194ic
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194j
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194k
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194la
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194lba
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194lbb
-DEL account.tax.template: l10n_in_tcs_tds.tds_10_us_194lbc
-DEL account.tax.template: l10n_in_tcs_tds.tds_15_6_us_195
-DEL account.tax.template: l10n_in_tcs_tds.tds_1_us_194c
-DEL account.tax.template: l10n_in_tcs_tds.tds_1_us_194ia
-DEL account.tax.template: l10n_in_tcs_tds.tds_1_us_194o
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_8_us_195
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_192a
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_193
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194a
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194c
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194d
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194da
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194e
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194ee
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194f
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194g
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194h
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194i
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194ia
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194ib
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194ic
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194j
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194k
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194la
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194lb
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194lba
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194lbb
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194m
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194n
-DEL account.tax.template: l10n_in_tcs_tds.tds_20_us_194o
-DEL account.tax.template: l10n_in_tcs_tds.tds_25_us_194lbc
-DEL account.tax.template: l10n_in_tcs_tds.tds_2_us_194c
-DEL account.tax.template: l10n_in_tcs_tds.tds_2_us_194i
-DEL account.tax.template: l10n_in_tcs_tds.tds_2_us_194j
-DEL account.tax.template: l10n_in_tcs_tds.tds_2_us_194n
-DEL account.tax.template: l10n_in_tcs_tds.tds_30_us_194b
-DEL account.tax.template: l10n_in_tcs_tds.tds_30_us_194bb
-DEL account.tax.template: l10n_in_tcs_tds.tds_30_us_194lbc
-DEL account.tax.template: l10n_in_tcs_tds.tds_31_2_us_195
-DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194d
-DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194da
-DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194g
-DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194h
-DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194ib
-DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194lb
-DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194m
-DEL account.tax.template: l10n_in_tcs_tds.tds_5_us_194n
-DEL ir.model.constraint: l10n_in.constraint_l10n_in_port_code_code_uniq
 NEW ir.ui.view: l10n_in.view_company_form
 DEL ir.ui.view: l10n_in.l10n_in_external_layout
-DEL ir.ui.view: l10n_in_tcs_tds.l10n_in_tcs_tds_view_partner_form
-DEL ir.ui.view: l10n_in_upi.view_company_form
+DEL ir.ui.view: l10n_in.report_invoice_with_payments
```

## odoo/addons/openupgrade_scripts/scripts/l10n_ke_edi_tremol/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,7 +1,8 @@
 ---Models in module 'l10n_ke_edi_tremol'---
 ---Fields in module 'l10n_ke_edi_tremol'---
 l10n_ke_edi_tremol / product.template         / l10n_ke_hsn_code (char)       : DEL
 l10n_ke_edi_tremol / product.template         / l10n_ke_hsn_name (char)       : DEL
 ---XML records in module 'l10n_ke_edi_tremol'---
+NEW ir.ui.view: l10n_ke_edi_tremol.account_move_send_form_inherit_l10n_ke_edi_tremol
 DEL ir.ui.view: l10n_ke_edi_tremol.l10n_ke_inherit_product_product_form_view
 DEL ir.ui.view: l10n_ke_edi_tremol.l10n_ke_inherit_product_template_form_view
```

## odoo/addons/openupgrade_scripts/scripts/l10n_latam_invoice_document/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,9 +1,9 @@
 ---Models in module 'l10n_latam_invoice_document'---
 ---Fields in module 'l10n_latam_invoice_document'---
 l10n_latam_invoice_document / l10n_latam.document.type / internal_type (selection)     : selection_keys is now '['all', 'credit_note', 'debit_note', 'invoice']' ('['credit_note', 'debit_note', 'invoice']')
 ---XML records in module 'l10n_latam_invoice_document'---
 NEW ir.model.access: l10n_latam_invoice_document.access_l10n_latam_document_type_invoice
 NEW ir.model.access: l10n_latam_invoice_document.access_l10n_latam_document_type_readonly
 DEL ir.model.access: l10n_latam_invoice_document.access_l10n_latam_document_type_all
-DEL ir.model.constraint: l10n_latam_account_sequence.constraint_account_move_unique_name
-DEL ir.model.constraint: l10n_latam_account_sequence.constraint_account_move_unique_name_latam
+NEW ir.model.constraint: l10n_latam_invoice_document.constraint_account_move_unique_name [renamed from l10n_latam_account_sequence module]
+NEW ir.model.constraint: l10n_latam_invoice_document.constraint_account_move_unique_name_latam [renamed from l10n_latam_account_sequence module]
```

## odoo/addons/openupgrade_scripts/scripts/l10n_lu/17.0.2.2/upgrade_analysis.txt

```diff
@@ -1,10 +1,46 @@
 ---Models in module 'l10n_lu'---
 ---Fields in module 'l10n_lu'---
 ---XML records in module 'l10n_lu'---
+NEW account.account.tag: l10n_lu.account_tag_appendix_188 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_190 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_239 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_244 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_247 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_250 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_253 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_260 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_269 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_283 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_285 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_289 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_293 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_301 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_305 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_307 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_310 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_316 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_324 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_326 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_327 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_328 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_330 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_331 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_332 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_336 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_337 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_343 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_345 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_347 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_349 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_351 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_353 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_355 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_358 (noupdate)
+NEW account.account.tag: l10n_lu.account_tag_appendix_361 (noupdate)
 DEL account.account.template: l10n_lu.lu_2011_account_101
 DEL account.account.template: l10n_lu.lu_2011_account_102
 DEL account.account.template: l10n_lu.lu_2011_account_103
 DEL account.account.template: l10n_lu.lu_2011_account_105
 DEL account.account.template: l10n_lu.lu_2011_account_10611
 DEL account.account.template: l10n_lu.lu_2011_account_10612
 DEL account.account.template: l10n_lu.lu_2011_account_10613
```

## odoo/addons/openupgrade_scripts/scripts/l10n_my/17.0.1.1/upgrade_analysis.txt

```diff
@@ -102,7 +102,8 @@
 NEW account.report.line: l10n_my.l10n_my_sst_taxable_5
 NEW account.report.line: l10n_my.l10n_my_sst_taxable_per_rate
 NEW account.report.line: l10n_my.l10n_my_sst_total_including_penalty
 DEL account.tax.group: l10n_my.tax_group_sst
 DEL account.tax.template: l10n_my.l10n_my_tax_sale_10
 DEL account.tax.template: l10n_my.l10n_my_tax_sale_5
 DEL account.tax.template: l10n_my.l10n_my_tax_sale_6
+DEL account.tax.template: l10n_my.l10n_my_tax_sale_8
```

## odoo/addons/openupgrade_scripts/scripts/l10n_pl/17.0.2.0/upgrade_analysis.txt

```diff
@@ -463,14 +463,15 @@
 DEL account.tax.template: l10n_pl.vz_kraj_usl_23
 DEL account.tax.template: l10n_pl.vz_kraj_zw
 DEL account.tax.template: l10n_pl.vz_nabu
 DEL account.tax.template: l10n_pl.vz_stal
 DEL account.tax.template: l10n_pl.vz_unia
 DEL account.tax.template: l10n_pl.vz_unia_triangular
 NEW ir.model.access: l10n_pl.access_l10n_pl_tax_office [renamed from l10n_pl_jpk module]
+NEW ir.model.constraint: l10n_pl.constraint_l10n_pl_l10n_pl_tax_office_code_company_uniq
 NEW ir.ui.view: l10n_pl.product_template_form
 NEW ir.ui.view: l10n_pl.res_config_settings_view_form
 NEW ir.ui.view: l10n_pl.res_partner_account_pl_form
 NEW ir.ui.view: l10n_pl.view_move_form_l10n_pl
 NEW l10n_pl.l10n_pl_tax_office: l10n_pl.pl_tax_office_0202
 NEW l10n_pl.l10n_pl_tax_office: l10n_pl.pl_tax_office_0203
 NEW l10n_pl.l10n_pl_tax_office: l10n_pl.pl_tax_office_0204
```

## odoo/addons/openupgrade_scripts/scripts/l10n_pt/17.0.1.0/upgrade_analysis.txt

```diff
@@ -380,15 +380,15 @@
 DEL account.account.template: l10n_pt.chart_89
 DEL account.chart.template: l10n_pt.pt_chart_template
 DEL account.fiscal.position.template: l10n_pt.fiscal_position_foreign_eu (noupdate)
 DEL account.fiscal.position.template: l10n_pt.fiscal_position_foreign_eu_private (noupdate)
 DEL account.fiscal.position.template: l10n_pt.fiscal_position_foreign_other (noupdate)
 DEL account.fiscal.position.template: l10n_pt.fiscal_position_national_customers (noupdate)
 NEW account.report: l10n_pt.tax_report_pt
-DEL account.report: l10n_pt.tax_report [renamed to l10n_dz module]
+DEL account.report: l10n_pt.tax_report [renamed to l10n_tn module]
 NEW account.report.expression: l10n_pt.trp_base_12_tag
 NEW account.report.expression: l10n_pt.trp_base_14_tag
 NEW account.report.expression: l10n_pt.trp_base_15_tag
 NEW account.report.expression: l10n_pt.trp_base_16_tag
 NEW account.report.expression: l10n_pt.trp_base_18_tag
 NEW account.report.expression: l10n_pt.trp_base_1_tag
 NEW account.report.expression: l10n_pt.trp_base_3_tag
```

## odoo/addons/openupgrade_scripts/scripts/l10n_ro_edi/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,5 +1,5 @@
 ---Models in module 'l10n_ro_edi'---
 new model account.edi.xml.ubl_ro [abstract]
 ---Fields in module 'l10n_ro_edi'---
-l10n_ro_edi  / res.partner              / ubl_cii_format (False)        : NEW selection_keys: ['ciusro', 'facturx', 'nlcius', 'oioubl_201', 'pint_jp', 'ubl_a_nz', 'ubl_bis3', 'ubl_sg', 'xrechnung'], mode: modify
+l10n_ro_edi  / res.partner              / ubl_cii_format (False)        : NEW selection_keys: ['ciusro', 'facturx', 'nlcius', 'oioubl_201', 'pint_jp', 'pint_my', 'ubl_a_nz', 'ubl_bis3', 'ubl_sg', 'xrechnung'], mode: modify
 ---XML records in module 'l10n_ro_edi'---
```

## odoo/addons/openupgrade_scripts/scripts/l10n_tn/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,11 +1,11 @@
 ---Models in module 'l10n_tn'---
 ---Fields in module 'l10n_tn'---
 ---XML records in module 'l10n_tn'---
-NEW account.report: l10n_tn.tax_report [renamed from l10n_hr_euro module]
+NEW account.report: l10n_tn.tax_report [renamed from l10n_pt module]
 NEW account.report.column: l10n_tn.l10n_tn_tr_column_base_amount
 NEW account.report.column: l10n_tn.l10n_tn_tr_column_deductible_vat
 NEW account.report.column: l10n_tn.l10n_tn_tr_column_vat_due
 NEW account.report.expression: l10n_tn.l10n_tn_tr_VAT_conclusion_after_carryover_deductible_vat_tag
 NEW account.report.expression: l10n_tn.l10n_tn_tr_VAT_conclusion_after_carryover_vat_due_tag
 NEW account.report.expression: l10n_tn.l10n_tn_tr_VAT_conclusion_carryover_deductible_vat_tag
 NEW account.report.expression: l10n_tn.l10n_tn_tr_VAT_conclusion_deductible_vat_tag
```

## odoo/addons/openupgrade_scripts/scripts/link_tracker/17.0.1.1/upgrade_analysis.txt

```diff
@@ -1,4 +1,4 @@
 ---Models in module 'link_tracker'---
 ---Fields in module 'link_tracker'---
 ---XML records in module 'link_tracker'---
-DEL ir.model.constraint: link_tracker.constraint_link_tracker_code_code
+---nothing has changed in this module--
```

## odoo/addons/openupgrade_scripts/scripts/loyalty/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,17 +1,11 @@
 ---Models in module 'loyalty'---
 ---Fields in module 'loyalty'---
 loyalty      / loyalty.card             / message_main_attachment_id (many2one): DEL relation: ir.attachment
 loyalty      / loyalty.card             / rating_ids (one2many)         : NEW relation: rating.rating
 loyalty      / loyalty.program          / date_from (date)              : NEW
 loyalty      / loyalty.program          / pricelist_ids (many2many)     : NEW relation: product.pricelist
 ---XML records in module 'loyalty'---
-DEL ir.model.constraint: loyalty.constraint_loyalty_card_card_code_unique
-DEL ir.model.constraint: loyalty.constraint_loyalty_program_check_max_usage
-DEL ir.model.constraint: loyalty.constraint_loyalty_reward_discount_positive
-DEL ir.model.constraint: loyalty.constraint_loyalty_reward_product_qty_positive
-DEL ir.model.constraint: loyalty.constraint_loyalty_reward_required_points_positive
-DEL ir.model.constraint: loyalty.constraint_loyalty_rule_reward_point_amount_positive
 NEW ir.ui.view: loyalty.res_partner_form
 NEW loyalty.program: loyalty.gift_card_program
 NEW loyalty.reward: loyalty.gift_card_program_reward
 NEW loyalty.rule: loyalty.gift_card_program_rule
```

## odoo/addons/openupgrade_scripts/scripts/lunch/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,9 +1,7 @@
 ---Models in module 'lunch'---
 ---Fields in module 'lunch'---
 lunch        / lunch.order              / name (char)                   : not stored anymore
 lunch        / lunch.supplier           / activity_user_id (many2one)   : not related anymore
 lunch        / lunch.supplier           / activity_user_id (many2one)   : now a function
 lunch        / lunch.supplier           / message_main_attachment_id (many2one): DEL relation: ir.attachment
 ---XML records in module 'lunch'---
-DEL ir.model.constraint: lunch.constraint_lunch_alert_notification_time_range
-DEL ir.model.constraint: lunch.constraint_lunch_supplier_automatic_email_time_range
```

## odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/noupdate_changes.xml

```diff
@@ -1,9 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <record id="mail_activity_data_todo" model="mail.activity.type">
     <field name="name">To-Do</field>
   </record>
+  <record id="mail_template_employee_rule" model="ir.rule">
+    <field name="domain_force">['|', ('create_uid', '=', user.id), ('user_id', '=', user.id)]</field>
+    <field name="name">Employees can only modify templates they have created or been assigned</field>
+  </record>
   <record id="module_install_notification" model="mail.message">
     <field name="model">discuss.channel</field>
   </record>
 </odoo>
```

## odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/upgrade_analysis.txt

```diff
@@ -131,15 +131,15 @@
 mail         / mail.gateway.allowed     / email (char)                  : now required
 mail         / mail.guest               / channel_ids (many2many)       : relation is now 'discuss.channel' ('mail.channel') [nothing to do]
 mail         / mail.guest               / channel_ids (many2many)       : table is now 'discuss_channel_member' ('mail_channel_member')
 mail         / mail.link.preview        / og_site_name (char)           : NEW
 mail         / mail.mail                / failure_type (selection)      : selection_keys is now '['mail_bl', 'mail_dup', 'mail_email_invalid', 'mail_email_missing', 'mail_from_invalid', 'mail_from_missing', 'mail_optout', 'mail_smtp', 'unknown']' ('['mail_bl', 'mail_dup', 'mail_email_invalid', 'mail_email_missing', 'mail_optout', 'mail_smtp', 'unknown']')
 mail         / mail.mail                / to_delete (boolean)           : DEL
 mail         / mail.message             / canned_response_ids (one2many): DEL relation: mail.shortcode
-mail         / mail.message             / message_type (selection)      : selection_keys is now '['auto_comment', 'comment', 'email', 'email_outgoing', 'notification', 'user_notification']' ('['comment', 'email', 'notification', 'user_notification']')
+mail         / mail.message             / message_type (selection)      : selection_keys is now '['auto_comment', 'comment', 'email', 'email_outgoing', 'notification', 'user_notification']' ('['auto_comment', 'comment', 'email', 'notification', 'user_notification']')
 mail         / mail.message             / pinned_at (datetime)          : NEW
 mail         / mail.message             / record_alias_domain_id (many2one): NEW relation: mail.alias.domain
 mail         / mail.message             / record_company_id (many2one)  : NEW relation: res.company
 mail         / mail.message.translation / body (html)                   : NEW required
 mail         / mail.message.translation / message_id (many2one)         : NEW relation: mail.message, required
 mail         / mail.message.translation / source_lang (char)            : NEW required
 mail         / mail.message.translation / target_lang (char)            : NEW required
@@ -252,29 +252,30 @@
 DEL ir.model.access: mail.access_mail_message_subtype_all
 DEL ir.model.access: mail.access_mail_tracking_value_all
 DEL ir.model.access: mail.access_mail_tracking_value_portal
 DEL ir.model.access: mail.access_mail_tracking_value_user
 DEL ir.model.access: mail.access_res_users_settings_all [renamed to base module]
 DEL ir.model.access: mail.access_res_users_settings_user [renamed to base module]
 DEL ir.model.access: mail.access_res_users_settings_volumes_all
-DEL ir.model.constraint: mail.constraint_bus_presence_partner_or_guest_exists
-DEL ir.model.constraint: mail.constraint_mail_activity_check_res_id_is_set
+NEW ir.model.constraint: mail.constraint_discuss_channel_channel_type_not_null
+NEW ir.model.constraint: mail.constraint_discuss_channel_group_public_id_check
+NEW ir.model.constraint: mail.constraint_discuss_channel_member_partner_or_guest_exists
+NEW ir.model.constraint: mail.constraint_discuss_channel_rtc_session_channel_member_unique
+NEW ir.model.constraint: mail.constraint_discuss_channel_uuid_unique
+NEW ir.model.constraint: mail.constraint_discuss_gif_favorite_user_gif_favorite
+NEW ir.model.constraint: mail.constraint_mail_alias_domain_bounce_email_uniques
+NEW ir.model.constraint: mail.constraint_mail_alias_domain_catchall_email_uniques
+NEW ir.model.constraint: mail.constraint_mail_partner_device_endpoint_unique
 DEL ir.model.constraint: mail.constraint_mail_alias_alias_unique
-DEL ir.model.constraint: mail.constraint_mail_blacklist_unique_email
 DEL ir.model.constraint: mail.constraint_mail_channel_channel_type_not_null
 DEL ir.model.constraint: mail.constraint_mail_channel_group_public_id_check
 DEL ir.model.constraint: mail.constraint_mail_channel_member_partner_or_guest_exists
 DEL ir.model.constraint: mail.constraint_mail_channel_rtc_session_channel_member_unique
 DEL ir.model.constraint: mail.constraint_mail_channel_uuid_unique
-DEL ir.model.constraint: mail.constraint_mail_followers_mail_followers_res_partner_res_model_id_uniq
-DEL ir.model.constraint: mail.constraint_mail_message_reaction_partner_or_guest_exists
-DEL ir.model.constraint: mail.constraint_mail_notification_notification_partner_required
-DEL ir.model.constraint: mail.constraint_res_users_notification_type
 DEL ir.model.constraint: mail.constraint_res_users_settings_unique_user_id [renamed to base module]
-DEL ir.model.constraint: mail.constraint_res_users_settings_volumes_partner_or_guest_exists
 NEW ir.rule: mail.discuss_gif_favorite_admin_rule (noupdate)
 NEW ir.rule: mail.discuss_gif_favorite_user_rule (noupdate)
 NEW ir.rule: mail.ir_rule_discuss_channel_all (noupdate)
 NEW ir.rule: mail.ir_rule_discuss_channel_group_system (noupdate)
 NEW ir.rule: mail.ir_rule_discuss_channel_member_create_is_group_matching_all (noupdate)
 NEW ir.rule: mail.ir_rule_discuss_channel_member_create_is_group_matching_group_user (noupdate)
 NEW ir.rule: mail.ir_rule_discuss_channel_member_create_is_member_group_user (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/mail_group/17.0.1.1/upgrade_analysis.txt

```diff
@@ -3,9 +3,7 @@
 ---XML records in module 'mail_group'---
 NEW ir.model.access: mail_group.access_mail_group_all_portal
 NEW ir.model.access: mail_group.access_mail_group_all_public
 NEW ir.model.access: mail_group.access_mail_group_message_all_portal
 NEW ir.model.access: mail_group.access_mail_group_message_all_public
 DEL ir.model.access: mail_group.access_mail_group_all
 DEL ir.model.access: mail_group.access_mail_group_message_all
-DEL ir.model.constraint: mail_group.constraint_mail_group_member_unique_partner
-DEL ir.model.constraint: mail_group.constraint_mail_group_moderation_mail_group_email_uniq
```

## odoo/addons/openupgrade_scripts/scripts/mail_plugin/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,5 +1,4 @@
 ---Models in module 'mail_plugin'---
 ---Fields in module 'mail_plugin'---
 ---XML records in module 'mail_plugin'---
-DEL ir.model.constraint: mail_plugin.constraint_res_partner_iap_unique_partner_id
 NEW ir.ui.view: mail_plugin.app_error
```

## odoo/addons/openupgrade_scripts/scripts/maintenance/17.0.1.0/upgrade_analysis.txt

```diff
@@ -21,12 +21,11 @@
 maintenance  / maintenance.request      / repeat_interval (integer)     : NEW hasdefault: default
 maintenance  / maintenance.request      / repeat_type (selection)       : NEW selection_keys: ['forever', 'until'], hasdefault: default
 maintenance  / maintenance.request      / repeat_unit (selection)       : NEW selection_keys: ['day', 'month', 'week', 'year'], hasdefault: default
 maintenance  / maintenance.request      / repeat_until (date)           : NEW
 ---XML records in module 'maintenance'---
 NEW ir.actions.act_window: maintenance.action_maintenance_configuration
 DEL ir.cron: maintenance.maintenance_requests_cron
-DEL ir.model.constraint: maintenance.constraint_maintenance_equipment_serial_no
 NEW ir.ui.menu: maintenance.menu_maintenance_config
 NEW ir.ui.view: maintenance.maintenance_request_view_activity
 NEW ir.ui.view: maintenance.res_config_settings_view_form
 DEL mail.alias: maintenance.mail_alias_equipment (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/mass_mailing/17.0.2.7/upgrade_analysis.txt

```diff
@@ -47,17 +47,16 @@
 mass_mailing / utm.campaign             / replied_ratio (integer)       : type is now 'float' ('integer')
 ---XML records in module 'mass_mailing'---
 NEW ir.actions.act_window: mass_mailing.mailing_subscription_action_report_optout
 NEW ir.actions.act_window: mass_mailing.mailing_subscription_optout_action
 NEW ir.model.access: mass_mailing.access_mailing_subscription_mm_user
 NEW ir.model.access: mass_mailing.access_mailing_subscription_optout_mm_user
 DEL ir.model.access: mass_mailing.access_mailing_contact_subscription_mm_user
+NEW ir.model.constraint: mass_mailing.constraint_mailing_subscription_unique_contact_list
 DEL ir.model.constraint: mass_mailing.constraint_mailing_contact_list_rel_unique_contact_list
-DEL ir.model.constraint: mass_mailing.constraint_mailing_mailing_percentage_valid
-DEL ir.model.constraint: mass_mailing.constraint_mailing_trace_check_res_id_is_set
 NEW ir.ui.menu: mass_mailing.mailing_menu_report_mailing
 NEW ir.ui.menu: mass_mailing.mailing_menu_report_subscribe_reason
 NEW ir.ui.menu: mass_mailing.mailing_subscription_optout_menu
 NEW ir.ui.view: mass_mailing.mail_blacklist_view_form
 NEW ir.ui.view: mass_mailing.mail_blacklist_view_search
 NEW ir.ui.view: mass_mailing.mail_blacklist_view_tree
 NEW ir.ui.view: mass_mailing.mailing_subscription_optout_view_form
```

## odoo/addons/openupgrade_scripts/scripts/membership/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,7 +1,5 @@
 ---Models in module 'membership'---
 ---Fields in module 'membership'---
 ---XML records in module 'membership'---
 NEW ir.model.access: membership.access_membership_membership_line_employee
 DEL ir.model.access: membership.access_membership_membership_line
-DEL ir.model.constraint: membership.constraint_product_template_membership_date_greater
-DEL ir.ui.menu: association.menu_event_config
```

## odoo/addons/openupgrade_scripts/scripts/microsoft_calendar/17.0.1.0/upgrade_analysis.txt

```diff
@@ -9,10 +9,11 @@
 microsoft_calendar / res.users                / microsoft_calendar_sync_token (char): not stored anymore
 microsoft_calendar / res.users                / microsoft_calendar_sync_token (char): now related
 microsoft_calendar / res.users                / microsoft_synchronization_stopped (boolean): not stored anymore
 microsoft_calendar / res.users                / microsoft_synchronization_stopped (boolean): now related
 ---XML records in module 'microsoft_calendar'---
 NEW ir.model.access: microsoft_calendar.access_microsoft_calendar_credentials
 NEW ir.model.access: microsoft_calendar.microsoft_calendar_manager
+NEW ir.model.constraint: microsoft_calendar.constraint_res_users_microsoft_token_uniq
 NEW ir.rule: microsoft_calendar.microsoft_calendar_not_own_token_rule (noupdate)
 NEW ir.rule: microsoft_calendar.microsoft_calendar_own_token_rule (noupdate)
 NEW ir.rule: microsoft_calendar.microsoft_calendar_token_system_access (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/mrp/17.0.2.0/upgrade_analysis.txt

```diff
@@ -50,21 +50,15 @@
 NEW ir.actions.client: mrp.action_mrp_display
 NEW ir.actions.client: mrp.action_mrp_display_fullscreen
 NEW ir.actions.client: mrp.action_report_mo_overview
 NEW ir.actions.report: mrp.action_report_mrp_mo_overview
 NEW ir.actions.server: mrp.action_plan_with_components_availability
 DEL ir.model.access: mrp.access_mrp_immediate_production
 DEL ir.model.access: mrp.access_mrp_immediate_production_line
-DEL ir.model.constraint: mrp.constraint_mrp_bom_line_bom_qty_zero
-DEL ir.model.constraint: mrp.constraint_mrp_bom_qty_positive
-DEL ir.model.constraint: mrp.constraint_mrp_production_name_uniq
-DEL ir.model.constraint: mrp.constraint_mrp_production_qty_positive
-DEL ir.model.constraint: mrp.constraint_mrp_workcenter_capacity_positive_capacity
-DEL ir.model.constraint: mrp.constraint_mrp_workcenter_capacity_unique_product
-DEL ir.model.constraint: mrp.constraint_mrp_workcenter_tag_tag_name_unique
+NEW ir.model.constraint: mrp.constraint_mrp_unbuild_qty_positive
 NEW ir.ui.menu: mrp.mrp_operation_picking
 DEL ir.ui.menu: mrp.menu_mrp_production_report
 NEW ir.ui.view: mrp.mo_overview_byproducts
 NEW ir.ui.view: mrp.mo_overview_components
 NEW ir.ui.view: mrp.mo_overview_content
 NEW ir.ui.view: mrp.mo_overview_line
 NEW ir.ui.view: mrp.mo_overview_operations
```

## odoo/addons/openupgrade_scripts/scripts/onboarding/17.0.1.2/upgrade_analysis.txt

```diff
@@ -15,11 +15,10 @@
 onboarding   / onboarding.onboarding.step / step_image_filename (char)    : NEW
 onboarding   / onboarding.progress      / progress_step_ids (one2many)  : table is now 'onboarding_progress_onboarding_progress_step_rel' ('False')
 onboarding   / onboarding.progress      / progress_step_ids (one2many)  : type is now 'many2many' ('one2many')
 onboarding   / onboarding.progress.step / company_id (many2one)         : NEW relation: res.company
 onboarding   / onboarding.progress.step / progress_id (many2one)        : DEL relation: onboarding.progress, required
 onboarding   / onboarding.progress.step / progress_ids (many2many)      : NEW relation: onboarding.progress
 ---XML records in module 'onboarding'---
-DEL ir.model.constraint: onboarding.constraint_onboarding_onboarding_route_name_uniq
 DEL ir.model.constraint: onboarding.constraint_onboarding_progress_onboarding_company_uniq
 DEL ir.model.constraint: onboarding.constraint_onboarding_progress_step_progress_step_uniq
 NEW ir.ui.view: onboarding.onboarding_step
```

## odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/noupdate_changes.xml

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <record id="payment_provider_adyen" model="payment.provider">
-    <field name="payment_method_ids" eval="[Command.set([                          ref('payment.payment_method_ach_direct_debit'),                          ref('payment.payment_method_affirm'),                          ref('payment.payment_method_afterpay'),                          ref('payment.payment_method_alipay'),                          ref('payment.payment_method_alipay_hk'),                          ref('payment.payment_method_alma'),                          ref('payment.payment_method_amazon_pay'),                          ref('payment.payment_method_bacs_direct_debit'),                          ref('payment.payment_method_bancontact'),                          ref('payment.payment_method_benefit'),                          ref('payment.payment_method_bizum'),                          ref('payment.payment_method_blik'),                          ref('payment.payment_method_card'),                          ref('payment.payment_method_cash_app_pay'),                          ref('payment.payment_method_clearpay'),                          ref('payment.payment_method_dana'),                          ref('payment.payment_method_duitnow'),                          ref('payment.payment_method_elo'),                          ref('payment.payment_method_eps'),                          ref('payment.payment_method_fpx'),                          ref('payment.payment_method_gcash'),                          ref('payment.payment_method_giropay'),                          ref('payment.payment_method_gopay'),                          ref('payment.payment_method_hipercard'),                          ref('payment.payment_method_ideal'),                          ref('payment.payment_method_kakaopay'),                          ref('payment.payment_method_klarna'),                          ref('payment.payment_method_klarna_paynow'),                          ref('payment.payment_method_klarna_pay_over_time'),                          ref('payment.payment_method_knet'),                          ref('payment.payment_method_mbway'),                          ref('payment.payment_method_mobile_pay'),                          ref('payment.payment_method_momo'),                          ref('payment.payment_method_multibanco'),                          ref('payment.payment_method_napas_card'),                          ref('payment.payment_method_online_banking_czech_republic'),                          ref('payment.payment_method_online_banking_india'),                          ref('payment.payment_method_online_banking_slovakia'),                          ref('payment.payment_method_online_banking_thailand'),                          ref('payment.payment_method_open_banking'),                          ref('payment.payment_method_p24'),                          ref('payment.payment_method_paybright'),                          ref('payment.payment_method_paysafecard'),                          ref('payment.payment_method_paynow'),                          ref('payment.payment_method_paypal'),                          ref('payment.payment_method_paytm'),                          ref('payment.payment_method_paytrail'),                          ref('payment.payment_method_pix'),                          ref('payment.payment_method_promptpay'),                          ref('payment.payment_method_ratepay'),                          ref('payment.payment_method_samsung_pay'),                          ref('payment.payment_method_sepa_direct_debit'),                          ref('payment.payment_method_sofort'),                          ref('payment.payment_method_swish'),                          ref('payment.payment_method_touch_n_go'),                          ref('payment.payment_method_trustly'),                          ref('payment.payment_method_twint'),                          ref('payment.payment_method_upi'),                          ref('payment.payment_method_vipps'),                          ref('payment.payment_method_wallets_india'),                          ref('payment.payment_method_walley'),                          ref('payment.payment_method_wechat_pay'),                          ref('payment.payment_method_zip'),                      ])]"/>
+    <field name="payment_method_ids" eval="[Command.set([                          ref('payment.payment_method_ach_direct_debit'),                          ref('payment.payment_method_affirm'),                          ref('payment.payment_method_afterpay'),                          ref('payment.payment_method_alipay'),                          ref('payment.payment_method_alipay_hk'),                          ref('payment.payment_method_alma'),                          ref('payment.payment_method_bacs_direct_debit'),                          ref('payment.payment_method_bancontact'),                          ref('payment.payment_method_benefit'),                          ref('payment.payment_method_bizum'),                          ref('payment.payment_method_blik'),                          ref('payment.payment_method_card'),                          ref('payment.payment_method_cash_app_pay'),                          ref('payment.payment_method_clearpay'),                          ref('payment.payment_method_dana'),                          ref('payment.payment_method_duitnow'),                          ref('payment.payment_method_elo'),                          ref('payment.payment_method_eps'),                          ref('payment.payment_method_fpx'),                          ref('payment.payment_method_gcash'),                          ref('payment.payment_method_giropay'),                          ref('payment.payment_method_gopay'),                          ref('payment.payment_method_hipercard'),                          ref('payment.payment_method_ideal'),                          ref('payment.payment_method_kakaopay'),                          ref('payment.payment_method_klarna'),                          ref('payment.payment_method_klarna_paynow'),                          ref('payment.payment_method_klarna_pay_over_time'),                          ref('payment.payment_method_knet'),                          ref('payment.payment_method_mbway'),                          ref('payment.payment_method_mobile_pay'),                          ref('payment.payment_method_momo'),                          ref('payment.payment_method_multibanco'),                          ref('payment.payment_method_napas_card'),                          ref('payment.payment_method_online_banking_czech_republic'),                          ref('payment.payment_method_online_banking_india'),                          ref('payment.payment_method_online_banking_slovakia'),                          ref('payment.payment_method_online_banking_thailand'),                          ref('payment.payment_method_open_banking'),                          ref('payment.payment_method_p24'),                          ref('payment.payment_method_paybright'),                          ref('payment.payment_method_paysafecard'),                          ref('payment.payment_method_paynow'),                          ref('payment.payment_method_paypal'),                          ref('payment.payment_method_paytm'),                          ref('payment.payment_method_paytrail'),                          ref('payment.payment_method_pix'),                          ref('payment.payment_method_promptpay'),                          ref('payment.payment_method_ratepay'),                          ref('payment.payment_method_samsung_pay'),                          ref('payment.payment_method_sepa_direct_debit'),                          ref('payment.payment_method_sofort'),                          ref('payment.payment_method_swish'),                          ref('payment.payment_method_touch_n_go'),                          ref('payment.payment_method_trustly'),                          ref('payment.payment_method_twint'),                          ref('payment.payment_method_upi'),                          ref('payment.payment_method_vipps'),                          ref('payment.payment_method_wallets_india'),                          ref('payment.payment_method_walley'),                          ref('payment.payment_method_wechat_pay'),                          ref('payment.payment_method_zip'),                      ])]"/>
   </record>
   <record id="payment_provider_aps" model="payment.provider">
     <field name="payment_method_ids" eval="[Command.set([                          ref('payment.payment_method_card'),                          ref('payment.payment_method_mada'),                          ref('payment.payment_method_knet'),                          ref('payment.payment_method_meeza'),                          ref('payment.payment_method_naps'),                          ref('payment.payment_method_omannet'),                          ref('payment.payment_method_benefit'),                      ])]"/>
   </record>
   <record id="payment_provider_asiapay" model="payment.provider">
     <field name="payment_method_ids" eval="[Command.set([                          ref('payment.payment_method_card'),                          ref('payment.payment_method_alipay'),                          ref('payment.payment_method_wechat_pay'),                          ref('payment.payment_method_poli'),                          ref('payment.payment_method_afterpay'),                          ref('payment.payment_method_clearpay'),                          ref('payment.payment_method_humm'),                          ref('payment.payment_method_zip'),                          ref('payment.payment_method_paypal'),                          ref('payment.payment_method_atome'),                          ref('payment.payment_method_pace'),                          ref('payment.payment_method_shopback'),                          ref('payment.payment_method_grabpay'),                          ref('payment.payment_method_samsung_pay'),                          ref('payment.payment_method_hoolah'),                          ref('payment.payment_method_boost'),                          ref('payment.payment_method_duitnow'),                          ref('payment.payment_method_touch_n_go'),                          ref('payment.payment_method_bancnet'),                          ref('payment.payment_method_gcash'),                          ref('payment.payment_method_paynow'),                          ref('payment.payment_method_linepay'),                          ref('payment.payment_method_bangkok_bank'),                          ref('payment.payment_method_krungthai_bank'),                          ref('payment.payment_method_uob'),                          ref('payment.payment_method_scb'),                          ref('payment.payment_method_bank_of_ayudhya'),                          ref('payment.payment_method_kasikorn_bank'),                          ref('payment.payment_method_rabbit_line_pay'),                          ref('payment.payment_method_truemoney'),                          ref('payment.payment_method_fpx'),                          ref('payment.payment_method_fps'),                          ref('payment.payment_method_hd'),                          ref('payment.payment_method_maybank'),                          ref('payment.payment_method_pay_id'),                          ref('payment.payment_method_promptpay'),                          ref('payment.payment_method_techcom'),                          ref('payment.payment_method_tienphong'),                          ref('payment.payment_method_ttb'),                          ref('payment.payment_method_upi'),                          ref('payment.payment_method_vietcom'),                          ref('payment.payment_method_tendopay'),                          ref('payment.payment_method_alipay_hk'),                          ref('payment.payment_method_bharatqr'),                          ref('payment.payment_method_momo'),                          ref('payment.payment_method_octopus'),                          ref('payment.payment_method_maya'),                          ref('payment.payment_method_uatp'),                          ref('payment.payment_method_tenpay'),                          ref('payment.payment_method_enets'),                          ref('payment.payment_method_jkopay'),                          ref('payment.payment_method_payme'),                          ref('payment.payment_method_tmb'),                      ])]"/>
   </record>
@@ -36,15 +36,15 @@
   <record id="payment_provider_sepa_direct_debit" model="payment.provider">
     <field name="payment_method_ids" eval="[Command.set([                      ref('payment.payment_method_sepa_direct_debit'),                  ])]"/>
   </record>
   <record id="payment_provider_sips" model="payment.provider">
     <field name="payment_method_ids" eval="[Command.set([                          ref('payment.payment_method_card'),                          ref('payment.payment_method_ideal'),                          ref('payment.payment_method_sofort'),                          ref('payment.payment_method_giropay'),                          ref('payment.payment_method_kbc_cbc'),                          ref('payment.payment_method_paypal'),                          ref('payment.payment_method_samsung_pay'),                          ref('payment.payment_method_bancontact'),                          ref('payment.payment_method_lyfpay'),                          ref('payment.payment_method_lydia'),                          ref('payment.payment_method_floa_bank'),                          ref('payment.payment_method_cofidis'),                          ref('payment.payment_method_frafinance'),                      ])]"/>
   </record>
   <record id="payment_provider_stripe" model="payment.provider">
-    <field name="payment_method_ids" eval="[Command.set([                          ref('payment.payment_method_ach_direct_debit'),                          ref('payment.payment_method_acss_debit'),                          ref('payment.payment_method_affirm'),                          ref('payment.payment_method_afterpay'),                          ref('payment.payment_method_alipay'),                          ref('payment.payment_method_bacs_direct_debit'),                          ref('payment.payment_method_bancontact'),                          ref('payment.payment_method_becs_direct_debit'),                          ref('payment.payment_method_blik'),                          ref('payment.payment_method_boleto'),                          ref('payment.payment_method_card'),                          ref('payment.payment_method_cash_app_pay'),                          ref('payment.payment_method_clearpay'),                          ref('payment.payment_method_eps'),                          ref('payment.payment_method_fpx'),                          ref('payment.payment_method_giropay'),                          ref('payment.payment_method_grabpay'),                          ref('payment.payment_method_ideal'),                          ref('payment.payment_method_klarna'),                          ref('payment.payment_method_mobile_pay'),                          ref('payment.payment_method_multibanco'),                          ref('payment.payment_method_p24'),                          ref('payment.payment_method_paynow'),                          ref('payment.payment_method_paypal'),                          ref('payment.payment_method_pix'),                          ref('payment.payment_method_promptpay'),                          ref('payment.payment_method_revolut_pay'),                          ref('payment.payment_method_sepa_direct_debit'),                          ref('payment.payment_method_sofort'),                          ref('payment.payment_method_upi'),                          ref('payment.payment_method_wechat_pay'),                          ref('payment.payment_method_zip'),                      ])]"/>
+    <field name="payment_method_ids" eval="[Command.set([                          ref('payment.payment_method_ach_direct_debit'),                          ref('payment.payment_method_acss_debit'),                          ref('payment.payment_method_affirm'),                          ref('payment.payment_method_afterpay'),                          ref('payment.payment_method_alipay'),                          ref('payment.payment_method_bacs_direct_debit'),                          ref('payment.payment_method_bancontact'),                          ref('payment.payment_method_becs_direct_debit'),                          ref('payment.payment_method_boleto'),                          ref('payment.payment_method_card'),                          ref('payment.payment_method_cash_app_pay'),                          ref('payment.payment_method_clearpay'),                          ref('payment.payment_method_eps'),                          ref('payment.payment_method_fpx'),                          ref('payment.payment_method_giropay'),                          ref('payment.payment_method_grabpay'),                          ref('payment.payment_method_ideal'),                          ref('payment.payment_method_klarna'),                          ref('payment.payment_method_mobile_pay'),                          ref('payment.payment_method_multibanco'),                          ref('payment.payment_method_p24'),                          ref('payment.payment_method_paynow'),                          ref('payment.payment_method_paypal'),                          ref('payment.payment_method_pix'),                          ref('payment.payment_method_promptpay'),                          ref('payment.payment_method_revolut_pay'),                          ref('payment.payment_method_sepa_direct_debit'),                          ref('payment.payment_method_sofort'),                          ref('payment.payment_method_upi'),                          ref('payment.payment_method_wechat_pay'),                          ref('payment.payment_method_zip'),                      ])]"/>
   </record>
   <record id="payment_token_company_rule" model="ir.rule">
     <field name="domain_force">[('company_id', 'parent_of', company_ids)]</field>
   </record>
   <record id="payment_token_user_rule" model="ir.rule">
     <field name="domain_force">[('partner_id', '=', user.partner_id.id)]</field>
     <field name="groups" eval="[(4, ref('base.group_user')),                                     (4, ref('base.group_portal')),                                     (4, ref('base.group_public'))]"/>
```

## odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/upgrade_analysis.txt

```diff
@@ -50,15 +50,14 @@
 NEW ir.model.access: payment.payment_token_public
 DEL ir.model.access: payment.payment_icon_all
 DEL ir.model.access: payment.payment_icon_system
 DEL ir.model.access: payment.payment_token_all
 DEL ir.model.access: payment.payment_token_user
 DEL ir.model.access: payment.payment_transaction_all
 DEL ir.model.access: payment.payment_transaction_user [renamed to account_payment module]
-DEL ir.model.constraint: payment.constraint_payment_transaction_reference_uniq
 NEW ir.rule: payment.payment_capture_wizard_rule (noupdate)
 DEL ir.rule: payment.payment_transaction_user_rule (noupdate)
 NEW ir.ui.view: payment.company_mismatch_warning
 NEW ir.ui.view: payment.form
 NEW ir.ui.view: payment.form_icon
 NEW ir.ui.view: payment.form_logo
 NEW ir.ui.view: payment.method_form
```

## odoo/addons/openupgrade_scripts/scripts/phone_validation/17.0.2.1/upgrade_analysis.txt

```diff
@@ -1,5 +1,4 @@
 ---Models in module 'phone_validation'---
 ---Fields in module 'phone_validation'---
 phone_validation / phone.blacklist          / message_main_attachment_id (many2one): DEL relation: ir.attachment
 ---XML records in module 'phone_validation'---
-DEL ir.model.constraint: phone_validation.constraint_phone_blacklist_unique_number
```

## odoo/addons/openupgrade_scripts/scripts/point_of_sale/17.0.1.0.1/upgrade_analysis.txt

```diff
@@ -1,12 +1,12 @@
 ---Models in module 'point_of_sale'---
-obsolete model pos.cache
 obsolete model pos.session.check_product_wizard [transient]
 new model pos.combo
 new model pos.combo.line
+model pos.daily.sales.reports.wizard (moved from pos_daily_sales_reports) [transient]
 new model pos.printer
 ---Fields in module 'point_of_sale'---
 point_of_sale / account.move             / pos_refunded_invoice_ids (many2many): NEW relation: account.move
 point_of_sale / pos.combo                / combo_line_ids (one2many)     : NEW relation: pos.combo.line
 point_of_sale / pos.combo                / name (char)                   : NEW required
 point_of_sale / pos.combo                / sequence (integer)            : NEW
 point_of_sale / pos.combo.line           / combo_id (many2one)           : NEW relation: pos.combo
@@ -40,68 +40,53 @@
 point_of_sale / pos.printer              / name (char)                   : NEW required, hasdefault: default
 point_of_sale / pos.printer              / printer_type (selection)      : NEW selection_keys: ['iot'], hasdefault: default
 point_of_sale / pos.printer              / product_categories_ids (many2many): NEW relation: pos.category
 point_of_sale / pos.printer              / proxy_ip (char)               : NEW
 point_of_sale / pos.session              / access_token (char)           : NEW
 point_of_sale / pos.session              / activity_user_id (many2one)   : not related anymore
 point_of_sale / pos.session              / activity_user_id (many2one)   : now a function
+point_of_sale / pos.session              / closing_notes (text)          : previously in module pos_daily_sales_reports
 point_of_sale / pos.session              / message_main_attachment_id (many2one): DEL relation: ir.attachment
 point_of_sale / pos.session              / rating_ids (one2many)         : NEW relation: rating.rating
 point_of_sale / product.attribute.custom.value / pos_order_line_id (many2one)  : NEW relation: pos.order.line
 point_of_sale / product.template         / combo_ids (many2many)         : NEW relation: pos.combo
 point_of_sale / product.template         / detailed_type (False)         : NEW selection_keys: ['combo', 'consu', 'product', 'service'], mode: modify
 point_of_sale / product.template         / pos_categ_id (many2one)       : DEL relation: pos.category
 point_of_sale / product.template         / pos_categ_ids (many2many)     : NEW relation: pos.category
 point_of_sale / product.template         / type (False)                  : NEW selection_keys: ['combo', 'consu', 'product', 'service'], mode: modify
 point_of_sale / res.company              / point_of_sale_ticket_unique_code (boolean): NEW
-pos_cache    / pos.cache                / cache (binary)                : DEL attachment: True
-pos_cache    / pos.cache                / compute_user_id (many2one)    : DEL relation: res.users, required
-pos_cache    / pos.cache                / config_id (many2one)          : DEL relation: pos.config, required
-pos_cache    / pos.cache                / product_domain (text)         : DEL required
-pos_cache    / pos.cache                / product_fields (text)         : DEL required
-pos_cache    / pos.config               / cache_ids (one2many)          : DEL relation: pos.cache
-pos_epson_printer_restaurant / restaurant.printer       / epson_printer_ip (char)       : DEL
-pos_epson_printer_restaurant / restaurant.printer       / printer_type (False)          : DEL selection_keys: ['epson_epos', 'iot'], mode: modify
 ---XML records in module 'point_of_sale'---
 NEW ir.actions.act_window: point_of_sale.action_pos_combo
 NEW ir.actions.act_window: point_of_sale.action_pos_config_tree
 NEW ir.actions.act_window: point_of_sale.action_pos_printer_form
 NEW ir.actions.act_window: point_of_sale.action_report_pos_daily_sales_reports [renamed from pos_daily_sales_reports module]
-DEL ir.actions.act_window: pos_daily_sales_reports.action_report_pos_daily_sales_reports [renamed to point_of_sale module]
 NEW ir.actions.client: point_of_sale.action_client_product_menu (noupdate)
-DEL ir.cron: pos_cache.refresh_pos_cache_cron
+NEW ir.model.access: point_of_sale.access_account_journal_entry
 NEW ir.model.access: point_of_sale.access_pos_combo_line_manager
 NEW ir.model.access: point_of_sale.access_pos_combo_line_user
 NEW ir.model.access: point_of_sale.access_pos_combo_manager
 NEW ir.model.access: point_of_sale.access_pos_combo_user
 NEW ir.model.access: point_of_sale.access_pos_daily_sales_reports_wizard [renamed from pos_daily_sales_reports module]
 NEW ir.model.access: point_of_sale.access_pos_printer
 NEW ir.model.access: point_of_sale.access_pos_printer_manager
 DEL ir.model.access: point_of_sale.access_account_bank_statement
 DEL ir.model.access: point_of_sale.access_account_bank_statement_manager
 DEL ir.model.access: point_of_sale.access_account_move
 DEL ir.model.access: point_of_sale.access_account_move_line
 DEL ir.model.access: point_of_sale.access_pos_session_check_product_wizard
-DEL ir.model.access: pos_cache.access_pos_cache
-DEL ir.model.access: pos_daily_sales_reports.access_pos_daily_sales_reports_wizard [renamed to point_of_sale module]
-DEL ir.model.constraint: point_of_sale.constraint_pos_session_uniq_name
+NEW ir.rule: point_of_sale.rule_invoice_pos_user (noupdate)
 DEL ir.rule: point_of_sale.rule_pos_account_move (noupdate)
 DEL ir.rule: point_of_sale.rule_pos_account_move_line (noupdate)
 NEW ir.ui.menu: point_of_sale.menu_point_of_sale_list
 NEW ir.ui.menu: point_of_sale.menu_pos_combo
 NEW ir.ui.menu: point_of_sale.menu_pos_preparation_printer
 NEW ir.ui.menu: point_of_sale.menu_report_daily_details [renamed from pos_daily_sales_reports module]
-DEL ir.ui.menu: pos_daily_sales_reports.menu_report_daily_details [renamed to point_of_sale module]
 NEW ir.ui.view: point_of_sale.account_product_template_form_view
 NEW ir.ui.view: point_of_sale.ticket_request_with_code
 NEW ir.ui.view: point_of_sale.view_pos_combo_form
 NEW ir.ui.view: point_of_sale.view_pos_combo_tree
 NEW ir.ui.view: point_of_sale.view_pos_daily_sales_reports_wizard
 NEW ir.ui.view: point_of_sale.view_pos_printer
 NEW ir.ui.view: point_of_sale.view_pos_printer_form
 DEL ir.ui.view: point_of_sale.assets_common
 DEL ir.ui.view: point_of_sale.qunit_suite_assets
 DEL ir.ui.view: point_of_sale.view_pos_session_check_product_wizard
-DEL ir.ui.view: pos_cache.view_pos_config_kanban
-DEL ir.ui.view: pos_daily_sales_reports.pos_daily_report
-DEL ir.ui.view: pos_daily_sales_reports.view_pos_daily_sales_reports_wizard
-DEL ir.ui.view: pos_epson_printer_restaurant.view_restaurant_printer_iot_form
```

## odoo/addons/openupgrade_scripts/scripts/product/17.0.1.2/upgrade_analysis.txt

```diff
@@ -36,19 +36,15 @@
 ---XML records in module 'product'---
 NEW ir.actions.report: product.report_product_template_label_2x7
 NEW ir.actions.report: product.report_product_template_label_4x12
 NEW ir.actions.report: product.report_product_template_label_4x12_noprice
 NEW ir.actions.report: product.report_product_template_label_4x7
 DEL ir.actions.report: product.report_product_template_label
 NEW ir.model.access: product.access_product_document_user
-DEL ir.model.constraint: product.constraint_product_attribute_value_value_company_uniq
-DEL ir.model.constraint: product.constraint_product_packaging_barcode_uniq
-DEL ir.model.constraint: product.constraint_product_packaging_positive_qty
-DEL ir.model.constraint: product.constraint_product_tag_name_uniq
-DEL ir.model.constraint: product.constraint_product_template_attribute_value_attribute_value_unique
+NEW ir.model.constraint: product.constraint_product_attribute_check_multi_checkbox_no_variant
 NEW ir.rule: product.product_document_comp_rule (noupdate)
 NEW ir.ui.view: product.product_attribute_value_list
 NEW ir.ui.view: product.product_document_form
 NEW ir.ui.view: product.product_document_kanban
 NEW ir.ui.view: product.product_document_list
 NEW ir.ui.view: product.product_document_search
 NEW ir.ui.view: product.product_product_view_tree_tag
```

## odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/noupdate_changes.xml

```diff
@@ -155,14 +155,15 @@
                 </t>
               </td>
             </tr>
           </tbody>
         </table>
       </div>
     </field>
+    <field name="subject">{{ object.project_id.company_id.name or user.env.company.name }}: Satisfaction Survey</field>
     <field name="active" eval="False"/>
   </record>
   <record id="report_project_task_user_report_comp_rule" model="ir.rule">
     <field name="domain_force">[('company_id', 'in', company_ids + [False])]</field>
   </record>
   <record id="task_comp_rule" model="ir.rule">
     <field name="domain_force">[('company_id', 'in', company_ids + [False])]</field>
```

## odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/upgrade_analysis.txt

```diff
@@ -100,18 +100,16 @@
 NEW ir.actions.server: project.action_server_convert_to_subtask
 NEW ir.actions.server: project.action_server_view_my_task
 NEW ir.actions.server: project.unlink_project_stage_action
 DEL ir.cron: project.ir_cron_recurring_tasks (noupdate)
 NEW ir.model.access: project.access_mail_activity_plan_project_manager
 NEW ir.model.access: project.access_mail_activity_plan_template_project_manager
 NEW ir.model.access: project.access_project_project_stage_delete_wizard
-DEL ir.model.constraint: project.constraint_project_collaborator_unique_collaborator
-DEL ir.model.constraint: project.constraint_project_project_project_date_greater
-DEL ir.model.constraint: project.constraint_project_tags_name_uniq
-DEL ir.model.constraint: project.constraint_project_task_user_rel_project_personal_stage_unique
+NEW ir.model.constraint: project.constraint_project_task_private_task_has_no_parent
+NEW ir.model.constraint: project.constraint_project_task_recurring_task_has_no_parent
 NEW ir.rule: project.mail_plan_rule_group_project_manager_task (noupdate)
 NEW ir.rule: project.mail_plan_templates_rule_group_project_manager_task (noupdate)
 NEW ir.rule: project.project_project_stage_rule (noupdate)
 NEW ir.ui.menu: project.mail_activity_plan_menu_config_project
 NEW ir.ui.menu: project.menu_project_management_all_tasks
 NEW ir.ui.menu: project.menu_project_management_my_tasks
 DEL ir.ui.menu: project.menu_tasks_config
```

## odoo/addons/openupgrade_scripts/scripts/project_todo/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,82 +1,31 @@
 ---Models in module 'project_todo'---
-obsolete model note.note
-obsolete model note.stage
-obsolete model note.tag
 new model mail.activity.todo.create [transient]
 ---Fields in module 'project_todo'---
-note         / mail.activity            / note_id (many2one)            : DEL relation: note.note
-note         / note.note                / activity_ids (one2many)       : DEL relation: mail.activity
-note         / note.note                / color (integer)               : DEL
-note         / note.note                / company_id (many2one)         : DEL relation: res.company
-note         / note.note                / date_done (date)              : DEL
-note         / note.note                / memo (html)                   : DEL
-note         / note.note                / message_follower_ids (one2many): DEL relation: mail.followers
-note         / note.note                / message_ids (one2many)        : DEL relation: mail.message
-note         / note.note                / message_main_attachment_id (many2one): DEL relation: ir.attachment
-note         / note.note                / name (text)                   : DEL
-note         / note.note                / open (boolean)                : DEL
-note         / note.note                / sequence (integer)            : DEL
-note         / note.note                / stage_ids (many2many)         : DEL relation: note.stage
-note         / note.note                / tag_ids (many2many)           : DEL relation: note.tag
-note         / note.note                / user_id (many2one)            : DEL relation: res.users
-note         / note.stage               / fold (boolean)                : DEL
-note         / note.stage               / name (char)                   : DEL required
-note         / note.stage               / sequence (integer)            : DEL
-note         / note.stage               / user_id (many2one)            : DEL relation: res.users, required
-note         / note.tag                 / color (integer)               : DEL
-note         / note.tag                 / name (char)                   : DEL required
+project_todo / mail.activity.type       / category (False)              : previously in module note
 ---XML records in module 'project_todo'---
 NEW ir.actions.act_window: project_todo.project_task_action_convert_todo_to_task
 NEW ir.actions.act_window: project_todo.project_task_action_todo
-DEL ir.actions.act_window: note.action_note_note
-DEL ir.actions.act_window: note.action_note_stage
-DEL ir.actions.act_window: note.note_tag_action
 NEW ir.actions.act_window.view: project_todo.project_task_action_convert_todo_to_task_form_view
 NEW ir.actions.act_window.view: project_todo.project_task_action_todo_activity_view
 NEW ir.actions.act_window.view: project_todo.project_task_action_todo_form_view
 NEW ir.actions.act_window.view: project_todo.project_task_action_todo_kanban_view
 NEW ir.actions.act_window.view: project_todo.project_task_action_todo_tree_view
 NEW ir.actions.server: project_todo.project_task_preload_action_todo
 NEW ir.model.access: project_todo.access_mail_activity_todo_create
 NEW ir.model.access: project_todo.access_project_tags_user
 NEW ir.model.access: project_todo.access_project_task_type_user
 NEW ir.model.access: project_todo.access_task_on_partner
-DEL ir.model.access: note.access_note_note
-DEL ir.model.access: note.access_note_stage
-DEL ir.model.access: note.access_note_tag
-DEL ir.model.constraint: note.constraint_note_tag_name_uniq
 NEW ir.rule: project_todo.task_edition_rule_internal (noupdate)
 NEW ir.rule: project_todo.task_visibility_rule_project_user (noupdate)
-DEL ir.rule: note.ir_rule_note_note_multi_company (noupdate)
-DEL ir.rule: note.note_note_create_unlink_global (noupdate)
-DEL ir.rule: note.note_note_rule_global (noupdate)
-DEL ir.rule: note.note_stage_rule_global (noupdate)
 NEW ir.ui.menu: project_todo.menu_todo_todos
-DEL ir.ui.menu: note.menu_note_configuration
-DEL ir.ui.menu: note.menu_note_notes
-DEL ir.ui.menu: note.menu_notes_stage
-DEL ir.ui.menu: note.notes_tag_menu
 NEW ir.ui.view: project_todo.mail_activity_todo_create_popup
 NEW ir.ui.view: project_todo.project_task_view_todo_activity
 NEW ir.ui.view: project_todo.project_task_view_todo_conversion_form
 NEW ir.ui.view: project_todo.project_task_view_todo_form
 NEW ir.ui.view: project_todo.project_task_view_todo_kanban
 NEW ir.ui.view: project_todo.project_task_view_todo_quick_create_form
 NEW ir.ui.view: project_todo.project_task_view_todo_search
 NEW ir.ui.view: project_todo.project_task_view_todo_tree
 NEW ir.ui.view: project_todo.todo_user_onboarding (noupdate)
-DEL ir.ui.view: note.note_tag_view_form
-DEL ir.ui.view: note.note_tag_view_tree
-DEL ir.ui.view: note.view_note_note_filter
-DEL ir.ui.view: note.view_note_note_form
-DEL ir.ui.view: note.view_note_note_kanban
-DEL ir.ui.view: note.view_note_note_tree
-DEL ir.ui.view: note.view_note_stage_form
-DEL ir.ui.view: note.view_note_stage_tree
 NEW mail.activity.type: project_todo.mail_activity_data_reminder [renamed from note module] (noupdate)
-DEL mail.activity.type: note.mail_activity_data_reminder [renamed to project_todo module] (noupdate)
-DEL note.stage: note.note_stage_00
-DEL note.stage: note.note_stage_01
-DEL note.stage: note.note_stage_02
-DEL note.stage: note.note_stage_03
 NEW res.groups: project_todo.group_onboarding_todo
```

## odoo/addons/openupgrade_scripts/scripts/purchase/17.0.1.2/upgrade_analysis.txt

```diff
@@ -3,14 +3,12 @@
 purchase     / purchase.order           / activity_user_id (many2one)   : not related anymore
 purchase     / purchase.order           / activity_user_id (many2one)   : now a function
 purchase     / purchase.order           / message_main_attachment_id (many2one): DEL relation: ir.attachment
 purchase     / purchase.order           / rating_ids (one2many)         : NEW relation: rating.rating
 purchase     / purchase.order.line      / discount (float)              : NEW hasdefault: compute
 purchase     / res.partner              / buyer_id (many2one)           : NEW relation: res.users
 ---XML records in module 'purchase'---
-DEL ir.model.constraint: purchase.constraint_purchase_order_line_accountable_required_fields
-DEL ir.model.constraint: purchase.constraint_purchase_order_line_non_accountable_null_fields
 NEW ir.ui.view: purchase.document_tax_totals
 NEW ir.ui.view: purchase.product_template_search_view_purchase
 NEW ir.ui.view: purchase.product_view_kanban_catalog_purchase_only
 NEW ir.ui.view: purchase.product_view_search_catalog
 NEW ir.ui.view: purchase.view_product_product_supplier_inherit
```

## odoo/addons/openupgrade_scripts/scripts/purchase_stock/17.0.1.2/upgrade_analysis.txt

```diff
@@ -1,15 +1,16 @@
 ---Models in module 'purchase_stock'---
 ---Fields in module 'purchase_stock'---
+purchase_stock / product.category         / property_account_creditor_price_difference_categ (many2one): previously in module purchase_price_diff
+purchase_stock / product.product          / property_account_creditor_price_difference (many2one): previously in module purchase_price_diff
+purchase_stock / product.template         / property_account_creditor_price_difference (many2one): previously in module purchase_price_diff
 purchase_stock / purchase.order.line      / move_dest_ids (one2many)      : table is now 'stock_move_created_purchase_line_rel' ('False')
 purchase_stock / purchase.order.line      / move_dest_ids (one2many)      : type is now 'many2many' ('one2many')
 purchase_stock / stock.move               / created_purchase_line_id (many2one): DEL relation: purchase.order.line
 purchase_stock / stock.move               / created_purchase_line_ids (many2many): NEW relation: purchase.order.line
 ---XML records in module 'purchase_stock'---
 NEW ir.ui.view: purchase_stock.product_template_form_view
 NEW ir.ui.view: purchase_stock.product_view_kanban_catalog_purchase_only
 NEW ir.ui.view: purchase_stock.stock_reorder_report_search_inherited_purchase_stock
 NEW ir.ui.view: purchase_stock.view_category_property_form
 NEW ir.ui.view: purchase_stock.view_product_replenish_form_inherit_stock
-DEL ir.ui.view: purchase_price_diff.product_template_form_view
-DEL ir.ui.view: purchase_price_diff.view_category_property_form
 DEL ir.ui.view: purchase_stock.purchase_report_product_product_replenishment
```

## odoo/addons/openupgrade_scripts/scripts/rating/17.0.1.1/upgrade_analysis.txt

```diff
@@ -15,8 +15,7 @@
 rating       / maintenance.request      / rating_ids (one2many)         : NEW relation: rating.rating
 rating       / phone.blacklist          / rating_ids (one2many)         : NEW relation: rating.rating
 rating       / product.pricelist        / rating_ids (one2many)         : NEW relation: rating.rating
 rating       / product.product          / rating_ids (one2many)         : previously in module website_sale
 rating       / product.template         / rating_ids (one2many)         : previously in module website_sale
 rating       / res.partner              / rating_ids (one2many)         : NEW relation: rating.rating
 ---XML records in module 'rating'---
-DEL ir.model.constraint: rating.constraint_rating_rating_rating_range
```

## odoo/addons/openupgrade_scripts/scripts/repair/17.0.1.0/upgrade_analysis.txt

```diff
@@ -86,15 +86,14 @@
 DEL ir.actions.act_window: repair.act_repair_invoice
 NEW ir.model.access: repair.access_repair_warn_uncomplete_move
 DEL ir.model.access: repair.access_account_tax_user
 DEL ir.model.access: repair.access_repair_fee_user
 DEL ir.model.access: repair.access_repair_line_user
 DEL ir.model.access: repair.access_repair_order_make_invoice
 DEL ir.model.constraint: repair.constraint_repair_order_name
-DEL ir.model.constraint: repair.constraint_repair_tags_name_uniq
 DEL ir.rule: repair.repair_fee_rule (noupdate)
 DEL ir.rule: repair.repair_line_rule (noupdate)
 DEL ir.sequence: repair.seq_repair (noupdate)
 NEW ir.ui.menu: repair.repair_order_menu
 NEW ir.ui.view: repair.repair_order_view_activity
 NEW ir.ui.view: repair.stock_repair_type_kanban
 NEW ir.ui.view: repair.view_product_template_form_inherit_repair
```

## odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/upgrade_analysis.txt

```diff
@@ -32,19 +32,16 @@
 DEL ir.actions.act_window: sale.action_open_sale_payment_provider_onboarding_wizard
 NEW ir.model.access: sale.access_account_move_send_salesman
 NEW ir.model.access: sale.access_mail_activity_plan_sale_manager
 NEW ir.model.access: sale.access_mail_activity_plan_template_sale_manager
 NEW ir.model.access: sale.access_sale_mass_cancel_orders
 NEW ir.model.access: sale.access_sale_order_discount
 DEL ir.model.access: sale.access_account_invoice_send_salesman
-DEL ir.model.constraint: sale.constraint_product_attribute_custom_value_sol_custom_value_unique
-DEL ir.model.constraint: sale.constraint_res_company_check_quotation_validity_days
-DEL ir.model.constraint: sale.constraint_sale_order_date_order_conditional_required
-DEL ir.model.constraint: sale.constraint_sale_order_line_accountable_required_fields
-DEL ir.model.constraint: sale.constraint_sale_order_line_non_accountable_null_fields
+ir.model.constraint: sale.constraint_res_company_check_quotation_validity_days (changed definition: is now 'check(quotation_validity_days >= 0)' ('check(quotation_validity_days > 0)'))
+ir.model.constraint: sale.constraint_sale_order_date_order_conditional_required (changed definition: is now 'check((state = 'sale' and date_order is not null) or state != 'sale')' ('check((state in('sale','done') and date_order is not null) or state not in('sale','done'))'))
 NEW ir.rule: sale.mail_plan_rule_group_sale_manager (noupdate)
 NEW ir.rule: sale.mail_plan_template_rule_group_sale_manager (noupdate)
 NEW ir.rule: sale.sale_mass_cancel_orders_rule (noupdate)
 NEW ir.ui.menu: sale.menu_product_categories
 NEW ir.ui.menu: sale.menu_reporting_customer
 NEW ir.ui.menu: sale.menu_reporting_product
 NEW ir.ui.menu: sale.menu_reporting_sales
```

## odoo/addons/openupgrade_scripts/scripts/sale_loyalty/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,5 +1,4 @@
 ---Models in module 'sale_loyalty'---
 ---Fields in module 'sale_loyalty'---
 ---XML records in module 'sale_loyalty'---
-DEL ir.model.constraint: sale_loyalty.constraint_sale_order_coupon_points_order_coupon_unique
 NEW ir.ui.view: sale_loyalty.res_partner_form
```

## odoo/addons/openupgrade_scripts/scripts/sale_loyalty_delivery/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,7 +1,6 @@
 ---Models in module 'sale_loyalty_delivery'---
 ---Fields in module 'sale_loyalty_delivery'---
+sale_loyalty_delivery / loyalty.reward           / reward_type (False)           : previously in module loyalty_delivery
 ---XML records in module 'sale_loyalty_delivery'---
 NEW ir.ui.view: sale_loyalty_delivery.loyalty_reward_view_form_inherit_loyalty_delivery
 NEW ir.ui.view: sale_loyalty_delivery.loyalty_reward_view_kanban_inherit_loyalty_delivery
-DEL ir.ui.view: loyalty_delivery.loyalty_reward_view_form_inherit_loyalty_delivery
-DEL ir.ui.view: loyalty_delivery.loyalty_reward_view_kanban_inherit_loyalty_delivery
```

## odoo/addons/openupgrade_scripts/scripts/sale_management/17.0.1.0/upgrade_analysis.txt

```diff
@@ -4,10 +4,8 @@
 sale_management / sale.order.template      / prepayment_percent (float)    : NEW hasdefault: compute
 ---XML records in module 'sale_management'---
 digest.tip: sale_management.digest_tip_sale1_management_0 (noupdate switched)
 digest.tip: sale_management.digest_tip_sale_management_1 (noupdate switched)
 NEW ir.model.access: sale_management.access_sale_order_option_invoice
 NEW ir.model.access: sale_management.access_sale_order_option_readonly
 DEL ir.model.access: sale_management.access_sale_order_option_all
-DEL ir.model.constraint: sale_management.constraint_sale_order_template_line_accountable_product_id_required
-DEL ir.model.constraint: sale_management.constraint_sale_order_template_line_non_accountable_fields_null
 DEL ir.ui.view: sale_management.res_config_settings_view_form_inherit_sale_management
```

## odoo/addons/openupgrade_scripts/scripts/sale_timesheet/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,16 +1,14 @@
 ---Models in module 'sale_timesheet'---
 ---Fields in module 'sale_timesheet'---
 sale_timesheet / project.project          / allocated_hours (False)       : DEL mode: modify
 sale_timesheet / project.project          / billing_type (selection)      : NEW required, selection_keys: ['manually', 'not_billable'], hasdefault: default
 sale_timesheet / project.project          / partner_id (False)            : module is now 'sale_project' ('sale_timesheet')
 sale_timesheet / project.task             / allow_billable (boolean)      : module is now 'sale_project' ('sale_timesheet')
 ---XML records in module 'sale_timesheet'---
-DEL ir.model.constraint: sale_timesheet.constraint_project_create_sale_order_line_unique_employee_per_wizard
-DEL ir.model.constraint: sale_timesheet.constraint_project_sale_line_employee_map_uniqueness_employee
 NEW ir.ui.view: sale_timesheet.project_task_view_search_inherit_sale_timesheet
 NEW ir.ui.view: sale_timesheet.view_hr_timesheet_line_graph_invoice_employee
 NEW ir.ui.view: sale_timesheet.view_hr_timesheet_line_pivot_inherited
 NEW ir.ui.view: sale_timesheet.view_task_project_user_pivot_inherited
 DEL ir.ui.view: sale_timesheet.project_project_view_form_simplified_inherit
 DEL ir.ui.view: sale_timesheet.project_sharing_inherit_project_task_view_tree_sale_timesheet
 DEL ir.ui.view: sale_timesheet.view_sale_service_inherit_form2
```

## odoo/addons/openupgrade_scripts/scripts/sales_team/17.0.1.1/upgrade_analysis.txt

```diff
@@ -1,9 +1,8 @@
 ---Models in module 'sales_team'---
 ---Fields in module 'sales_team'---
 sales_team   / crm.team                 / message_main_attachment_id (many2one): DEL relation: ir.attachment
 sales_team   / crm.team                 / rating_ids (one2many)         : NEW relation: rating.rating
 sales_team   / crm.team.member          / message_main_attachment_id (many2one): DEL relation: ir.attachment
 sales_team   / crm.team.member          / rating_ids (one2many)         : NEW relation: rating.rating
 ---XML records in module 'sales_team'---
-DEL ir.model.constraint: sales_team.constraint_crm_tag_name_uniq
 DEL ir.ui.menu: sales_team.menu_sale_config
```

## odoo/addons/openupgrade_scripts/scripts/sms/17.0.3.0/upgrade_analysis.txt

```diff
@@ -2,22 +2,24 @@
 obsolete model sms.api [abstract]
 new model sms.tracker
 ---Fields in module 'sms'---
 sms          / hr.contract              / message_has_sms_error (boolean): module is now 'hr_contract' ('sms')
 sms          / hr.leave                 / message_has_sms_error (boolean): module is now 'hr_holidays' ('sms')
 sms          / hr.leave.allocation      / message_has_sms_error (boolean): module is now 'hr_holidays' ('sms')
 sms          / ir.actions.server        / state (False)                 : selection_keys is now '['code', 'followers', 'mail_post', 'multi', 'next_activity', 'object_create', 'object_write', 'remove_followers', 'sms', 'webhook']' ('['code', 'followers', 'mail_post', 'multi', 'next_activity', 'object_create', 'object_write', 'sms']')
-sms          / mail.message             / message_type (False)          : selection_keys is now '['auto_comment', 'comment', 'email', 'email_outgoing', 'notification', 'sms', 'user_notification']' ('['comment', 'email', 'notification', 'sms', 'user_notification']')
+sms          / mail.message             / message_type (False)          : selection_keys is now '['auto_comment', 'comment', 'email', 'email_outgoing', 'notification', 'sms', 'user_notification']' ('['auto_comment', 'comment', 'email', 'notification', 'sms', 'user_notification']')
 sms          / mail.notification        / failure_type (False)          : selection_keys is now '['mail_bounce', 'mail_email_invalid', 'mail_email_missing', 'mail_from_invalid', 'mail_from_missing', 'mail_smtp', 'sms_acc', 'sms_country_not_supported', 'sms_credit', 'sms_expired', 'sms_invalid_destination', 'sms_not_allowed', 'sms_not_delivered', 'sms_number_format', 'sms_number_missing', 'sms_registration_needed', 'sms_rejected', 'sms_server', 'unknown']' ('['mail_email_invalid', 'mail_email_missing', 'mail_smtp', 'sms_acc', 'sms_credit', 'sms_number_format', 'sms_number_missing', 'sms_server', 'unknown']')
 sms          / mail.notification        / sms_id (many2one)             : not stored anymore
 sms          / mail.notification        / sms_id (many2one)             : now a function
 sms          / mail.notification        / sms_id_int (integer)          : NEW
 sms          / mail.notification        / sms_tracker_ids (one2many)    : NEW relation: sms.tracker
 sms          / sms.sms                  / failure_type (selection)      : selection_keys is now '['sms_acc', 'sms_blacklist', 'sms_country_not_supported', 'sms_credit', 'sms_duplicate', 'sms_number_format', 'sms_number_missing', 'sms_optout', 'sms_registration_needed', 'sms_server', 'unknown']' ('['sms_acc', 'sms_blacklist', 'sms_credit', 'sms_duplicate', 'sms_number_format', 'sms_number_missing', 'sms_optout', 'sms_server']')
 sms          / sms.sms                  / state (selection)             : selection_keys is now '['canceled', 'error', 'outgoing', 'pending', 'process', 'sent']' ('['canceled', 'error', 'outgoing', 'sent']')
 sms          / sms.sms                  / to_delete (boolean)           : NEW hasdefault: default
 sms          / sms.sms                  / uuid (char)                   : NEW
 sms          / sms.tracker              / mail_notification_id (many2one): NEW relation: mail.notification
 sms          / sms.tracker              / sms_uuid (char)               : NEW required
 ---XML records in module 'sms'---
 NEW ir.model.access: sms.access_sms_tracker_all
 NEW ir.model.access: sms.access_sms_tracker_system
+NEW ir.model.constraint: sms.constraint_sms_sms_uuid_unique
+NEW ir.model.constraint: sms.constraint_sms_tracker_sms_uuid_unique
```

## odoo/addons/openupgrade_scripts/scripts/snailmail/17.0.0.4/upgrade_analysis.txt

```diff
@@ -1,8 +1,8 @@
 ---Models in module 'snailmail'---
 obsolete model snailmail.confirm [abstract]
 ---Fields in module 'snailmail'---
-snailmail    / mail.message             / message_type (False)          : selection_keys is now '['auto_comment', 'comment', 'email', 'email_outgoing', 'notification', 'sms', 'snailmail', 'user_notification']' ('['comment', 'email', 'notification', 'sms', 'snailmail', 'user_notification']')
+snailmail    / mail.message             / message_type (False)          : selection_keys is now '['auto_comment', 'comment', 'email', 'email_outgoing', 'notification', 'sms', 'snailmail', 'user_notification']' ('['auto_comment', 'comment', 'email', 'notification', 'sms', 'snailmail', 'user_notification']')
 snailmail    / mail.notification        / failure_type (False)          : selection_keys is now '['mail_bounce', 'mail_email_invalid', 'mail_email_missing', 'mail_from_invalid', 'mail_from_missing', 'mail_smtp', 'sms_acc', 'sms_country_not_supported', 'sms_credit', 'sms_expired', 'sms_invalid_destination', 'sms_not_allowed', 'sms_not_delivered', 'sms_number_format', 'sms_number_missing', 'sms_registration_needed', 'sms_rejected', 'sms_server', 'sn_credit', 'sn_error', 'sn_fields', 'sn_format', 'sn_price', 'sn_trial', 'unknown']' ('['mail_email_invalid', 'mail_email_missing', 'mail_smtp', 'sms_acc', 'sms_credit', 'sms_number_format', 'sms_number_missing', 'sms_server', 'sn_credit', 'sn_error', 'sn_fields', 'sn_format', 'sn_price', 'sn_trial', 'unknown']')
 snailmail    / snailmail.letter         / error_code (selection)        : selection_keys is now '['ATTACHMENT_ERROR', 'CREDIT_ERROR', 'FORMAT_ERROR', 'MISSING_REQUIRED_FIELDS', 'NO_PRICE_AVAILABLE', 'TRIAL_ERROR', 'UNKNOWN_ERROR']' ('['CREDIT_ERROR', 'FORMAT_ERROR', 'MISSING_REQUIRED_FIELDS', 'NO_PRICE_AVAILABLE', 'TRIAL_ERROR', 'UNKNOWN_ERROR']')
 ---XML records in module 'snailmail'---
 DEL ir.ui.view: snailmail.snailmail_confirm_view
```

## odoo/addons/openupgrade_scripts/scripts/stock/17.0.1.1/upgrade_analysis.txt

```diff
@@ -76,33 +76,21 @@
 NEW ir.actions.client: stock.stock_forecasted_product_template_action
 DEL ir.actions.client: stock.stock_replenishment_product_product_action
 DEL ir.actions.client: stock.stock_replenishment_product_template_action
 NEW ir.actions.report: stock.return_label_report
 NEW ir.actions.server: stock.action_scrap
 NEW ir.actions.server: stock.action_toggle_is_locked
 NEW ir.actions.server: stock.action_view_set_to_zero_quants_tree
+DEL ir.actions.server: stock.stock_quant_stock_move_line_desynchronization
 NEW ir.model.access: stock.access_stock_quant_relocate
 DEL ir.model.access: stock.access_stock_immediate_transfer
 DEL ir.model.access: stock.access_stock_immediate_transfer_line
-DEL ir.model.constraint: stock.constraint_stock_location_barcode_company_uniq
-DEL ir.model.constraint: stock.constraint_stock_location_inventory_freq_nonneg
-DEL ir.model.constraint: stock.constraint_stock_package_type_barcode_uniq
-DEL ir.model.constraint: stock.constraint_stock_package_type_positive_height
-DEL ir.model.constraint: stock.constraint_stock_package_type_positive_length
-DEL ir.model.constraint: stock.constraint_stock_package_type_positive_max_weight
-DEL ir.model.constraint: stock.constraint_stock_package_type_positive_width
-DEL ir.model.constraint: stock.constraint_stock_picking_name_uniq
-DEL ir.model.constraint: stock.constraint_stock_storage_category_capacity_positive_quantity
-DEL ir.model.constraint: stock.constraint_stock_storage_category_capacity_unique_package_type
-DEL ir.model.constraint: stock.constraint_stock_storage_category_capacity_unique_product
-DEL ir.model.constraint: stock.constraint_stock_storage_category_positive_max_weight
-DEL ir.model.constraint: stock.constraint_stock_warehouse_orderpoint_product_location_check
-DEL ir.model.constraint: stock.constraint_stock_warehouse_orderpoint_qty_multiple_check
-DEL ir.model.constraint: stock.constraint_stock_warehouse_warehouse_code_uniq
-DEL ir.model.constraint: stock.constraint_stock_warehouse_warehouse_name_uniq
+ir.model.constraint: stock.constraint_stock_package_type_positive_height (changed definition: is now 'check(height>=0.0)' ('check(height>=0)'))
+ir.model.constraint: stock.constraint_stock_package_type_positive_length (changed definition: is now 'check(packaging_length>=0.0)' ('check(packaging_length>=0)'))
+ir.model.constraint: stock.constraint_stock_package_type_positive_width (changed definition: is now 'check(width>=0.0)' ('check(width>=0)'))
 NEW ir.ui.menu: stock.in_picking
 NEW ir.ui.menu: stock.int_picking
 NEW ir.ui.menu: stock.menu_stock_adjustments
 NEW ir.ui.menu: stock.menu_stock_procurement
 NEW ir.ui.menu: stock.menu_stock_transfers
 NEW ir.ui.menu: stock.out_picking
 DEL ir.ui.menu: stock.all_picking
```

## odoo/addons/openupgrade_scripts/scripts/stock_account/17.0.1.1/upgrade_analysis.txt

```diff
@@ -2,12 +2,15 @@
 ---Fields in module 'stock_account'---
 stock_account / account.move.line        / cogs_origin_id (many2one)     : NEW relation: account.move.line
 stock_account / stock.move               / analytic_account_line_id (many2one): DEL relation: account.analytic.line
 stock_account / stock.move               / analytic_account_line_ids (many2many): NEW relation: account.analytic.line
 stock_account / stock.valuation.layer    / categ_id (many2one)           : is now stored
 ---XML records in module 'stock_account'---
 NEW ir.actions.act_window: stock_account.inventory_aging_action
+NEW ir.filters: stock_account.filter_invoice_inventory_valuation
+DEL ir.property: stock_account.property_stock_account_input_categ_id (noupdate)
+DEL ir.property: stock_account.property_stock_account_output_categ_id (noupdate)
 NEW ir.ui.menu: stock_account.menu_inventory_aging
 NEW ir.ui.view: stock_account.stock_valuation_layer_graph
 NEW ir.ui.view: stock_account.stock_valuation_layer_valuation_at_date_tree_inherited
 DEL ir.ui.view: stock_account.stock_account_report_product_product_replenishment
 NEW res.groups: stock_account.group_stock_accounting_automatic (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/survey/17.0.3.6/upgrade_analysis.txt

```diff
@@ -13,31 +13,14 @@
 survey       / survey.survey            / survey_type (selection)       : NEW required, selection_keys: ['assessment', 'custom', 'live_session', 'survey'], hasdefault: default
 survey       / survey.user_input        / activity_user_id (many2one)   : not related anymore
 survey       / survey.user_input        / activity_user_id (many2one)   : now a function
 survey       / survey.user_input        / message_main_attachment_id (many2one): DEL relation: ir.attachment
 survey       / survey.user_input        / rating_ids (one2many)         : NEW relation: rating.rating
 survey       / survey.user_input        / survey_first_submitted (boolean): NEW
 ---XML records in module 'survey'---
-DEL ir.model.constraint: survey.constraint_survey_question_positive_answer_score
-DEL ir.model.constraint: survey.constraint_survey_question_positive_len_max
-DEL ir.model.constraint: survey.constraint_survey_question_positive_len_min
-DEL ir.model.constraint: survey.constraint_survey_question_scored_date_have_answers
-DEL ir.model.constraint: survey.constraint_survey_question_scored_datetime_have_answers
-DEL ir.model.constraint: survey.constraint_survey_question_validation_date
-DEL ir.model.constraint: survey.constraint_survey_question_validation_datetime
-DEL ir.model.constraint: survey.constraint_survey_question_validation_float
-DEL ir.model.constraint: survey.constraint_survey_question_validation_length
-DEL ir.model.constraint: survey.constraint_survey_survey_access_token_unique
-DEL ir.model.constraint: survey.constraint_survey_survey_attempts_limit_check
-DEL ir.model.constraint: survey.constraint_survey_survey_badge_uniq
-DEL ir.model.constraint: survey.constraint_survey_survey_certification_check
-DEL ir.model.constraint: survey.constraint_survey_survey_scoring_success_min_check
-DEL ir.model.constraint: survey.constraint_survey_survey_session_code_unique
-DEL ir.model.constraint: survey.constraint_survey_survey_time_limit_check
-DEL ir.model.constraint: survey.constraint_survey_user_input_unique_token
 NEW ir.ui.view: survey.certification_report_view_general
 NEW ir.ui.view: survey.survey_access_error
 NEW ir.ui.view: survey.survey_survey_view_activity
 DEL ir.ui.view: survey.certification_report_view_classic
 DEL ir.ui.view: survey.certification_report_view_modern
 NEW mail.message.subtype: survey.mt_survey_survey_user_input_completed (noupdate)
 NEW mail.message.subtype: survey.mt_survey_user_input_completed (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/uom/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,6 +1,4 @@
 ---Models in module 'uom'---
 ---Fields in module 'uom'---
 ---XML records in module 'uom'---
-DEL ir.model.constraint: uom.constraint_uom_uom_factor_gt_zero
-DEL ir.model.constraint: uom.constraint_uom_uom_factor_reference_is_one
-DEL ir.model.constraint: uom.constraint_uom_uom_rounding_gt_zero
+---nothing has changed in this module--
```

## odoo/addons/openupgrade_scripts/scripts/utm/17.0.1.1/upgrade_analysis.txt

```diff
@@ -1,9 +1,5 @@
 ---Models in module 'utm'---
 ---Fields in module 'utm'---
 utm          / utm.campaign             / active (boolean)              : NEW hasdefault: default
 ---XML records in module 'utm'---
-DEL ir.model.constraint: utm.constraint_utm_campaign_unique_name
-DEL ir.model.constraint: utm.constraint_utm_medium_unique_name
-DEL ir.model.constraint: utm.constraint_utm_source_unique_name
-DEL ir.model.constraint: utm.constraint_utm_tag_name_uniq
 NEW ir.ui.view: utm.utm_stage_view_form
```

## odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/noupdate_changes.xml

### odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/noupdate_changes.xml

```diff
@@ -1,95 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
-  <record id="library_image_02" model="ir.attachment">
-    <field name="name">library_image_02.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_02.jpg</field>
+  <record id="contactus_page" model="website.page">
+    <field name="website_meta_description">This is the contact us page of the website</field>
   </record>
-  <record id="library_image_03" model="ir.attachment">
-    <field name="name">library_image_03.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_03.jpg</field>
-  </record>
-  <record id="library_image_05" model="ir.attachment">
-    <field name="name">library_image_05.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_05.jpg</field>
-  </record>
-  <record id="library_image_07" model="ir.attachment">
-    <field name="name">library_image_07.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_07.jpg</field>
-  </record>
-  <record id="library_image_08" model="ir.attachment">
-    <field name="name">library_image_08.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_08.jpg</field>
-  </record>
-  <record id="library_image_10" model="ir.attachment">
-    <field name="name">library_image_10.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_10.jpg</field>
-  </record>
-  <record id="library_image_11" model="ir.attachment">
-    <field name="name">library_image_11.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_11.jpg</field>
-  </record>
-  <record id="library_image_13" model="ir.attachment">
-    <field name="name">library_image_13.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_13.jpg</field>
-  </record>
-  <record id="library_image_14" model="ir.attachment">
-    <field name="name">library_image_14.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_14.jpg</field>
-  </record>
-  <record id="library_image_16" model="ir.attachment">
-    <field name="name">library_image_16.jpg</field>
-    <field name="url">/website/static/src/img/library/library_image_16.jpg</field>
-  </record>
-  <record id="s_blockquote_default_image" model="ir.attachment">
-    <field name="url">/website/static/src/img/snippets_demo/s_team_member_2.jpg</field>
-  </record>
-  <record id="s_company_team_image_1" model="ir.attachment">
-    <field name="name">s_company_team_image_1.jpg</field>
-    <field name="url">/website/static/src/img/snippets_demo/s_team_member_1.jpg</field>
-  </record>
-  <record id="s_company_team_image_2" model="ir.attachment">
-    <field name="name">s_company_team_image_2.jpg</field>
-    <field name="url">/website/static/src/img/snippets_demo/s_team_member_2.jpg</field>
-  </record>
-  <record id="s_company_team_image_3" model="ir.attachment">
-    <field name="name">s_company_team_image_3.jpg</field>
-    <field name="url">/website/static/src/img/snippets_demo/s_team_member_3.jpg</field>
-  </record>
-  <record id="s_company_team_image_4" model="ir.attachment">
-    <field name="name">s_company_team_image_4.jpg</field>
-    <field name="url">/website/static/src/img/snippets_demo/s_team_member_4.jpg</field>
-  </record>
-  <record id="s_product_list_default_image_1" model="ir.attachment">
-    <field name="url">/website/static/src/img/snippets_demo/s_product_list_1.jpg</field>
-  </record>
-  <record id="s_product_list_default_image_2" model="ir.attachment">
-    <field name="url">/website/static/src/img/snippets_demo/s_product_list_2.jpg</field>
-  </record>
-  <record id="s_product_list_default_image_3" model="ir.attachment">
-    <field name="url">/website/static/src/img/snippets_demo/s_product_list_3.jpg</field>
-  </record>
-  <record id="s_product_list_default_image_4" model="ir.attachment">
-    <field name="url">/website/static/src/img/snippets_demo/s_product_list_4.jpg</field>
-  </record>
-  <record id="s_product_list_default_image_5" model="ir.attachment">
-    <field name="url">/website/static/src/img/snippets_demo/s_product_list_5.jpg</field>
-  </record>
-  <record id="s_product_list_default_image_6" model="ir.attachment">
-    <field name="url">/website/static/src/img/snippets_demo/s_product_list_6.jpg</field>
-  </record>
-  <record id="s_quotes_carousel_demo_image_0" model="ir.attachment">
-    <field name="url">/website/static/src/img/snippets_demo/s_quotes_carousel_0.jpg</field>
-  </record>
-  <record id="s_quotes_carousel_demo_image_3" model="ir.attachment">
-    <field name="name">s_quotes_carousel_image_3.jpg</field>
-    <field name="url">/website/static/src/img/snippets_demo/s_team_member_3.jpg</field>
-  </record>
-  <record id="s_quotes_carousel_demo_image_4" model="ir.attachment">
-    <field name="name">s_quotes_carousel_image_4.jpg</field>
-    <field name="url">/website/static/src/img/snippets_demo/s_team_member_2.jpg</field>
-  </record>
-  <record id="s_quotes_carousel_demo_image_5" model="ir.attachment">
-    <field name="name">s_quotes_carousel_image_5.jpg</field>
-    <field name="url">/website/static/src/img/snippets_demo/s_team_member_4.jpg</field>
+  <record id="homepage_page" model="website.page">
+    <field name="website_meta_description">This is the homepage of the website</field>
   </record>
 </odoo>
```

## odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/upgrade_analysis.txt

```diff
@@ -19,18 +19,124 @@
 ---XML records in module 'website'---
 NEW ir.actions.act_window: website.action_website_controller_pages_list
 DEL ir.actions.act_window: website.action_show_viewhierarchy
 NEW ir.actions.client: website.action_website_view_hierarchy
 NEW ir.asset: website.s_instagram_page_000_js
 NEW ir.asset: website.s_instagram_page_000_scss
 NEW ir.asset: website.s_text_cover_000_scss
-NEW ir.attachment: website.library_image_team (noupdate)
-NEW ir.attachment: website.s_banner_default_image_2 (noupdate)
-NEW ir.attachment: website.s_banner_default_image_3 (noupdate)
-NEW ir.attachment: website.s_text_cover_default_image (noupdate)
+ir.attachment: website.business_conference (noupdate switched)
+ir.attachment: website.header_image_1_default_image (noupdate switched)
+ir.attachment: website.library_image_01 (noupdate switched)
+ir.attachment: website.library_image_02 (noupdate switched)
+ir.attachment: website.library_image_03 (noupdate switched)
+ir.attachment: website.library_image_04 (noupdate switched)
+ir.attachment: website.library_image_05 (noupdate switched)
+ir.attachment: website.library_image_06 (noupdate switched)
+ir.attachment: website.library_image_07 (noupdate switched)
+ir.attachment: website.library_image_08 (noupdate switched)
+ir.attachment: website.library_image_09 (noupdate switched)
+ir.attachment: website.library_image_10 (noupdate switched)
+ir.attachment: website.library_image_11 (noupdate switched)
+ir.attachment: website.library_image_12 (noupdate switched)
+ir.attachment: website.library_image_13 (noupdate switched)
+ir.attachment: website.library_image_14 (noupdate switched)
+ir.attachment: website.library_image_15 (noupdate switched)
+ir.attachment: website.library_image_16 (noupdate switched)
+ir.attachment: website.library_image_17 (noupdate switched)
+ir.attachment: website.library_image_18 (noupdate switched)
+NEW ir.attachment: website.library_image_team
+ir.attachment: website.s_background_image_01 (noupdate switched)
+ir.attachment: website.s_background_image_02 (noupdate switched)
+ir.attachment: website.s_background_image_03 (noupdate switched)
+ir.attachment: website.s_background_image_04 (noupdate switched)
+ir.attachment: website.s_background_image_05 (noupdate switched)
+ir.attachment: website.s_background_image_06 (noupdate switched)
+ir.attachment: website.s_background_image_07 (noupdate switched)
+ir.attachment: website.s_background_image_08 (noupdate switched)
+ir.attachment: website.s_background_image_09 (noupdate switched)
+ir.attachment: website.s_banner_default_image (noupdate switched)
+NEW ir.attachment: website.s_banner_default_image_2
+NEW ir.attachment: website.s_banner_default_image_3
+ir.attachment: website.s_blockquote_cover_default_image (noupdate switched)
+ir.attachment: website.s_blockquote_default_image (noupdate switched)
+ir.attachment: website.s_carousel_default_image_1 (noupdate switched)
+ir.attachment: website.s_carousel_default_image_2 (noupdate switched)
+ir.attachment: website.s_carousel_default_image_3 (noupdate switched)
+ir.attachment: website.s_company_team_image_1 (noupdate switched)
+ir.attachment: website.s_company_team_image_2 (noupdate switched)
+ir.attachment: website.s_company_team_image_3 (noupdate switched)
+ir.attachment: website.s_company_team_image_4 (noupdate switched)
+ir.attachment: website.s_cover_default_image (noupdate switched)
+ir.attachment: website.s_image_text_default_image (noupdate switched)
+ir.attachment: website.s_masonry_block_default_image_1 (noupdate switched)
+ir.attachment: website.s_masonry_block_default_image_2 (noupdate switched)
+ir.attachment: website.s_media_list_default_image_1 (noupdate switched)
+ir.attachment: website.s_media_list_default_image_2 (noupdate switched)
+ir.attachment: website.s_media_list_default_image_3 (noupdate switched)
+ir.attachment: website.s_mega_menu_cards_default_image_1 (noupdate switched)
+ir.attachment: website.s_mega_menu_cards_default_image_2 (noupdate switched)
+ir.attachment: website.s_mega_menu_cards_default_image_3 (noupdate switched)
+ir.attachment: website.s_mega_menu_cards_default_image_4 (noupdate switched)
+ir.attachment: website.s_mega_menu_cards_default_image_5 (noupdate switched)
+ir.attachment: website.s_mega_menu_cards_default_image_6 (noupdate switched)
+ir.attachment: website.s_mega_menu_cards_default_image_7 (noupdate switched)
+ir.attachment: website.s_mega_menu_cards_default_image_8 (noupdate switched)
+ir.attachment: website.s_mega_menu_images_subtitles_default_image_1 (noupdate switched)
+ir.attachment: website.s_mega_menu_images_subtitles_default_image_2 (noupdate switched)
+ir.attachment: website.s_mega_menu_images_subtitles_default_image_3 (noupdate switched)
+ir.attachment: website.s_mega_menu_images_subtitles_default_image_4 (noupdate switched)
+ir.attachment: website.s_mega_menu_images_subtitles_default_image_5 (noupdate switched)
+ir.attachment: website.s_mega_menu_images_subtitles_default_image_6 (noupdate switched)
+ir.attachment: website.s_mega_menu_images_subtitles_default_image_7 (noupdate switched)
+ir.attachment: website.s_mega_menu_menu_image_menu_default_image (noupdate switched)
+ir.attachment: website.s_mega_menu_menus_logos_default_image (noupdate switched)
+ir.attachment: website.s_mega_menu_menus_logos_default_logo_1 (noupdate switched)
+ir.attachment: website.s_mega_menu_menus_logos_default_logo_2 (noupdate switched)
+ir.attachment: website.s_mega_menu_menus_logos_default_logo_3 (noupdate switched)
+ir.attachment: website.s_mega_menu_menus_logos_default_logo_4 (noupdate switched)
+ir.attachment: website.s_mega_menu_menus_logos_default_logo_5 (noupdate switched)
+ir.attachment: website.s_mega_menu_menus_logos_default_logo_6 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_1 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_10 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_11 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_2 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_3 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_4 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_5 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_6 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_7 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_8 (noupdate switched)
+ir.attachment: website.s_mega_menu_thumbnails_default_image_9 (noupdate switched)
+ir.attachment: website.s_parallax_default_image (noupdate switched)
+ir.attachment: website.s_picture_default_image (noupdate switched)
+ir.attachment: website.s_popup_default_image (noupdate switched)
+ir.attachment: website.s_product_catalog_default_image (noupdate switched)
+ir.attachment: website.s_product_list_default_image_1 (noupdate switched)
+ir.attachment: website.s_product_list_default_image_2 (noupdate switched)
+ir.attachment: website.s_product_list_default_image_3 (noupdate switched)
+ir.attachment: website.s_product_list_default_image_4 (noupdate switched)
+ir.attachment: website.s_product_list_default_image_5 (noupdate switched)
+ir.attachment: website.s_product_list_default_image_6 (noupdate switched)
+ir.attachment: website.s_quotes_carousel_demo_image_0 (noupdate switched)
+ir.attachment: website.s_quotes_carousel_demo_image_1 (noupdate switched)
+ir.attachment: website.s_quotes_carousel_demo_image_2 (noupdate switched)
+ir.attachment: website.s_quotes_carousel_demo_image_3 (noupdate switched)
+ir.attachment: website.s_quotes_carousel_demo_image_4 (noupdate switched)
+ir.attachment: website.s_quotes_carousel_demo_image_5 (noupdate switched)
+ir.attachment: website.s_reference_default_image_6 (noupdate switched)
+ir.attachment: website.s_reference_demo_image_1 (noupdate switched)
+ir.attachment: website.s_reference_demo_image_2 (noupdate switched)
+ir.attachment: website.s_reference_demo_image_3 (noupdate switched)
+ir.attachment: website.s_reference_demo_image_4 (noupdate switched)
+ir.attachment: website.s_reference_demo_image_5 (noupdate switched)
+NEW ir.attachment: website.s_text_cover_default_image
+ir.attachment: website.s_text_image_default_image (noupdate switched)
+ir.attachment: website.s_three_columns_default_image_1 (noupdate switched)
+ir.attachment: website.s_three_columns_default_image_2 (noupdate switched)
+ir.attachment: website.s_three_columns_default_image_3 (noupdate switched)
 NEW ir.model.access: website.access_seo_public_employee
 NEW ir.model.access: website.access_seo_public_portal
 NEW ir.model.access: website.access_seo_public_public
 NEW ir.model.access: website.access_website_controller_page_designer
 NEW ir.model.access: website.access_website_controller_page_public
 NEW ir.model.access: website.access_website_menu_employee
 NEW ir.model.access: website.access_website_menu_portal
@@ -38,17 +144,14 @@
 NEW ir.model.access: website.access_website_public_employee
 NEW ir.model.access: website.access_website_public_portal
 NEW ir.model.access: website.access_website_public_public
 DEL ir.model.access: website.access_seo_public
 DEL ir.model.access: website.access_website_menu
 DEL ir.model.access: website.access_website_page
 DEL ir.model.access: website.access_website_public
-DEL ir.model.constraint: website.constraint_res_users_login_key
-DEL ir.model.constraint: website.constraint_website_domain_unique
-DEL ir.model.constraint: website.constraint_website_visitor_access_token_unique
 NEW ir.rule: website.website_page_controller_rule_public
 NEW ir.ui.menu: website.menu_website_controller_pages_list
 NEW ir.ui.view: website.column_count_option
 NEW ir.ui.view: website.footer_language_selector_code
 NEW ir.ui.view: website.grid_layout_options
 NEW ir.ui.view: website.header_call_to_action_large
 NEW ir.ui.view: website.header_call_to_action_sidebar
```

## odoo/addons/openupgrade_scripts/scripts/website_blog/17.0.1.1/upgrade_analysis.txt

```diff
@@ -17,9 +17,7 @@
 NEW ir.model.access: website_blog.blog_tag_employee
 NEW ir.model.access: website_blog.blog_tag_portal
 NEW ir.model.access: website_blog.blog_tag_public
 DEL ir.model.access: website_blog.blog_blog_all
 DEL ir.model.access: website_blog.blog_post_all
 DEL ir.model.access: website_blog.blog_tag
 DEL ir.model.access: website_blog.blog_tag_category_all
-DEL ir.model.constraint: website_blog.constraint_blog_tag_category_name_uniq
-DEL ir.model.constraint: website_blog.constraint_blog_tag_name_uniq
```

## odoo/addons/openupgrade_scripts/scripts/website_crm_iap_reveal/17.0.1.1/upgrade_analysis.txt

```diff
@@ -1,4 +1,4 @@
 ---Models in module 'website_crm_iap_reveal'---
 ---Fields in module 'website_crm_iap_reveal'---
 ---XML records in module 'website_crm_iap_reveal'---
-DEL ir.model.constraint: website_crm_iap_reveal.constraint_crm_reveal_rule_limit_extra_contacts
+---nothing has changed in this module--
```

## odoo/addons/openupgrade_scripts/scripts/website_event/17.0.1.4/upgrade_analysis.txt

```diff
@@ -68,14 +68,15 @@
 NEW ir.model.access: website_event.access_website_event_menu_portal
 NEW ir.model.access: website_event.access_website_event_menu_public
 DEL ir.model.access: website_event.access_event_event
 DEL ir.model.access: website_event.access_event_event_ticket
 DEL ir.model.access: website_event.access_event_tag
 DEL ir.model.access: website_event.access_event_tag_category
 DEL ir.model.access: website_event.access_website_event_menu
+NEW ir.model.constraint: website_event.constraint_event_registration_answer_value_check [renamed from website_event_questions module]
 NEW ir.rule: website_event.ir_rule_event_question_answer_event_user [renamed from website_event_questions module] (noupdate)
 NEW ir.rule: website_event.ir_rule_event_question_answer_published [renamed from website_event_questions module] (noupdate)
 NEW ir.rule: website_event.ir_rule_event_question_event_user [renamed from website_event_questions module] (noupdate)
 NEW ir.rule: website_event.ir_rule_event_question_published [renamed from website_event_questions module] (noupdate)
 NEW ir.ui.view: website_event.event_empty_events_svg
 NEW ir.ui.view: website_event.event_question_view_form
 NEW ir.ui.view: website_event.event_registration_answer_view_graph
```

## odoo/addons/openupgrade_scripts/scripts/website_event_track/17.0.1.3/upgrade_analysis.txt

```diff
@@ -15,8 +15,7 @@
 NEW ir.model.access: website_event_track.access_event_track_tag_portal
 NEW ir.model.access: website_event_track.access_event_track_tag_public
 DEL ir.model.access: website_event_track.access_event_track
 DEL ir.model.access: website_event_track.access_event_track_location
 DEL ir.model.access: website_event_track.access_event_track_stage
 DEL ir.model.access: website_event_track.access_event_track_tag
 DEL ir.model.access: website_event_track.access_event_track_tag_category
-DEL ir.model.constraint: website_event_track.constraint_event_track_tag_name_uniq
```

## odoo/addons/openupgrade_scripts/scripts/website_forum/17.0.1.2/upgrade_analysis.txt

```diff
@@ -27,16 +27,14 @@
 DEL ir.actions.act_window: website_forum.action_forum_post
 DEL ir.actions.act_window: website_forum.action_forum_posts
 DEL ir.actions.act_window: website_forum.forum_post_reasons_action
 NEW ir.model.access: website_forum.access_forum_forum_employee
 NEW ir.model.access: website_forum.access_forum_forum_portal
 NEW ir.model.access: website_forum.access_forum_forum_public
 DEL ir.model.access: website_forum.access_forum_forum
-DEL ir.model.constraint: website_forum.constraint_forum_post_vote_vote_uniq
-DEL ir.model.constraint: website_forum.constraint_forum_tag_name_uniq
 NEW ir.ui.view: website_forum.follow
 NEW ir.ui.view: website_forum.forum_forum_view_form
 NEW ir.ui.view: website_forum.forum_forum_view_search
 NEW ir.ui.view: website_forum.forum_forum_view_tree
 NEW ir.ui.view: website_forum.forum_index_tags
 NEW ir.ui.view: website_forum.forum_model_nav
 NEW ir.ui.view: website_forum.forum_post_view_form (noupdate)
```

## odoo/addons/openupgrade_scripts/scripts/website_sale/17.0.1.1/upgrade_analysis.txt

```diff
@@ -1,26 +1,32 @@
 ---Models in module 'website_sale'---
 ---Fields in module 'website_sale'---
+website_sale / delivery.carrier         / can_publish (boolean)         : previously in module website_sale_delivery
+website_sale / delivery.carrier         / is_published (boolean)        : previously in module website_sale_delivery
+website_sale / delivery.carrier         / website_description (text)    : previously in module website_sale_delivery
+website_sale / delivery.carrier         / website_id (many2one)         : previously in module website_sale_delivery
+website_sale / delivery.carrier         / website_published (boolean)   : previously in module website_sale_delivery
+website_sale / delivery.carrier         / website_url (char)            : previously in module website_sale_delivery
 website_sale / product.document         / shown_on_product_page (boolean): NEW
 website_sale / product.product          / rating_ids (one2many)         : is now stored
 website_sale / product.product          / rating_ids (one2many)         : module is now 'rating' ('website_sale')
 website_sale / product.product          / rating_ids (one2many)         : not related anymore
 website_sale / product.product          / ribbon_id (many2one)          : NEW relation: product.ribbon
 website_sale / product.ribbon           / product_tag_ids (one2many)    : DEL relation: product.tag
 website_sale / product.tag              / image (binary)                : NEW attachment: True
 website_sale / product.tag              / ribbon_id (many2one)          : DEL relation: product.ribbon
 website_sale / product.tag              / visible_on_ecommerce (boolean): NEW hasdefault: default
 website_sale / product.template         / description_ecommerce (html)  : NEW
 website_sale / product.template         / rating_ids (one2many)         : module is now 'rating' ('website_sale')
 website_sale / res.company              / website_sale_onboarding_payment_provider_state (selection): DEL selection_keys: ['done', 'just_done', 'not_done']
 website_sale / sale.order               / access_point_address (json)   : NEW
+website_sale / sale.order               / amount_delivery (float)       : previously in module website_sale_delivery
 website_sale / website                  / currency_id (many2one)        : not related anymore
 website_sale / website                  / currency_id (many2one)        : now a function
 website_sale / website                  / show_line_subtotals_tax_selection (selection): NEW required, selection_keys: ['tax_excluded', 'tax_included'], hasdefault: default
-website_sale_delivery / sale.order               / amount_delivery (float)       : not stored anymore
 ---XML records in module 'website_sale'---
 DEL ir.actions.act_window: website_sale.action_invoices_ecommerce
 DEL ir.actions.act_window: website_sale.product_public_tags_action
 DEL ir.actions.act_window: website_sale.website_product_pricelist3
 NEW ir.asset: website_sale.s_popup_000_js
 NEW ir.model.access: website_sale.access_ecom_extra_fields_public_employee
 NEW ir.model.access: website_sale.access_ecom_extra_fields_public_portal
@@ -86,15 +92,14 @@
 DEL ir.model.access: website_sale.access_product_template_attribute_line_public
 DEL ir.model.access: website_sale.access_product_template_public
 DEL ir.model.access: website_sale.access_website_base_unit_public
 NEW ir.ui.menu: website_sale.menu_delivery_zip_prefix
 NEW ir.ui.menu: website_sale.menu_ecommerce_delivery [renamed from website_sale_delivery module]
 NEW ir.ui.menu: website_sale.menu_ecommerce_payment_methods
 DEL ir.ui.menu: website_sale.menu_ecommerce_payment_icons
-DEL ir.ui.menu: website_sale_delivery.menu_ecommerce_delivery [renamed to website_sale module]
 NEW ir.ui.view: website_sale.accept_terms_and_conditions
 NEW ir.ui.view: website_sale.badge_extra_price
 NEW ir.ui.view: website_sale.cart_delivery
 NEW ir.ui.view: website_sale.checkout_layout
 NEW ir.ui.view: website_sale.filter_products_tags
 NEW ir.ui.view: website_sale.filter_products_tags_list
 NEW ir.ui.view: website_sale.navigation_buttons
@@ -130,15 +135,7 @@
 DEL ir.ui.view: website_sale.template_header_contact
 DEL ir.ui.view: website_sale.template_header_hamburger_full
 DEL ir.ui.view: website_sale.template_header_image
 DEL ir.ui.view: website_sale.template_header_magazine
 DEL ir.ui.view: website_sale.template_header_slogan
 DEL ir.ui.view: website_sale.view_order_tree
 DEL ir.ui.view: website_sale.view_quotation_tree
-DEL ir.ui.view: website_sale_delivery.cart_delivery
-DEL ir.ui.view: website_sale_delivery.payment_delivery
-DEL ir.ui.view: website_sale_delivery.payment_delivery_methods
-DEL ir.ui.view: website_sale_delivery.payment_delivery_shipping_method
-DEL ir.ui.view: website_sale_delivery.res_config_settings_view_form
-DEL ir.ui.view: website_sale_delivery.view_delivery_carrier_form_website_delivery
-DEL ir.ui.view: website_sale_delivery.view_delivery_carrier_search_inherit_website_sale_delivery
-DEL ir.ui.view: website_sale_delivery.view_delivery_carrier_tree_inherit_website_sale_delivery
```

## odoo/addons/openupgrade_scripts/scripts/website_sale_mondialrelay/17.0.0.1/upgrade_analysis.txt

```diff
@@ -1,12 +1,7 @@
 ---Models in module 'website_sale_mondialrelay'---
 ---Fields in module 'website_sale_mondialrelay'---
 ---XML records in module 'website_sale_mondialrelay'---
 NEW ir.ui.view: website_sale_mondialrelay.delivery_carrier_view_search
 NEW ir.ui.view: website_sale_mondialrelay.res_config_settings_view_form
 NEW ir.ui.view: website_sale_mondialrelay.website_sale_mondialrelay_address_kanban
 NEW ir.ui.view: website_sale_mondialrelay.website_sale_mondialrelay_address_on_payment
-DEL ir.ui.view: website_sale_delivery_mondialrelay.delivery_carrier_view_search_inherit_website_sale_delivery_mondialrelay
-DEL ir.ui.view: website_sale_delivery_mondialrelay.res_config_settings_view_form_inherit_website_sale_delivery_mondial_relay
-DEL ir.ui.view: website_sale_delivery_mondialrelay.website_sale_delivery_mondialrelay_address_kanban
-DEL ir.ui.view: website_sale_delivery_mondialrelay.website_sale_delivery_mondialrelay_address_on_payment
-DEL ir.ui.view: website_sale_delivery_mondialrelay.website_sale_delivery_mondialrelay_checkout
```

## odoo/addons/openupgrade_scripts/scripts/website_sale_product_configurator/17.0.1.0/upgrade_analysis.txt

```diff
@@ -4,8 +4,7 @@
 NEW ir.ui.view: website_sale_product_configurator.configure_optional_products
 NEW ir.ui.view: website_sale_product_configurator.optional_product_items
 NEW ir.ui.view: website_sale_product_configurator.optional_products_modal
 NEW ir.ui.view: website_sale_product_configurator.product_quantity_config
 DEL ir.ui.view: website_sale_product_configurator.configure_optional_products_website
 DEL ir.ui.view: website_sale_product_configurator.optional_product_items_website
 DEL ir.ui.view: website_sale_product_configurator.product_quantity_config_website
-DEL ir.ui.view: website_sale_stock_product_configurator.website_sale_stock_modal
```

## odoo/addons/openupgrade_scripts/scripts/website_sale_slides/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,5 +1,4 @@
 ---Models in module 'website_sale_slides'---
 ---Fields in module 'website_sale_slides'---
 website_sale_slides / product.template         / detailed_type (False)         : selection_keys is now '['combo', 'consu', 'course', 'event', 'event_booth', 'product', 'service']' ('['consu', 'course', 'event', 'product', 'service']')
 ---XML records in module 'website_sale_slides'---
-DEL ir.model.constraint: website_sale_slides.constraint_slide_channel_product_id_check
```

## odoo/addons/openupgrade_scripts/scripts/website_sale_wishlist/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,11 +1,10 @@
 ---Models in module 'website_sale_wishlist'---
 ---Fields in module 'website_sale_wishlist'---
 ---XML records in module 'website_sale_wishlist'---
-DEL ir.model.constraint: website_sale_wishlist.constraint_product_wishlist_product_unique_partner_id
 NEW ir.ui.view: website_sale_wishlist.template_header_mobile
 NEW ir.ui.view: website_sale_wishlist.template_header_sales_four
 NEW ir.ui.view: website_sale_wishlist.template_header_sales_one
 NEW ir.ui.view: website_sale_wishlist.template_header_sales_three
 NEW ir.ui.view: website_sale_wishlist.template_header_sales_two
 NEW ir.ui.view: website_sale_wishlist.template_header_search
 NEW ir.ui.view: website_sale_wishlist.template_header_stretch
```

## odoo/addons/openupgrade_scripts/scripts/website_slides/17.0.2.7/upgrade_analysis.txt

```diff
@@ -45,22 +45,15 @@
 DEL ir.model.access: website_slides.access_slide_channel_all
 DEL ir.model.access: website_slides.access_slide_channel_tag_all
 DEL ir.model.access: website_slides.access_slide_channel_tag_group_all
 DEL ir.model.access: website_slides.access_slide_embed_all
 DEL ir.model.access: website_slides.access_slide_question_all
 DEL ir.model.access: website_slides.access_slide_slide_all
 DEL ir.model.access: website_slides.access_slide_tag_all
-DEL ir.model.constraint: website_slides.constraint_slide_channel_partner_channel_partner_uniq
-DEL ir.model.constraint: website_slides.constraint_slide_channel_partner_check_completion
-DEL ir.model.constraint: website_slides.constraint_slide_slide_exclusion_html_content_and_url
-DEL ir.model.constraint: website_slides.constraint_slide_slide_partner_check_vote
-DEL ir.model.constraint: website_slides.constraint_slide_slide_partner_slide_partner_uniq
-DEL ir.model.constraint: website_slides.constraint_slide_slide_resource_check_file_type
-DEL ir.model.constraint: website_slides.constraint_slide_slide_resource_check_url
-DEL ir.model.constraint: website_slides.constraint_slide_tag_slide_tag_unique
+NEW ir.model.constraint: website_slides.constraint_slide_channel_check_enroll
 NEW ir.rule: website_slides.rule_slide_channel_visibility_public_user (noupdate)
 NEW ir.rule: website_slides.rule_slide_channel_visibility_signed_in_user (noupdate)
 NEW ir.rule: website_slides.rule_slide_slide_public_user (noupdate)
 NEW ir.rule: website_slides.rule_slide_slide_signed_in_user (noupdate)
 DEL ir.rule: website_slides.rule_slide_channel_not_website (noupdate)
 DEL ir.rule: website_slides.rule_slide_slide_not_website (noupdate)
 NEW ir.ui.view: website_slides.course_slides_list_placeholder
```

## odoo/addons/openupgrade_scripts/scripts/website_slides_forum/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,11 +1,10 @@
 ---Models in module 'website_slides_forum'---
 ---Fields in module 'website_slides_forum'---
 website_slides_forum / forum.forum              / image_1920 (False)            : NEW mode: modify, hasdefault: compute
 ---XML records in module 'website_slides_forum'---
-DEL ir.model.constraint: website_slides_forum.constraint_slide_channel_forum_uniq
 NEW ir.rule: website_slides_forum.website_slides_forum_post_signed_in_user (noupdate)
 NEW ir.rule: website_slides_forum.website_slides_forum_signed_in_user (noupdate)
 NEW ir.rule: website_slides_forum.website_slides_forum_tag_signed_in_user (noupdate)
 NEW ir.ui.view: website_slides_forum.forum_all_all_entries
 NEW ir.ui.view: website_slides_forum.website_slides_forum_breadcrumb
 DEL ir.ui.view: website_slides_forum.website_slides_forum_header
```

## odoo/addons/openupgrade_scripts/scripts/website_slides_survey/17.0.1.0/upgrade_analysis.txt

```diff
@@ -1,6 +1,4 @@
 ---Models in module 'website_slides_survey'---
 ---Fields in module 'website_slides_survey'---
 ---XML records in module 'website_slides_survey'---
-DEL ir.model.constraint: website_slides_survey.constraint_slide_slide_check_certification_preview
-DEL ir.model.constraint: website_slides_survey.constraint_slide_slide_check_survey_id
 DEL ir.ui.view: website_slides_survey.slide_icon_inherit_survey
```

## Comparing `odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/METADATA` & `odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addon-openupgrade_scripts
-Version: 17.0.1.0.1.2
+Version: 17.0.1.0.1.3
 Requires-Python: >=3.10
 Requires-Dist: odoo>=17.0a,<17.1dev
 Requires-Dist: openupgradelib
 Summary: Module that contains all the migrations analysis and scripts for migrate Odoo SA modules.
 Home-page: https://github.com/OCA/OpenUpgrade
 License: AGPL-3
 Author: Odoo Community Association (OCA)
```

## Comparing `odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/RECORD` & `odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,158 +1,171 @@
 odoo/addons/openupgrade_scripts/README.rst,sha256=F-NgZfCSC-In2HctZruRu5RXLtEBFegzZYW5KpobcWU,3182
 odoo/addons/openupgrade_scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 odoo/addons/openupgrade_scripts/__manifest__.py,sha256=7Yx2vwKl2vEHnUbDuuTprHLg2oQrKQMkpWEfyFneA0Q,614
 odoo/addons/openupgrade_scripts/apriori.py,sha256=TzllFdpnxImAmChrKjrKW9t2-AqEpTwdpWA5F6TjDSM,1591
 odoo/addons/openupgrade_scripts/readme/CONFIGURE.md,sha256=rnx8ADTYzVUB93PIG3Lib0iWBrphSfVRs6RMikklf3M,238
 odoo/addons/openupgrade_scripts/readme/DESCRIPTION.md,sha256=HPjPs_KluLFMYXPaJcnoneY8BAh-XPwEAP71I7VTTbo,86
 odoo/addons/openupgrade_scripts/readme/INSTALL.md,sha256=NDKVZRv0J8BTqcSTD7JwUXL_AY-cDJoegn5IUTbEOFk,113
-odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/noupdate_changes.xml,sha256=q0BQyYFdqLTMc_9qMzhjlAcD4lKwASCdpskQyeqBP78,8333
-odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/upgrade_analysis.txt,sha256=J_alkLv7DEl3HkhRGwNsBSK383zk4gmaT784EWxhf98,37610
+odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/noupdate_changes.xml,sha256=B-xlSUOS9JtZsLSCDGiGF4Fi8WzHrxIWiO05nmV9P-o,8378
+odoo/addons/openupgrade_scripts/scripts/account/17.0.1.2/upgrade_analysis.txt,sha256=URTXWBpBpRhfCg-0GQzvSpfC3VnkpF9bYvKISfAJcKk,36863
 odoo/addons/openupgrade_scripts/scripts/account_audit_trail/17.0.1.0/upgrade_analysis.txt,sha256=6W6bG6eWaZn1NGmjGLO1G_h7nmbqvO5_yNNIFGP3RUc,601
 odoo/addons/openupgrade_scripts/scripts/account_check_printing/17.0.1.0/upgrade_analysis.txt,sha256=LLJ88stlAeeCNgxAIiORZjQjbY-Sir138GI_FBpjIeE,189
 odoo/addons/openupgrade_scripts/scripts/account_debit_note/17.0.1.0/upgrade_analysis.txt,sha256=oir9cI7nADk67Hu51_8WZ6zg6obvGn-KZ8nC_85RKwQ,202
 odoo/addons/openupgrade_scripts/scripts/account_edi/17.0.1.0/noupdate_changes.xml,sha256=hZQIaHT1HSoT2REXWCzUI5eJYPvdyizNEE0KE6w4kmY,186
 odoo/addons/openupgrade_scripts/scripts/account_edi/17.0.1.0/upgrade_analysis.txt,sha256=zTxmxvBq8XHAIjUuiae3lg1Ooeu02jfwPEfz3cb-joo,429
-odoo/addons/openupgrade_scripts/scripts/account_edi_proxy_client/17.0.1.0/upgrade_analysis.txt,sha256=uMneajXOA2q-LwUgMzhCNyXOJkOOrXMP5JMQudrHdic,785
+odoo/addons/openupgrade_scripts/scripts/account_edi_proxy_client/17.0.1.0/upgrade_analysis.txt,sha256=AgcygzVKbroOjZcAsz3zN9YdS-Jy_qiAzCkhFJNOh3E,920
 odoo/addons/openupgrade_scripts/scripts/account_edi_ubl_cii/17.0.1.0/upgrade_analysis.txt,sha256=81G1mgzvO3cUftEVcJL9yRQ1Vj5bMYq2siU3nqkX3sI,3209
 odoo/addons/openupgrade_scripts/scripts/account_fleet/17.0.1.0/upgrade_analysis.txt,sha256=4ACWUpmQ7qvzWsQSP3Z3qbz5Z3YpOFAN7V5wC69WxmA,162
-odoo/addons/openupgrade_scripts/scripts/account_payment/17.0.2.0/upgrade_analysis.txt,sha256=WTLNOTe71aYwbIyyC8xdkJFVdu49j9rSirTfziwxJeQ,1228
+odoo/addons/openupgrade_scripts/scripts/account_payment/17.0.2.0/upgrade_analysis.txt,sha256=HlVJTXAJ1bU3dcKyp8D8hAKYCjNo3tCOUsiW4k6hmk4,908
 odoo/addons/openupgrade_scripts/scripts/account_payment_term/17.0.1.0/upgrade_analysis.txt,sha256=Cx9wSdzYjFyaVjVjQQaIad_o7GCftb3Chh8eL-QH1zI,532
-odoo/addons/openupgrade_scripts/scripts/account_peppol/17.0.1.0/upgrade_analysis.txt,sha256=EnqykoQQyEjQwXcuhLPZ1iMuvldOEzp12sxI5cqSjrc,2637
+odoo/addons/openupgrade_scripts/scripts/account_peppol/17.0.1.0/upgrade_analysis.txt,sha256=DOMUCypS5DmUrB45tdKImXpSXdJkzm7zZBH76QGu-b0,2666
 odoo/addons/openupgrade_scripts/scripts/account_qr_code_emv/17.0.1.0/upgrade_analysis.txt,sha256=RKD_mJf90K267j-Rvq-dAocXkgXv64i3DPWm42acxtU,516
 odoo/addons/openupgrade_scripts/scripts/account_tax_python/17.0.1.0/upgrade_analysis.txt,sha256=71VQVnwf1DecQpUjgJWr_6BPWXRJmEjT63S8AtDpHRM,469
 odoo/addons/openupgrade_scripts/scripts/analytic/17.0.1.1/upgrade_analysis.txt,sha256=QvqEqA2DKpDqb3U2ZI27zTnIBBUGG3TZFqE4jSjYGlQ,1252
 odoo/addons/openupgrade_scripts/scripts/auth_ldap/17.0.1.0/upgrade_analysis.txt,sha256=QB9DfdWzmE0oR4fsd-qPQ9JF5W_uZFNYpvKmNVs_TZw,150
-odoo/addons/openupgrade_scripts/scripts/auth_oauth/17.0.1.0/upgrade_analysis.txt,sha256=FB7tQGprcxaSIFMUqJW0ZS3jbMRMyCdXQtMPayIhHZs,206
+odoo/addons/openupgrade_scripts/scripts/auth_oauth/17.0.1.0/upgrade_analysis.txt,sha256=FxJ3tHzlvJtzEN8spiXAXZf7832DrzQ71MkfayvDt_o,153
 odoo/addons/openupgrade_scripts/scripts/auth_signup/17.0.1.0/noupdate_changes.xml,sha256=V7cwFVd1beUN7HYPkT1KB1HHc7WVwtPe0LWviVylITA,12678
 odoo/addons/openupgrade_scripts/scripts/auth_signup/17.0.1.0/upgrade_analysis.txt,sha256=EKdCu5FHnTUpceYltMg4yhM8I0IwbuohkoVBa8SWK54,279
 odoo/addons/openupgrade_scripts/scripts/auth_totp/17.0.1.0/upgrade_analysis.txt,sha256=kM7HlwgVRwa67MFDCi_fRAf8vNOzdUTK-xEHI5lkajo,150
 odoo/addons/openupgrade_scripts/scripts/auth_totp_mail/17.0.1.0/upgrade_analysis.txt,sha256=_wKImBYVLiHWkRoeKbDLt1YTXQ49JmgTgnMWKynCDlE,188
 odoo/addons/openupgrade_scripts/scripts/auth_totp_mail_enforce/17.0.1.0/upgrade_analysis.txt,sha256=FMeF8St_Piud_mwB9YE4jRpVTa--NsX0-TgUzamELME,189
 odoo/addons/openupgrade_scripts/scripts/barcodes/17.0.2.0/upgrade_analysis.txt,sha256=aVHHJpenY6xHfF_YxGygdm9MRLo165JzMd-zXtDl1nE,147
 odoo/addons/openupgrade_scripts/scripts/barcodes_gs1_nomenclature/17.0.1.0/upgrade_analysis.txt,sha256=M2_LcBV8IPACyjPo3ecgVy7GSuyFITBZRojGfi37HM4,198
-odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/noupdate_changes.xml,sha256=8YYHYTRnlgHsx4vaRAROIhVGzeBz5-5jMgeQlCnN1zU,1097
-odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_analysis.txt,sha256=FAGNfntq5ZjGD8YLx55Cv9kYrIr3li_dVgD0sEeJzTo,13341
-odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_general_log.txt,sha256=8OSatT9xO5ZdhA_HxYn-K5S7rTWM1HBxvCHFGxHrxhQ,47834
+odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/noupdate_changes.xml,sha256=QAH6Unq3OPunRldIzwASK96dLPWAOgIDs16_PglRF8g,1372
+odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_analysis.txt,sha256=Sh7c1180mPs3FneWBGCNYSMcKqEkZ0P5KybAhtxYFPc,13821
+odoo/addons/openupgrade_scripts/scripts/base/17.0.1.3/upgrade_general_log.txt,sha256=bj1xexwv7w-E0CiP2V_KqIGER5Hkavr3agJrmldkJVs,293354
 odoo/addons/openupgrade_scripts/scripts/base_address_extended/17.0.1.1/upgrade_analysis.txt,sha256=ASu66ZAbmDdq4hDHw_jHbavco76PjR0kFfvKSZ0bSI4,198
 odoo/addons/openupgrade_scripts/scripts/base_automation/17.0.1.0/noupdate_changes.xml,sha256=JUepQ4WdQ8g01-jvRxEW2ZEl_jjZWqyCUGu6wU6DutI,200
 odoo/addons/openupgrade_scripts/scripts/base_automation/17.0.1.0/upgrade_analysis.txt,sha256=HnBmJd91LSYEPhwYRffQFxA5-v4YvON5WlATvJzUJiQ,2474
 odoo/addons/openupgrade_scripts/scripts/base_geolocalize/17.0.2.1/upgrade_analysis.txt,sha256=Bm_lKaW84WXUAyI49HewdVmRG2HmHhLEP2xz5_e7t6M,187
 odoo/addons/openupgrade_scripts/scripts/base_import/17.0.2.0/upgrade_analysis.txt,sha256=_u8p6w0pKHUhdUA_nsWTKTEdeGDWhQpFtIS9YOMG5xE,4560
 odoo/addons/openupgrade_scripts/scripts/base_import_module/17.0.1.0/upgrade_analysis.txt,sha256=Lr2II0Q7Iv_ZrO02UctYuhPZ0-JjmdJYXbUvviD6v-Q,539
 odoo/addons/openupgrade_scripts/scripts/base_install_request/17.0.1.0/upgrade_analysis.txt,sha256=88mf6PwlB0WGU_7_cN4QwNbb7uKIHWsh7ItFr4YMsEQ,183
 odoo/addons/openupgrade_scripts/scripts/base_sparse_field/17.0.1.0/upgrade_analysis.txt,sha256=shg-2JSIpxi-K20IWUbWROaY5CNsHdGaBUbNizYU8dk,174
 odoo/addons/openupgrade_scripts/scripts/base_vat/17.0.1.0/upgrade_analysis.txt,sha256=GVnmfjEfyKFByPEzjHMjv7unM_s--dfvLeVfptPRADU,283
 odoo/addons/openupgrade_scripts/scripts/board/17.0.1.0/noupdate_changes.xml,sha256=_6VDikhTEqo0Zkm2PiW8qmFOc2VR5MoXEu-lTgAf0GY,198
 odoo/addons/openupgrade_scripts/scripts/board/17.0.1.0/upgrade_analysis.txt,sha256=Xl5TzyuBSsACKcv80s8z9wRqjM0jzYLnryGXjsa_H6A,138
 odoo/addons/openupgrade_scripts/scripts/bus/17.0.1.0/upgrade_analysis.txt,sha256=SPdBhavq0qsW3s3Uj-NEYd5ba_DDDwkvoVXy6NBbxfA,132
-odoo/addons/openupgrade_scripts/scripts/calendar/17.0.1.1/noupdate_changes.xml,sha256=6ehU4AnTpko_ZElLkNMSup8BNFQoflpSuo520LsIldU,23184
+odoo/addons/openupgrade_scripts/scripts/calendar/17.0.1.1/noupdate_changes.xml,sha256=QDtRQpvidkYIghSt_LecB0564FYjAiyppsfxElOSxG0,16199
 odoo/addons/openupgrade_scripts/scripts/calendar/17.0.1.1/upgrade_analysis.txt,sha256=0KcHUxcEnqxKVmzlig9bOFcjqF5lvT316MgrXMQSzZM,1633
 odoo/addons/openupgrade_scripts/scripts/calendar_sms/17.0.1.1/upgrade_analysis.txt,sha256=ov0HAtIQqr4W1AZIQ-NMGlXb_gSZsbqm5mq-kn2Zre4,199
-odoo/addons/openupgrade_scripts/scripts/crm/17.0.1.8/upgrade_analysis.txt,sha256=tPOM90nLCkKqLt9shQgNxOOHktSyslL48SX5UeYeaWE,1632
-odoo/addons/openupgrade_scripts/scripts/crm_iap_enrich/17.0.1.1/noupdate_changes.xml,sha256=_xJdmPzFPGBwYHRNQ6mSp13Ea04hkIGZp1u-foGPoMI,695
+odoo/addons/openupgrade_scripts/scripts/crm/17.0.1.8/upgrade_analysis.txt,sha256=ZsCcp6uA15KE3LExKlK3aCCSzenNfiPoOTcVWmZh-wk,1483
+odoo/addons/openupgrade_scripts/scripts/crm_iap_enrich/17.0.1.1/noupdate_changes.xml,sha256=-izWXk6Bj_LdL2MvG6TYJSV4HWy4PuI8vOLeK4ET9Q0,645
 odoo/addons/openupgrade_scripts/scripts/crm_iap_enrich/17.0.1.1/upgrade_analysis.txt,sha256=n6quRXxaa0Eja2cD9MiahP67CbyHHJ-iD6YWg-iP6EI,165
-odoo/addons/openupgrade_scripts/scripts/crm_iap_mine/17.0.1.2/upgrade_analysis.txt,sha256=XC7BPZPy4kiDlZQ7Qr6UswgFtnyC2y1MDEzI8q2R0BM,465
+odoo/addons/openupgrade_scripts/scripts/crm_iap_mine/17.0.1.2/upgrade_analysis.txt,sha256=zy8cIWN2w2yeL75ibIGR8SJxoW-AhVREU_OZ-keAvUQ,225
 odoo/addons/openupgrade_scripts/scripts/crm_livechat/17.0.1.0/upgrade_analysis.txt,sha256=R6N3_32MoL3cP-Ip_SxLqnn9u74__Jz8QrvfrCdBJmw,159
 odoo/addons/openupgrade_scripts/scripts/crm_sms/17.0.1.1/upgrade_analysis.txt,sha256=f-qV7_a33-EjMmoJ4o9c-GO8xBW9uajH7lKGW5brStw,169
-odoo/addons/openupgrade_scripts/scripts/data_recycle/17.0.1.3/upgrade_analysis.txt,sha256=iowuA1IQf-DGommF0ciJKzxgSGYhWqYjF1tfoOIDl4o,204
-odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/noupdate_changes.xml,sha256=bPpMPuGVQOvmr0zIaJBVWkb1NevNOIon5TAr3AfP3nc,540
-odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/upgrade_analysis.txt,sha256=1pjzlSeNMQHbwiDPq5ilj8UHAoE9LK0qOjFyvX9GBlQ,6693
+odoo/addons/openupgrade_scripts/scripts/data_recycle/17.0.1.3/upgrade_analysis.txt,sha256=wdeiKYCMj5MW7YVu94llE2nXsKYPHFjeGN3v3aw2X0U,159
+odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/noupdate_changes.xml,sha256=K6UMnLtao919y3ULDOlgL-Ih3t2PEr3SD9BPavsyavs,517
+odoo/addons/openupgrade_scripts/scripts/delivery/17.0.1.0/upgrade_analysis.txt,sha256=AUmpffyaYe8pLnXlIxT8f7OvPldcknJ-PXQLy4xFHrY,6596
 odoo/addons/openupgrade_scripts/scripts/delivery_mondialrelay/17.0.0.1/upgrade_analysis.txt,sha256=b8I5lcmNozL7-QxXWat4eRogSuXBKJ2yoDt_hOP1Kqk,186
 odoo/addons/openupgrade_scripts/scripts/delivery_stock_picking_batch/17.0.1.0/upgrade_analysis.txt,sha256=0-syDUbB9TRxr5bObpQpVaNLL2hJVGF1-JgnNuEoBqA,207
-odoo/addons/openupgrade_scripts/scripts/digest/17.0.1.1/noupdate_changes.xml,sha256=FE-tKmM98FJWrYy9gkfVEH8DE379Gavv8wLtHiSw4c4,19989
+odoo/addons/openupgrade_scripts/scripts/digest/17.0.1.1/noupdate_changes.xml,sha256=xwMvzujXqHa9nTQZGs9Wk6zB0UZaWFpWqtS1u6ccaOU,19965
 odoo/addons/openupgrade_scripts/scripts/digest/17.0.1.1/upgrade_analysis.txt,sha256=oPv4iPppLTf4jX6IovBfLVYGjqEvmWix7HiIjgeSkao,396
 odoo/addons/openupgrade_scripts/scripts/event/17.0.1.8/noupdate_changes.xml,sha256=vbzFv1zIDYFJsnlowgUaC6WQUtEILyB6dmnCxESzFyI,51945
-odoo/addons/openupgrade_scripts/scripts/event/17.0.1.8/upgrade_analysis.txt,sha256=0xBdEXQe3qnolsLWHpe6QfwORVcdiqCCKnAXm4vmQBY,4074
+odoo/addons/openupgrade_scripts/scripts/event/17.0.1.8/upgrade_analysis.txt,sha256=5FaEY5kMt6XA2T3VzU8F5u2CTmh7WZchRjKHl-keSew,4154
 odoo/addons/openupgrade_scripts/scripts/event_booth/17.0.1.1/noupdate_changes.xml,sha256=iipsblz99fuanBEY661nPirN39O3eOGjW1bT2JwiWss,2381
 odoo/addons/openupgrade_scripts/scripts/event_booth/17.0.1.1/upgrade_analysis.txt,sha256=sF-T-vRsKVL8z6zOaXX1EzIZa7WJ1hL9-dlN5wq5mEk,588
-odoo/addons/openupgrade_scripts/scripts/event_booth_sale/17.0.1.2/upgrade_analysis.txt,sha256=PSodIdhFemOIoPkHQwMrWN6e9ycVUnUUBzetpgDiiyc,650
+odoo/addons/openupgrade_scripts/scripts/event_booth_sale/17.0.1.2/upgrade_analysis.txt,sha256=93zxvY5pNeVDm0H25cv9YJmV45VQ0rN12h9uAqabxzU,552
 odoo/addons/openupgrade_scripts/scripts/event_crm/17.0.1.0/upgrade_analysis.txt,sha256=Omj6WoajseGGw6gBGTMatYXmTY873d1s05eJjw-Wpnc,150
 odoo/addons/openupgrade_scripts/scripts/event_sale/17.0.1.3/upgrade_analysis.txt,sha256=87X1DXbr7IAzhar_2v--b0nh3ndj6nw-ERskhtznfOc,1134
 odoo/addons/openupgrade_scripts/scripts/event_sms/17.0.1.0/noupdate_changes.xml,sha256=zCF9IS2bFYTsShraPQSxHkrQ0dQJTnPIlper2DFueHY,690
 odoo/addons/openupgrade_scripts/scripts/event_sms/17.0.1.0/upgrade_analysis.txt,sha256=pnGaVYE8aFEgrU4s_krQnKOo6SP1RrkO7AcMnjAJDt8,150
-odoo/addons/openupgrade_scripts/scripts/fleet/17.0.0.1/upgrade_analysis.txt,sha256=YtEiTToE2PhC-T-4mpYj_NIOGMsEJCkCbiUQnAT45f4,2889
-odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/noupdate_changes.xml,sha256=c39PYPCRf-Y6Y-oF1VR3SkO9jlxlJ9z6pJg8ib5s9tc,8753
-odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/upgrade_analysis.txt,sha256=aMJEYyCja74ycMHBvpY0YZQUPpO1K06KhaYSz0LMMZ0,1843
+odoo/addons/openupgrade_scripts/scripts/fleet/17.0.0.1/upgrade_analysis.txt,sha256=c7bQPAHj7d_apltC_ufIfe_HDuKMIFaOIbb1Q1xnY58,2652
+odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/noupdate_changes.xml,sha256=hpyPZKPTOBzQGm8fTMLxw-mb6LCxiG78ZvvNQ796JLc,10428
+odoo/addons/openupgrade_scripts/scripts/gamification/17.0.1.0/upgrade_analysis.txt,sha256=uQ615j87AWn7vqb0D6D72iGJPuHJFm9vx8iasz-jKT4,1754
 odoo/addons/openupgrade_scripts/scripts/google_account/17.0.1.0/upgrade_analysis.txt,sha256=hiDG-xTUfbSEAoh1Of3lwHn5UyurLiFn_7cWUcr_MG8,165
-odoo/addons/openupgrade_scripts/scripts/google_calendar/17.0.1.0/upgrade_analysis.txt,sha256=o8pMYQAtHrP0rH3JW_VBV5JgMkR61UzuXHPAaunRGl0,457
+odoo/addons/openupgrade_scripts/scripts/google_calendar/17.0.1.0/upgrade_analysis.txt,sha256=nQfV_h_moxZ00umo8nRUiUoJaWiASy-cflfLoTDQBIE,377
 odoo/addons/openupgrade_scripts/scripts/google_gmail/17.0.1.2/upgrade_analysis.txt,sha256=az3DyzT1W7a0qBw78ZDiO5mC3K2ESONVyPJwtakQgIU,296
 odoo/addons/openupgrade_scripts/scripts/hr/17.0.1.1/noupdate_changes.xml,sha256=IUNbRow7DkDP7neVrlvWj7X-80S_n9oJaeLYceCJ5tE,1783
-odoo/addons/openupgrade_scripts/scripts/hr/17.0.1.1/upgrade_analysis.txt,sha256=ctaAc8ps2_2lyXvfAGm3Rr5mAzWUj3JReFOzrr7U_Mg,8407
+odoo/addons/openupgrade_scripts/scripts/hr/17.0.1.1/upgrade_analysis.txt,sha256=2-psfC4gjDnpgAUrl397_yTrt7KG0JYZUxsit64bNBE,8075
 odoo/addons/openupgrade_scripts/scripts/hr_attendance/17.0.2.0/upgrade_analysis.txt,sha256=ktiyZgjaASUbYSnMG6OdNse9DchedxPqneC7F5W4Vjw,5377
 odoo/addons/openupgrade_scripts/scripts/hr_contract/17.0.1.0/noupdate_changes.xml,sha256=1NemwLIilOOpHDoCFdWOx6FPBx4REo_Wvpe5mb1a28A,518
 odoo/addons/openupgrade_scripts/scripts/hr_contract/17.0.1.0/upgrade_analysis.txt,sha256=UGFMWkoi2FdlkIYF85f5v3lhF52ahVhnU3WKiW7Figg,1400
 odoo/addons/openupgrade_scripts/scripts/hr_expense/17.0.2.0/noupdate_changes.xml,sha256=VGA0w2RW19Uxs3F7HhIa3goV2kcBQPsJbdXxCmgU9yc,2462
-odoo/addons/openupgrade_scripts/scripts/hr_expense/17.0.2.0/upgrade_analysis.txt,sha256=2Zzy_LgPNQKAnnezF6Q1b1vL0izMYuQZexM85YPs-3A,4765
+odoo/addons/openupgrade_scripts/scripts/hr_expense/17.0.2.0/upgrade_analysis.txt,sha256=Yx8U6AjBBz4fleqgeEsdmhbeitPvc9YCvQl5vIxHN84,4674
 odoo/addons/openupgrade_scripts/scripts/hr_fleet/17.0.1.0/upgrade_analysis.txt,sha256=AH2qC-3jaxRo-eCAnuK_WTlhVhQFCRS73OKLyyggR9U,361
 odoo/addons/openupgrade_scripts/scripts/hr_gamification/17.0.1.0/upgrade_analysis.txt,sha256=cMaEUAXfvHRW3vwIZMIrGROH5eDQjRAbqLkraqvEj-4,168
 odoo/addons/openupgrade_scripts/scripts/hr_holidays/17.0.1.6/noupdate_changes.xml,sha256=ngK6UV9iUDEkgGvTKifohVBMsXBTVj9pZDrBYLnAC5U,1399
-odoo/addons/openupgrade_scripts/scripts/hr_holidays/17.0.1.6/upgrade_analysis.txt,sha256=5ajOj8tQgYBoBK1WKN3mnKwGHNjB_99WRkjyYP5tijk,9856
+odoo/addons/openupgrade_scripts/scripts/hr_holidays/17.0.1.6/upgrade_analysis.txt,sha256=flWyUrKNGlbsBeLBaQvOsTAou1pweol29cRpTdLkp8s,10388
 odoo/addons/openupgrade_scripts/scripts/hr_holidays_attendance/17.0.1.0/upgrade_analysis.txt,sha256=C1HtkWT1AE5_bnw2wey2xca4d1aAHM1zMAL5JwbzCys,439
-odoo/addons/openupgrade_scripts/scripts/hr_homeworking/17.0.1.0/upgrade_analysis.txt,sha256=z-nvH4wApzc3Bejlxo8lbbcR0wpOjV-qOhKGIyHcMAI,2519
+odoo/addons/openupgrade_scripts/scripts/hr_homeworking/17.0.1.0/upgrade_analysis.txt,sha256=rK4daLDP1VqHK9Pkf7_nc3wgs8dncc5msOekWr31Scg,2616
 odoo/addons/openupgrade_scripts/scripts/hr_hourly_cost/17.0.1.0/upgrade_analysis.txt,sha256=TuvRvqvFxqrIEX9EyxEIJUFPbycloeTMjmSua_BK-Nk,165
 odoo/addons/openupgrade_scripts/scripts/hr_livechat/17.0.1.0/upgrade_analysis.txt,sha256=W8JExkRgrCIHqf6N4vyP_8sqeyhVrzTLFoRkM-z9-sg,172
 odoo/addons/openupgrade_scripts/scripts/hr_maintenance/17.0.1.0/upgrade_analysis.txt,sha256=yu4-K8VQ4jtiDZvIlVIyIZJuj8gnN_qT4qI5RcYzTZM,165
 odoo/addons/openupgrade_scripts/scripts/hr_org_chart/17.0.1.0/upgrade_analysis.txt,sha256=D33TI799LDGbuh2JyC5MHJZoKQRUd-KpYT91pZMDOiw,421
 odoo/addons/openupgrade_scripts/scripts/hr_presence/17.0.1.0/upgrade_analysis.txt,sha256=mBkYdBGJaMjyA8jiDOd8MPqOmFxNOGEx_xYuJM6PiOs,156
-odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/noupdate_changes.xml,sha256=IfWQdgNEorzpivCcje9FKl-MlF8HivZimj9NYCqSFWA,1438
-odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/upgrade_analysis.txt,sha256=AQ-aj3liSF9vxPpik-KBZtB0vLCXeJWjoJxxwA1SKQQ,2913
-odoo/addons/openupgrade_scripts/scripts/hr_recruitment_skills/17.0.1.0/upgrade_analysis.txt,sha256=ecnyjxCLWoryexeE6Fb2Q0c_8v6AbspxcYLUYJqcUJA,453
+odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/noupdate_changes.xml,sha256=U9oPwS9J9j4in9Rql0Xy0QcCCEcXE_zI1hKHZ_tznFo,1399
+odoo/addons/openupgrade_scripts/scripts/hr_recruitment/17.0.1.1/upgrade_analysis.txt,sha256=MYAeSt-rVK7fBsEX1kG188sYXfUJrVnGIuE1tSy4Lzc,2549
+odoo/addons/openupgrade_scripts/scripts/hr_recruitment_skills/17.0.1.0/upgrade_analysis.txt,sha256=7lV9xkknBnwVY7qGmJzwBnHP4-LI2gMnoEalMTocuWs,362
 odoo/addons/openupgrade_scripts/scripts/hr_recruitment_survey/17.0.1.0/noupdate_changes.xml,sha256=hHeibk-MYVeJ3PkGHZ5axWyrwIi9fp2IOTdhZ4yAm2k,581
 odoo/addons/openupgrade_scripts/scripts/hr_recruitment_survey/17.0.1.0/upgrade_analysis.txt,sha256=iyLAH-U6La6-yjIbfXEpoQw_xHE9CmH0qyHVC-5YoK4,681
-odoo/addons/openupgrade_scripts/scripts/hr_skills/17.0.1.0/upgrade_analysis.txt,sha256=5WWwigR5PpggUb0VsVctQPptnmwLtCORoX1gZcXJoCM,1217
+odoo/addons/openupgrade_scripts/scripts/hr_skills/17.0.1.0/upgrade_analysis.txt,sha256=06OqKTUamjUL1Ui7l6POXHoQKmy38FEO4mLZsGDbgHw,899
 odoo/addons/openupgrade_scripts/scripts/hr_skills_slides/17.0.1.0/upgrade_analysis.txt,sha256=oQB8tjhHAghJ25JskMaQEBVgDe2p4uz0qvWqX-QBuwQ,171
 odoo/addons/openupgrade_scripts/scripts/hr_skills_survey/17.0.1.0/upgrade_analysis.txt,sha256=3tgY89XspEDlIcKoxy6bnt4bJmvJt-UZwzcXVOyDTMM,715
-odoo/addons/openupgrade_scripts/scripts/hr_timesheet/17.0.1.0/upgrade_analysis.txt,sha256=M3ksmKrl_xouT1hQvDEQyCXPOzy9yFN8fHFuanMwYGo,1862
+odoo/addons/openupgrade_scripts/scripts/hr_timesheet/17.0.1.0/upgrade_analysis.txt,sha256=crjTeU81FGUKyW8vZmuSCXLbrTLMQvmbefqqEqKQY-E,2057
 odoo/addons/openupgrade_scripts/scripts/hr_timesheet_attendance/17.0.1.1/noupdate_changes.xml,sha256=Pn8knBBRt3Mo6t3lNpdm5ANlCoyzZuUcqvcX7v7OOLo,222
 odoo/addons/openupgrade_scripts/scripts/hr_timesheet_attendance/17.0.1.1/upgrade_analysis.txt,sha256=BuiW1HztzK7B4xdg5UVhWJFTSc2Ra5msHmDDNcjsYek,233
-odoo/addons/openupgrade_scripts/scripts/hr_work_entry/17.0.1.0/upgrade_analysis.txt,sha256=aSfeRl1m1WDoBvn6ESue2tJqfancR-Wg7o9iFhb_a0A,738
+odoo/addons/openupgrade_scripts/scripts/hr_work_entry/17.0.1.0/upgrade_analysis.txt,sha256=HjLcWFrP1MUO3f21UUH1ejUur7wQdp0u44OzKK29pq0,264
 odoo/addons/openupgrade_scripts/scripts/hr_work_entry_contract/17.0.1.0/upgrade_analysis.txt,sha256=ci4PEjbKpDZr4lAikNgyQSjrVYKMRw-bXpm7DeZZJ6Y,189
 odoo/addons/openupgrade_scripts/scripts/hr_work_entry_holidays/17.0.1.0/upgrade_analysis.txt,sha256=xiIE52fmSt8O6Eas8502Dg-Rb1ht_MPZZuifH2wuJyY,220
 odoo/addons/openupgrade_scripts/scripts/iap/17.0.1.1/upgrade_analysis.txt,sha256=AvYS4Q0MRIMGV99LTKJdHZLv6qN8ItMupPDQCOLB8LQ,485
 odoo/addons/openupgrade_scripts/scripts/iap_crm/17.0.1.0/upgrade_analysis.txt,sha256=Qxdh9V6HQd4HpmXsmxEMxN3Vu7y8Q6v0NWL3ZrRK1oA,144
 odoo/addons/openupgrade_scripts/scripts/im_livechat/17.0.1.0/noupdate_changes.xml,sha256=Nmw3l-OlwZF_nh98WpwmNu50uUTM1gqPOx1A2he54mg,6236
-odoo/addons/openupgrade_scripts/scripts/im_livechat/17.0.1.0/upgrade_analysis.txt,sha256=-eb9QSP4m3_N9I-OmGupSyivNjLBrE59gAB8rgzcUXU,5508
+odoo/addons/openupgrade_scripts/scripts/im_livechat/17.0.1.0/upgrade_analysis.txt,sha256=AcJuXqDSUAnuAn_BRAmBYSR5LGBaHuAG_4EgD7DEzsE,5505
 odoo/addons/openupgrade_scripts/scripts/im_livechat_mail_bot/17.0.1.0/upgrade_analysis.txt,sha256=xGhm2WEi7ACkVuwg3tKYA2ItfbahG5H9UENyFMPk78A,183
 odoo/addons/openupgrade_scripts/scripts/l10n_ae/17.0.1.0/upgrade_analysis.txt,sha256=FKJXw9sFEWcMxRmzINOn2o1q7FqzeNcRYW7zyFEmsBE,12145
-odoo/addons/openupgrade_scripts/scripts/l10n_ar/17.0.3.5/upgrade_analysis.txt,sha256=ngf6MI03ug8KRq_xIhEiY93kyTPHXAUfvBGQhZO6TEg,34529
+odoo/addons/openupgrade_scripts/scripts/l10n_ar/17.0.3.5/upgrade_analysis.txt,sha256=OrvZfW3-60hg0uKJvI8hiWoDu_8gN6oJ-pEvEqEhHng,34365
 odoo/addons/openupgrade_scripts/scripts/l10n_ar_pos/17.0.1.0/upgrade_analysis.txt,sha256=jaI_2SveViPyrgHBNBkNeK3bD1poCV-xGXqpWXn1FkM,169
-odoo/addons/openupgrade_scripts/scripts/l10n_ar_withholding/17.0.1.0/upgrade_analysis.txt,sha256=YF7q-JwNm3Tl6LR3HNUHs4fKY7Lfsfs5y2qJNXOpDAc,979
+odoo/addons/openupgrade_scripts/scripts/l10n_ar_withholding/17.0.1.0/upgrade_analysis.txt,sha256=HYXY9GrVpmSxPzGyyA9zUoHK_f8VFzn_LOvW3SOnb10,1000
 odoo/addons/openupgrade_scripts/scripts/l10n_at/17.0.3.1/upgrade_analysis.txt,sha256=P9Ku1Ks500ey0OLGjKxQhSUUXdRkN7Oj9Mn2FZjAyLY,79751
 odoo/addons/openupgrade_scripts/scripts/l10n_au/17.0.1.1/upgrade_analysis.txt,sha256=6HVzaEQsQBD2Z05YyguvEJlSLyujCVJgC5w4ihY5ZZk,9905
+odoo/addons/openupgrade_scripts/scripts/l10n_bd/17.0.1.0/upgrade_analysis.txt,sha256=CNx7I0zcDMoW8bpt55ptAAaTQuB9EVWkNm7FtRoZCzE,3156
 odoo/addons/openupgrade_scripts/scripts/l10n_be/17.0.2.0/upgrade_analysis.txt,sha256=ViRzhwT5SF432W1aK6Bu_PrMVAaAxb_k6_onryqsjCU,45436
+odoo/addons/openupgrade_scripts/scripts/l10n_bf/17.0.1.0/upgrade_analysis.txt,sha256=lioSQm7aLULEHKWNs11XmWUXpk1CDiVufQMYYAb--rY,6101
 odoo/addons/openupgrade_scripts/scripts/l10n_bg/17.0.1.0/upgrade_analysis.txt,sha256=vTBlAuoTbZdQjP9VJYD6xTRXm13zoTkjTpsJxAB_Nls,23622
+odoo/addons/openupgrade_scripts/scripts/l10n_bj/17.0.1.0/upgrade_analysis.txt,sha256=XZmsTciGpWCC5CKov2ObuiLkJQQMbMUOeHp77fJoxBU,3115
 odoo/addons/openupgrade_scripts/scripts/l10n_bo/17.0.2.0/upgrade_analysis.txt,sha256=xy7viXWjfebwRzwQTrPgWxIOm4R35g6oao1__xMxCgc,11394
 odoo/addons/openupgrade_scripts/scripts/l10n_br/17.0.1.0/upgrade_analysis.txt,sha256=nEn0y4RWq5L4yPehYgwcOWR3OFGGY9Px6Lr0QTcGXI8,79062
+odoo/addons/openupgrade_scripts/scripts/l10n_br_pix/17.0.1.0/upgrade_analysis.txt,sha256=UvkX7VKVwxnogm8z3kfhOVRs0FXtbtkAZRdRz0KC93w,451
 odoo/addons/openupgrade_scripts/scripts/l10n_br_sales/17.0.1.0/upgrade_analysis.txt,sha256=bxzwioW-lTPMiSPeSp_jt-AIu97YiA0osErDTrJctrQ,361
 odoo/addons/openupgrade_scripts/scripts/l10n_br_website_sale/17.0.1.0/upgrade_analysis.txt,sha256=9ayJBLpWPrNNsvhAEkdQH3477nUFyNZMEoJ9VC7N0Io,250
 odoo/addons/openupgrade_scripts/scripts/l10n_ca/17.0.1.0/upgrade_analysis.txt,sha256=H93DJx4zY3z7WA12ZNuLrROls5K7joMVHWBMljDKZz8,30677
+odoo/addons/openupgrade_scripts/scripts/l10n_cd/17.0.1.0/upgrade_analysis.txt,sha256=Sl8yKva27TQ-RuRakMFWpqr0U-qrjqasfiMnBmwXBh0,8459
+odoo/addons/openupgrade_scripts/scripts/l10n_cf/17.0.1.0/upgrade_analysis.txt,sha256=mYxDSQ4-sEh5sPUV7anTPfqrtfFXO9OLPfI2Rs0SNEc,2917
+odoo/addons/openupgrade_scripts/scripts/l10n_cg/17.0.1.0/upgrade_analysis.txt,sha256=QIdRmpcA4-AuO31hmiFdjViHAk2DsEuj55wfEyJrWOs,2587
 odoo/addons/openupgrade_scripts/scripts/l10n_ch/17.0.11.2/upgrade_analysis.txt,sha256=9UQdCMm0EEXngd_ar4WEQv_DDL04v96EcgL1D2QazQM,14425
+odoo/addons/openupgrade_scripts/scripts/l10n_ch/17.0.11.3/upgrade_analysis.txt,sha256=9UQdCMm0EEXngd_ar4WEQv_DDL04v96EcgL1D2QazQM,14425
+odoo/addons/openupgrade_scripts/scripts/l10n_ci/17.0.1.0/upgrade_analysis.txt,sha256=KGvmwuphqCu6bqtUm_RR2veiDWY5ciUujmIDpGJK6BI,4822
 odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/noupdate_changes.xml,sha256=bOYBzstYvJt5lGld6QRM5yzwlEkxhAcZtGyTMH1X7T8,887
-odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/upgrade_analysis.txt,sha256=D9_MMZjWEHzT10Mq1wuT0EKl651c3Idw1dlLsqvzAJ8,14277
+odoo/addons/openupgrade_scripts/scripts/l10n_cl/17.0.3.0/upgrade_analysis.txt,sha256=cZ5AM1PjZmyoMUrLipIoCZneLUpZUpdz7Fjd27mfHK8,14330
+odoo/addons/openupgrade_scripts/scripts/l10n_cm/17.0.1.0/upgrade_analysis.txt,sha256=rpUYIyagHzoOWdZVd_8rpe75lrHKWSDmZQyYwSe1x7Q,4948
 odoo/addons/openupgrade_scripts/scripts/l10n_cn/17.0.1.8/upgrade_analysis.txt,sha256=XZVzbWWYbmOmAMbCOaY-Q4Bq1N1d97An4hPSs2XwU2Q,4790
 odoo/addons/openupgrade_scripts/scripts/l10n_co/17.0.0.8/upgrade_analysis.txt,sha256=zs-LcUCN6O9NI5_bbAyDRJWklMLZaByOOn46j3MlBxY,24365
+odoo/addons/openupgrade_scripts/scripts/l10n_co/17.0.0.9/upgrade_analysis.txt,sha256=zs-LcUCN6O9NI5_bbAyDRJWklMLZaByOOn46j3MlBxY,24365
 odoo/addons/openupgrade_scripts/scripts/l10n_cr/17.0.1.0/upgrade_analysis.txt,sha256=PhVDTcekSBWfdnUBM7BpCTk_DGZRBkUbse5M3AE61aM,7396
 odoo/addons/openupgrade_scripts/scripts/l10n_cz/17.0.1.1/upgrade_analysis.txt,sha256=jEqDI0XxwiCkNG39JsfKp-E24gTqXLp8xWVnuspuxfs,31915
-odoo/addons/openupgrade_scripts/scripts/l10n_de/17.0.2.0/upgrade_analysis.txt,sha256=M-gvoGL4wA5Fici-xJCJK7VGp87s8NRR2D6oiDbm-dc,165698
+odoo/addons/openupgrade_scripts/scripts/l10n_de/17.0.2.0/upgrade_analysis.txt,sha256=O6rjzO902C-KjRn4hqNfEZH-zq3ec605WG34fzU5jyE,182
 odoo/addons/openupgrade_scripts/scripts/l10n_din5008/17.0.1.0/upgrade_analysis.txt,sha256=7MFzfst9KxBiHelWboppSpkpQinzNOx-r-V2KcT2_2g,159
 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_purchase/17.0.1.0/upgrade_analysis.txt,sha256=IsmNuWcW2tGP6jLMY3_hhC8K8tlnYRJVuAte8B5pH-4,186
 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_repair/17.0.1.0/upgrade_analysis.txt,sha256=DYtFt3vnBVNxuDh0X-d4Yu2qM2MlP3YJydyazJUp-Gw,180
 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_sale/17.0.1.0/upgrade_analysis.txt,sha256=Ur6CJpngXbcFyCiwJBtBa9rnwBOF4xajiMtOEIFFai4,174
 odoo/addons/openupgrade_scripts/scripts/l10n_din5008_stock/17.0.1.0/upgrade_analysis.txt,sha256=ubVKLoW_MJ-MNmvqnz3bYuoQ3rfQ2XTHH9JI47GX9t0,177
 odoo/addons/openupgrade_scripts/scripts/l10n_dk/17.0.1.1/noupdate_changes.xml,sha256=IpF6kmJwFYu_ftXO36MkfXxSDec9UAG5OCrqOC2rTQs,4165
 odoo/addons/openupgrade_scripts/scripts/l10n_dk/17.0.1.1/upgrade_analysis.txt,sha256=D71J5WpI8ImFv9WcfnXfZQRz9yx0_RPH7IvDXjdDvCY,27657
 odoo/addons/openupgrade_scripts/scripts/l10n_dk_bookkeeping/17.0.1.0/upgrade_analysis.txt,sha256=ZGidg3LsMXzohP3jEeUYTg9NhlGLwwqrBLhPiKjFLCU,391
-odoo/addons/openupgrade_scripts/scripts/l10n_dk_oioubl/17.0.0.1/upgrade_analysis.txt,sha256=rwIfn_deBq2ctT7ykDrQrT9UMi65vg0L9DLh1E8QjHE,432
+odoo/addons/openupgrade_scripts/scripts/l10n_dk_oioubl/17.0.0.1/upgrade_analysis.txt,sha256=SrSrm4m8nJ8VpZz4dq7ti8n9nL-OMiAKOyqc3mltPp4,443
 odoo/addons/openupgrade_scripts/scripts/l10n_do/17.0.2.0/upgrade_analysis.txt,sha256=wxrmCynLZE15Jzt_u28-ZkbWkBvc2ZIdwf_NPOAAbcc,36437
-odoo/addons/openupgrade_scripts/scripts/l10n_dz/17.0.1.0/upgrade_analysis.txt,sha256=DHmXteOY_oFZVuJAsPc9luEX0_T-OvGZRtmoNyC3M44,54666
+odoo/addons/openupgrade_scripts/scripts/l10n_dz/17.0.1.0/upgrade_analysis.txt,sha256=zPymahz_mGhQD2_yzsWASNW8d9lDSRyRUDHX77xLoac,54636
 odoo/addons/openupgrade_scripts/scripts/l10n_ec/17.0.3.5/upgrade_analysis.txt,sha256=1JkjQd3A78IDcmnYfD7L-jRdfJG3YUX5bv6xR3Q7HMA,37793
+odoo/addons/openupgrade_scripts/scripts/l10n_ec/17.0.3.8/upgrade_analysis.txt,sha256=SkmX2FUJRMUeN4GmOG58yHI0ktMStxUxJHsuq6SALfc,42096
+odoo/addons/openupgrade_scripts/scripts/l10n_ec_website_sale/17.0.1.0/upgrade_analysis.txt,sha256=mnWhTMaC5c9taWObgCQ83G1Vuqpmd0pwl7d4Y8W4X08,476
 odoo/addons/openupgrade_scripts/scripts/l10n_ee/17.0.1.1/upgrade_analysis.txt,sha256=w0b-agNi4Ue2QQ-RWQ5dzkTRmj6DqK6lhOLFleJhgDY,22251
 odoo/addons/openupgrade_scripts/scripts/l10n_eg/17.0.1.0/upgrade_analysis.txt,sha256=BOXJ8pdDnI9ZxtPq7AowVTrPmpvYHAXq55AYrRJP5CA,13603
-odoo/addons/openupgrade_scripts/scripts/l10n_eg_edi_eta/17.0.0.2/upgrade_analysis.txt,sha256=hZ_8pBVwiZMYQ_c24sWtQ8A8e6RAVCccaIBzS2_Cwl4,220
+odoo/addons/openupgrade_scripts/scripts/l10n_eg_edi_eta/17.0.0.2/upgrade_analysis.txt,sha256=f2AaXZRdCljxh7HjEHarlfgonOcm-NqVuLmhfAR_y4c,168
 odoo/addons/openupgrade_scripts/scripts/l10n_es/17.0.5.2/upgrade_analysis.txt,sha256=LUHatWaeN4lbxNlcDgdMmvh7cZz8bU2Yl_anFzNv8yw,210204
 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_facturae/17.0.1.0/upgrade_analysis.txt,sha256=7Qv71rXs6ax9Du2w339UQ5_pDbOwcRrEQczmwcKQMJo,3975
 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_facturae_adm_centers/17.0.1.0/upgrade_analysis.txt,sha256=Kz2Ew4HxZmsxFhUCoPO-F-hPusUcdVBKro63__UzABo,2620
 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_facturae_invoice_period/17.0.1.0/upgrade_analysis.txt,sha256=Hy7who6IeUM1qSWGiUEe7fb_oFjepVVQdX3RPMjpX1Q,479
 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_sii/17.0.1.0/upgrade_analysis.txt,sha256=yTeUK5UogbA92To-c7SZq-OlaMlUoSnJeGwk12Oos3s,1541
 odoo/addons/openupgrade_scripts/scripts/l10n_es_edi_tbai/17.0.1.0/upgrade_analysis.txt,sha256=HjN5fqxWm7GTI9F6Wbmi4eq__eKZcuCqaRjFQQE-dfE,171
 odoo/addons/openupgrade_scripts/scripts/l10n_es_pos/17.0.1.0/upgrade_analysis.txt,sha256=-ujmU1jhx1tjpmlr8e8YtxH6-OrIrittrJVAmb9UwSQ,625
@@ -160,119 +173,141 @@
 odoo/addons/openupgrade_scripts/scripts/l10n_fi/17.0.13.0.1/noupdate_changes.xml,sha256=b1ODUR3WVyZBGrLESgWGStvZl8e1F9dR6HKdyfBgso0,22062
 odoo/addons/openupgrade_scripts/scripts/l10n_fi/17.0.13.0.1/upgrade_analysis.txt,sha256=PVWECDJe0nxQlqlG2E5zTWYCSwnyWbDm5rff3aZwCdM,17560
 odoo/addons/openupgrade_scripts/scripts/l10n_fr/17.0.2.1/upgrade_analysis.txt,sha256=XSjlDfoc0Jo-7pCMwCYMkfhLa1DPxPchdk3CBy8EdrA,56284
 odoo/addons/openupgrade_scripts/scripts/l10n_fr_facturx_chorus_pro/17.0.1.0/upgrade_analysis.txt,sha256=pCTtVTixXRGAtRdfheNzj6S7NvIIcoimpk6UWyiip48,201
 odoo/addons/openupgrade_scripts/scripts/l10n_fr_fec/17.0.1.0/upgrade_analysis.txt,sha256=965QMMGisRYTsw_asToJYNh4sQVPPR39fpWryP-gSIk,156
 odoo/addons/openupgrade_scripts/scripts/l10n_fr_hr_holidays/17.0.1.0/upgrade_analysis.txt,sha256=6Fkv8lDyfleOnOSC6soYAGm4umO1nL82IeLYFl3GaH8,479
 odoo/addons/openupgrade_scripts/scripts/l10n_fr_pos_cert/17.0.1.0/upgrade_analysis.txt,sha256=6YOthNLbBr_cYsnI3gFrnNtagXxh_diJTCncPD5dfsg,171
+odoo/addons/openupgrade_scripts/scripts/l10n_ga/17.0.1.0/upgrade_analysis.txt,sha256=qJozEmhIqZnKYEYaON7MBlsG4gS5cl7doOQuSqohuzw,13592
 odoo/addons/openupgrade_scripts/scripts/l10n_gcc_invoice/17.0.1.0.0/upgrade_analysis.txt,sha256=lkiz5pSPZlpcTRbKiVGCDjKl7aGj_auOsk8ALXATHFg,193
+odoo/addons/openupgrade_scripts/scripts/l10n_gn/17.0.1.0/upgrade_analysis.txt,sha256=27e_fgbiTVK9YPw6vPVFgLH4e3IUZRr_sGwH1YW2K_A,2994
+odoo/addons/openupgrade_scripts/scripts/l10n_gq/17.0.1.0/upgrade_analysis.txt,sha256=JhL_XRWcX0xznnJBtNoshEKtXQkxihMbiv-QDlTSlVo,2822
 odoo/addons/openupgrade_scripts/scripts/l10n_gr/17.0.1.0/upgrade_analysis.txt,sha256=azT1N8RPxUSs33AXv-VqEJk-yUW2lCGT3MqFDunKi1A,71841
 odoo/addons/openupgrade_scripts/scripts/l10n_gt/17.0.3.0/upgrade_analysis.txt,sha256=Qkn-8Tiw7k0hVSQAOOLHe8lLZvxDoRc7-Rztd5ZX3Oo,1890
+odoo/addons/openupgrade_scripts/scripts/l10n_gw/17.0.1.0/upgrade_analysis.txt,sha256=xwGC6SUfff3gdJ51ACX1f6-Gw_5uMaQ5lHhFjH8abAk,2991
 odoo/addons/openupgrade_scripts/scripts/l10n_hk/17.0.1.0/upgrade_analysis.txt,sha256=ltsT_tag6KUs9nZESuqkh2c8GHEy0lzheWuThDF7wrw,4020
 odoo/addons/openupgrade_scripts/scripts/l10n_hn/17.0.0.2/upgrade_analysis.txt,sha256=S_goCeLTAJ-e7wCHxvWTNO1y6Qa9P_JzVid1F8iCa8M,1986
-odoo/addons/openupgrade_scripts/scripts/l10n_hr/17.0.13.0/upgrade_analysis.txt,sha256=DzNtTwVVvV75MPz_1BXVg5UuiHUpYwQpX0An5o05CGk,169033
+odoo/addons/openupgrade_scripts/scripts/l10n_hr/17.0.13.0/upgrade_analysis.txt,sha256=lZfyJT5vs9Vi9E-AbdTcjFVikLEm1c5GzMtggj9jO5g,117045
 odoo/addons/openupgrade_scripts/scripts/l10n_hu/17.0.3.0/upgrade_analysis.txt,sha256=bVCAL4Pl1jp83ctkTzt0ESAB-qVpi8Z42RJDE2Ralk4,27037
+odoo/addons/openupgrade_scripts/scripts/l10n_hu_edi/17.0.1.0.0/upgrade_analysis.txt,sha256=jJhUUjaUz2ecdEnZrRVh_9W5bdkdgYc1ZIZ2Z0ekRRM,4915
 odoo/addons/openupgrade_scripts/scripts/l10n_id/17.0.1.0/upgrade_analysis.txt,sha256=Wahsy9yBmjKbI9LQIw9rmT9GPhVXHAURM7zugvSVVxM,6289
 odoo/addons/openupgrade_scripts/scripts/l10n_id_efaktur/17.0.1.0/upgrade_analysis.txt,sha256=ktlY54OdWRlzsMO4LQCQw18iOtQd6VIwBDnFE9VfUFI,168
 odoo/addons/openupgrade_scripts/scripts/l10n_ie/17.0.2.0/upgrade_analysis.txt,sha256=uGMOZYGxhL3TcdKX28G-uerx8dNxlIh5AvZHFbG9PVE,7279
 odoo/addons/openupgrade_scripts/scripts/l10n_il/17.0.1.0/upgrade_analysis.txt,sha256=JlONhk5XCIFXXXkpw7I0gY1kOs3vwkrgyVXlesWcr3M,7752
-odoo/addons/openupgrade_scripts/scripts/l10n_in/17.0.2.0/upgrade_analysis.txt,sha256=KiVKva0RZte6uAjE9o6P8tGxxTAFJ6xy63FcqpWh-us,38104
+odoo/addons/openupgrade_scripts/scripts/l10n_in/17.0.2.0/upgrade_analysis.txt,sha256=gRQiRKevznPwfCmExhsuUzW1ebcKjxymprPhyUB8MSI,23012
 odoo/addons/openupgrade_scripts/scripts/l10n_in_edi/17.0.1.03.00/upgrade_analysis.txt,sha256=Zn4snNNdw22KavOYtS7nq9YanDe1V5AM66lfZEAF5D0,156
 odoo/addons/openupgrade_scripts/scripts/l10n_in_edi_ewaybill/17.0.1.03.00/upgrade_analysis.txt,sha256=2nLeUh_4yrSArPTz1bjeLkZN5bphfCYyqZ3jWDOQG-c,183
+odoo/addons/openupgrade_scripts/scripts/l10n_in_ewaybill_stock/17.0.1.0/upgrade_analysis.txt,sha256=J_sD34dqwxNz2TcPaYhWGSMHxjOMENaevJRhs5w9cSo,5323
 odoo/addons/openupgrade_scripts/scripts/l10n_in_purchase/17.0.1.0/upgrade_analysis.txt,sha256=tBcVmarcazJEMcT_gadsHodUheqVYZJbMCgg3y-McCg,239
 odoo/addons/openupgrade_scripts/scripts/l10n_in_purchase_stock/17.0.1.0/upgrade_analysis.txt,sha256=3aizS70nFiymBOv2XhtnfWsxqvyZUBoeI5lpDWRYNLo,353
 odoo/addons/openupgrade_scripts/scripts/l10n_in_sale/17.0.1.0/upgrade_analysis.txt,sha256=FhP7FNQBByR1Etu7E4l-xO9dM48n2yhKBFPuo1xAaeA,323
 odoo/addons/openupgrade_scripts/scripts/l10n_in_sale_stock/17.0.0.1/upgrade_analysis.txt,sha256=y4OIIoAuFuEMRo3BMA6W5Bv-uvBr8pG0wXPdGMRQdJE,329
 odoo/addons/openupgrade_scripts/scripts/l10n_it/17.0.0.5/upgrade_analysis.txt,sha256=1hGmCeqxFBoHg55bYa-9tbjlREsa3wO04y44Di0RwTg,12277
+odoo/addons/openupgrade_scripts/scripts/l10n_it/17.0.0.6/upgrade_analysis.txt,sha256=1hGmCeqxFBoHg55bYa-9tbjlREsa3wO04y44Di0RwTg,12277
 odoo/addons/openupgrade_scripts/scripts/l10n_it_edi/17.0.0.3/upgrade_analysis.txt,sha256=E_O6i1jDEBWISm8Qwm8BYJCPKZkUNjNhNMW3jl0X3nA,4193
+odoo/addons/openupgrade_scripts/scripts/l10n_it_edi/17.0.0.4/upgrade_analysis.txt,sha256=thaW5MEH4sXkOnHtDNotY2hDfgr0Kqgx1drV7Rrt-j4,4086
 odoo/addons/openupgrade_scripts/scripts/l10n_it_edi_withholding/17.0.0.1/upgrade_analysis.txt,sha256=SzOYgJBAIT9rumd-BDKzEdUmYXIqB-dfxwONsftyBVo,1913
 odoo/addons/openupgrade_scripts/scripts/l10n_it_stock_ddt/17.0.0.1/upgrade_analysis.txt,sha256=IS3Qs6krllkgHhzEZbo2CWjzErAp4v1TYTc2YTD5HB8,174
 odoo/addons/openupgrade_scripts/scripts/l10n_jp/17.0.2.3/upgrade_analysis.txt,sha256=oHlGW-6iUaW_N5cwwh_9EMhey8Qv8vGsuCe_0PEjRCg,10154
 odoo/addons/openupgrade_scripts/scripts/l10n_jp_ubl_pint/17.0.1.0/upgrade_analysis.txt,sha256=XKm51vLyt6MOtLrXhDx9YDIXj5fuE0jhvf1VO7aydhI,368
 odoo/addons/openupgrade_scripts/scripts/l10n_ke/17.0.1.0/upgrade_analysis.txt,sha256=J1q2L422dLwl8s7KuqSyhXZJr0Y_Ivkx9v01pbEG2vc,23082
-odoo/addons/openupgrade_scripts/scripts/l10n_ke_edi_tremol/17.0.1.0/upgrade_analysis.txt,sha256=cJ2MzbhJik3eIQlmil8rfTnzvho91MuBlZz-t9jz85Y,460
+odoo/addons/openupgrade_scripts/scripts/l10n_ke_edi_tremol/17.0.1.0/upgrade_analysis.txt,sha256=T7JWk0Jp8KH8n_KkcQ27mnZe7FFrXzVSYorZ3CGEQds,545
+odoo/addons/openupgrade_scripts/scripts/l10n_km/17.0.1.0/upgrade_analysis.txt,sha256=NY10j6Tkjjzj5JX4oplsHahZ4DQOM-lhsO2XONgMnh8,2666
 odoo/addons/openupgrade_scripts/scripts/l10n_kz/17.0.1.0/upgrade_analysis.txt,sha256=Zo7E53iCyaRkUUkBiqZPG0WA0b2KNKtowZcoFsDhfSo,8080
 odoo/addons/openupgrade_scripts/scripts/l10n_latam_base/17.0.1.0/upgrade_analysis.txt,sha256=p-t_Q1E60Oh2v-aNA3aM6Rr_BsrGe6i7Y3Up9t06V9A,282
 odoo/addons/openupgrade_scripts/scripts/l10n_latam_check/17.0.1.0.0/upgrade_analysis.txt,sha256=gjEIQGsrUS1Xdm-foqH5KTrIXzQlDp-0qhtcjyGcA6Q,171
-odoo/addons/openupgrade_scripts/scripts/l10n_latam_invoice_document/17.0.1.0/upgrade_analysis.txt,sha256=g3iudhilYuO6zMsGqrWNlCzvjZQhYpGZjxBLB4umIcg,818
+odoo/addons/openupgrade_scripts/scripts/l10n_latam_invoice_document/17.0.1.0/upgrade_analysis.txt,sha256=teQ9wcojRBufHpwWWJNbVZGDqICgdcSGVOSBPCY0Ckw,918
 odoo/addons/openupgrade_scripts/scripts/l10n_lt/17.0.1.0.0/upgrade_analysis.txt,sha256=Pj2UJqNW5ExSuRZwcwaSZM5O0QYZI4PZzdzd5b5pQs0,15271
-odoo/addons/openupgrade_scripts/scripts/l10n_lu/17.0.2.2/upgrade_analysis.txt,sha256=bRP-zHkm0sb4uOpuaJgXU7a2c-qkzgiSSpIbpDjaLx4,122361
+odoo/addons/openupgrade_scripts/scripts/l10n_lu/17.0.2.2/upgrade_analysis.txt,sha256=42DfYB1BrOs0hU6bhVsu0Un5LUFxFaFmlt1-HwYqoPE,124845
 odoo/addons/openupgrade_scripts/scripts/l10n_lv/17.0.1.0.0/upgrade_analysis.txt,sha256=0PRFPe3buaXd8Tc97Xx9LMDoaiSqOYyUV-cU0vNcfGI,18165
 odoo/addons/openupgrade_scripts/scripts/l10n_ma/17.0.1.0/upgrade_analysis.txt,sha256=DAXOZzXFKBXOqXdBYiGqAz319IZE3blNOtO3pQtqoU4,55975
+odoo/addons/openupgrade_scripts/scripts/l10n_ml/17.0.1.0/upgrade_analysis.txt,sha256=VEsN8jLAlNALcGlzeepZNPHMCA0AFQVdcBQpW_jYuz8,4112
 odoo/addons/openupgrade_scripts/scripts/l10n_mn/17.0.1.1/upgrade_analysis.txt,sha256=F1fuIwtlUxmDjLsPdVTCKGcyB0MsM4ik4foLzPuYkpk,39171
+odoo/addons/openupgrade_scripts/scripts/l10n_mt/17.0.1.0/upgrade_analysis.txt,sha256=rH7fJD6R0Fq7Bi3CwKEvdve4zAiKQwFPw2NHs8Xb1sI,5919
+odoo/addons/openupgrade_scripts/scripts/l10n_mu_account/17.0.1.0/upgrade_analysis.txt,sha256=SRREjqID840O7gHDWG6JQUY9gGVjE52lMrKU_aCM4jA,5012
 odoo/addons/openupgrade_scripts/scripts/l10n_mx/17.0.2.0/upgrade_analysis.txt,sha256=cjJRUwQ9m-VHNFGzVCHgbn4Z4wyPzFVwasWCjqqJToE,105353
+odoo/addons/openupgrade_scripts/scripts/l10n_mx/17.0.2.1/upgrade_analysis.txt,sha256=cjJRUwQ9m-VHNFGzVCHgbn4Z4wyPzFVwasWCjqqJToE,105353
 odoo/addons/openupgrade_scripts/scripts/l10n_mx_hr/17.0.1.0/upgrade_analysis.txt,sha256=wATDEKCI3KIYw9VR1JAn-vdceJ4m8So5fBsa1eq2U1s,153
-odoo/addons/openupgrade_scripts/scripts/l10n_my/17.0.1.1/upgrade_analysis.txt,sha256=5t3PfxwSDkF6mLxVETTrSEI5FZiWo7Q2tMy-IOwqZsA,5852
+odoo/addons/openupgrade_scripts/scripts/l10n_my/17.0.1.1/upgrade_analysis.txt,sha256=T5LyoP8lfKfLVa93ClANhWFvzkoGl8RBF6AMhMzxkDY,5905
+odoo/addons/openupgrade_scripts/scripts/l10n_my_ubl_pint/17.0.1.0/upgrade_analysis.txt,sha256=5R3WBdHiZGYkeiyPUnfbkvDGsK0MSrFu1XffPWhm40E,1052
 odoo/addons/openupgrade_scripts/scripts/l10n_mz/17.0.1.0/upgrade_analysis.txt,sha256=E3Bt7GZbxyYM7r_240f0Wa0N61uBzWfSAt-UsLCftnI,26131
+odoo/addons/openupgrade_scripts/scripts/l10n_ne/17.0.1.0/upgrade_analysis.txt,sha256=BedJTsBFTe7nYiPo58r008o2KDSJEFcRKwzvk1dD50E,3978
+odoo/addons/openupgrade_scripts/scripts/l10n_ng/17.0.1.0/upgrade_analysis.txt,sha256=VVRlY4G4WJA5z0DdADPJ1-tySL8EFAIuQ-oSIYOmUjM,3079
 odoo/addons/openupgrade_scripts/scripts/l10n_nl/17.0.3.2/upgrade_analysis.txt,sha256=7RB-HkjMT43c0Sqbo4mjg0e-wl-o8YWZaKxSZ0xvJlA,23323
 odoo/addons/openupgrade_scripts/scripts/l10n_no/17.0.2.1/upgrade_analysis.txt,sha256=8xBVQgGOEdM9GGgciEAliOJeK3Vrkp_g8lyYbUcK1Cs,24279
 odoo/addons/openupgrade_scripts/scripts/l10n_nz/17.0.1.1/upgrade_analysis.txt,sha256=wF6d1lDm9YcKO9WZJJ7pH2Kbgea2rZvX-45X0E72oSA,5850
 odoo/addons/openupgrade_scripts/scripts/l10n_pa/17.0.1.0/upgrade_analysis.txt,sha256=ibpT30z6qAiK-TpOxXv8HnWSRB_h498vZUTvnPsNgPQ,5072
 odoo/addons/openupgrade_scripts/scripts/l10n_pe/17.0.3.0/upgrade_analysis.txt,sha256=YKHEK9jaqOmotOFQFbFXshRsba4POKdlJyS7viKXLCE,66374
 odoo/addons/openupgrade_scripts/scripts/l10n_pe_pos/17.0.1.0/upgrade_analysis.txt,sha256=tC_IF86oSJ1rfhOGv-L3mTVUUlbcgDFFLDSY_IG2R5I,223
 odoo/addons/openupgrade_scripts/scripts/l10n_pe_website_sale/17.0.0.1/upgrade_analysis.txt,sha256=WkbcG8UkYRCE48jDYy01r7KgkEOanjCX0ecKR81RLBY,418
 odoo/addons/openupgrade_scripts/scripts/l10n_ph/17.0.1.1/upgrade_analysis.txt,sha256=5mcI7N6rgM9HCNNXystRRLclEa0bo7iAWukEGLZlFKA,14223
 odoo/addons/openupgrade_scripts/scripts/l10n_pk/17.0.1.0/upgrade_analysis.txt,sha256=XV5YNtfiML_sScoKSJ6L3YbbJAX9pIt-vdfSkGxwREg,9396
-odoo/addons/openupgrade_scripts/scripts/l10n_pl/17.0.2.0/upgrade_analysis.txt,sha256=HGsFgLIJiQ6lW0_6TaaXVkCGWB-3NTbsHkFRhuc8ZKc,50948
-odoo/addons/openupgrade_scripts/scripts/l10n_pt/17.0.1.0/upgrade_analysis.txt,sha256=1dKbGpa3GG_KK2k80LNlpMX1WIJjdr3eAUGBUNS_hCQ,32597
+odoo/addons/openupgrade_scripts/scripts/l10n_pl/17.0.2.0/upgrade_analysis.txt,sha256=V3zRGC4PZ5GOmKnfs1EUmNZH-vutwhONewLvCYBfwIU,51037
+odoo/addons/openupgrade_scripts/scripts/l10n_pt/17.0.1.0/upgrade_analysis.txt,sha256=XO_E12q6yup73hIkaYK_M99HMCnXXXnRpfniAvylQ4w,32597
 odoo/addons/openupgrade_scripts/scripts/l10n_ro/17.0.1.0/upgrade_analysis.txt,sha256=ELAxo_Sr9gjqQR3jPeM5M6SJDSJqe54e_pOOAf0CkNk,43740
-odoo/addons/openupgrade_scripts/scripts/l10n_ro_edi/17.0.1.0/upgrade_analysis.txt,sha256=N99PIShMQycbdaCHtRhisld_YOTygiC-yjaF1Ofo2UA,372
+odoo/addons/openupgrade_scripts/scripts/l10n_ro_edi/17.0.1.0/upgrade_analysis.txt,sha256=Bua5BSwluMfh5oNEGvt8o56fE4a6gTHtzySuUjbbe8A,383
 odoo/addons/openupgrade_scripts/scripts/l10n_rs/17.0.1.0/upgrade_analysis.txt,sha256=uUy8DJl9XAu_nPeINcBAhUsQrGj3Q7a0-cfjHU0c7y4,24804
+odoo/addons/openupgrade_scripts/scripts/l10n_rw/17.0.1.0/upgrade_analysis.txt,sha256=ZtL7pOIlznd-CtGUwlbSJrWCOzV8DVjwQ4D2s5eZXNc,3031
 odoo/addons/openupgrade_scripts/scripts/l10n_sa/17.0.2.0/upgrade_analysis.txt,sha256=q82aFlmxabk909yE5ad_JuIrpG_N34MhJGDq51aeIuQ,11074
 odoo/addons/openupgrade_scripts/scripts/l10n_sa_edi/17.0.0.1/upgrade_analysis.txt,sha256=SscM-Qa5TyQP8SqyMbzbuJSUjBDmNA3OC193ISlL5FM,754
 odoo/addons/openupgrade_scripts/scripts/l10n_se/17.0.1.0/upgrade_analysis.txt,sha256=aQH0MAvJGcFdIwasXsOF0TQL84P8hb1io6ZCfItvA08,59152
 odoo/addons/openupgrade_scripts/scripts/l10n_sg/17.0.2.2/upgrade_analysis.txt,sha256=nQE_H2373Sgb-MjRct5chRXkygClVxF4KrI20wV4bI0,11360
 odoo/addons/openupgrade_scripts/scripts/l10n_si/17.0.1.1/upgrade_analysis.txt,sha256=u_z8rSX5yYajU5p_CYVVfCo8x-yebPDKXspuVq4wl5Y,31221
 odoo/addons/openupgrade_scripts/scripts/l10n_sk/17.0.1.0/upgrade_analysis.txt,sha256=LX3fK0SHyMpLZNL4O6bDo7dC_8ODDDeumfhYQ_4jXvo,29204
+odoo/addons/openupgrade_scripts/scripts/l10n_sn/17.0.1.0/upgrade_analysis.txt,sha256=nZVeD4Jj0zakKYw84bkTZ1vCDpEmDIQQkTPzBP_tI_0,4108
 odoo/addons/openupgrade_scripts/scripts/l10n_syscohada/17.0.1.0/upgrade_analysis.txt,sha256=qsfmkR_eaqyCAjOgMll5hbrvaElVeNPvkfvJcbsqJAY,61515
+odoo/addons/openupgrade_scripts/scripts/l10n_td/17.0.1.0/upgrade_analysis.txt,sha256=bY9Ko_QMg1hTwWeK013lCCCloWnxrf1fcwpdWiLIsnQ,2624
+odoo/addons/openupgrade_scripts/scripts/l10n_tg/17.0.1.0/upgrade_analysis.txt,sha256=7t5LoI0okAOztUXi85ZaTh-A7cjOMJhVR1_g488Vrwk,4249
 odoo/addons/openupgrade_scripts/scripts/l10n_th/17.0.2.0/upgrade_analysis.txt,sha256=b-Tsxk6R4Oz_GtQ53ErP3kTaQ8GM9smcH0pMZDDLj-c,2918
-odoo/addons/openupgrade_scripts/scripts/l10n_tn/17.0.1.0/upgrade_analysis.txt,sha256=hc5lESdrbmKg9yadGUOVl9neebwDX-YMFXOZ8TYP5vw,5715
+odoo/addons/openupgrade_scripts/scripts/l10n_tn/17.0.1.0/upgrade_analysis.txt,sha256=UUEoi7iRhS9QqYWzm42zCNxfcfjOhPq_qwB4YSPEYAc,5710
 odoo/addons/openupgrade_scripts/scripts/l10n_tr/17.0.1.1/upgrade_analysis.txt,sha256=q1shwrQA39v_cMDgowIYgEBNlcfQvn1uGmnBLij828Q,15173
 odoo/addons/openupgrade_scripts/scripts/l10n_tw/17.0.1.0/upgrade_analysis.txt,sha256=vsiF7X5XAe_6Vq-dbOdmF6wVfzFM9uV6ze-_NTSXDLk,6370
 odoo/addons/openupgrade_scripts/scripts/l10n_ua/17.0.1.4/upgrade_analysis.txt,sha256=gexXdv-iP_cSmrhYHiqaXxvVoz-_zH5v0COZ67wQm7k,24232
 odoo/addons/openupgrade_scripts/scripts/l10n_ug/17.0.1.0.0/upgrade_analysis.txt,sha256=s9XH8RpkZtsWSw_gyngNG2tiuHLto46BLdVd2SRAkxc,4525
 odoo/addons/openupgrade_scripts/scripts/l10n_uk/17.0.1.0/upgrade_analysis.txt,sha256=lxHhBfE8KqstgeoCKWj8EZwnwxECIDFLdIlvFb967tM,5043
 odoo/addons/openupgrade_scripts/scripts/l10n_us/17.0.1.1/upgrade_analysis.txt,sha256=51Rh03FF-TtMNgBFnSEhlaAYuLGpJF7WKp6bL6jSs8s,144
 odoo/addons/openupgrade_scripts/scripts/l10n_uy/17.0.0.1/upgrade_analysis.txt,sha256=Gs2KyHAyGEjmhFBdr4xKnkipD2y0MNbjSdD9yJSimOs,12484
 odoo/addons/openupgrade_scripts/scripts/l10n_ve/17.0.1.0/upgrade_analysis.txt,sha256=bVzcxa-Tq5tRplK3hfECj5Oxw1OIsr2lkKX6XOMeves,19110
 odoo/addons/openupgrade_scripts/scripts/l10n_vn/17.0.2.0.2/upgrade_analysis.txt,sha256=bcwfroXtnxHJlL_J42TuHBjxcSMW5iZeS7vB_yaS2pg,10061
+odoo/addons/openupgrade_scripts/scripts/l10n_vn/17.0.2.0.3/upgrade_analysis.txt,sha256=g3iY3r3XnUAVEN3cGuIx7VqqUsjhHL5CESP0U32IUZ0,10357
 odoo/addons/openupgrade_scripts/scripts/l10n_za/17.0.1.0/upgrade_analysis.txt,sha256=jSHUTK6JelHn7KLHqsIOFMzU43P20lzvfgnm_H35ymg,5865
-odoo/addons/openupgrade_scripts/scripts/link_tracker/17.0.1.1/upgrade_analysis.txt,sha256=rg9wP40ezjFxhTmCDIFNL35QrL1Xk4y576z2Xe8Z5gk,191
-odoo/addons/openupgrade_scripts/scripts/loyalty/17.0.1.0/upgrade_analysis.txt,sha256=QAninJTXF1aA_Li7fMre7xiQdut90FXSXsmHVAvh0BM,1166
-odoo/addons/openupgrade_scripts/scripts/lunch/17.0.1.0/upgrade_analysis.txt,sha256=BXRTmytlJS7-6c1lmSifxKCQ4hlNJUvwNajs0Vffk0c,645
-odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/noupdate_changes.xml,sha256=PdOXeVoRJiAP_E-6UTiD6JzhqdpKpvgJqrjOu8yRRpE,295
-odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/upgrade_analysis.txt,sha256=K2_AZ0zicVbPRskYLLjsf03g9_lB0xQUt9wo8_xwKJs,29124
+odoo/addons/openupgrade_scripts/scripts/l10n_zm_account/17.0.1.0.0/upgrade_analysis.txt,sha256=f-cpEdre1AIw_17-8tOMHS4CB6IrMNjVvHe0HnYCqIU,6759
+odoo/addons/openupgrade_scripts/scripts/link_tracker/17.0.1.1/upgrade_analysis.txt,sha256=Ph-CuEBHU1WnRHswlXmC4YvE1LOo-0EpydbqIJ4VBSU,159
+odoo/addons/openupgrade_scripts/scripts/loyalty/17.0.1.0/upgrade_analysis.txt,sha256=jWV55rwgBPyCjXd0gEJnIEisKco9NECZ2seDTfB7iK0,689
+odoo/addons/openupgrade_scripts/scripts/lunch/17.0.1.0/upgrade_analysis.txt,sha256=tTe-ZlM47vbXf75E9H8TVoqH5QMiwIx5MeRcsX4SWeo,483
+odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/noupdate_changes.xml,sha256=iOXTf9rRqmvM-3sDVcpZloO4TbYSLHfFTxvnAS8e03Y,571
+odoo/addons/openupgrade_scripts/scripts/mail/17.0.1.15/upgrade_analysis.txt,sha256=GyLpga-5sv4cRCbvixwqt1OTzLQXgeomkqZqms-01HY,29205
 odoo/addons/openupgrade_scripts/scripts/mail_bot/17.0.1.2/upgrade_analysis.txt,sha256=ejERvDwnBDajVnF6gvSuVxwZ_y6EfX2_oL7s0BM8u8M,147
-odoo/addons/openupgrade_scripts/scripts/mail_group/17.0.1.1/upgrade_analysis.txt,sha256=CwOepUVWXx2WqyZlRYufgo2pO12-OXwLGpHz8KWrcgw,660
-odoo/addons/openupgrade_scripts/scripts/mail_plugin/17.0.1.0/upgrade_analysis.txt,sha256=Z19OC0sGlFH2o2Vg7Ab3PxHH4mEfDTiM6EQX_gjVmso,236
+odoo/addons/openupgrade_scripts/scripts/mail_group/17.0.1.1/upgrade_analysis.txt,sha256=E0agjcK6Npj-0X_35yQi_ecGrkAR7qjEHVrTVtNuH-4,489
+odoo/addons/openupgrade_scripts/scripts/mail_plugin/17.0.1.0/upgrade_analysis.txt,sha256=h6XIVfM3wiiw-zTZJGStrvhE2Yl99HnLUU2aMhwzQlQ,154
 odoo/addons/openupgrade_scripts/scripts/maintenance/17.0.1.0/noupdate_changes.xml,sha256=uygqhU4b0ic9c3pZgCJNm7lo7i7Ak1rpgAaWDzzN3ec,324
-odoo/addons/openupgrade_scripts/scripts/maintenance/17.0.1.0/upgrade_analysis.txt,sha256=8dnmZBSRj1u_MfQkmLKxV8MB4mTmSCCn0D8rADjokWg,2646
+odoo/addons/openupgrade_scripts/scripts/maintenance/17.0.1.0/upgrade_analysis.txt,sha256=fh-mn82bXY9wHefpPp-eTr1mNghugC38UbRRHj9xZuc,2566
 odoo/addons/openupgrade_scripts/scripts/mass_mailing/17.0.2.7/noupdate_changes.xml,sha256=RKyrNMRIRgC-aVyUGSRPCIHhGgJPSoCelpxc0vqk1Qc,1285
-odoo/addons/openupgrade_scripts/scripts/mass_mailing/17.0.2.7/upgrade_analysis.txt,sha256=KH1mwxwvBjFIuigfFrmxlNXGgvNUWhgtDbdvr4q7HT4,7962
+odoo/addons/openupgrade_scripts/scripts/mass_mailing/17.0.2.7/upgrade_analysis.txt,sha256=6S9Nqf8jVsJ7Yl-9LARWYpLS3-jg4tnEJG3-R62KX7g,7887
 odoo/addons/openupgrade_scripts/scripts/mass_mailing_crm/17.0.1.0/upgrade_analysis.txt,sha256=BVrq7-HrrvKTT70fOrzoLLJcKJE9l0ha0pQFQCxIraw,171
 odoo/addons/openupgrade_scripts/scripts/mass_mailing_crm_sms/17.0.1.0/upgrade_analysis.txt,sha256=d0q6azg3QaDVK3BUFFU2oezpoAroXvP86cy9MfBG0nQ,183
 odoo/addons/openupgrade_scripts/scripts/mass_mailing_sale/17.0.1.0/upgrade_analysis.txt,sha256=n8hHiyB7ic-SLmZiXuIF6aJCwvHKMz0DvSI9-6BgmO8,174
 odoo/addons/openupgrade_scripts/scripts/mass_mailing_sale_sms/17.0.1.0/upgrade_analysis.txt,sha256=utUZ_Od1hP8vgomiOt0J2osjPFbyiPlsr_0PfofGZOA,186
 odoo/addons/openupgrade_scripts/scripts/mass_mailing_sms/17.0.1.1/upgrade_analysis.txt,sha256=ooMFxakFOuZ3BuI9CPQ8ObsPDDAIEOUCi_-zGbfrYb0,1452
 odoo/addons/openupgrade_scripts/scripts/mass_mailing_themes/17.0.1.2/upgrade_analysis.txt,sha256=HQrh6bPZbbwLR4Jidz8y2OcRA4m0EI0dfWSlykClaJY,1032
-odoo/addons/openupgrade_scripts/scripts/membership/17.0.1.0/upgrade_analysis.txt,sha256=84eqRJamaUV1VrR_ftlWug7ScHb2Gm7ovgI92bNCM8E,388
+odoo/addons/openupgrade_scripts/scripts/membership/17.0.1.0/upgrade_analysis.txt,sha256=wWAm-YkWtrr2dsyDIjW-T45qz2rYWj2Z8_BYLD8S9gw,254
 odoo/addons/openupgrade_scripts/scripts/microsoft_account/17.0.1.0/upgrade_analysis.txt,sha256=A-hAfz4jaf1_-Uw2-6JP4inCGDe6LXPvVvXb7Dk9Nyc,174
-odoo/addons/openupgrade_scripts/scripts/microsoft_calendar/17.0.1.0/upgrade_analysis.txt,sha256=Gzn-1-1ANpfEG7V-6IA7mRebH-qBFJ0fftDbBeAEhNk,1511
+odoo/addons/openupgrade_scripts/scripts/microsoft_calendar/17.0.1.0/upgrade_analysis.txt,sha256=EHFEvy7AiiO0ZtkXFxTv4k_pjvLONtoHy_-lF_Ufou0,1597
 odoo/addons/openupgrade_scripts/scripts/microsoft_outlook/17.0.1.1/upgrade_analysis.txt,sha256=AN9OrdoYh8Y4Fk0wPIc2_UuVePoboGlV1VonIbSS1Lk,338
-odoo/addons/openupgrade_scripts/scripts/mrp/17.0.2.0/upgrade_analysis.txt,sha256=qmse93_OsWeUkDmTU62UJN9hwe_GZ5z4VUDZ34qhdko,5891
+odoo/addons/openupgrade_scripts/scripts/mrp/17.0.2.0/upgrade_analysis.txt,sha256=SUyfsy7gSwA3JjijwDpzeAbnEOQ_9CgXrjSI1QyUmhA,5460
 odoo/addons/openupgrade_scripts/scripts/mrp_account/17.0.1.0/upgrade_analysis.txt,sha256=skwQ5fex7b4rCA-ybCPnM2OoirPpiArMDM6BLt8jN3Q,3346
 odoo/addons/openupgrade_scripts/scripts/mrp_landed_costs/17.0.1.0/upgrade_analysis.txt,sha256=5nXyL4HwISqtYoWtiWaRdUNUoUOIK0JpvbyhG2vN-qo,171
 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting/17.0.0.1/upgrade_analysis.txt,sha256=AkP3hDgUkv3hFtRAP6PRm4x4qMN3PnEmJmZ2PuifLe0,228
 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting_dropshipping/17.0.0.1/upgrade_analysis.txt,sha256=pLdZ-5FaS_z13cr2LSIb9wNj1OQbvWbngccheKzZ0WM,216
 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting_purchase/17.0.0.1/upgrade_analysis.txt,sha256=nHbm5OAhiaJSooOQhPdHdTKv7Fw4M74JtqGFLs1Nh6E,204
 odoo/addons/openupgrade_scripts/scripts/mrp_subcontracting_repair/17.0.1.0/upgrade_analysis.txt,sha256=UJG7h7RycYDJhDS8aYUjG4NPD10fHmmqdiSFn_TCtuM,334
-odoo/addons/openupgrade_scripts/scripts/onboarding/17.0.1.2/upgrade_analysis.txt,sha256=VHGZTnBrE2QrvY64fmyJmw6ZmIv9cwdzpziMBRosu0o,2393
+odoo/addons/openupgrade_scripts/scripts/onboarding/17.0.1.2/upgrade_analysis.txt,sha256=tNmwSx9jop0RrJYtrrnNhfX2LWTCC3BFgCyAmXlDRf8,2308
 odoo/addons/openupgrade_scripts/scripts/partner_autocomplete/17.0.1.1/upgrade_analysis.txt,sha256=paOY8Lbl9k1Jia6eIWsY_xqS8Kx-eqlazzgUVKmtvF8,226
-odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/noupdate_changes.xml,sha256=lsTXdJzgNlb_epNXYnallUL_pz1YYyvFIFpd7L9Igjc,17137
-odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/upgrade_analysis.txt,sha256=DD3i56nCigS5R9_mYzvC1Z1y7Q3XmQI8Btn3alMog8o,19599
+odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/noupdate_changes.xml,sha256=xK0P6eZCmne2ymz0YA4C-bFcTW3vvLeQV-C4mrKtDvo,17009
+odoo/addons/openupgrade_scripts/scripts/payment/17.0.2.0/upgrade_analysis.txt,sha256=5Yr64t5JwAzvJQbAQVCUmZem0iP_TkQScI8Bn_0yJm8,19520
 odoo/addons/openupgrade_scripts/scripts/payment_adyen/17.0.2.0/upgrade_analysis.txt,sha256=SRNjWvxDZsXfmhLBdRjmCe5UjcP4gUDIg3frg2HVRlk,616
 odoo/addons/openupgrade_scripts/scripts/payment_aps/17.0.1.0/upgrade_analysis.txt,sha256=2nnydSFnYzm-7cyQnuwLNiYmBBqVzhlWILLjf8ncTGU,156
 odoo/addons/openupgrade_scripts/scripts/payment_asiapay/17.0.1.0/upgrade_analysis.txt,sha256=UwiZakgNyVZBEPfHdr2DnEnoUm-ou60biaIsBE1ETF8,397
 odoo/addons/openupgrade_scripts/scripts/payment_authorize/17.0.2.0/upgrade_analysis.txt,sha256=EYIclOtewm01Z5JwohstVM-VwRdyyHzQ_-o625-N2mM,526
 odoo/addons/openupgrade_scripts/scripts/payment_buckaroo/17.0.2.0/upgrade_analysis.txt,sha256=g1jJNuVhi9T4-5DuZtkV4SjIQxt8OGy6qTdHNqM3_F8,171
 odoo/addons/openupgrade_scripts/scripts/payment_custom/17.0.2.0/noupdate_changes.xml,sha256=JWcF3Qwm5su55-D-Owu_PKApAeWJ2sUsk0La_hAFSEM,304
 odoo/addons/openupgrade_scripts/scripts/payment_custom/17.0.2.0/upgrade_analysis.txt,sha256=oGadMzoHyKTbpLK1Tjshjt94QfrFDcuQlVw0FTOQbPE,384
@@ -283,160 +318,163 @@
 odoo/addons/openupgrade_scripts/scripts/payment_mollie/17.0.1.0/upgrade_analysis.txt,sha256=8tsBPF01-wXrb46gx8SWqYU-qqLr_ei17ZRdzJU0wOU,165
 odoo/addons/openupgrade_scripts/scripts/payment_paypal/17.0.2.0/upgrade_analysis.txt,sha256=0nV4MCJ_14f6DtDTK62E2jjyYmXyuVURxfXwJXVnZ2o,362
 odoo/addons/openupgrade_scripts/scripts/payment_razorpay/17.0.1.0/upgrade_analysis.txt,sha256=ClntnGJTic21gEZlM223TvcYyePPPhPlg6oW5VHpmAg,171
 odoo/addons/openupgrade_scripts/scripts/payment_sips/17.0.2.0/upgrade_analysis.txt,sha256=jcNAnS3qIQ_cwRKtwGlnRMOp93z86Dt25oXuziyUZp8,159
 odoo/addons/openupgrade_scripts/scripts/payment_stripe/17.0.2.0/noupdate_changes.xml,sha256=ZpbCtVdmQ-xDYb92ZSlz_oKfPpcKycmLR826EU6R-V8,197
 odoo/addons/openupgrade_scripts/scripts/payment_stripe/17.0.2.0/upgrade_analysis.txt,sha256=C8v3ngfImENCbbM7zx2kgbjS-ICtxK0xu0m6Azl9ZOQ,450
 odoo/addons/openupgrade_scripts/scripts/payment_xendit/17.0.1.0/upgrade_analysis.txt,sha256=RM5ORztDmdzXwxOs0m6ZR7bFQ9xmckKm6l9FS52ERuw,670
-odoo/addons/openupgrade_scripts/scripts/phone_validation/17.0.2.1/upgrade_analysis.txt,sha256=JsqK81vlbMbIuP3thPhMjyjPM6ITOszLFVZCXTQ27Z4,327
+odoo/addons/openupgrade_scripts/scripts/phone_validation/17.0.2.1/upgrade_analysis.txt,sha256=WYwF7sN06juJO8wJgo3x5a3zGPiK7elW0VPONJAcFlQ,244
 odoo/addons/openupgrade_scripts/scripts/point_of_sale/17.0.1.0.1/noupdate_changes.xml,sha256=F4Kh_Yt5cGoCpZHwkEoQcYinUAA2fWVBi9caOpQ3HIM,1703
-odoo/addons/openupgrade_scripts/scripts/point_of_sale/17.0.1.0.1/upgrade_analysis.txt,sha256=0SGW7Ncecbj8JVh4Z2FmpYcbuS955JXszTwh19qjgXg,8810
+odoo/addons/openupgrade_scripts/scripts/point_of_sale/17.0.1.0.1/upgrade_analysis.txt,sha256=BCxMx5uMa7_Q9n3dAc3xPT7AQFueSHPW5ZQyttdWFb8,7525
 odoo/addons/openupgrade_scripts/scripts/portal/17.0.1.0/noupdate_changes.xml,sha256=C95FpUACAYgKGXgvgM_1k2M9KWQf388BMez1aezBpnM,6652
 odoo/addons/openupgrade_scripts/scripts/portal/17.0.1.0/upgrade_analysis.txt,sha256=wVgFbe9vvSwfQ_3TLIPqg0UwuRe7DFF45cysJi2EXG8,976
 odoo/addons/openupgrade_scripts/scripts/portal_rating/17.0.1.0/upgrade_analysis.txt,sha256=dt8MndjuYESltTYyrh13cfmzzjrF_Brunh5zVVq9fPI,162
 odoo/addons/openupgrade_scripts/scripts/pos_adyen/17.0.1.0/upgrade_analysis.txt,sha256=ioVjKoLZ5SzBZenooNNKgKwAaYLNRN1VQkOQNryoky8,150
 odoo/addons/openupgrade_scripts/scripts/pos_discount/17.0.1.0/upgrade_analysis.txt,sha256=ouZ1QrOAtVH6WODXjgDIy5rkoXbI8c_PJsqLZ69pl7U,159
 odoo/addons/openupgrade_scripts/scripts/pos_epson_printer/17.0.1.0/upgrade_analysis.txt,sha256=8LygfjEmUtAdvToAxgrx7qaH3hw_Y2kfRU_felLx8LA,428
 odoo/addons/openupgrade_scripts/scripts/pos_hr/17.0.1.0/upgrade_analysis.txt,sha256=lgWW5l0qorpLgVFB0GeoDiGtGV0jfEQzzkRWPWcueNY,404
 odoo/addons/openupgrade_scripts/scripts/pos_loyalty/17.0.2.0/upgrade_analysis.txt,sha256=MXLSCU4IZdzuhRMSc3-rJI26Ig6I4USV6DlTZH1zPOI,161
+odoo/addons/openupgrade_scripts/scripts/pos_mercado_pago/17.0.1.0/upgrade_analysis.txt,sha256=iWs9vjZmWB9kSaGDXabwGt2q2F_ixk9UV6YnPsb_Xzc,548
 odoo/addons/openupgrade_scripts/scripts/pos_mercury/17.0.1.0/upgrade_analysis.txt,sha256=bySWnWZbZBC_QeNjERtsGmHj-4zVfHKr_drN9lVxrGQ,269
 odoo/addons/openupgrade_scripts/scripts/pos_online_payment/17.0.1.0/upgrade_analysis.txt,sha256=CAl8kOyWMJe__4JqS3q2tPy8WCQdMm-0JttcPWptHdA,1452
 odoo/addons/openupgrade_scripts/scripts/pos_online_payment_self_order/17.0.1.0/upgrade_analysis.txt,sha256=mnClgb82R34_OsFAvyMexVHsC31BZZAuF7r1vlrB_4s,524
 odoo/addons/openupgrade_scripts/scripts/pos_paytm/17.0.1.0/upgrade_analysis.txt,sha256=L919F_OMTaimxlqwIwm5obBmcLm0DV5yO2pRrvqejP8,1403
+odoo/addons/openupgrade_scripts/scripts/pos_razorpay/17.0.1.0/upgrade_analysis.txt,sha256=4sobPz7dRnyzVabeE4g4xu63fVz-ziArt0q2Q7zBif4,1368
 odoo/addons/openupgrade_scripts/scripts/pos_restaurant/17.0.1.0/upgrade_analysis.txt,sha256=VkKGMS_ORc32c-t4U3oKBVbjIjEaizxdR2Dfhv8WbBY,2288
 odoo/addons/openupgrade_scripts/scripts/pos_restaurant_adyen/17.0.1.0/upgrade_analysis.txt,sha256=Tm2XlP6Xsn-oIwmeP2NtJVhLNxYn4BPoB3nw8b7CMJ4,183
 odoo/addons/openupgrade_scripts/scripts/pos_sale/17.0.1.1/upgrade_analysis.txt,sha256=7y3xpcTs8PhH6C_P4n6MaH4MFNXEbMx940jxajG4qQA,147
 odoo/addons/openupgrade_scripts/scripts/pos_self_order/17.0.1.0/upgrade_analysis.txt,sha256=j5VuWsvHqQ01z5Y0b6x5XrXp2CTskoAncWn2mtmiPDE,4099
 odoo/addons/openupgrade_scripts/scripts/pos_self_order_sale/17.0.1.0/upgrade_analysis.txt,sha256=JvKCInWRG8uEaf4Cg0nydcTvdGBzwrzKGCEVhIctVJ0,271
 odoo/addons/openupgrade_scripts/scripts/pos_self_order_stripe/17.0.1.0/upgrade_analysis.txt,sha256=yjYh_tfKaznEoffuHtXtYACTWoFRkuhr03o_XjJ9FDg,191
 odoo/addons/openupgrade_scripts/scripts/pos_six/17.0.1.0/upgrade_analysis.txt,sha256=eSB7CkTlGUXTkAucjdslQ67sKZusoPgVinvkbI-Ae-c,144
 odoo/addons/openupgrade_scripts/scripts/pos_stripe/17.0.1.0/upgrade_analysis.txt,sha256=msYJoACfH4fpPoraAn3Z6NoclsSl2D3-B1v-CkNcCMM,153
 odoo/addons/openupgrade_scripts/scripts/pos_viva_wallet/17.0.1.0/upgrade_analysis.txt,sha256=iRc5yKlN7cDEvxOgMzjyO4Ov5p9IERgRXQKSZaZiioo,983
 odoo/addons/openupgrade_scripts/scripts/privacy_lookup/17.0.1.0/upgrade_analysis.txt,sha256=l6bZO4RUtpRzJYYglTiPCXBa2Lni5Tl4AqAHkL0qU6g,165
 odoo/addons/openupgrade_scripts/scripts/product/17.0.1.2/noupdate_changes.xml,sha256=RSxFOsd4wdaBB3sPTKLB-280CYCCltUK29A7wt04uvA,990
-odoo/addons/openupgrade_scripts/scripts/product/17.0.1.2/upgrade_analysis.txt,sha256=S8HVAqTyxQsIYcy4XWhwm5irmWIMFi6Ddd9Ie6yGoUQ,4946
+odoo/addons/openupgrade_scripts/scripts/product/17.0.1.2/upgrade_analysis.txt,sha256=rBuU0mMaB8rZJOWdY1adG50c-nm79Jw7zPsK3JhPFrY,4637
 odoo/addons/openupgrade_scripts/scripts/product_email_template/17.0.1.0/upgrade_analysis.txt,sha256=Dx6pySBrbJMWmtd4YMb2kJvvwUS13cMjXP0r6zLfLWk,189
 odoo/addons/openupgrade_scripts/scripts/product_expiry/17.0.1.0/upgrade_analysis.txt,sha256=VADhu7NUifZB0Q9deDB7ZYLYxXIQ4X7XhUAtbFu-nkc,611
 odoo/addons/openupgrade_scripts/scripts/product_images/17.0.1.0/upgrade_analysis.txt,sha256=ZFdJzO3tOMvoa1XV86Kzqw5uqUSHhXmQjlN8ebFkbS8,165
 odoo/addons/openupgrade_scripts/scripts/product_margin/17.0.1.0/upgrade_analysis.txt,sha256=4ttHOXP24HQX80aD5j6gIjzZBzhAD599KgvOxkR9wmM,165
-odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/noupdate_changes.xml,sha256=5g_wIW2pm2io5zvP9M22uUsm2lzIOIPML84Xpw4K0DM,6545
-odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/upgrade_analysis.txt,sha256=i7k4QY5ZbmgUpx2bTt7FOTTEVSGbTkW5ZuyB_3TrJDo,14255
+odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/noupdate_changes.xml,sha256=kuc_hH18-FzRvDUBYZ-PZak_1MlhVqZOA0YY1mXNah8,6665
+odoo/addons/openupgrade_scripts/scripts/project/17.0.1.3/upgrade_analysis.txt,sha256=IplxnUO7IaWhFqn-cdKH6WrsihyAqOHQh8_jmdeWycQ,14096
 odoo/addons/openupgrade_scripts/scripts/project_account/17.0.1.0/upgrade_analysis.txt,sha256=lx-fG9hTBhBenpcIyDgWbGbyeiOgNnI8zaDZQYaog0Y,651
 odoo/addons/openupgrade_scripts/scripts/project_hr_expense/17.0.1.0/upgrade_analysis.txt,sha256=yACyVRcjb1HQpDunih7oLjN_mOPWDyMhm6JOgYUhNmM,177
 odoo/addons/openupgrade_scripts/scripts/project_mrp/17.0.1.0/upgrade_analysis.txt,sha256=-MQoSXEnRnNoFaQbQ3KinscFFDASuoP70EbSph6GiyQ,156
 odoo/addons/openupgrade_scripts/scripts/project_purchase/17.0.1.0/upgrade_analysis.txt,sha256=jgjpdClHsIsq53eXrIju1wh8NCuO-1F-e5flC_6q39k,171
 odoo/addons/openupgrade_scripts/scripts/project_sms/17.0.1.0/upgrade_analysis.txt,sha256=dR99xE_4XIcYrpFBaImCpc-lyQqpXvh7cCaCftuygr0,156
 odoo/addons/openupgrade_scripts/scripts/project_timesheet_holidays/17.0.1.0/upgrade_analysis.txt,sha256=4IIM7egSe9vXluupDMJC7lvBiT3_Ap054Pw0nK8r_z4,225
-odoo/addons/openupgrade_scripts/scripts/project_todo/17.0.1.0/upgrade_analysis.txt,sha256=88bgGroE5pXWTcX4mBVsKqbBw-2yLYOih57RpCcApo4,5194
+odoo/addons/openupgrade_scripts/scripts/project_todo/17.0.1.0/upgrade_analysis.txt,sha256=NHv0b_S2IGg6I4cbhnhlz7LWqwAWG4bC53jsx58rR6c,2038
 odoo/addons/openupgrade_scripts/scripts/purchase/17.0.1.2/noupdate_changes.xml,sha256=wH17u5OtfBg5DfINZ_tHHkZwLGE67IG9D5Z2VIT1cPM,3109
-odoo/addons/openupgrade_scripts/scripts/purchase/17.0.1.2/upgrade_analysis.txt,sha256=cfNHhZnc98yB3Kej1Is4R7SMQOYzSATTjGFndLMdB3E,1174
+odoo/addons/openupgrade_scripts/scripts/purchase/17.0.1.2/upgrade_analysis.txt,sha256=JjGlWWzK2biZHwSLPLA8zrrS2tRUUMqPWsDoOorBWW8,988
 odoo/addons/openupgrade_scripts/scripts/purchase_mrp/17.0.1.0/upgrade_analysis.txt,sha256=E4pgWF7i8oHH6mklWCxmWBkBx8TymHlxBQeYemt09p0,188
 odoo/addons/openupgrade_scripts/scripts/purchase_product_matrix/17.0.1.0/upgrade_analysis.txt,sha256=ziZfZQGATL_2VPdgw-7hgS7661nkDbbYuT_SgMrpFmw,192
 odoo/addons/openupgrade_scripts/scripts/purchase_requisition/17.0.0.1/upgrade_analysis.txt,sha256=-3eCb_nikz-NG3FR7NH6RanmKPBFiTxMVuQXI-aNkcM,642
 odoo/addons/openupgrade_scripts/scripts/purchase_requisition_stock/17.0.1.2/upgrade_analysis.txt,sha256=VBgWrgfN-tlD1isnEjx1DbRhTjvxqZIleJCKlwtjLNo,201
-odoo/addons/openupgrade_scripts/scripts/purchase_stock/17.0.1.2/upgrade_analysis.txt,sha256=ZOQeVbbvlXvWNaEqfZLu8YqO-fFwTA0otAahC_zsGSc,1159
-odoo/addons/openupgrade_scripts/scripts/rating/17.0.1.1/upgrade_analysis.txt,sha256=IWID8xPpz-MV39EBcB-FDlLhEUKiOT1DoOqK2njZV9g,2029
+odoo/addons/openupgrade_scripts/scripts/purchase_stock/17.0.1.2/upgrade_analysis.txt,sha256=xwI3gUi7TJsdNZRCB8f7RAz-P8nOTQZEKYfWLlDwwXI,1458
+odoo/addons/openupgrade_scripts/scripts/rating/17.0.1.1/upgrade_analysis.txt,sha256=cTANEQNjoLgOX8Pq00i60pFdnveHqQ3r641__q41B9I,1959
 odoo/addons/openupgrade_scripts/scripts/repair/17.0.1.0/noupdate_changes.xml,sha256=SsODI46tUtKZGQdz1meM6VsGmT_udVIzdxrWu34fPEs,202
-odoo/addons/openupgrade_scripts/scripts/repair/17.0.1.0/upgrade_analysis.txt,sha256=NjdxJ7x92GvbuGKJnGLFly4hj7NJ_WIIl3klGJwZ02s,9355
+odoo/addons/openupgrade_scripts/scripts/repair/17.0.1.0/upgrade_analysis.txt,sha256=9nq-cpzaimD41mz-A6Y30DYJmblITlWDqShK6AYvufg,9290
 odoo/addons/openupgrade_scripts/scripts/resource/17.0.1.1/upgrade_analysis.txt,sha256=k8PlbWG4vwnNVFc8HjZCH7_eeqIaBU4ZSTn6AUY--MU,939
 odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/noupdate_changes.xml,sha256=wh7d2nRJLcvN16KYMDdTiNqRT0O8siPsNpKlyQGRNxc,13187
-odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/upgrade_analysis.txt,sha256=0YUWjAprMIwzcW3Kdl0KQY-POvfXHA9o5dNx5t5qDe0,5986
+odoo/addons/openupgrade_scripts/scripts/sale/17.0.1.2/upgrade_analysis.txt,sha256=bzIP0uZgpiCqOmfzU1XVfmbi8wAwbA0OoNAAI2quN2w,6014
+odoo/addons/openupgrade_scripts/scripts/sale_async_emails/17.0.1.0/upgrade_analysis.txt,sha256=JkvRgvp29pq_FGyqKSyInOfmQf2N9MCheOEXHc_BHfQ,361
 odoo/addons/openupgrade_scripts/scripts/sale_crm/17.0.1.0/upgrade_analysis.txt,sha256=lv8jHV4r15aW7GmffXmW3R6DrZAoKEC60trv5mjtbdU,147
 odoo/addons/openupgrade_scripts/scripts/sale_expense/17.0.1.0/upgrade_analysis.txt,sha256=fmL9ehU0qjB23ZWgU66K05YBEvF1kjLmbV3p28-CU3M,159
 odoo/addons/openupgrade_scripts/scripts/sale_expense_margin/17.0.1.0/upgrade_analysis.txt,sha256=9d62c8OD-bC7sknkGNfwteGPhnmi9OnL7DDCGu8F-Po,180
-odoo/addons/openupgrade_scripts/scripts/sale_loyalty/17.0.1.0/upgrade_analysis.txt,sha256=Rt05JNKZrnkfCaXwy3Yf00Sha6Ona3Jfy2GcCzKMuYY,259
-odoo/addons/openupgrade_scripts/scripts/sale_loyalty_delivery/17.0.1.0/upgrade_analysis.txt,sha256=bD23IfjJVBYjQBhY16UgcqAARKgsyluEBJAjY07pp08,492
-odoo/addons/openupgrade_scripts/scripts/sale_management/17.0.1.0/upgrade_analysis.txt,sha256=podO42wXHWlLiaMHUDLFMLYHkozFuazXhVTapRSiMDE,998
+odoo/addons/openupgrade_scripts/scripts/sale_loyalty/17.0.1.0/upgrade_analysis.txt,sha256=LhAwNdgq-WE7cBBg7sVusy_5-VwbKTOp7NghdGNP0XE,165
+odoo/addons/openupgrade_scripts/scripts/sale_loyalty_delivery/17.0.1.0/upgrade_analysis.txt,sha256=fpOAUF5-Dt7AhTpQ0iMjbRykigCzXrFYImsQ3j9I4-Q,445
+odoo/addons/openupgrade_scripts/scripts/sale_management/17.0.1.0/upgrade_analysis.txt,sha256=TAqojbmiEub0qQin2F8S0UHFxo1bkc8fPKTIC1aMarU,784
 odoo/addons/openupgrade_scripts/scripts/sale_margin/17.0.1.0/upgrade_analysis.txt,sha256=kCC8jeJAQaUIr1kUQpjMHFA2mFb5xFmapcvXPMwRk7k,156
 odoo/addons/openupgrade_scripts/scripts/sale_mrp/17.0.1.0/upgrade_analysis.txt,sha256=9wUIk_OUtTOJXJKJcKIYhlq1wxaxdPHRpHZ8570WV9g,147
 odoo/addons/openupgrade_scripts/scripts/sale_pdf_quote_builder/17.0.1.0/upgrade_analysis.txt,sha256=dr4vitgrdj5OeL4oIFgOQqqdNfrfVIFpJ2tgzbWjKOQ,1366
 odoo/addons/openupgrade_scripts/scripts/sale_product_configurator/17.0.1.0/upgrade_analysis.txt,sha256=r1WkDZ05m3-WG6lLp_QwJ8hrLZvrOOeCMYQC8J10MT4,477
 odoo/addons/openupgrade_scripts/scripts/sale_product_matrix/17.0.1.0/upgrade_analysis.txt,sha256=-_99R6PnRJKHWr1zvrruy5m0RYjMSSK-QIlU_CNEJjk,180
 odoo/addons/openupgrade_scripts/scripts/sale_project/17.0.1.0/noupdate_changes.xml,sha256=4X3C7DU7KHvzvThgefOMjG2FeaBao3JhWpMcXneIQD8,284
 odoo/addons/openupgrade_scripts/scripts/sale_project/17.0.1.0/upgrade_analysis.txt,sha256=_8PaYQYPR4ktTkgIrbAyenZqhekBQwMkco8yD9vkj6Y,1191
 odoo/addons/openupgrade_scripts/scripts/sale_purchase/17.0.1.0/upgrade_analysis.txt,sha256=zU3l9u9sVc2vJxUfjkE4VbO1T0haJ7jpWA0n28Ks9_A,162
 odoo/addons/openupgrade_scripts/scripts/sale_service/17.0.1.0/upgrade_analysis.txt,sha256=Lhprha4HoPrmPzgSgsg3SdLzr9cy19trFmWZGhwcyKs,227
 odoo/addons/openupgrade_scripts/scripts/sale_stock/17.0.1.0/upgrade_analysis.txt,sha256=XxcJseqIZQZS-XnS07ueuYr6ot_W-XVluSFPnx0Bdqs,454
 odoo/addons/openupgrade_scripts/scripts/sale_timesheet/17.0.1.0/noupdate_changes.xml,sha256=yGW3ZrY1z-siMMt4DreIW96BQevct1WGif1Hwi1_q0s,172
-odoo/addons/openupgrade_scripts/scripts/sale_timesheet/17.0.1.0/upgrade_analysis.txt,sha256=Lr7eocwpT1W2HzB7vrybLnGArLYZeTUYeRhFLo819rQ,1361
-odoo/addons/openupgrade_scripts/scripts/sales_team/17.0.1.1/upgrade_analysis.txt,sha256=tf3uU82T3VsNfWPSe-NcP3pMfp1EshyQPIMIf-vprcE,644
-odoo/addons/openupgrade_scripts/scripts/sms/17.0.3.0/upgrade_analysis.txt,sha256=rjxVwi19OEaCGPbgiwx51ImqiUlOjTKYG4Dy0qG4sZA,3165
-odoo/addons/openupgrade_scripts/scripts/snailmail/17.0.0.4/upgrade_analysis.txt,sha256=pAbPhwnD8aQxIRgW2hRp-SUzEy91PDf4ZNo9xbvxHnA,1610
+odoo/addons/openupgrade_scripts/scripts/sale_timesheet/17.0.1.0/upgrade_analysis.txt,sha256=A_nXJBOM1ztD2XR9xKvGGl97GTTaR8wswLJGKpY0yWA,1150
+odoo/addons/openupgrade_scripts/scripts/sales_team/17.0.1.1/upgrade_analysis.txt,sha256=VMb2vV6ZCh2oqJEOMAaS2O_2MSF9V_O_E5vb3UHIXGI,579
+odoo/addons/openupgrade_scripts/scripts/sms/17.0.3.0/upgrade_analysis.txt,sha256=Y_8Hs8o6T5rlTnFlXiRFXK11NhP1V4NH4_-r1mqYeKI,3309
+odoo/addons/openupgrade_scripts/scripts/snailmail/17.0.0.4/upgrade_analysis.txt,sha256=DcixjzZMn2A0eGYcgIHBt9mPexQ7764YamSkARZx-Js,1626
 odoo/addons/openupgrade_scripts/scripts/snailmail_account/17.0.0.1/upgrade_analysis.txt,sha256=2X6KuuAqhblfZlcMDpqkn9LJCyVniu2kXxgKdtRdZvc,412
 odoo/addons/openupgrade_scripts/scripts/social_media/17.0.0.1/upgrade_analysis.txt,sha256=o56bAP5vcYlwtDp-xJocqYHfOUU8mQ0ct6Gl0GQPG-8,197
 odoo/addons/openupgrade_scripts/scripts/spreadsheet/17.0.1.0/upgrade_analysis.txt,sha256=7dsZj4-m8gQEWWfZBaMz7CZoS21LXopdR49H9qd9pr8,209
 odoo/addons/openupgrade_scripts/scripts/spreadsheet_dashboard/17.0.1.0/upgrade_analysis.txt,sha256=Avy6tI5qUcLVzk5YxyfHLpNU0bVgVnUs4NxvNByZo_I,1397
 odoo/addons/openupgrade_scripts/scripts/spreadsheet_dashboard_website_sale/17.0.1.0/upgrade_analysis.txt,sha256=AlqrVVhJ3H_Flt1BmWCRt9LzKtsOKuIqf5Bl8LR6H8A,279
 odoo/addons/openupgrade_scripts/scripts/stock/17.0.1.1/noupdate_changes.xml,sha256=YGDqhBLeLXWAemP0jvJnpOH5A-v2dz4UYkjqESa2NHs,358
-odoo/addons/openupgrade_scripts/scripts/stock/17.0.1.1/upgrade_analysis.txt,sha256=9SuFBEnOw-jQmU5LWuE3TemEsCWVdCvoBKbhNQr1Uk4,9797
-odoo/addons/openupgrade_scripts/scripts/stock_account/17.0.1.1/upgrade_analysis.txt,sha256=Eb4Gmy9RdH9kUDt2m78l9D88s-KknZNOk6HwhnXrmaQ,965
+odoo/addons/openupgrade_scripts/scripts/stock/17.0.1.1/upgrade_analysis.txt,sha256=0RgaAJFzljGj8kQVeQdGE7FXrSnDWnhT_wXw7m0ToHc,9017
+odoo/addons/openupgrade_scripts/scripts/stock_account/17.0.1.1/upgrade_analysis.txt,sha256=_ofS0N620PedBYmOA8N9ZVMYRI9wLpwFWdI6LYgwn4s,1191
 odoo/addons/openupgrade_scripts/scripts/stock_delivery/17.0.1.0/upgrade_analysis.txt,sha256=CLgw08khF3b9hOisl8TGCFjl6B39MDMIimyNDq25AzA,6177
 odoo/addons/openupgrade_scripts/scripts/stock_dropshipping/17.0.1.0/upgrade_analysis.txt,sha256=hcBfhjP7WZQKAPAP1YrQ27M7wowBjSoq3KdMomof7w8,555
 odoo/addons/openupgrade_scripts/scripts/stock_landed_costs/17.0.1.1/upgrade_analysis.txt,sha256=Br1-ciAX9gqR-PM5ehCWgKjpsWUrtaJHYowwvZIzNik,677
 odoo/addons/openupgrade_scripts/scripts/stock_landed_costs_company/17.0.1.0/upgrade_analysis.txt,sha256=gCAzd0WhYUClb548cJUaF2UGrlj4X0N1KGkmp9J1xNE,297
 odoo/addons/openupgrade_scripts/scripts/stock_picking_batch/17.0.1.0/upgrade_analysis.txt,sha256=D5ga0lVXgepoip2hpy8IkAyPIUx9JK7S6rgegxP_Hq0,696
 odoo/addons/openupgrade_scripts/scripts/stock_sms/17.0.1.0/upgrade_analysis.txt,sha256=WmtD-QRPZnTjNKvErYIFRz_n-t4C2ttxPz_9eYkTOrw,150
-odoo/addons/openupgrade_scripts/scripts/survey/17.0.3.6/upgrade_analysis.txt,sha256=LAhcENO3fWc0Q2LMB0Z8QHluRHMzxNCrpmLp5N6DExI,3699
+odoo/addons/openupgrade_scripts/scripts/survey/17.0.3.6/upgrade_analysis.txt,sha256=4pKxvlMav-PO7Hd44Bp1rW-EavfQpql6aNw_ugn6fwk,2379
 odoo/addons/openupgrade_scripts/scripts/transifex/17.0.1.0/upgrade_analysis.txt,sha256=9js2BMOhvgwKRc7amc1kIms0LLC9u6-SmqbXAl4MlUk,150
-odoo/addons/openupgrade_scripts/scripts/uom/17.0.1.0/upgrade_analysis.txt,sha256=ihT9Q7-bE_CIw5b1CzeR87Je1S0j9zSxAeoIYwOKY10,292
-odoo/addons/openupgrade_scripts/scripts/utm/17.0.1.1/upgrade_analysis.txt,sha256=uEQUaIHnHDdcr3MOF_0BMAmPKftIde1iLtL_pAqpNRU,479
+odoo/addons/openupgrade_scripts/scripts/uom/17.0.1.0/upgrade_analysis.txt,sha256=QNpF0ZKtfvAQ5CYA-S7iCVvfMBnNQZXwNhgtA6am5JM,132
+odoo/addons/openupgrade_scripts/scripts/utm/17.0.1.1/upgrade_analysis.txt,sha256=_OOLVSiucvspEHo_3R5b5ikUC1Fbrsf8Xek6KUgUs5c,230
 odoo/addons/openupgrade_scripts/scripts/web/17.0.1.0/upgrade_analysis.txt,sha256=altsaAj1SIkDUKxSNpzJcXzkaufkODuPQkig7ZAa2Rs,628
 odoo/addons/openupgrade_scripts/scripts/web_editor/17.0.1.0/upgrade_analysis.txt,sha256=9B7LNAniPqQGyI_zBwkY8TEvWc6eRyfeDVQd2JQP98g,265
 odoo/addons/openupgrade_scripts/scripts/web_hierarchy/17.0.1.0/upgrade_analysis.txt,sha256=XjtmSJk6VIM6hi3PqyPSwNejLebxNidQ4Spir5fxLWE,430
 odoo/addons/openupgrade_scripts/scripts/web_tour/17.0.0.1/upgrade_analysis.txt,sha256=s140_WtORGtzpb8A4VHm0LTT8XbotPX7DvT_9-6GWto,147
-odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/noupdate_changes.xml,sha256=ORHfzcVoIj27TPiCM-Yk5Fk0iN1QDklHbKZFN79oJ6o,4998
-odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/upgrade_analysis.txt,sha256=q63jRqt36mRl4AB5kMayEa232hB9nCCBJfv9mXyWtS0,15644
-odoo/addons/openupgrade_scripts/scripts/website_blog/17.0.1.1/upgrade_analysis.txt,sha256=NeJJLjhhpGNuWnm-gTDZRZahsDcUPlH8rDnjlsCtgGs,1522
+odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/noupdate_changes.xml,sha256=qZdjILumk1gNqxC3qQrZ9ltbTYjjrHl458VwtAEWlLc,362
+odoo/addons/openupgrade_scripts/scripts/website/17.0.1.0/upgrade_analysis.txt,sha256=f1VN1XwAxqYpqk9j_zDA5Fpo0UsduG3hsuOJIRfMhq8,23040
+odoo/addons/openupgrade_scripts/scripts/website_blog/17.0.1.1/upgrade_analysis.txt,sha256=ddg1heDlJbZKOl9DXIq2LBJlXIluxdvkPzXUYTA-n8Y,1377
 odoo/addons/openupgrade_scripts/scripts/website_cf_turnstile/17.0.1.0/upgrade_analysis.txt,sha256=tW5rUHn4MR1VgqwW0qUYkcVXv5adb6qck43TN8q8EB0,210
 odoo/addons/openupgrade_scripts/scripts/website_crm/17.0.2.1/upgrade_analysis.txt,sha256=y6ZeGUo8Je1ompJpIV8Yn_mMeHTD4TtOGTAnwAArIHo,156
-odoo/addons/openupgrade_scripts/scripts/website_crm_iap_reveal/17.0.1.1/upgrade_analysis.txt,sha256=cSXy1MAJZk_jGLJifBwO6zqV5UNjf-Lyrsb43KEK3FM,245
+odoo/addons/openupgrade_scripts/scripts/website_crm_iap_reveal/17.0.1.1/upgrade_analysis.txt,sha256=6dkVtQb1BZFoAJ8vq1BVh72DQgR-NTj5UJUYX_nZ_68,189
 odoo/addons/openupgrade_scripts/scripts/website_crm_livechat/17.0.1.0/upgrade_analysis.txt,sha256=GAii12o9_VRFYIAM7-IkJjfOqnyuKJAPRzMd6aH1UEI,183
 odoo/addons/openupgrade_scripts/scripts/website_crm_partner_assign/17.0.1.2/upgrade_analysis.txt,sha256=Y3DLpC8wNPscsQj-3XGZB2kGiktdZWkKCCYgmJFnvAE,300
 odoo/addons/openupgrade_scripts/scripts/website_customer/17.0.1.0/upgrade_analysis.txt,sha256=ml1mfj5PM97j8y7LfCPPth7JblWYmkrfbyKGGTYkN8o,617
-odoo/addons/openupgrade_scripts/scripts/website_event/17.0.1.4/upgrade_analysis.txt,sha256=jnvb78WqSwCjKDviGXWWJfxZTPjaur5fdULGREhmkmk,8026
+odoo/addons/openupgrade_scripts/scripts/website_event/17.0.1.4/upgrade_analysis.txt,sha256=iDj2bJYBAVNcb3tZcPonbrB7K4svFoNWyHMATTK8xzU,8160
 odoo/addons/openupgrade_scripts/scripts/website_event_booth/17.0.1.0/upgrade_analysis.txt,sha256=c6fXPFpRf4wBL-wo1LC_27EfLNr8mZHuCQ3qdcYz1G0,615
 odoo/addons/openupgrade_scripts/scripts/website_event_booth_exhibitor/17.0.1.1/upgrade_analysis.txt,sha256=m61WjKd1Qbo78pNqEjrg0Oo8OQqMSjDRoSpC8JGM2Yk,210
 odoo/addons/openupgrade_scripts/scripts/website_event_booth_sale/17.0.1.0/upgrade_analysis.txt,sha256=2jjCDZ4uHskU6CMZLdQvHJuaCbribCHOHiJKETHbE_I,297
 odoo/addons/openupgrade_scripts/scripts/website_event_booth_sale_exhibitor/17.0.1.0/upgrade_analysis.txt,sha256=5DW4vW8QV3NJW7Y1dXqHJghzFwdgOoN6bHnww3cqxrM,225
 odoo/addons/openupgrade_scripts/scripts/website_event_exhibitor/17.0.1.1/upgrade_analysis.txt,sha256=uMWy08V7ommbUVUv7bBo-rctIJoTlmSGwfQZK_1ribA,1080
 odoo/addons/openupgrade_scripts/scripts/website_event_meet/17.0.1.0/upgrade_analysis.txt,sha256=8n6r65MGuzUsRuwI8Wg4GEc-4xf9Gxpc7apDpq7o_T4,424
 odoo/addons/openupgrade_scripts/scripts/website_event_sale/17.0.1.0/upgrade_analysis.txt,sha256=RD6Mzk_JereQL4WGK6xwcVlWKSSWUb4gVT1fTYWheKc,443
-odoo/addons/openupgrade_scripts/scripts/website_event_track/17.0.1.3/upgrade_analysis.txt,sha256=XJ4DVtchZuoFFQSChm6pAl2_gNW0UDS2AFbG7wW8sCY,1615
+odoo/addons/openupgrade_scripts/scripts/website_event_track/17.0.1.3/upgrade_analysis.txt,sha256=4gw_RM8A1lVugLBL49EjxWi0hGaUdIx-06yetcDVrY4,1533
 odoo/addons/openupgrade_scripts/scripts/website_event_track_live/17.0.1.0/upgrade_analysis.txt,sha256=nkw3qu5MZkHIEhC1Ysc3gid3fMt8wW0fmhDZs9h8pck,195
 odoo/addons/openupgrade_scripts/scripts/website_event_track_quiz/17.0.1.0/upgrade_analysis.txt,sha256=UhqqYMoCUY3akNEdgtGeVw35anBJUQjSgit8c1xx_PA,195
 odoo/addons/openupgrade_scripts/scripts/website_form_project/17.0.1.0/upgrade_analysis.txt,sha256=ZOWcB0tufrrhjRnUwoW2RRk638uox68dGHZ1CM1RR5g,266
 odoo/addons/openupgrade_scripts/scripts/website_forum/17.0.1.2/noupdate_changes.xml,sha256=WMg5aQakOKsPS7IS8IeM8Siqnx22XwCEBPD1WvpjNvk,203
-odoo/addons/openupgrade_scripts/scripts/website_forum/17.0.1.2/upgrade_analysis.txt,sha256=B2OijDYw62VIlfFPSGpM81BV2SWMDcqLdmB7QnGFNWc,4871
+odoo/addons/openupgrade_scripts/scripts/website_forum/17.0.1.2/upgrade_analysis.txt,sha256=maKZgyf6btXV16pKT1OGCoLQmvDm8AA1rvODhjs5lMc,4725
 odoo/addons/openupgrade_scripts/scripts/website_hr_recruitment/17.0.1.1/upgrade_analysis.txt,sha256=fgkQdUCtQylRlge2ReZ4TXhBs2KXEeFuHroNSLvPgFY,799
 odoo/addons/openupgrade_scripts/scripts/website_jitsi/17.0.1.0/upgrade_analysis.txt,sha256=UzHl2nfT05b9LOrVtS0ZMq1JlSmG2lWMuoMqOk-ib68,162
 odoo/addons/openupgrade_scripts/scripts/website_livechat/17.0.1.0/upgrade_analysis.txt,sha256=w8uxRaVdRFHLb96GlDsbSWz5fkjrcENAIWLspjUPtS0,871
 odoo/addons/openupgrade_scripts/scripts/website_mass_mailing/17.0.1.0/upgrade_analysis.txt,sha256=c1WE8hDv2O0F3IakOGJfcYwmdEZ8nc11sojJaXBF4-8,203
 odoo/addons/openupgrade_scripts/scripts/website_membership/17.0.1.0/upgrade_analysis.txt,sha256=Qlr3fzc4r6U5TPDsQ96SDEaRaGDOfWB46en4SmAKMus,299
 odoo/addons/openupgrade_scripts/scripts/website_partner/17.0.0.1/upgrade_analysis.txt,sha256=AqFRpGpvtcKlPvvOoTRK8Q7EEA_Bu2wDMvzlhPhwVMM,168
 odoo/addons/openupgrade_scripts/scripts/website_payment/17.0.1.0/upgrade_analysis.txt,sha256=-ZiUNuGcPdUUJYFgvyYehHG9YntLvTAJt14EBYOoalk,406
 odoo/addons/openupgrade_scripts/scripts/website_profile/17.0.1.0/noupdate_changes.xml,sha256=u7GQ77qaXZ4hsr61IqsHM9FzKSriI3ZxpLOgDVrMaXo,5763
 odoo/addons/openupgrade_scripts/scripts/website_profile/17.0.1.0/upgrade_analysis.txt,sha256=sw2P2EUshSepfxC15Zsapn6tgFQYkqysPzQ0vDr2bzo,334
 odoo/addons/openupgrade_scripts/scripts/website_sale/17.0.1.1/noupdate_changes.xml,sha256=JUdxsvgxuZUYwOhYcxqePkslg25_vMbpZA1oZQJTnoY,183
-odoo/addons/openupgrade_scripts/scripts/website_sale/17.0.1.1/upgrade_analysis.txt,sha256=9GOdA1JcyPPw7Df1UVJxFdC9QbOlFxhqnoU75DrO8nc,10047
+odoo/addons/openupgrade_scripts/scripts/website_sale/17.0.1.1/upgrade_analysis.txt,sha256=K2IaitjpS6GQHkUtidHRe_3-yptSvE8_O6rQSyuAwN4,10086
 odoo/addons/openupgrade_scripts/scripts/website_sale_autocomplete/17.0.1.0/upgrade_analysis.txt,sha256=YswdVijMPe2DoMTSlJqSbdFd1ZcTK4PfRvXvm1cd3XM,198
 odoo/addons/openupgrade_scripts/scripts/website_sale_comparison/17.0.1.0/upgrade_analysis.txt,sha256=hLGynBKTJICGodg9l88vtm6YgbNQwOZXBdZ4y4pIT9Q,519
 odoo/addons/openupgrade_scripts/scripts/website_sale_loyalty/17.0.1.0/upgrade_analysis.txt,sha256=99KJxKrOFiemi2WA9ihfINnYz0wn2i2kg2TcD1fjztE,183
-odoo/addons/openupgrade_scripts/scripts/website_sale_mondialrelay/17.0.0.1/upgrade_analysis.txt,sha256=Fpp9J2ckhIKHJaaw36279bmBOIOPcBsON5PKwHa9_Zk,1020
+odoo/addons/openupgrade_scripts/scripts/website_sale_mondialrelay/17.0.0.1/upgrade_analysis.txt,sha256=L4EDMDJph1fWMh5fdgOaWpDWlyHFEURlD_QCT2k9_TI,471
 odoo/addons/openupgrade_scripts/scripts/website_sale_picking/17.0.1.0/upgrade_analysis.txt,sha256=o9JJTmYOOMlQwYSt82mzINOj2BXhZeMv9O3wXtHcQSk,322
-odoo/addons/openupgrade_scripts/scripts/website_sale_product_configurator/17.0.1.0/upgrade_analysis.txt,sha256=YG9z6ZZ57_niOK0hyT9oBR3qsOgp7uk137B_VfeLKzY,811
-odoo/addons/openupgrade_scripts/scripts/website_sale_slides/17.0.1.0/upgrade_analysis.txt,sha256=WuxOxxpZBMrp910qBtksvtYU4Vi3f1WD7GIO5Ja1RQQ,462
+odoo/addons/openupgrade_scripts/scripts/website_sale_product_configurator/17.0.1.0/upgrade_analysis.txt,sha256=SDUMpA_zys-sWFPgoZSj8su-63RjU7vFU-8dkxiNO8M,730
+odoo/addons/openupgrade_scripts/scripts/website_sale_slides/17.0.1.0/upgrade_analysis.txt,sha256=zSCD3PSy3II0eoBSPAjfyFHDix1gwSJebRjGnbVny8c,375
 odoo/addons/openupgrade_scripts/scripts/website_sale_stock/17.0.1.0/upgrade_analysis.txt,sha256=83FSWs7pVR2819cnLXLKq5mTdA6TOz86OK1H2mEsKK8,177
 odoo/addons/openupgrade_scripts/scripts/website_sale_stock_wishlist/17.0.1.0/upgrade_analysis.txt,sha256=FQ7SA9DTeLURU0dXB-jklh-56MxR2nKextuHgB13SnM,204
-odoo/addons/openupgrade_scripts/scripts/website_sale_wishlist/17.0.1.0/upgrade_analysis.txt,sha256=RWvQuFAMlLPa9ftnQsTE4Ff5omjps-98-HkuEvUICIg,1073
+odoo/addons/openupgrade_scripts/scripts/website_sale_wishlist/17.0.1.0/upgrade_analysis.txt,sha256=o6ZGigBPC8hlpMzof4UOUkBCplKALiCphKnUrLIfb10,972
 odoo/addons/openupgrade_scripts/scripts/website_slides/17.0.2.7/noupdate_changes.xml,sha256=K1zKtQ9xzSJ34oIrC_LNNlf3ax6RAXiQbPq6u-Q3HKU,5201
-odoo/addons/openupgrade_scripts/scripts/website_slides/17.0.2.7/upgrade_analysis.txt,sha256=X57np4mpcax-2rXbwwL5Uh2StiqfvgSl5XNZVN3ozuI,5765
+odoo/addons/openupgrade_scripts/scripts/website_slides/17.0.2.7/upgrade_analysis.txt,sha256=cH4hNngP6sjbzajk3ovouYMFovJiditWcsR6_smiQ24,5145
 odoo/addons/openupgrade_scripts/scripts/website_slides_forum/17.0.1.0/noupdate_changes.xml,sha256=mDNdQOQ3VJZSd_HQNh5iI8nWyUdJlw3z8pX8bSLhh5c,1172
-odoo/addons/openupgrade_scripts/scripts/website_slides_forum/17.0.1.0/upgrade_analysis.txt,sha256=Yk7gAzBK19ts56uy_hFgIhqhKX0cbaZZPUAaJW72Bls,790
-odoo/addons/openupgrade_scripts/scripts/website_slides_survey/17.0.1.0/upgrade_analysis.txt,sha256=vfzu6D3iJVu4eJedCqoyfdCX6LXp7PxJWDsB9YIga8U,394
+odoo/addons/openupgrade_scripts/scripts/website_slides_forum/17.0.1.0/upgrade_analysis.txt,sha256=FKHtRCOeB1rA5AaWgcWQi6zDIgohHJlKGrTTsPmj9Es,708
+odoo/addons/openupgrade_scripts/scripts/website_slides_survey/17.0.1.0/upgrade_analysis.txt,sha256=9fjMS7VqhSVDSkhRX9OII63hQPg3xrr6OgZkVvy4R4I,210
 odoo/addons/openupgrade_scripts/scripts/website_twitter/17.0.1.0/upgrade_analysis.txt,sha256=LkD-dmj3O-mCIQ1tlhgb4JpGIQ8_lw_apInOSN8O93o,443
 odoo/addons/openupgrade_scripts/static/description/banner.png,sha256=KTIBu4gfxeZVw9zjs_fivTgFEOeaAorlBxajmCA1p6k,26859
 odoo/addons/openupgrade_scripts/static/description/icon.png,sha256=6xBPJauaFOF0KDHfHgQopSc28kKvxMaeoQFQWZtfZDo,9455
 odoo/addons/openupgrade_scripts/static/description/index.html,sha256=iV41-zYBM4uvZPuunpcr7bQeRgBaojVsKo_gkeyJyA4,12639
-odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/METADATA,sha256=qrDRE9Bj7TfipquCDHmK4E5PZXahyLiu5iY9I1_azFg,3784
-odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/WHEEL,sha256=8Rd4enx1PCuyDWP4SABqO5Fv8rpaknqp3VzjoFFLa6c,83
-odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/top_level.txt,sha256=QE6RBQ0QX5f4eFuUcGgU5Kbq1A_qJcDs-e_vpr6pmfU,4
-odoo_addon_openupgrade_scripts-17.0.1.0.1.2.dist-info/RECORD,,
+odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/METADATA,sha256=6apJV0ZKCCL6uWhTT5pM4i6BcFDs8wa8hz4S-2xYn3M,3784
+odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/WHEEL,sha256=8Rd4enx1PCuyDWP4SABqO5Fv8rpaknqp3VzjoFFLa6c,83
+odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/top_level.txt,sha256=QE6RBQ0QX5f4eFuUcGgU5Kbq1A_qJcDs-e_vpr6pmfU,4
+odoo_addon_openupgrade_scripts-17.0.1.0.1.3.dist-info/RECORD,,
```

