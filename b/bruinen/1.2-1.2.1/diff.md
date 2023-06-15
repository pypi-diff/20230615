# Comparing `tmp/bruinen-1.2.tar.gz` & `tmp/bruinen-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bruinen-1.2.tar", max compression
+gzip compressed data, was "bruinen-1.2.1.tar", max compression
```

## Comparing `bruinen-1.2.tar` & `bruinen-1.2.1.tar`

### file list

```diff
@@ -1,250 +1,250 @@
--rw-r--r--   0        0        0      733 2023-06-09 17:43:51.803315 bruinen-1.2/README.md
--rw-r--r--   0        0        0      559 2023-06-14 23:13:09.859524 bruinen-1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 21:25:54.158184 bruinen-1.2/src/bruinen/__init__.py
--rw-r--r--   0        0        0      155 2023-06-13 22:28:47.788326 bruinen-1.2/src/bruinen/client/__init__.py
--rw-r--r--   0        0        0       47 2023-06-13 22:28:46.187061 bruinen-1.2/src/bruinen/client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 22:28:46.206027 bruinen-1.2/src/bruinen/client/api/accounts/__init__.py
--rw-r--r--   0        0        0     2659 2023-06-13 22:28:47.820237 bruinen-1.2/src/bruinen/client/api/accounts/account_counts_for_policy.py
--rw-r--r--   0        0        0     3992 2023-06-13 22:28:47.841641 bruinen-1.2/src/bruinen/client/api/accounts/accounts_controller_deactivate.py
--rw-r--r--   0        0        0     4074 2023-06-13 22:28:47.848025 bruinen-1.2/src/bruinen/client/api/accounts/accounts_controller_get_accounts.py
--rw-r--r--   0        0        0     4080 2023-06-13 22:28:47.847277 bruinen-1.2/src/bruinen/client/api/accounts/find_all_accounts_for_user.py
--rw-r--r--   0        0        0     4087 2023-06-13 22:28:47.861973 bruinen-1.2/src/bruinen/client/api/accounts/find_all_active_for_user.py
--rw-r--r--   0        0        0     4094 2023-06-13 22:28:47.866459 bruinen-1.2/src/bruinen/client/api/accounts/find_all_active_with_policy_for_user.py
--rw-r--r--   0        0        0     3704 2023-06-13 22:28:47.858873 bruinen-1.2/src/bruinen/client/api/accounts/get_account.py
--rw-r--r--   0        0        0        0 2023-06-13 22:28:46.208236 bruinen-1.2/src/bruinen/client/api/auth/__init__.py
--rw-r--r--   0        0        0     3614 2023-06-13 22:28:47.866146 bruinen-1.2/src/bruinen/client/api/auth/get_user_auth_token.py
--rw-r--r--   0        0        0        0 2023-06-13 22:28:46.222925 bruinen-1.2/src/bruinen/client/api/confirm/__init__.py
--rw-r--r--   0        0        0     4144 2023-06-13 22:28:47.898774 bruinen-1.2/src/bruinen/client/api/confirm/create.py
--rw-r--r--   0        0        0     3703 2023-06-13 22:28:47.878975 bruinen-1.2/src/bruinen/client/api/confirm/find_one.py
--rw-r--r--   0        0        0        0 2023-06-13 22:28:46.208644 bruinen-1.2/src/bruinen/client/api/connection_requests/__init__.py
--rw-r--r--   0        0        0     4173 2023-06-13 22:28:47.867049 bruinen-1.2/src/bruinen/client/api/connection_requests/connection_requests_controller_find_all.py
--rw-r--r--   0        0        0     4319 2023-06-13 22:28:47.897008 bruinen-1.2/src/bruinen/client/api/connection_requests/create.py
--rw-r--r--   0        0        0     3668 2023-06-13 22:28:47.925526 bruinen-1.2/src/bruinen/client/api/connection_requests/get.py
--rw-r--r--   0        0        0        0 2023-06-13 22:28:46.221426 bruinen-1.2/src/bruinen/client/api/source_policy/__init__.py
--rw-r--r--   0        0        0     3791 2023-06-13 22:28:47.899363 bruinen-1.2/src/bruinen/client/api/source_policy/source_policy_controller_get_all_active_for_client.py
--rw-r--r--   0        0        0     3800 2023-06-13 22:28:47.906100 bruinen-1.2/src/bruinen/client/api/source_policy/source_policy_controller_get_defaults_for_client.py
--rw-r--r--   0        0        0     3780 2023-06-13 22:28:47.911587 bruinen-1.2/src/bruinen/client/api/source_policy/source_policy_controller_get_policy_by_id.py
--rw-r--r--   0        0        0     3785 2023-06-13 22:28:47.926710 bruinen-1.2/src/bruinen/client/api/source_policy/source_policy_controller_set_default.py
--rw-r--r--   0        0        0        0 2023-06-13 22:28:46.209695 bruinen-1.2/src/bruinen/client/api/sources/__init__.py
--rw-r--r--   0        0        0     3963 2023-06-13 22:28:47.931798 bruinen-1.2/src/bruinen/client/api/sources/github_controller_profile.py
--rw-r--r--   0        0        0     4195 2023-06-13 22:28:47.937119 bruinen-1.2/src/bruinen/client/api/sources/github_controller_repos.py
--rw-r--r--   0        0        0     4371 2023-06-13 22:28:47.948811 bruinen-1.2/src/bruinen/client/api/sources/google_controller_calendar.py
--rw-r--r--   0        0        0     6460 2023-06-13 22:28:47.973077 bruinen-1.2/src/bruinen/client/api/sources/google_controller_calendars.py
--rw-r--r--   0        0        0     4272 2023-06-13 22:28:47.939939 bruinen-1.2/src/bruinen/client/api/sources/google_controller_draft.py
--rw-r--r--   0        0        0     4983 2023-06-13 22:28:47.973527 bruinen-1.2/src/bruinen/client/api/sources/google_controller_drafts.py
--rw-r--r--   0        0        0     5256 2023-06-13 22:28:47.970177 bruinen-1.2/src/bruinen/client/api/sources/google_controller_event.py
--rw-r--r--   0        0        0    11601 2023-06-13 22:28:48.073451 bruinen-1.2/src/bruinen/client/api/sources/google_controller_events.py
--rw-r--r--   0        0        0     4272 2023-06-13 22:28:47.974168 bruinen-1.2/src/bruinen/client/api/sources/google_controller_label.py
--rw-r--r--   0        0        0     3949 2023-06-13 22:28:47.966849 bruinen-1.2/src/bruinen/client/api/sources/google_controller_labels.py
--rw-r--r--   0        0        0     4338 2023-06-13 22:28:48.003630 bruinen-1.2/src/bruinen/client/api/sources/google_controller_message.py
--rw-r--r--   0        0        0     5587 2023-06-13 22:28:48.002210 bruinen-1.2/src/bruinen/client/api/sources/google_controller_messages.py
--rw-r--r--   0        0        0     4357 2023-06-13 22:28:48.028386 bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_draft.py
--rw-r--r--   0        0        0     5068 2023-06-13 22:28:48.033699 bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_drafts.py
--rw-r--r--   0        0        0     4423 2023-06-13 22:28:48.043408 bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_message.py
--rw-r--r--   0        0        0     5672 2023-06-13 22:28:48.058378 bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_messages.py
--rw-r--r--   0        0        0     4390 2023-06-13 22:28:48.025787 bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_thread.py
--rw-r--r--   0        0        0     5658 2023-06-13 22:28:48.054173 bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_threads.py
--rw-r--r--   0        0        0     3963 2023-06-13 22:28:48.039363 bruinen-1.2/src/bruinen/client/api/sources/google_controller_profile.py
--rw-r--r--   0        0        0     4305 2023-06-13 22:28:48.072819 bruinen-1.2/src/bruinen/client/api/sources/google_controller_thread.py
--rw-r--r--   0        0        0     5573 2023-06-13 22:28:48.092643 bruinen-1.2/src/bruinen/client/api/sources/google_controller_threads.py
--rw-r--r--   0        0        0     2349 2023-06-13 22:28:48.054421 bruinen-1.2/src/bruinen/client/api/sources/sources_controller_get_metadata.py
--rw-r--r--   0        0        0     4208 2023-06-13 22:28:48.077476 bruinen-1.2/src/bruinen/client/api/sources/sources_controller_get_metadata_for_source.py
--rw-r--r--   0        0        0        0 2023-06-13 22:28:46.220354 bruinen-1.2/src/bruinen/client/api/usage/__init__.py
--rw-r--r--   0        0        0     3984 2023-06-13 22:28:48.079637 bruinen-1.2/src/bruinen/client/api/usage/usage_controller_find_all.py
--rw-r--r--   0        0        0     2482 2023-06-13 22:28:48.083475 bruinen-1.2/src/bruinen/client/api/usage/usage_controller_find_one.py
--rw-r--r--   0        0        0     3417 2023-06-13 22:28:48.087518 bruinen-1.2/src/bruinen/client/api/usage/usage_controller_get_client_data.py
--rw-r--r--   0        0        0        0 2023-06-13 22:28:46.193044 bruinen-1.2/src/bruinen/client/api/users/__init__.py
--rw-r--r--   0        0        0     3991 2023-06-13 22:28:48.116874 bruinen-1.2/src/bruinen/client/api/users/users_controller_create.py
--rw-r--r--   0        0        0     3682 2023-06-13 22:28:48.123024 bruinen-1.2/src/bruinen/client/api/users/users_controller_find_all.py
--rw-r--r--   0        0        0     3667 2023-06-13 22:28:48.120957 bruinen-1.2/src/bruinen/client/api/users/users_controller_find_one.py
--rw-r--r--   0        0        0     3405 2023-06-13 22:28:48.160307 bruinen-1.2/src/bruinen/client/api/users/users_controller_find_user_from_token.py
--rw-r--r--   0        0        0     4200 2023-06-13 22:28:48.117105 bruinen-1.2/src/bruinen/client/api/users/users_controller_update.py
--rw-r--r--   0        0        0     3998 2023-06-13 22:28:48.126934 bruinen-1.2/src/bruinen/client/api/users/users_controller_upsert_user.py
--rw-r--r--   0        0        0     2817 2023-06-13 22:28:48.137189 bruinen-1.2/src/bruinen/client/client.py
--rw-r--r--   0        0        0      470 2023-06-13 22:28:48.095218 bruinen-1.2/src/bruinen/client/errors.py
--rw-r--r--   0        0        0    21276 2023-06-13 22:28:46.920808 bruinen-1.2/src/bruinen/client/models/__init__.py
--rw-r--r--   0        0        0      214 2023-06-13 22:28:46.978382 bruinen-1.2/src/bruinen/client/models/account_status.py
--rw-r--r--   0        0        0     1296 2023-06-13 22:28:48.129258 bruinen-1.2/src/bruinen/client/models/accounts_controller_deactivate_response_200.py
--rw-r--r--   0        0        0     1327 2023-06-13 22:28:48.130185 bruinen-1.2/src/bruinen/client/models/accounts_controller_get_accounts_response_200_item.py
--rw-r--r--   0        0        0     1394 2023-06-13 22:28:48.162900 bruinen-1.2/src/bruinen/client/models/auth.py
--rw-r--r--   0        0        0     2933 2023-06-13 22:28:48.199959 bruinen-1.2/src/bruinen/client/models/client_usage_data.py
--rw-r--r--   0        0        0      245 2023-06-13 22:28:47.023528 bruinen-1.2/src/bruinen/client/models/confirmation_status.py
--rw-r--r--   0        0        0     1360 2023-06-13 22:28:48.166999 bruinen-1.2/src/bruinen/client/models/connection_requests_controller_find_all_response_200_item.py
--rw-r--r--   0        0        0     3000 2023-06-13 22:28:48.201101 bruinen-1.2/src/bruinen/client/models/create_confirm_dto.py
--rw-r--r--   0        0        0     1208 2023-06-13 22:28:48.139358 bruinen-1.2/src/bruinen/client/models/create_confirm_dto_params.py
--rw-r--r--   0        0        0     2064 2023-06-13 22:28:48.195288 bruinen-1.2/src/bruinen/client/models/create_confirm_returned_dto.py
--rw-r--r--   0        0        0     2988 2023-06-13 22:28:48.188593 bruinen-1.2/src/bruinen/client/models/create_connection_request_dto.py
--rw-r--r--   0        0        0     1261 2023-06-13 22:28:48.202398 bruinen-1.2/src/bruinen/client/models/create_connection_request_dto_source.py
--rw-r--r--   0        0        0     2362 2023-06-13 22:28:48.203635 bruinen-1.2/src/bruinen/client/models/create_user_dto.py
--rw-r--r--   0        0        0      193 2023-06-13 22:28:46.938516 bruinen-1.2/src/bruinen/client/models/credential_provider.py
--rw-r--r--   0        0        0     2141 2023-06-13 22:28:48.202918 bruinen-1.2/src/bruinen/client/models/endpoint_data.py
--rw-r--r--   0        0        0     1165 2023-06-13 22:28:48.186200 bruinen-1.2/src/bruinen/client/models/get_response_200.py
--rw-r--r--   0        0        0    13880 2023-06-13 22:28:48.355893 bruinen-1.2/src/bruinen/client/models/github_profile.py
--rw-r--r--   0        0        0    27798 2023-06-13 22:28:48.522192 bruinen-1.2/src/bruinen/client/models/github_repo.py
--rw-r--r--   0        0        0    13906 2023-06-13 22:28:48.321878 bruinen-1.2/src/bruinen/client/models/github_repo_owner.py
--rw-r--r--   0        0        0     2751 2023-06-13 22:28:48.240119 bruinen-1.2/src/bruinen/client/models/github_repo_permissions.py
--rw-r--r--   0        0        0     4464 2023-06-13 22:28:48.252859 bruinen-1.2/src/bruinen/client/models/google_calendar.py
--rw-r--r--   0        0        0     2188 2023-06-13 22:28:48.214310 bruinen-1.2/src/bruinen/client/models/google_calendar_conference_properties.py
--rw-r--r--   0        0        0     3595 2023-06-13 22:28:48.233407 bruinen-1.2/src/bruinen/client/models/google_calendars.py
--rw-r--r--   0        0        0    10266 2023-06-13 22:28:48.289579 bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item.py
--rw-r--r--   0        0        0     2264 2023-06-13 22:28:48.241949 bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item_conference_properties.py
--rw-r--r--   0        0        0     2024 2023-06-13 22:28:48.254718 bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item_default_reminders.py
--rw-r--r--   0        0        0     3002 2023-06-13 22:28:48.253806 bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item_notification_settings.py
--rw-r--r--   0        0        0     2052 2023-06-13 22:28:48.262514 bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item_notification_settings_notifications_item.py
--rw-r--r--   0        0        0     2268 2023-06-13 22:28:48.293494 bruinen-1.2/src/bruinen/client/models/google_draft.py
--rw-r--r--   0        0        0     4723 2023-06-13 22:28:48.316434 bruinen-1.2/src/bruinen/client/models/google_draft_message.py
--rw-r--r--   0        0        0     5102 2023-06-13 22:28:48.344255 bruinen-1.2/src/bruinen/client/models/google_draft_message_payload.py
--rw-r--r--   0        0        0     2138 2023-06-13 22:28:48.307538 bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_body.py
--rw-r--r--   0        0        0     1830 2023-06-13 22:28:48.333903 bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_headers_item.py
--rw-r--r--   0        0        0     5385 2023-06-13 22:28:48.364957 bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item.py
--rw-r--r--   0        0        0     2186 2023-06-13 22:28:48.328003 bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_body.py
--rw-r--r--   0        0        0     1881 2023-06-13 22:28:48.332722 bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_headers_item.py
--rw-r--r--   0        0        0     4547 2023-06-13 22:28:48.399354 bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item.py
--rw-r--r--   0        0        0     1908 2023-06-13 22:28:48.356175 bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_body.py
--rw-r--r--   0        0        0     1932 2023-06-13 22:28:48.355745 bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_headers_item.py
--rw-r--r--   0        0        0     3038 2023-06-13 22:28:48.366503 bruinen-1.2/src/bruinen/client/models/google_drafts.py
--rw-r--r--   0        0        0     2403 2023-06-13 22:28:48.379662 bruinen-1.2/src/bruinen/client/models/google_drafts_drafts_item.py
--rw-r--r--   0        0        0     1887 2023-06-13 22:28:48.375471 bruinen-1.2/src/bruinen/client/models/google_drafts_drafts_item_message.py
--rw-r--r--   0        0        0    21058 2023-06-13 22:28:48.822943 bruinen-1.2/src/bruinen/client/models/google_event.py
--rw-r--r--   0        0        0     2812 2023-06-13 22:28:48.382352 bruinen-1.2/src/bruinen/client/models/google_event_attachments_item.py
--rw-r--r--   0        0        0     4469 2023-06-13 22:28:48.416200 bruinen-1.2/src/bruinen/client/models/google_event_attendees_item.py
--rw-r--r--   0        0        0     5871 2023-06-13 22:28:48.419427 bruinen-1.2/src/bruinen/client/models/google_event_conference_data.py
--rw-r--r--   0        0        0     3028 2023-06-13 22:28:48.442576 bruinen-1.2/src/bruinen/client/models/google_event_conference_data_conference_solution.py
--rw-r--r--   0        0        0     1694 2023-06-13 22:28:48.407300 bruinen-1.2/src/bruinen/client/models/google_event_conference_data_conference_solution_key.py
--rw-r--r--   0        0        0     4265 2023-06-13 22:28:48.458206 bruinen-1.2/src/bruinen/client/models/google_event_conference_data_create_request.py
--rw-r--r--   0        0        0     1796 2023-06-13 22:28:48.423505 bruinen-1.2/src/bruinen/client/models/google_event_conference_data_create_request_conference_solution_key.py
--rw-r--r--   0        0        0     1766 2023-06-13 22:28:48.449369 bruinen-1.2/src/bruinen/client/models/google_event_conference_data_create_request_status.py
--rw-r--r--   0        0        0     3860 2023-06-13 22:28:48.472435 bruinen-1.2/src/bruinen/client/models/google_event_conference_data_entry_points_item.py
--rw-r--r--   0        0        0     2401 2023-06-13 22:28:48.478901 bruinen-1.2/src/bruinen/client/models/google_event_creator.py
--rw-r--r--   0        0        0     2127 2023-06-13 22:28:48.443305 bruinen-1.2/src/bruinen/client/models/google_event_end.py
--rw-r--r--   0        0        0     3226 2023-06-13 22:28:48.470286 bruinen-1.2/src/bruinen/client/models/google_event_extended_properties.py
--rw-r--r--   0        0        0     1323 2023-06-13 22:28:48.451349 bruinen-1.2/src/bruinen/client/models/google_event_extended_properties_private.py
--rw-r--r--   0        0        0     1317 2023-06-13 22:28:48.467768 bruinen-1.2/src/bruinen/client/models/google_event_extended_properties_shared.py
--rw-r--r--   0        0        0     4170 2023-06-13 22:28:48.518263 bruinen-1.2/src/bruinen/client/models/google_event_gadget.py
--rw-r--r--   0        0        0     1266 2023-06-13 22:28:48.472873 bruinen-1.2/src/bruinen/client/models/google_event_gadget_preferences.py
--rw-r--r--   0        0        0     2421 2023-06-13 22:28:48.505430 bruinen-1.2/src/bruinen/client/models/google_event_organizer.py
--rw-r--r--   0        0        0     2259 2023-06-13 22:28:48.486956 bruinen-1.2/src/bruinen/client/models/google_event_original_start_time.py
--rw-r--r--   0        0        0     2753 2023-06-13 22:28:48.496659 bruinen-1.2/src/bruinen/client/models/google_event_reminders.py
--rw-r--r--   0        0        0     1953 2023-06-13 22:28:48.495857 bruinen-1.2/src/bruinen/client/models/google_event_reminders_overrides_item.py
--rw-r--r--   0        0        0     1785 2023-06-13 22:28:48.514728 bruinen-1.2/src/bruinen/client/models/google_event_source.py
--rw-r--r--   0        0        0     2145 2023-06-13 22:28:48.515998 bruinen-1.2/src/bruinen/client/models/google_event_start.py
--rw-r--r--   0        0        0     6772 2023-06-13 22:28:48.560942 bruinen-1.2/src/bruinen/client/models/google_events.py
--rw-r--r--   0        0        0     1924 2023-06-13 22:28:48.536583 bruinen-1.2/src/bruinen/client/models/google_events_default_reminders_item.py
--rw-r--r--   0        0        0    22193 2023-06-13 22:28:48.970290 bruinen-1.2/src/bruinen/client/models/google_events_events_item.py
--rw-r--r--   0        0        0     2873 2023-06-13 22:28:48.547171 bruinen-1.2/src/bruinen/client/models/google_events_events_item_attachments_item.py
--rw-r--r--   0        0        0     4530 2023-06-13 22:28:48.549707 bruinen-1.2/src/bruinen/client/models/google_events_events_item_attendees_item.py
--rw-r--r--   0        0        0     6310 2023-06-13 22:28:48.567446 bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data.py
--rw-r--r--   0        0        0     3181 2023-06-13 22:28:48.557977 bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution.py
--rw-r--r--   0        0        0     1755 2023-06-13 22:28:48.553386 bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution_key.py
--rw-r--r--   0        0        0     4541 2023-06-13 22:28:48.585032 bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_create_request.py
--rw-r--r--   0        0        0     1857 2023-06-13 22:28:48.567446 bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_create_request_conference_solution_key.py
--rw-r--r--   0        0        0     1827 2023-06-13 22:28:48.577243 bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_create_request_status.py
--rw-r--r--   0        0        0     3921 2023-06-13 22:28:48.842425 bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_entry_points_item.py
--rw-r--r--   0        0        0     2462 2023-06-13 22:28:48.593027 bruinen-1.2/src/bruinen/client/models/google_events_events_item_creator.py
--rw-r--r--   0        0        0     2188 2023-06-13 22:28:48.781923 bruinen-1.2/src/bruinen/client/models/google_events_events_item_end.py
--rw-r--r--   0        0        0     3579 2023-06-13 22:28:48.612565 bruinen-1.2/src/bruinen/client/models/google_events_events_item_extended_properties.py
--rw-r--r--   0        0        0     1384 2023-06-13 22:28:48.603607 bruinen-1.2/src/bruinen/client/models/google_events_events_item_extended_properties_private.py
--rw-r--r--   0        0        0     1378 2023-06-13 22:28:48.608925 bruinen-1.2/src/bruinen/client/models/google_events_events_item_extended_properties_shared.py
--rw-r--r--   0        0        0     4323 2023-06-13 22:28:48.878512 bruinen-1.2/src/bruinen/client/models/google_events_events_item_gadget.py
--rw-r--r--   0        0        0     1327 2023-06-13 22:28:48.613818 bruinen-1.2/src/bruinen/client/models/google_events_events_item_gadget_preferences.py
--rw-r--r--   0        0        0     2482 2023-06-13 22:28:48.910917 bruinen-1.2/src/bruinen/client/models/google_events_events_item_organizer.py
--rw-r--r--   0        0        0     2320 2023-06-13 22:28:48.850848 bruinen-1.2/src/bruinen/client/models/google_events_events_item_original_start_time.py
--rw-r--r--   0        0        0     2920 2023-06-13 22:28:48.709569 bruinen-1.2/src/bruinen/client/models/google_events_events_item_reminders.py
--rw-r--r--   0        0        0     2014 2023-06-13 22:28:48.898873 bruinen-1.2/src/bruinen/client/models/google_events_events_item_reminders_overrides_item.py
--rw-r--r--   0        0        0     1846 2023-06-13 22:28:48.810519 bruinen-1.2/src/bruinen/client/models/google_events_events_item_source.py
--rw-r--r--   0        0        0     2206 2023-06-13 22:28:48.892481 bruinen-1.2/src/bruinen/client/models/google_events_events_item_start.py
--rw-r--r--   0        0        0     5170 2023-06-13 22:28:48.921772 bruinen-1.2/src/bruinen/client/models/google_label.py
--rw-r--r--   0        0        0     1927 2023-06-13 22:28:48.892705 bruinen-1.2/src/bruinen/client/models/google_label_color.py
--rw-r--r--   0        0        0     2652 2023-06-13 22:28:48.910461 bruinen-1.2/src/bruinen/client/models/google_labels.py
--rw-r--r--   0        0        0     2945 2023-06-13 22:28:48.920220 bruinen-1.2/src/bruinen/client/models/google_labels_labels_item.py
--rw-r--r--   0        0        0     4411 2023-06-13 22:28:48.965530 bruinen-1.2/src/bruinen/client/models/google_message.py
--rw-r--r--   0        0        0     4958 2023-06-13 22:28:48.963041 bruinen-1.2/src/bruinen/client/models/google_message_payload.py
--rw-r--r--   0        0        0     2110 2023-06-13 22:28:48.919449 bruinen-1.2/src/bruinen/client/models/google_message_payload_body.py
--rw-r--r--   0        0        0     1802 2023-06-13 22:28:48.924412 bruinen-1.2/src/bruinen/client/models/google_message_payload_headers_item.py
--rw-r--r--   0        0        0     4162 2023-06-13 22:28:48.961524 bruinen-1.2/src/bruinen/client/models/google_message_payload_parts_item.py
--rw-r--r--   0        0        0     2158 2023-06-13 22:28:48.970964 bruinen-1.2/src/bruinen/client/models/google_message_payload_parts_item_body.py
--rw-r--r--   0        0        0     1853 2023-06-13 22:28:48.974875 bruinen-1.2/src/bruinen/client/models/google_message_payload_parts_item_headers_item.py
--rw-r--r--   0        0        0     3115 2023-06-13 22:28:48.982418 bruinen-1.2/src/bruinen/client/models/google_messages.py
--rw-r--r--   0        0        0     1844 2023-06-13 22:28:48.955408 bruinen-1.2/src/bruinen/client/models/google_messages_messages_item.py
--rw-r--r--   0        0        0     4814 2023-06-13 22:28:49.017346 bruinen-1.2/src/bruinen/client/models/google_parsed_draft.py
--rw-r--r--   0        0        0     3902 2023-06-13 22:28:49.010189 bruinen-1.2/src/bruinen/client/models/google_parsed_draft_attachments_item.py
--rw-r--r--   0        0        0     5378 2023-06-13 22:28:49.038770 bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers.py
--rw-r--r--   0        0        0     1865 2023-06-13 22:28:48.987267 bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers_bcc_item.py
--rw-r--r--   0        0        0     1857 2023-06-13 22:28:49.007066 bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers_cc_item.py
--rw-r--r--   0        0        0     1858 2023-06-13 22:28:49.001270 bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers_from.py
--rw-r--r--   0        0        0     1879 2023-06-13 22:28:49.006929 bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers_to_item.py
--rw-r--r--   0        0        0     3122 2023-06-13 22:28:49.005109 bruinen-1.2/src/bruinen/client/models/google_parsed_drafts.py
--rw-r--r--   0        0        0     5048 2023-06-13 22:28:49.034087 bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item.py
--rw-r--r--   0        0        0     3963 2023-06-13 22:28:49.033575 bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_attachments_item.py
--rw-r--r--   0        0        0     5799 2023-06-13 22:28:49.056612 bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers.py
--rw-r--r--   0        0        0     1926 2023-06-13 22:28:49.028775 bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_bcc_item.py
--rw-r--r--   0        0        0     1918 2023-06-13 22:28:49.025653 bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_cc_item.py
--rw-r--r--   0        0        0     1919 2023-06-13 22:28:49.034726 bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_from.py
--rw-r--r--   0        0        0     1940 2023-06-13 22:28:49.032461 bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_to_item.py
--rw-r--r--   0        0        0     4552 2023-06-13 22:28:49.076366 bruinen-1.2/src/bruinen/client/models/google_parsed_message.py
--rw-r--r--   0        0        0     3914 2023-06-13 22:28:49.059009 bruinen-1.2/src/bruinen/client/models/google_parsed_message_attachments_item.py
--rw-r--r--   0        0        0     5460 2023-06-13 22:28:49.136027 bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers.py
--rw-r--r--   0        0        0     1877 2023-06-13 22:28:49.062327 bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers_bcc_item.py
--rw-r--r--   0        0        0     1869 2023-06-13 22:28:49.065775 bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers_cc_item.py
--rw-r--r--   0        0        0     1870 2023-06-13 22:28:49.047374 bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers_from.py
--rw-r--r--   0        0        0     1891 2023-06-13 22:28:49.050838 bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers_to_item.py
--rw-r--r--   0        0        0     3199 2023-06-13 22:28:49.098420 bruinen-1.2/src/bruinen/client/models/google_parsed_messages.py
--rw-r--r--   0        0        0     4853 2023-06-13 22:28:49.103026 bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item.py
--rw-r--r--   0        0        0     3985 2023-06-13 22:28:49.093418 bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_attachments_item.py
--rw-r--r--   0        0        0     6075 2023-06-13 22:28:49.139324 bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers.py
--rw-r--r--   0        0        0     1948 2023-06-13 22:28:49.090459 bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers_bcc_item.py
--rw-r--r--   0        0        0     1940 2023-06-13 22:28:49.082047 bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers_cc_item.py
--rw-r--r--   0        0        0     1941 2023-06-13 22:28:49.137885 bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers_from.py
--rw-r--r--   0        0        0     1962 2023-06-13 22:28:49.108806 bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers_to_item.py
--rw-r--r--   0        0        0     2583 2023-06-13 22:28:49.106121 bruinen-1.2/src/bruinen/client/models/google_parsed_thread.py
--rw-r--r--   0        0        0     4837 2023-06-13 22:28:49.227113 bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item.py
--rw-r--r--   0        0        0     3975 2023-06-13 22:28:49.166314 bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_attachments_item.py
--rw-r--r--   0        0        0     5948 2023-06-13 22:28:49.252508 bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers.py
--rw-r--r--   0        0        0     1938 2023-06-13 22:28:49.202256 bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers_bcc_item.py
--rw-r--r--   0        0        0     1930 2023-06-13 22:28:49.165798 bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers_cc_item.py
--rw-r--r--   0        0        0     1931 2023-06-13 22:28:49.161402 bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers_from.py
--rw-r--r--   0        0        0     1952 2023-06-13 22:28:49.162152 bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers_to_item.py
--rw-r--r--   0        0        0     3152 2023-06-13 22:28:49.231235 bruinen-1.2/src/bruinen/client/models/google_parsed_threads.py
--rw-r--r--   0        0        0     2730 2023-06-13 22:28:49.200024 bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item.py
--rw-r--r--   0        0        0     5163 2023-06-13 22:28:49.282405 bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item.py
--rw-r--r--   0        0        0     4041 2023-06-13 22:28:49.229218 bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_attachments_item.py
--rw-r--r--   0        0        0     6454 2023-06-13 22:28:49.256548 bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers.py
--rw-r--r--   0        0        0     2004 2023-06-13 22:28:49.237683 bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_bcc_item.py
--rw-r--r--   0        0        0     1996 2023-06-13 22:28:49.226823 bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_cc_item.py
--rw-r--r--   0        0        0     1997 2023-06-13 22:28:49.281426 bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_from.py
--rw-r--r--   0        0        0     2018 2023-06-13 22:28:49.278196 bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_to_item.py
--rw-r--r--   0        0        0     2662 2023-06-13 22:28:49.285920 bruinen-1.2/src/bruinen/client/models/google_profile.py
--rw-r--r--   0        0        0     3121 2023-06-13 22:28:49.321794 bruinen-1.2/src/bruinen/client/models/google_thread.py
--rw-r--r--   0        0        0     4544 2023-06-13 22:28:49.329615 bruinen-1.2/src/bruinen/client/models/google_thread_messages_item.py
--rw-r--r--   0        0        0     5273 2023-06-13 22:28:49.371268 bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload.py
--rw-r--r--   0        0        0     2171 2023-06-13 22:28:49.282377 bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_body.py
--rw-r--r--   0        0        0     1863 2023-06-13 22:28:49.309501 bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_headers_item.py
--rw-r--r--   0        0        0     4480 2023-06-13 22:28:49.374148 bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_parts_item.py
--rw-r--r--   0        0        0     2219 2023-06-13 22:28:49.347284 bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_body.py
--rw-r--r--   0        0        0     1914 2023-06-13 22:28:49.320552 bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_headers_item.py
--rw-r--r--   0        0        0     3068 2023-06-13 22:28:49.340367 bruinen-1.2/src/bruinen/client/models/google_threads.py
--rw-r--r--   0        0        0     2135 2023-06-13 22:28:49.326683 bruinen-1.2/src/bruinen/client/models/google_threads_threads_item.py
--rw-r--r--   0        0        0     3499 2023-06-13 22:28:49.363181 bruinen-1.2/src/bruinen/client/models/returned_account_dto.py
--rw-r--r--   0        0        0     4714 2023-06-13 22:28:49.380607 bruinen-1.2/src/bruinen/client/models/returned_confirm_dto.py
--rw-r--r--   0        0        0     1218 2023-06-13 22:28:49.380108 bruinen-1.2/src/bruinen/client/models/returned_confirm_dto_params.py
--rw-r--r--   0        0        0     3613 2023-06-13 22:28:49.361914 bruinen-1.2/src/bruinen/client/models/returned_connection_request_dto.py
--rw-r--r--   0        0        0     1271 2023-06-13 22:28:49.378219 bruinen-1.2/src/bruinen/client/models/returned_connection_request_dto_source.py
--rw-r--r--   0        0        0     4313 2023-06-13 22:28:49.416927 bruinen-1.2/src/bruinen/client/models/returned_source_policy_dto.py
--rw-r--r--   0        0        0     2719 2023-06-13 22:28:49.429967 bruinen-1.2/src/bruinen/client/models/returned_user_dto.py
--rw-r--r--   0        0        0     2901 2023-06-13 22:28:49.405957 bruinen-1.2/src/bruinen/client/models/source_data.py
--rw-r--r--   0        0        0      177 2023-06-13 22:28:46.969084 bruinen-1.2/src/bruinen/client/models/source_policy_status.py
--rw-r--r--   0        0        0      549 2023-06-13 22:28:46.910848 bruinen-1.2/src/bruinen/client/models/source_type.py
--rw-r--r--   0        0        0     1350 2023-06-13 22:28:49.409644 bruinen-1.2/src/bruinen/client/models/sources_controller_get_metadata_for_source_response_200.py
--rw-r--r--   0        0        0     2362 2023-06-13 22:28:49.422625 bruinen-1.2/src/bruinen/client/models/update_user_dto.py
--rw-r--r--   0        0        0     2362 2023-06-13 22:28:49.428908 bruinen-1.2/src/bruinen/client/models/upsert_user_dto.py
--rw-r--r--   0        0        0     1292 2023-06-13 22:28:49.421934 bruinen-1.2/src/bruinen/client/models/usage_controller_find_all_response_200_item.py
--rw-r--r--   0        0        0       25 2023-06-13 22:28:46.071821 bruinen-1.2/src/bruinen/client/py.typed
--rw-r--r--   0        0        0      993 2023-06-13 22:28:49.391265 bruinen-1.2/src/bruinen/client/types.py
--rw-r--r--   0        0        0       36 2023-06-09 17:40:25.908847 bruinen-1.2/src/bruinen/confirm/__init__.py
--rw-r--r--   0        0        0     2032 2023-05-30 21:25:54.185883 bruinen-1.2/src/bruinen/confirm/confirm.py
--rw-r--r--   0        0        0        0 2023-05-30 21:25:54.185920 bruinen-1.2/src/bruinen/langchain/__init__.py
--rw-r--r--   0        0        0     6508 2023-06-14 22:02:55.783039 bruinen-1.2/src/bruinen/langchain/github.py
--rw-r--r--   0        0        0    73029 2023-06-14 22:02:55.783839 bruinen-1.2/src/bruinen/langchain/google.py
--rw-r--r--   0        0        0       34 2023-06-06 18:24:40.536279 bruinen-1.2/src/bruinen/langchain/parsers/__init__.py
--rw-r--r--   0        0        0     4398 2023-06-09 17:40:25.910512 bruinen-1.2/src/bruinen/langchain/parsers/sql_parser.py
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 bruinen-1.2/PKG-INFO
+-rw-r--r--   0        0        0      733 2023-06-09 17:43:51.803315 bruinen-1.2.1/README.md
+-rw-r--r--   0        0        0      561 2023-06-15 02:43:43.397905 bruinen-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 21:25:54.158184 bruinen-1.2.1/src/bruinen/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-13 22:28:47.788326 bruinen-1.2.1/src/bruinen/client/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-13 22:28:46.187061 bruinen-1.2.1/src/bruinen/client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:28:46.206027 bruinen-1.2.1/src/bruinen/client/api/accounts/__init__.py
+-rw-r--r--   0        0        0     2659 2023-06-13 22:28:47.820237 bruinen-1.2.1/src/bruinen/client/api/accounts/account_counts_for_policy.py
+-rw-r--r--   0        0        0     3992 2023-06-13 22:28:47.841641 bruinen-1.2.1/src/bruinen/client/api/accounts/accounts_controller_deactivate.py
+-rw-r--r--   0        0        0     4074 2023-06-13 22:28:47.848025 bruinen-1.2.1/src/bruinen/client/api/accounts/accounts_controller_get_accounts.py
+-rw-r--r--   0        0        0     4080 2023-06-13 22:28:47.847277 bruinen-1.2.1/src/bruinen/client/api/accounts/find_all_accounts_for_user.py
+-rw-r--r--   0        0        0     4087 2023-06-13 22:28:47.861973 bruinen-1.2.1/src/bruinen/client/api/accounts/find_all_active_for_user.py
+-rw-r--r--   0        0        0     4094 2023-06-13 22:28:47.866459 bruinen-1.2.1/src/bruinen/client/api/accounts/find_all_active_with_policy_for_user.py
+-rw-r--r--   0        0        0     3704 2023-06-13 22:28:47.858873 bruinen-1.2.1/src/bruinen/client/api/accounts/get_account.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:28:46.208236 bruinen-1.2.1/src/bruinen/client/api/auth/__init__.py
+-rw-r--r--   0        0        0     3614 2023-06-13 22:28:47.866146 bruinen-1.2.1/src/bruinen/client/api/auth/get_user_auth_token.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:28:46.222925 bruinen-1.2.1/src/bruinen/client/api/confirm/__init__.py
+-rw-r--r--   0        0        0     4144 2023-06-13 22:28:47.898774 bruinen-1.2.1/src/bruinen/client/api/confirm/create.py
+-rw-r--r--   0        0        0     3703 2023-06-13 22:28:47.878975 bruinen-1.2.1/src/bruinen/client/api/confirm/find_one.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:28:46.208644 bruinen-1.2.1/src/bruinen/client/api/connection_requests/__init__.py
+-rw-r--r--   0        0        0     4173 2023-06-13 22:28:47.867049 bruinen-1.2.1/src/bruinen/client/api/connection_requests/connection_requests_controller_find_all.py
+-rw-r--r--   0        0        0     4319 2023-06-13 22:28:47.897008 bruinen-1.2.1/src/bruinen/client/api/connection_requests/create.py
+-rw-r--r--   0        0        0     3668 2023-06-13 22:28:47.925526 bruinen-1.2.1/src/bruinen/client/api/connection_requests/get.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:28:46.221426 bruinen-1.2.1/src/bruinen/client/api/source_policy/__init__.py
+-rw-r--r--   0        0        0     3791 2023-06-13 22:28:47.899363 bruinen-1.2.1/src/bruinen/client/api/source_policy/source_policy_controller_get_all_active_for_client.py
+-rw-r--r--   0        0        0     3800 2023-06-13 22:28:47.906100 bruinen-1.2.1/src/bruinen/client/api/source_policy/source_policy_controller_get_defaults_for_client.py
+-rw-r--r--   0        0        0     3780 2023-06-13 22:28:47.911587 bruinen-1.2.1/src/bruinen/client/api/source_policy/source_policy_controller_get_policy_by_id.py
+-rw-r--r--   0        0        0     3785 2023-06-13 22:28:47.926710 bruinen-1.2.1/src/bruinen/client/api/source_policy/source_policy_controller_set_default.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:28:46.209695 bruinen-1.2.1/src/bruinen/client/api/sources/__init__.py
+-rw-r--r--   0        0        0     3963 2023-06-13 22:28:47.931798 bruinen-1.2.1/src/bruinen/client/api/sources/github_controller_profile.py
+-rw-r--r--   0        0        0     4195 2023-06-13 22:28:47.937119 bruinen-1.2.1/src/bruinen/client/api/sources/github_controller_repos.py
+-rw-r--r--   0        0        0     4371 2023-06-13 22:28:47.948811 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_calendar.py
+-rw-r--r--   0        0        0     6460 2023-06-13 22:28:47.973077 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_calendars.py
+-rw-r--r--   0        0        0     4272 2023-06-13 22:28:47.939939 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_draft.py
+-rw-r--r--   0        0        0     4983 2023-06-13 22:28:47.973527 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_drafts.py
+-rw-r--r--   0        0        0     5256 2023-06-13 22:28:47.970177 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_event.py
+-rw-r--r--   0        0        0    11601 2023-06-13 22:28:48.073451 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_events.py
+-rw-r--r--   0        0        0     4272 2023-06-13 22:28:47.974168 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_label.py
+-rw-r--r--   0        0        0     3949 2023-06-13 22:28:47.966849 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_labels.py
+-rw-r--r--   0        0        0     4338 2023-06-13 22:28:48.003630 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_message.py
+-rw-r--r--   0        0        0     5587 2023-06-13 22:28:48.002210 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_messages.py
+-rw-r--r--   0        0        0     4357 2023-06-13 22:28:48.028386 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_draft.py
+-rw-r--r--   0        0        0     5068 2023-06-15 02:42:26.228146 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_drafts.py
+-rw-r--r--   0        0        0     4423 2023-06-13 22:28:48.043408 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_message.py
+-rw-r--r--   0        0        0     5672 2023-06-15 02:42:26.228509 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_messages.py
+-rw-r--r--   0        0        0     4390 2023-06-13 22:28:48.025787 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_thread.py
+-rw-r--r--   0        0        0     5658 2023-06-15 02:42:26.228838 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_threads.py
+-rw-r--r--   0        0        0     3963 2023-06-13 22:28:48.039363 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_profile.py
+-rw-r--r--   0        0        0     4305 2023-06-13 22:28:48.072819 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_thread.py
+-rw-r--r--   0        0        0     5573 2023-06-13 22:28:48.092643 bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_threads.py
+-rw-r--r--   0        0        0     2349 2023-06-13 22:28:48.054421 bruinen-1.2.1/src/bruinen/client/api/sources/sources_controller_get_metadata.py
+-rw-r--r--   0        0        0     4208 2023-06-13 22:28:48.077476 bruinen-1.2.1/src/bruinen/client/api/sources/sources_controller_get_metadata_for_source.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:28:46.220354 bruinen-1.2.1/src/bruinen/client/api/usage/__init__.py
+-rw-r--r--   0        0        0     3984 2023-06-13 22:28:48.079637 bruinen-1.2.1/src/bruinen/client/api/usage/usage_controller_find_all.py
+-rw-r--r--   0        0        0     2482 2023-06-13 22:28:48.083475 bruinen-1.2.1/src/bruinen/client/api/usage/usage_controller_find_one.py
+-rw-r--r--   0        0        0     3417 2023-06-13 22:28:48.087518 bruinen-1.2.1/src/bruinen/client/api/usage/usage_controller_get_client_data.py
+-rw-r--r--   0        0        0        0 2023-06-13 22:28:46.193044 bruinen-1.2.1/src/bruinen/client/api/users/__init__.py
+-rw-r--r--   0        0        0     3991 2023-06-13 22:28:48.116874 bruinen-1.2.1/src/bruinen/client/api/users/users_controller_create.py
+-rw-r--r--   0        0        0     3682 2023-06-13 22:28:48.123024 bruinen-1.2.1/src/bruinen/client/api/users/users_controller_find_all.py
+-rw-r--r--   0        0        0     3667 2023-06-13 22:28:48.120957 bruinen-1.2.1/src/bruinen/client/api/users/users_controller_find_one.py
+-rw-r--r--   0        0        0     3405 2023-06-13 22:28:48.160307 bruinen-1.2.1/src/bruinen/client/api/users/users_controller_find_user_from_token.py
+-rw-r--r--   0        0        0     4200 2023-06-13 22:28:48.117105 bruinen-1.2.1/src/bruinen/client/api/users/users_controller_update.py
+-rw-r--r--   0        0        0     3998 2023-06-13 22:28:48.126934 bruinen-1.2.1/src/bruinen/client/api/users/users_controller_upsert_user.py
+-rw-r--r--   0        0        0     2817 2023-06-13 22:28:48.137189 bruinen-1.2.1/src/bruinen/client/client.py
+-rw-r--r--   0        0        0      470 2023-06-13 22:28:48.095218 bruinen-1.2.1/src/bruinen/client/errors.py
+-rw-r--r--   0        0        0    21276 2023-06-15 02:42:26.229189 bruinen-1.2.1/src/bruinen/client/models/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-13 22:28:46.978382 bruinen-1.2.1/src/bruinen/client/models/account_status.py
+-rw-r--r--   0        0        0     1296 2023-06-13 22:28:48.129258 bruinen-1.2.1/src/bruinen/client/models/accounts_controller_deactivate_response_200.py
+-rw-r--r--   0        0        0     1327 2023-06-13 22:28:48.130185 bruinen-1.2.1/src/bruinen/client/models/accounts_controller_get_accounts_response_200_item.py
+-rw-r--r--   0        0        0     1394 2023-06-13 22:28:48.162900 bruinen-1.2.1/src/bruinen/client/models/auth.py
+-rw-r--r--   0        0        0     2933 2023-06-13 22:28:48.199959 bruinen-1.2.1/src/bruinen/client/models/client_usage_data.py
+-rw-r--r--   0        0        0      245 2023-06-13 22:28:47.023528 bruinen-1.2.1/src/bruinen/client/models/confirmation_status.py
+-rw-r--r--   0        0        0     1360 2023-06-13 22:28:48.166999 bruinen-1.2.1/src/bruinen/client/models/connection_requests_controller_find_all_response_200_item.py
+-rw-r--r--   0        0        0     3000 2023-06-13 22:28:48.201101 bruinen-1.2.1/src/bruinen/client/models/create_confirm_dto.py
+-rw-r--r--   0        0        0     1208 2023-06-13 22:28:48.139358 bruinen-1.2.1/src/bruinen/client/models/create_confirm_dto_params.py
+-rw-r--r--   0        0        0     2064 2023-06-13 22:28:48.195288 bruinen-1.2.1/src/bruinen/client/models/create_confirm_returned_dto.py
+-rw-r--r--   0        0        0     2988 2023-06-13 22:28:48.188593 bruinen-1.2.1/src/bruinen/client/models/create_connection_request_dto.py
+-rw-r--r--   0        0        0     1261 2023-06-13 22:28:48.202398 bruinen-1.2.1/src/bruinen/client/models/create_connection_request_dto_source.py
+-rw-r--r--   0        0        0     2362 2023-06-13 22:28:48.203635 bruinen-1.2.1/src/bruinen/client/models/create_user_dto.py
+-rw-r--r--   0        0        0      193 2023-06-13 22:28:46.938516 bruinen-1.2.1/src/bruinen/client/models/credential_provider.py
+-rw-r--r--   0        0        0     2141 2023-06-13 22:28:48.202918 bruinen-1.2.1/src/bruinen/client/models/endpoint_data.py
+-rw-r--r--   0        0        0     1165 2023-06-13 22:28:48.186200 bruinen-1.2.1/src/bruinen/client/models/get_response_200.py
+-rw-r--r--   0        0        0    13880 2023-06-13 22:28:48.355893 bruinen-1.2.1/src/bruinen/client/models/github_profile.py
+-rw-r--r--   0        0        0    27798 2023-06-13 22:28:48.522192 bruinen-1.2.1/src/bruinen/client/models/github_repo.py
+-rw-r--r--   0        0        0    13906 2023-06-13 22:28:48.321878 bruinen-1.2.1/src/bruinen/client/models/github_repo_owner.py
+-rw-r--r--   0        0        0     2751 2023-06-13 22:28:48.240119 bruinen-1.2.1/src/bruinen/client/models/github_repo_permissions.py
+-rw-r--r--   0        0        0     4464 2023-06-13 22:28:48.252859 bruinen-1.2.1/src/bruinen/client/models/google_calendar.py
+-rw-r--r--   0        0        0     2188 2023-06-13 22:28:48.214310 bruinen-1.2.1/src/bruinen/client/models/google_calendar_conference_properties.py
+-rw-r--r--   0        0        0     3595 2023-06-13 22:28:48.233407 bruinen-1.2.1/src/bruinen/client/models/google_calendars.py
+-rw-r--r--   0        0        0    10266 2023-06-13 22:28:48.289579 bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item.py
+-rw-r--r--   0        0        0     2264 2023-06-13 22:28:48.241949 bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item_conference_properties.py
+-rw-r--r--   0        0        0     2024 2023-06-13 22:28:48.254718 bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item_default_reminders.py
+-rw-r--r--   0        0        0     3002 2023-06-13 22:28:48.253806 bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item_notification_settings.py
+-rw-r--r--   0        0        0     2052 2023-06-13 22:28:48.262514 bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item_notification_settings_notifications_item.py
+-rw-r--r--   0        0        0     2268 2023-06-13 22:28:48.293494 bruinen-1.2.1/src/bruinen/client/models/google_draft.py
+-rw-r--r--   0        0        0     4723 2023-06-13 22:28:48.316434 bruinen-1.2.1/src/bruinen/client/models/google_draft_message.py
+-rw-r--r--   0        0        0     5102 2023-06-13 22:28:48.344255 bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload.py
+-rw-r--r--   0        0        0     2138 2023-06-13 22:28:48.307538 bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_body.py
+-rw-r--r--   0        0        0     1830 2023-06-13 22:28:48.333903 bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_headers_item.py
+-rw-r--r--   0        0        0     5385 2023-06-13 22:28:48.364957 bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item.py
+-rw-r--r--   0        0        0     2186 2023-06-13 22:28:48.328003 bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_body.py
+-rw-r--r--   0        0        0     1881 2023-06-13 22:28:48.332722 bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_headers_item.py
+-rw-r--r--   0        0        0     4547 2023-06-13 22:28:48.399354 bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item.py
+-rw-r--r--   0        0        0     1908 2023-06-13 22:28:48.356175 bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_body.py
+-rw-r--r--   0        0        0     1932 2023-06-13 22:28:48.355745 bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_headers_item.py
+-rw-r--r--   0        0        0     3038 2023-06-13 22:28:48.366503 bruinen-1.2.1/src/bruinen/client/models/google_drafts.py
+-rw-r--r--   0        0        0     2403 2023-06-13 22:28:48.379662 bruinen-1.2.1/src/bruinen/client/models/google_drafts_drafts_item.py
+-rw-r--r--   0        0        0     1887 2023-06-13 22:28:48.375471 bruinen-1.2.1/src/bruinen/client/models/google_drafts_drafts_item_message.py
+-rw-r--r--   0        0        0    21058 2023-06-13 22:28:48.822943 bruinen-1.2.1/src/bruinen/client/models/google_event.py
+-rw-r--r--   0        0        0     2812 2023-06-13 22:28:48.382352 bruinen-1.2.1/src/bruinen/client/models/google_event_attachments_item.py
+-rw-r--r--   0        0        0     4469 2023-06-13 22:28:48.416200 bruinen-1.2.1/src/bruinen/client/models/google_event_attendees_item.py
+-rw-r--r--   0        0        0     5871 2023-06-13 22:28:48.419427 bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data.py
+-rw-r--r--   0        0        0     3028 2023-06-13 22:28:48.442576 bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_conference_solution.py
+-rw-r--r--   0        0        0     1694 2023-06-13 22:28:48.407300 bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_conference_solution_key.py
+-rw-r--r--   0        0        0     4265 2023-06-13 22:28:48.458206 bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_create_request.py
+-rw-r--r--   0        0        0     1796 2023-06-13 22:28:48.423505 bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_create_request_conference_solution_key.py
+-rw-r--r--   0        0        0     1766 2023-06-13 22:28:48.449369 bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_create_request_status.py
+-rw-r--r--   0        0        0     3860 2023-06-13 22:28:48.472435 bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_entry_points_item.py
+-rw-r--r--   0        0        0     2401 2023-06-13 22:28:48.478901 bruinen-1.2.1/src/bruinen/client/models/google_event_creator.py
+-rw-r--r--   0        0        0     2127 2023-06-13 22:28:48.443305 bruinen-1.2.1/src/bruinen/client/models/google_event_end.py
+-rw-r--r--   0        0        0     3226 2023-06-13 22:28:48.470286 bruinen-1.2.1/src/bruinen/client/models/google_event_extended_properties.py
+-rw-r--r--   0        0        0     1323 2023-06-13 22:28:48.451349 bruinen-1.2.1/src/bruinen/client/models/google_event_extended_properties_private.py
+-rw-r--r--   0        0        0     1317 2023-06-13 22:28:48.467768 bruinen-1.2.1/src/bruinen/client/models/google_event_extended_properties_shared.py
+-rw-r--r--   0        0        0     4170 2023-06-13 22:28:48.518263 bruinen-1.2.1/src/bruinen/client/models/google_event_gadget.py
+-rw-r--r--   0        0        0     1266 2023-06-13 22:28:48.472873 bruinen-1.2.1/src/bruinen/client/models/google_event_gadget_preferences.py
+-rw-r--r--   0        0        0     2421 2023-06-13 22:28:48.505430 bruinen-1.2.1/src/bruinen/client/models/google_event_organizer.py
+-rw-r--r--   0        0        0     2259 2023-06-13 22:28:48.486956 bruinen-1.2.1/src/bruinen/client/models/google_event_original_start_time.py
+-rw-r--r--   0        0        0     2753 2023-06-13 22:28:48.496659 bruinen-1.2.1/src/bruinen/client/models/google_event_reminders.py
+-rw-r--r--   0        0        0     1953 2023-06-13 22:28:48.495857 bruinen-1.2.1/src/bruinen/client/models/google_event_reminders_overrides_item.py
+-rw-r--r--   0        0        0     1785 2023-06-13 22:28:48.514728 bruinen-1.2.1/src/bruinen/client/models/google_event_source.py
+-rw-r--r--   0        0        0     2145 2023-06-13 22:28:48.515998 bruinen-1.2.1/src/bruinen/client/models/google_event_start.py
+-rw-r--r--   0        0        0     6772 2023-06-13 22:28:48.560942 bruinen-1.2.1/src/bruinen/client/models/google_events.py
+-rw-r--r--   0        0        0     1924 2023-06-13 22:28:48.536583 bruinen-1.2.1/src/bruinen/client/models/google_events_default_reminders_item.py
+-rw-r--r--   0        0        0    22193 2023-06-13 22:28:48.970290 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item.py
+-rw-r--r--   0        0        0     2873 2023-06-13 22:28:48.547171 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_attachments_item.py
+-rw-r--r--   0        0        0     4530 2023-06-13 22:28:48.549707 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_attendees_item.py
+-rw-r--r--   0        0        0     6310 2023-06-13 22:28:48.567446 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data.py
+-rw-r--r--   0        0        0     3181 2023-06-13 22:28:48.557977 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution.py
+-rw-r--r--   0        0        0     1755 2023-06-13 22:28:48.553386 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution_key.py
+-rw-r--r--   0        0        0     4541 2023-06-13 22:28:48.585032 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request.py
+-rw-r--r--   0        0        0     1857 2023-06-13 22:28:48.567446 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request_conference_solution_key.py
+-rw-r--r--   0        0        0     1827 2023-06-13 22:28:48.577243 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request_status.py
+-rw-r--r--   0        0        0     3921 2023-06-13 22:28:48.842425 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_entry_points_item.py
+-rw-r--r--   0        0        0     2462 2023-06-13 22:28:48.593027 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_creator.py
+-rw-r--r--   0        0        0     2188 2023-06-13 22:28:48.781923 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_end.py
+-rw-r--r--   0        0        0     3579 2023-06-13 22:28:48.612565 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_extended_properties.py
+-rw-r--r--   0        0        0     1384 2023-06-13 22:28:48.603607 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_extended_properties_private.py
+-rw-r--r--   0        0        0     1378 2023-06-13 22:28:48.608925 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_extended_properties_shared.py
+-rw-r--r--   0        0        0     4323 2023-06-13 22:28:48.878512 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_gadget.py
+-rw-r--r--   0        0        0     1327 2023-06-13 22:28:48.613818 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_gadget_preferences.py
+-rw-r--r--   0        0        0     2482 2023-06-13 22:28:48.910917 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_organizer.py
+-rw-r--r--   0        0        0     2320 2023-06-13 22:28:48.850848 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_original_start_time.py
+-rw-r--r--   0        0        0     2920 2023-06-13 22:28:48.709569 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_reminders.py
+-rw-r--r--   0        0        0     2014 2023-06-13 22:28:48.898873 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_reminders_overrides_item.py
+-rw-r--r--   0        0        0     1846 2023-06-13 22:28:48.810519 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_source.py
+-rw-r--r--   0        0        0     2206 2023-06-13 22:28:48.892481 bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_start.py
+-rw-r--r--   0        0        0     5170 2023-06-13 22:28:48.921772 bruinen-1.2.1/src/bruinen/client/models/google_label.py
+-rw-r--r--   0        0        0     1927 2023-06-13 22:28:48.892705 bruinen-1.2.1/src/bruinen/client/models/google_label_color.py
+-rw-r--r--   0        0        0     2652 2023-06-13 22:28:48.910461 bruinen-1.2.1/src/bruinen/client/models/google_labels.py
+-rw-r--r--   0        0        0     2945 2023-06-13 22:28:48.920220 bruinen-1.2.1/src/bruinen/client/models/google_labels_labels_item.py
+-rw-r--r--   0        0        0     4411 2023-06-13 22:28:48.965530 bruinen-1.2.1/src/bruinen/client/models/google_message.py
+-rw-r--r--   0        0        0     4958 2023-06-13 22:28:48.963041 bruinen-1.2.1/src/bruinen/client/models/google_message_payload.py
+-rw-r--r--   0        0        0     2110 2023-06-13 22:28:48.919449 bruinen-1.2.1/src/bruinen/client/models/google_message_payload_body.py
+-rw-r--r--   0        0        0     1802 2023-06-13 22:28:48.924412 bruinen-1.2.1/src/bruinen/client/models/google_message_payload_headers_item.py
+-rw-r--r--   0        0        0     4162 2023-06-13 22:28:48.961524 bruinen-1.2.1/src/bruinen/client/models/google_message_payload_parts_item.py
+-rw-r--r--   0        0        0     2158 2023-06-13 22:28:48.970964 bruinen-1.2.1/src/bruinen/client/models/google_message_payload_parts_item_body.py
+-rw-r--r--   0        0        0     1853 2023-06-13 22:28:48.974875 bruinen-1.2.1/src/bruinen/client/models/google_message_payload_parts_item_headers_item.py
+-rw-r--r--   0        0        0     3115 2023-06-13 22:28:48.982418 bruinen-1.2.1/src/bruinen/client/models/google_messages.py
+-rw-r--r--   0        0        0     1844 2023-06-13 22:28:48.955408 bruinen-1.2.1/src/bruinen/client/models/google_messages_messages_item.py
+-rw-r--r--   0        0        0     4814 2023-06-13 22:28:49.017346 bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft.py
+-rw-r--r--   0        0        0     3902 2023-06-13 22:28:49.010189 bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_attachments_item.py
+-rw-r--r--   0        0        0     5378 2023-06-13 22:28:49.038770 bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers.py
+-rw-r--r--   0        0        0     1865 2023-06-13 22:28:48.987267 bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers_bcc_item.py
+-rw-r--r--   0        0        0     1857 2023-06-13 22:28:49.007066 bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers_cc_item.py
+-rw-r--r--   0        0        0     1858 2023-06-13 22:28:49.001270 bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers_from.py
+-rw-r--r--   0        0        0     1879 2023-06-13 22:28:49.006929 bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers_to_item.py
+-rw-r--r--   0        0        0     3122 2023-06-15 02:42:26.229396 bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts.py
+-rw-r--r--   0        0        0     5048 2023-06-15 02:42:26.229607 bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item.py
+-rw-r--r--   0        0        0     3963 2023-06-15 02:42:26.229826 bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_attachments_item.py
+-rw-r--r--   0        0        0     5799 2023-06-15 02:42:26.230045 bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers.py
+-rw-r--r--   0        0        0     1926 2023-06-15 02:42:26.230366 bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_bcc_item.py
+-rw-r--r--   0        0        0     1918 2023-06-15 02:42:26.230562 bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_cc_item.py
+-rw-r--r--   0        0        0     1919 2023-06-15 02:42:26.230767 bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_from.py
+-rw-r--r--   0        0        0     1940 2023-06-15 02:42:26.230958 bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_to_item.py
+-rw-r--r--   0        0        0     4552 2023-06-13 22:28:49.076366 bruinen-1.2.1/src/bruinen/client/models/google_parsed_message.py
+-rw-r--r--   0        0        0     3914 2023-06-13 22:28:49.059009 bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_attachments_item.py
+-rw-r--r--   0        0        0     5460 2023-06-13 22:28:49.136027 bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers.py
+-rw-r--r--   0        0        0     1877 2023-06-13 22:28:49.062327 bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers_bcc_item.py
+-rw-r--r--   0        0        0     1869 2023-06-13 22:28:49.065775 bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers_cc_item.py
+-rw-r--r--   0        0        0     1870 2023-06-13 22:28:49.047374 bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers_from.py
+-rw-r--r--   0        0        0     1891 2023-06-13 22:28:49.050838 bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers_to_item.py
+-rw-r--r--   0        0        0     3199 2023-06-15 02:42:26.231152 bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages.py
+-rw-r--r--   0        0        0     4853 2023-06-15 02:42:26.231353 bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item.py
+-rw-r--r--   0        0        0     3985 2023-06-15 02:42:26.231562 bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_attachments_item.py
+-rw-r--r--   0        0        0     6075 2023-06-15 02:42:26.231771 bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers.py
+-rw-r--r--   0        0        0     1948 2023-06-15 02:42:26.232200 bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers_bcc_item.py
+-rw-r--r--   0        0        0     1940 2023-06-15 02:42:26.232503 bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers_cc_item.py
+-rw-r--r--   0        0        0     1941 2023-06-15 02:42:26.232709 bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers_from.py
+-rw-r--r--   0        0        0     1962 2023-06-15 02:42:26.233013 bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers_to_item.py
+-rw-r--r--   0        0        0     2583 2023-06-13 22:28:49.106121 bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread.py
+-rw-r--r--   0        0        0     4837 2023-06-13 22:28:49.227113 bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item.py
+-rw-r--r--   0        0        0     3975 2023-06-13 22:28:49.166314 bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_attachments_item.py
+-rw-r--r--   0        0        0     5948 2023-06-13 22:28:49.252508 bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers.py
+-rw-r--r--   0        0        0     1938 2023-06-13 22:28:49.202256 bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_bcc_item.py
+-rw-r--r--   0        0        0     1930 2023-06-13 22:28:49.165798 bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_cc_item.py
+-rw-r--r--   0        0        0     1931 2023-06-13 22:28:49.161402 bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_from.py
+-rw-r--r--   0        0        0     1952 2023-06-13 22:28:49.162152 bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_to_item.py
+-rw-r--r--   0        0        0     3152 2023-06-15 02:42:26.233306 bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads.py
+-rw-r--r--   0        0        0     2730 2023-06-15 02:42:26.233561 bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item.py
+-rw-r--r--   0        0        0     5163 2023-06-15 02:42:26.233761 bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item.py
+-rw-r--r--   0        0        0     4041 2023-06-15 02:42:26.233950 bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_attachments_item.py
+-rw-r--r--   0        0        0     6454 2023-06-15 02:42:26.234131 bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers.py
+-rw-r--r--   0        0        0     2004 2023-06-15 02:42:26.234298 bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_bcc_item.py
+-rw-r--r--   0        0        0     1996 2023-06-15 02:42:26.234464 bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_cc_item.py
+-rw-r--r--   0        0        0     1997 2023-06-15 02:42:26.234627 bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_from.py
+-rw-r--r--   0        0        0     2018 2023-06-15 02:42:26.234799 bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_to_item.py
+-rw-r--r--   0        0        0     2662 2023-06-13 22:28:49.285920 bruinen-1.2.1/src/bruinen/client/models/google_profile.py
+-rw-r--r--   0        0        0     3121 2023-06-13 22:28:49.321794 bruinen-1.2.1/src/bruinen/client/models/google_thread.py
+-rw-r--r--   0        0        0     4544 2023-06-13 22:28:49.329615 bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item.py
+-rw-r--r--   0        0        0     5273 2023-06-13 22:28:49.371268 bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload.py
+-rw-r--r--   0        0        0     2171 2023-06-13 22:28:49.282377 bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_body.py
+-rw-r--r--   0        0        0     1863 2023-06-13 22:28:49.309501 bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_headers_item.py
+-rw-r--r--   0        0        0     4480 2023-06-13 22:28:49.374148 bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item.py
+-rw-r--r--   0        0        0     2219 2023-06-13 22:28:49.347284 bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_body.py
+-rw-r--r--   0        0        0     1914 2023-06-13 22:28:49.320552 bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_headers_item.py
+-rw-r--r--   0        0        0     3068 2023-06-13 22:28:49.340367 bruinen-1.2.1/src/bruinen/client/models/google_threads.py
+-rw-r--r--   0        0        0     2135 2023-06-13 22:28:49.326683 bruinen-1.2.1/src/bruinen/client/models/google_threads_threads_item.py
+-rw-r--r--   0        0        0     3499 2023-06-13 22:28:49.363181 bruinen-1.2.1/src/bruinen/client/models/returned_account_dto.py
+-rw-r--r--   0        0        0     4714 2023-06-13 22:28:49.380607 bruinen-1.2.1/src/bruinen/client/models/returned_confirm_dto.py
+-rw-r--r--   0        0        0     1218 2023-06-13 22:28:49.380108 bruinen-1.2.1/src/bruinen/client/models/returned_confirm_dto_params.py
+-rw-r--r--   0        0        0     3613 2023-06-13 22:28:49.361914 bruinen-1.2.1/src/bruinen/client/models/returned_connection_request_dto.py
+-rw-r--r--   0        0        0     1271 2023-06-13 22:28:49.378219 bruinen-1.2.1/src/bruinen/client/models/returned_connection_request_dto_source.py
+-rw-r--r--   0        0        0     4313 2023-06-13 22:28:49.416927 bruinen-1.2.1/src/bruinen/client/models/returned_source_policy_dto.py
+-rw-r--r--   0        0        0     2719 2023-06-13 22:28:49.429967 bruinen-1.2.1/src/bruinen/client/models/returned_user_dto.py
+-rw-r--r--   0        0        0     2901 2023-06-13 22:28:49.405957 bruinen-1.2.1/src/bruinen/client/models/source_data.py
+-rw-r--r--   0        0        0      177 2023-06-13 22:28:46.969084 bruinen-1.2.1/src/bruinen/client/models/source_policy_status.py
+-rw-r--r--   0        0        0      549 2023-06-13 22:28:46.910848 bruinen-1.2.1/src/bruinen/client/models/source_type.py
+-rw-r--r--   0        0        0     1350 2023-06-13 22:28:49.409644 bruinen-1.2.1/src/bruinen/client/models/sources_controller_get_metadata_for_source_response_200.py
+-rw-r--r--   0        0        0     2362 2023-06-13 22:28:49.422625 bruinen-1.2.1/src/bruinen/client/models/update_user_dto.py
+-rw-r--r--   0        0        0     2362 2023-06-13 22:28:49.428908 bruinen-1.2.1/src/bruinen/client/models/upsert_user_dto.py
+-rw-r--r--   0        0        0     1292 2023-06-13 22:28:49.421934 bruinen-1.2.1/src/bruinen/client/models/usage_controller_find_all_response_200_item.py
+-rw-r--r--   0        0        0       25 2023-06-13 22:28:46.071821 bruinen-1.2.1/src/bruinen/client/py.typed
+-rw-r--r--   0        0        0      993 2023-06-13 22:28:49.391265 bruinen-1.2.1/src/bruinen/client/types.py
+-rw-r--r--   0        0        0       36 2023-06-09 17:40:25.908847 bruinen-1.2.1/src/bruinen/confirm/__init__.py
+-rw-r--r--   0        0        0     2032 2023-05-30 21:25:54.185883 bruinen-1.2.1/src/bruinen/confirm/confirm.py
+-rw-r--r--   0        0        0        0 2023-05-30 21:25:54.185920 bruinen-1.2.1/src/bruinen/langchain/__init__.py
+-rw-r--r--   0        0        0     6508 2023-06-15 02:43:01.941566 bruinen-1.2.1/src/bruinen/langchain/github.py
+-rw-r--r--   0        0        0    73035 2023-06-15 02:43:01.942715 bruinen-1.2.1/src/bruinen/langchain/google.py
+-rw-r--r--   0        0        0       34 2023-06-06 18:24:40.536279 bruinen-1.2.1/src/bruinen/langchain/parsers/__init__.py
+-rw-r--r--   0        0        0     4398 2023-06-09 17:40:25.910512 bruinen-1.2.1/src/bruinen/langchain/parsers/sql_parser.py
+-rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 bruinen-1.2.1/PKG-INFO
```

### Comparing `bruinen-1.2/README.md` & `bruinen-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/pyproject.toml` & `bruinen-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bruinen"
-version = "1.2"
+version = "1.2.1"
 description = "A client library for accessing Bruinen API"
 authors = []
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = ">=0.15.4,<0.25.0"
```

### Comparing `bruinen-1.2/src/bruinen/client/api/accounts/account_counts_for_policy.py` & `bruinen-1.2.1/src/bruinen/client/api/accounts/account_counts_for_policy.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/accounts/accounts_controller_deactivate.py` & `bruinen-1.2.1/src/bruinen/client/api/accounts/accounts_controller_deactivate.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/accounts/accounts_controller_get_accounts.py` & `bruinen-1.2.1/src/bruinen/client/api/accounts/accounts_controller_get_accounts.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/accounts/find_all_accounts_for_user.py` & `bruinen-1.2.1/src/bruinen/client/api/accounts/find_all_accounts_for_user.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/accounts/find_all_active_for_user.py` & `bruinen-1.2.1/src/bruinen/client/api/accounts/find_all_active_for_user.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/accounts/find_all_active_with_policy_for_user.py` & `bruinen-1.2.1/src/bruinen/client/api/accounts/find_all_active_with_policy_for_user.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/accounts/get_account.py` & `bruinen-1.2.1/src/bruinen/client/api/accounts/get_account.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/auth/get_user_auth_token.py` & `bruinen-1.2.1/src/bruinen/client/api/auth/get_user_auth_token.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/confirm/create.py` & `bruinen-1.2.1/src/bruinen/client/api/confirm/create.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/confirm/find_one.py` & `bruinen-1.2.1/src/bruinen/client/api/confirm/find_one.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/connection_requests/connection_requests_controller_find_all.py` & `bruinen-1.2.1/src/bruinen/client/api/connection_requests/connection_requests_controller_find_all.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/connection_requests/create.py` & `bruinen-1.2.1/src/bruinen/client/api/connection_requests/create.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/connection_requests/get.py` & `bruinen-1.2.1/src/bruinen/client/api/connection_requests/get.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/source_policy/source_policy_controller_get_all_active_for_client.py` & `bruinen-1.2.1/src/bruinen/client/api/source_policy/source_policy_controller_get_all_active_for_client.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/source_policy/source_policy_controller_get_defaults_for_client.py` & `bruinen-1.2.1/src/bruinen/client/api/source_policy/source_policy_controller_get_defaults_for_client.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/source_policy/source_policy_controller_get_policy_by_id.py` & `bruinen-1.2.1/src/bruinen/client/api/source_policy/source_policy_controller_get_policy_by_id.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/source_policy/source_policy_controller_set_default.py` & `bruinen-1.2.1/src/bruinen/client/api/source_policy/source_policy_controller_set_default.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/github_controller_profile.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/github_controller_profile.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/github_controller_repos.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/github_controller_repos.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_calendar.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_calendar.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_calendars.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_calendars.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_draft.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_draft.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_drafts.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_drafts.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_event.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_event.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_events.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_events.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_label.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_label.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_labels.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_labels.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_message.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_messages.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_messages.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_draft.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_draft.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_drafts.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_drafts.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_message.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_messages.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_messages.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_thread.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_thread.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_parsed_threads.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_parsed_threads.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_profile.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_profile.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_thread.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_thread.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/google_controller_threads.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/google_controller_threads.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/sources_controller_get_metadata.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/sources_controller_get_metadata.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/sources/sources_controller_get_metadata_for_source.py` & `bruinen-1.2.1/src/bruinen/client/api/sources/sources_controller_get_metadata_for_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/usage/usage_controller_find_all.py` & `bruinen-1.2.1/src/bruinen/client/api/usage/usage_controller_find_all.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/usage/usage_controller_find_one.py` & `bruinen-1.2.1/src/bruinen/client/api/usage/usage_controller_find_one.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/usage/usage_controller_get_client_data.py` & `bruinen-1.2.1/src/bruinen/client/api/usage/usage_controller_get_client_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/users/users_controller_create.py` & `bruinen-1.2.1/src/bruinen/client/api/users/users_controller_create.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/users/users_controller_find_all.py` & `bruinen-1.2.1/src/bruinen/client/api/users/users_controller_find_all.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/users/users_controller_find_one.py` & `bruinen-1.2.1/src/bruinen/client/api/users/users_controller_find_one.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/users/users_controller_find_user_from_token.py` & `bruinen-1.2.1/src/bruinen/client/api/users/users_controller_find_user_from_token.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/users/users_controller_update.py` & `bruinen-1.2.1/src/bruinen/client/api/users/users_controller_update.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/api/users/users_controller_upsert_user.py` & `bruinen-1.2.1/src/bruinen/client/api/users/users_controller_upsert_user.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/client.py` & `bruinen-1.2.1/src/bruinen/client/client.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/__init__.py` & `bruinen-1.2.1/src/bruinen/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/accounts_controller_deactivate_response_200.py` & `bruinen-1.2.1/src/bruinen/client/models/accounts_controller_deactivate_response_200.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/accounts_controller_get_accounts_response_200_item.py` & `bruinen-1.2.1/src/bruinen/client/models/accounts_controller_get_accounts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/auth.py` & `bruinen-1.2.1/src/bruinen/client/models/auth.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/client_usage_data.py` & `bruinen-1.2.1/src/bruinen/client/models/client_usage_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/connection_requests_controller_find_all_response_200_item.py` & `bruinen-1.2.1/src/bruinen/client/models/connection_requests_controller_find_all_response_200_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/create_confirm_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/create_confirm_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/create_confirm_dto_params.py` & `bruinen-1.2.1/src/bruinen/client/models/create_confirm_dto_params.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/create_confirm_returned_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/create_confirm_returned_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/create_connection_request_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/create_connection_request_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/create_connection_request_dto_source.py` & `bruinen-1.2.1/src/bruinen/client/models/create_connection_request_dto_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/create_user_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/create_user_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/endpoint_data.py` & `bruinen-1.2.1/src/bruinen/client/models/endpoint_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/get_response_200.py` & `bruinen-1.2.1/src/bruinen/client/models/get_response_200.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/github_profile.py` & `bruinen-1.2.1/src/bruinen/client/models/github_profile.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/github_repo.py` & `bruinen-1.2.1/src/bruinen/client/models/github_repo.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/github_repo_owner.py` & `bruinen-1.2.1/src/bruinen/client/models/github_repo_owner.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/github_repo_permissions.py` & `bruinen-1.2.1/src/bruinen/client/models/github_repo_permissions.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_calendar.py` & `bruinen-1.2.1/src/bruinen/client/models/google_calendar.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_calendar_conference_properties.py` & `bruinen-1.2.1/src/bruinen/client/models/google_calendar_conference_properties.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_calendars.py` & `bruinen-1.2.1/src/bruinen/client/models/google_calendars.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item_conference_properties.py` & `bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item_conference_properties.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item_default_reminders.py` & `bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item_default_reminders.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item_notification_settings.py` & `bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item_notification_settings.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_calendars_calendars_item_notification_settings_notifications_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_calendars_calendars_item_notification_settings_notifications_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message_payload.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_body.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_headers_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_body.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_headers_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_body.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_headers_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_draft_message_payload_parts_item_parts_item_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_drafts.py` & `bruinen-1.2.1/src/bruinen/client/models/google_drafts.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_drafts_drafts_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_drafts_drafts_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_drafts_drafts_item_message.py` & `bruinen-1.2.1/src/bruinen/client/models/google_drafts_drafts_item_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_attachments_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_attendees_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_attendees_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_conference_data.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_conference_data_conference_solution.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_conference_solution.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_conference_data_conference_solution_key.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_conference_solution_key.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_conference_data_create_request.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_create_request.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_conference_data_create_request_conference_solution_key.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_create_request_conference_solution_key.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_conference_data_create_request_status.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_create_request_status.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_conference_data_entry_points_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_conference_data_entry_points_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_creator.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_creator.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_end.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_end.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_extended_properties.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_extended_properties.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_extended_properties_private.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_extended_properties_private.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_extended_properties_shared.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_extended_properties_shared.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_gadget.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_gadget.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_gadget_preferences.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_gadget_preferences.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_organizer.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_organizer.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_original_start_time.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_original_start_time.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_reminders.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_reminders.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_reminders_overrides_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_reminders_overrides_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_source.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_event_start.py` & `bruinen-1.2.1/src/bruinen/client/models/google_event_start.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_default_reminders_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_default_reminders_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_attachments_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_attendees_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_attendees_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution_key.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_conference_solution_key.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_create_request.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_create_request_conference_solution_key.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request_conference_solution_key.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_create_request_status.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_create_request_status.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_conference_data_entry_points_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_conference_data_entry_points_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_creator.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_creator.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_end.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_end.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_extended_properties.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_extended_properties.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_extended_properties_private.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_extended_properties_private.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_extended_properties_shared.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_extended_properties_shared.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_gadget.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_gadget.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_gadget_preferences.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_gadget_preferences.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_organizer.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_organizer.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_original_start_time.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_original_start_time.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_reminders.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_reminders.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_reminders_overrides_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_reminders_overrides_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_source.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_events_events_item_start.py` & `bruinen-1.2.1/src/bruinen/client/models/google_events_events_item_start.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_label.py` & `bruinen-1.2.1/src/bruinen/client/models/google_label.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_label_color.py` & `bruinen-1.2.1/src/bruinen/client/models/google_label_color.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_labels.py` & `bruinen-1.2.1/src/bruinen/client/models/google_labels.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_labels_labels_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_labels_labels_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_message.py` & `bruinen-1.2.1/src/bruinen/client/models/google_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_message_payload.py` & `bruinen-1.2.1/src/bruinen/client/models/google_message_payload.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_message_payload_body.py` & `bruinen-1.2.1/src/bruinen/client/models/google_message_payload_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_message_payload_headers_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_message_payload_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_message_payload_parts_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_message_payload_parts_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_message_payload_parts_item_body.py` & `bruinen-1.2.1/src/bruinen/client/models/google_message_payload_parts_item_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_message_payload_parts_item_headers_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_message_payload_parts_item_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_messages.py` & `bruinen-1.2.1/src/bruinen/client/models/google_messages.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_messages_messages_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_messages_messages_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_draft.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_draft_attachments_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers_bcc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers_bcc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers_cc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers_cc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers_from.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers_from.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_draft_headers_to_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_draft_headers_to_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_drafts.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_attachments_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_bcc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_bcc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_cc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_cc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_from.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_from.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_to_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_drafts_drafts_item_headers_to_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_message.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_message.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_message_attachments_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers_bcc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers_bcc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers_cc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers_cc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers_from.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers_from.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_message_headers_to_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_message_headers_to_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_messages.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_attachments_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers_bcc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers_bcc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers_cc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers_cc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers_from.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers_from.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_messages_messages_item_headers_to_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_messages_messages_item_headers_to_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_thread.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_attachments_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers_bcc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_bcc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers_cc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_cc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers_from.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_from.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_thread_messages_item_headers_to_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_thread_messages_item_headers_to_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_threads.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_attachments_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_attachments_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_bcc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_bcc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_cc_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_cc_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_from.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_from.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_to_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_parsed_threads_threads_item_messages_item_headers_to_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_profile.py` & `bruinen-1.2.1/src/bruinen/client/models/google_profile.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_thread.py` & `bruinen-1.2.1/src/bruinen/client/models/google_thread.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_thread_messages_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload.py` & `bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_body.py` & `bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_headers_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_parts_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_body.py` & `bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_body.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_headers_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_thread_messages_item_payload_parts_item_headers_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_threads.py` & `bruinen-1.2.1/src/bruinen/client/models/google_threads.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/google_threads_threads_item.py` & `bruinen-1.2.1/src/bruinen/client/models/google_threads_threads_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/returned_account_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/returned_account_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/returned_confirm_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/returned_confirm_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/returned_confirm_dto_params.py` & `bruinen-1.2.1/src/bruinen/client/models/returned_confirm_dto_params.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/returned_connection_request_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/returned_connection_request_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/returned_connection_request_dto_source.py` & `bruinen-1.2.1/src/bruinen/client/models/returned_connection_request_dto_source.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/returned_source_policy_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/returned_source_policy_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/returned_user_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/returned_user_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/source_data.py` & `bruinen-1.2.1/src/bruinen/client/models/source_data.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/source_type.py` & `bruinen-1.2.1/src/bruinen/client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/sources_controller_get_metadata_for_source_response_200.py` & `bruinen-1.2.1/src/bruinen/client/models/sources_controller_get_metadata_for_source_response_200.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/update_user_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/update_user_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/upsert_user_dto.py` & `bruinen-1.2.1/src/bruinen/client/models/upsert_user_dto.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/models/usage_controller_find_all_response_200_item.py` & `bruinen-1.2.1/src/bruinen/client/models/usage_controller_find_all_response_200_item.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/client/types.py` & `bruinen-1.2.1/src/bruinen/client/types.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/confirm/confirm.py` & `bruinen-1.2.1/src/bruinen/confirm/confirm.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/src/bruinen/langchain/github.py` & `bruinen-1.2.1/src/bruinen/langchain/github.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from ..client.api.sources import github_controller_repos
 from ..client.models import GithubRepo
 from ..client.api.sources import github_controller_profile
 from ..client.models import GithubProfile
 
 
 class GithubAuthenticatorTool(BaseTool):
-    name = 'Github Authenticator Tool'
+    name = 'github_authenticator_tool'
     description = """Useful for when a user's Github account is not authenticated.
 
     Input to the tool should be an empty string.
 
     The response from the tool will be a URL that you return to the user for them to complete auth.
     The URL will be your final answer.
     """
@@ -62,15 +62,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GithubGetReposTool(BaseTool):
-    name = "Github Get Repos Tool"
+    name = "github_get_repos_tool"
     description = """Useful for when you need to get a user's Github repos.
     
     Input should be the question that you want to know the answer to.
     
     Output will be the text response from the Github API.
     """
 
@@ -115,15 +115,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GithubGetProfileTool(BaseTool):
-    name = "Github Get Profile Tool"
+    name = "github_get_profile_tool"
     description = """Useful for when you need to get a user's Github profile.
     
     Input should be the question that you want to know the answer to.
     
     Output will be the text response from the Github API.
     """
```

### Comparing `bruinen-1.2/src/bruinen/langchain/google.py` & `bruinen-1.2.1/src/bruinen/langchain/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from ..client.api.sources import google_controller_events
 from ..client.models import GoogleEvents
 from ..client.api.sources import google_controller_event
 from ..client.models import GoogleEvent
 
 
 class GoogleAuthenticatorTool(BaseTool):
-    name = 'Google Authenticator Tool'
+    name = 'google_authenticator_tool'
     description = """Useful for when a user's Google account is not authenticated.
 
     Input to the tool should be an empty string.
 
     The response from the tool will be a URL that you return to the user for them to complete auth.
     The URL will be your final answer.
     """
@@ -96,15 +96,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetProfileTool(BaseTool):
-    name = "Google Get Profile Tool"
+    name = "google_get_profile_tool"
     description = """Useful for when you need to get a user's Google profile.
     
     Input should be the question that you want to know the answer to.
     
     Output will be the text response from the Google API.
     """
 
@@ -148,15 +148,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetDraftsTool(BaseTool):
-    name = "Google Get Drafts Tool"
+    name = "google_get_drafts_tool"
     description = """Useful for when you need to get a user's Google drafts.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -235,15 +235,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetParsedDraftsTool(BaseTool):
-    name = "Google Get ParsedDrafts Tool"
+    name = "google_get_parsed_drafts_tool"
     description = """Useful for when you need to get a user's Google parsed_drafts.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -322,15 +322,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetDraftTool(BaseTool):
-    name = "Google Get Draft Tool"
+    name = "google_get_draft_tool"
     description = """Useful for when you need to get a user's Google draft.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -407,15 +407,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetParsedDraftTool(BaseTool):
-    name = "Google Get ParsedDraft Tool"
+    name = "google_get_parsed_draft_tool"
     description = """Useful for when you need to get a user's Google parsed_draft.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -492,15 +492,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetLabelsTool(BaseTool):
-    name = "Google Get Labels Tool"
+    name = "google_get_labels_tool"
     description = """Useful for when you need to get a user's Google labels.
     
     Input should be the question that you want to know the answer to.
     
     Output will be the text response from the Google API.
     """
 
@@ -544,15 +544,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetLabelTool(BaseTool):
-    name = "Google Get Label Tool"
+    name = "google_get_label_tool"
     description = """Useful for when you need to get a user's Google label.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -629,15 +629,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetMessagesTool(BaseTool):
-    name = "Google Get Messages Tool"
+    name = "google_get_messages_tool"
     description = """Useful for when you need to get a user's Google messages.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -718,15 +718,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetParsedMessagesTool(BaseTool):
-    name = "Google Get ParsedMessages Tool"
+    name = "google_get_parsed_messages_tool"
     description = """Useful for when you need to get a user's Google parsed_messages.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -807,15 +807,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetMessageTool(BaseTool):
-    name = "Google Get Message Tool"
+    name = "google_get_message_tool"
     description = """Useful for when you need to get a user's Google message.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -892,15 +892,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetParsedMessageTool(BaseTool):
-    name = "Google Get ParsedMessage Tool"
+    name = "google_get_parsed_message_tool"
     description = """Useful for when you need to get a user's Google parsed_message.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -977,15 +977,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetThreadsTool(BaseTool):
-    name = "Google Get Threads Tool"
+    name = "google_get_threads_tool"
     description = """Useful for when you need to get a user's Google threads.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -1066,15 +1066,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetParsedThreadsTool(BaseTool):
-    name = "Google Get ParsedThreads Tool"
+    name = "google_get_parsed_threads_tool"
     description = """Useful for when you need to get a user's Google parsed_threads.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -1155,15 +1155,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetThreadTool(BaseTool):
-    name = "Google Get Thread Tool"
+    name = "google_get_thread_tool"
     description = """Useful for when you need to get a user's Google thread.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -1240,15 +1240,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetParsedThreadTool(BaseTool):
-    name = "Google Get ParsedThread Tool"
+    name = "google_get_parsed_thread_tool"
     description = """Useful for when you need to get a user's Google parsed_thread.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -1325,15 +1325,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetCalendarsTool(BaseTool):
-    name = "Google Get Calendars Tool"
+    name = "google_get_calendars_tool"
     description = """Useful for when you need to get a user's Google calendars.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -1416,15 +1416,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetCalendarTool(BaseTool):
-    name = "Google Get Calendar Tool"
+    name = "google_get_calendar_tool"
     description = """Useful for when you need to get a user's Google calendar.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -1501,15 +1501,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetEventsTool(BaseTool):
-    name = "Google Get Events Tool"
+    name = "google_get_events_tool"
     description = """Useful for when you need to get a user's Google events.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
@@ -1610,15 +1610,15 @@
         run_manager: Optional[AsyncCallbackManagerForToolRun] = None,
     ) -> str:
         """Run the tool asynchronously."""
         return await self._run(query, run_manager)
 
 
 class GoogleGetEventTool(BaseTool):
-    name = "Google Get Event Tool"
+    name = "google_get_event_tool"
     description = """Useful for when you need to get a user's Google event.
     
     Input should be a string containing the question that you want to know the answer to.
     Do not pass parameters as JSON, instead pass the string to the tool as is.
     
     Output will be the text response from the Google API.
     """
```

### Comparing `bruinen-1.2/src/bruinen/langchain/parsers/sql_parser.py` & `bruinen-1.2.1/src/bruinen/langchain/parsers/sql_parser.py`

 * *Files identical despite different names*

### Comparing `bruinen-1.2/PKG-INFO` & `bruinen-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bruinen
-Version: 1.2
+Version: 1.2.1
 Summary: A client library for accessing Bruinen API
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

