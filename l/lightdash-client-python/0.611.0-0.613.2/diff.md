# Comparing `tmp/lightdash_client_python-0.611.0.tar.gz` & `tmp/lightdash_client_python-0.613.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_client_python-0.611.0.tar", last modified: Wed Jun 14 04:54:50 2023, max compression
+gzip compressed data, was "lightdash_client_python-0.613.2.tar", last modified: Thu Jun 15 08:00:02 2023, max compression
```

## Comparing `lightdash_client_python-0.611.0.tar` & `lightdash_client_python-0.613.2.tar`

### file list

```diff
@@ -1,248 +1,250 @@
--rw-r--r--   0        0        0      804 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1849 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2335 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1115 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3078 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.gitignore
--rw-r--r--   0        0        0     1040 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.openapi-generator-ignore
--rw-r--r--   0        0        0     6821 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.openapi-generator/FILES
--rw-r--r--   0        0        0        6 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.openapi-generator/VERSION
--rw-r--r--   0        0        0     1266 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14088 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.pylintrc
--rw-r--r--   0        0        0      150 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.pypirc
--rw-r--r--   0        0        0        8 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.python-version
--rw-r--r--   0        0        0       32 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/.style.yapf
--rw-r--r--   0        0        0    11357 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/LICENSE
--rw-r--r--   0        0        0      717 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/Makefile
--rw-r--r--   0        0        0     3258 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/README.md
--rwxr-xr-x   0        0        0     1121 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/clean.sh
--rw-r--r--   0        0        0     2115 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/generate_clients.sh
--rw-r--r--   0        0        0      974 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/lint.sh
--rw-r--r--   0        0        0      211 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/openapi-python-client.yml
--rwxr-xr-x   0        0        0     1391 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/publish.sh
--rw-r--r--   0        0        0      152 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/schemas/README.md
--rw-r--r--   0        0        0   199906 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/schemas/swagger.json
--rwxr-xr-x   0        0        0     1023 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/setup.sh
--rwxr-xr-x   0        0        0      958 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/dev/test_python.sh
--rw-r--r--   0        0        0      201 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/__init__.py
--rw-r--r--   0        0        0       47 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/charts/__init__.py
--rw-r--r--   0        0        0     4680 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/charts/post_chart_results.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/content/__init__.py
--rw-r--r--   0        0        0     4483 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/content/get_pinned_items.py
--rw-r--r--   0        0        0     5511 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/content/update_pinned_items_order.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exploring/__init__.py
--rw-r--r--   0        0        0     5017 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exploring/post_run_query.py
--rw-r--r--   0        0        0     5095 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exploring/post_run_underlying_data_query.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exports/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/exports/get_csv_url.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/__init__.py
--rw-r--r--   0        0        0     4403 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     2743 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     4847 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
--rw-r--r--   0        0        0     3651 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_slack_channels.py
--rw-r--r--   0        0        0     2734 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/__init__.py
--rw-r--r--   0        0        0     2573 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/create_email_one_time_passcode.py
--rw-r--r--   0        0        0     3501 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/delete_me.py
--rw-r--r--   0        0        0     3021 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/get_email_verification_status.py
--rw-r--r--   0        0        0     4793 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/join_organization.py
--rw-r--r--   0        0        0     4349 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/my_account/list_my_available_organizations.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/__init__.py
--rw-r--r--   0        0        0     4634 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/create_group_in_organization.py
--rw-r--r--   0        0        0     4256 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/delete_my_organization.py
--rw-r--r--   0        0        0     4057 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/delete_organization_member.py
--rw-r--r--   0        0        0     3589 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/get_my_organization.py
--rw-r--r--   0        0        0     3739 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_groups_in_organization.py
--rw-r--r--   0        0        0     3983 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_organization_email_domains.py
--rw-r--r--   0        0        0     3859 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_organization_members.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/__init__.py
--rw-r--r--   0        0        0     5756 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/get_latest_validation_results.py
--rw-r--r--   0        0        0     4187 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/list_charts_in_project.py
--rw-r--r--   0        0        0     4187 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/list_spaces_in_project.py
--rw-r--r--   0        0        0     6428 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/projects/validate_project.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/__init__.py
--rw-r--r--   0        0        0     2984 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/create_space_in_project.py
--rw-r--r--   0        0        0     4928 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/get_project_access_list.py
--rw-r--r--   0        0        0     4648 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
--rw-r--r--   0        0        0     4794 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
--rw-r--r--   0        0        0     5026 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/update_project_access_for_user.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/__init__.py
--rw-r--r--   0        0        0     4176 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/delete_scheduler.py
--rw-r--r--   0        0        0     4147 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduled_jobs.py
--rw-r--r--   0        0        0     2633 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler.py
--rw-r--r--   0        0        0     4201 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler_job_status.py
--rw-r--r--   0        0        0     2620 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler_logs.py
--rw-r--r--   0        0        0     2919 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/schedulers/update_scheduler.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/share_links/__init__.py
--rw-r--r--   0        0        0     3960 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/share_links/get_share_url.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/spaces/__init__.py
--rw-r--r--   0        0        0     4429 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/spaces/delete_space.py
--rw-r--r--   0        0        0     2881 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/spaces/get_space.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/ssh_keypairs/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
--rw-r--r--   0        0        0        0 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/__init__.py
--rw-r--r--   0        0        0     4365 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/add_user_to_group.py
--rw-r--r--   0        0        0     3927 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/delete_group.py
--rw-r--r--   0        0        0     3949 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/get_group.py
--rw-r--r--   0        0        0     4073 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/get_group_members.py
--rw-r--r--   0        0        0     4348 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/api/user_groups/remove_user_from_group.py
--rw-r--r--   0        0        0     2906 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/client.py
--rw-r--r--   0        0        0      470 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/errors.py
--rw-r--r--   0        0        0    15782 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/__init__.py
--rw-r--r--   0        0        0     4166 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/additional_metric.py
--rw-r--r--   0        0        0     2422 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/allowed_email_domains.py
--rw-r--r--   0        0        0     2410 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_chart_summary_list_response.py
--rw-r--r--   0        0        0      152 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_chart_summary_list_response_status.py
--rw-r--r--   0        0        0     2106 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_csv_url_response.py
--rw-r--r--   0        0        0     1652 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_csv_url_response_results.py
--rw-r--r--   0        0        0      142 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_csv_url_response_status.py
--rw-r--r--   0        0        0     2254 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_metrics.py
--rw-r--r--   0        0        0      143 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_metrics_status.py
--rw-r--r--   0        0        0     2119 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
--rw-r--r--   0        0        0      157 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
--rw-r--r--   0        0        0      147 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_email_status_response_status.py
--rw-r--r--   0        0        0     2139 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_error_payload.py
--rw-r--r--   0        0        0     2386 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_error_payload_error.py
--rw-r--r--   0        0        0      146 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_error_payload_status.py
--rw-r--r--   0        0        0     2285 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_list_response.py
--rw-r--r--   0        0        0      145 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_list_response_status.py
--rw-r--r--   0        0        0     2359 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_members_response.py
--rw-r--r--   0        0        0      148 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_members_response_status.py
--rw-r--r--   0        0        0     1951 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_response.py
--rw-r--r--   0        0        0      141 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_group_response_status.py
--rw-r--r--   0        0        0     2208 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response.py
--rw-r--r--   0        0        0     1548 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response_results.py
--rw-r--r--   0        0        0      148 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response_status.py
--rw-r--r--   0        0        0     2157 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response.py
--rw-r--r--   0        0        0     1535 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response_results.py
--rw-r--r--   0        0        0      145 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response_status.py
--rw-r--r--   0        0        0     2019 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization.py
--rw-r--r--   0        0        0     2241 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_allowed_email_domains.py
--rw-r--r--   0        0        0      159 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_allowed_email_domains_status.py
--rw-r--r--   0        0        0     2270 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profile.py
--rw-r--r--   0        0        0      153 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profile_status.py
--rw-r--r--   0        0        0     2519 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profiles.py
--rw-r--r--   0        0        0      154 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profiles_status.py
--rw-r--r--   0        0        0      140 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_organization_status.py
--rw-r--r--   0        0        0     4825 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_pinned_items.py
--rw-r--r--   0        0        0      139 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_pinned_items_status.py
--rw-r--r--   0        0        0     2478 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_project_access_list_response.py
--rw-r--r--   0        0        0      153 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_project_access_list_response_status.py
--rw-r--r--   0        0        0     2140 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response.py
--rw-r--r--   0        0        0     2051 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response_results.py
--rw-r--r--   0        0        0      144 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response_status.py
--rw-r--r--   0        0        0     2383 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_scheduled_jobs_response.py
--rw-r--r--   0        0        0      149 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_scheduled_jobs_response_status.py
--rw-r--r--   0        0        0      155 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_scheduler_and_targets_response_status.py
--rw-r--r--   0        0        0      149 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_scheduler_logs_response_status.py
--rw-r--r--   0        0        0     2129 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_share_response.py
--rw-r--r--   0        0        0      141 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_share_response_status.py
--rw-r--r--   0        0        0     2376 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_slack_channels_response.py
--rw-r--r--   0        0        0      149 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_slack_channels_response_status.py
--rw-r--r--   0        0        0      141 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_space_response_status.py
--rw-r--r--   0        0        0     2410 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_space_summary_list_response.py
--rw-r--r--   0        0        0      152 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_space_summary_list_response_status.py
--rw-r--r--   0        0        0     2208 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_ssh_key_pair_response.py
--rw-r--r--   0        0        0      146 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_ssh_key_pair_response_status.py
--rw-r--r--   0        0        0     1937 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_success_empty.py
--rw-r--r--   0        0        0      140 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_success_empty_status.py
--rw-r--r--   0        0        0     2569 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_user_allowed_organizations_response.py
--rw-r--r--   0        0        0      160 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_user_allowed_organizations_response_status.py
--rw-r--r--   0        0        0     4732 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_validate_response.py
--rw-r--r--   0        0        0      144 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_validate_response_status.py
--rw-r--r--   0        0        0     1737 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_validation_dismiss_response.py
--rw-r--r--   0        0        0      153 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/api_validation_dismiss_response_status.py
--rw-r--r--   0        0        0      316 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/chart_kind.py
--rw-r--r--   0        0        0     3776 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/chart_summary.py
--rw-r--r--   0        0        0      192 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/chart_type.py
--rw-r--r--   0        0        0      220 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/compact.py
--rw-r--r--   0        0        0      272 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/compact_or_alias_type_1.py
--rw-r--r--   0        0        0     1937 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/create_project_member.py
--rw-r--r--   0        0        0     2646 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/create_space.py
--rw-r--r--   0        0        0     2229 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
--rw-r--r--   0        0        0     2494 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/dbt_cloud_metric.py
--rw-r--r--   0        0        0     2051 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/delete_scheduler_response_201.py
--rw-r--r--   0        0        0      151 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/delete_scheduler_response_201_status.py
--rw-r--r--   0        0        0     2003 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/email_one_time_password.py
--rw-r--r--   0        0        0     2749 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/email_one_time_password_expiring.py
--rw-r--r--   0        0        0     2458 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/email_status.py
--rw-r--r--   0        0        0     1664 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/filter_group_response_type_0.py
--rw-r--r--   0        0        0     1674 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/filter_group_response_type_1.py
--rw-r--r--   0        0        0     4615 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/filters.py
--rw-r--r--   0        0        0     2247 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/group.py
--rw-r--r--   0        0        0     2163 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/group_member.py
--rw-r--r--   0        0        0     4963 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/metric_query_response.py
--rw-r--r--   0        0        0      383 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/metric_type.py
--rw-r--r--   0        0        0     2812 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/organization.py
--rw-r--r--   0        0        0     3539 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/organization_member_profile.py
--rw-r--r--   0        0        0      287 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/organization_member_role.py
--rw-r--r--   0        0        0     2377 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
--rw-r--r--   0        0        0     2120 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/partial_pick_organization_member_profile_role.py
--rw-r--r--   0        0        0     2628 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/partial_pick_space_is_private_or_access.py
--rw-r--r--   0        0        0     2493 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
--rw-r--r--   0        0        0     1841 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
--rw-r--r--   0        0        0     1565 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_create_group_name.py
--rw-r--r--   0        0        0     6625 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1532 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_group_name.py
--rw-r--r--   0        0        0     1566 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_organization_name.py
--rw-r--r--   0        0        0     2016 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     3781 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
--rw-r--r--   0        0        0     4585 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1757 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_share_url_path_or_params.py
--rw-r--r--   0        0        0     1502 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_name.py
--rw-r--r--   0        0        0     1768 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_name_or_is_private.py
--rw-r--r--   0        0        0     2609 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
--rw-r--r--   0        0        0     3420 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
--rw-r--r--   0        0        0     1601 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_space_share_user_uuid.py
--rw-r--r--   0        0        0     1619 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_ssh_key_pair_public_key.py
--rw-r--r--   0        0        0     3860 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
--rw-r--r--   0        0        0     2266 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
--rw-r--r--   0        0        0     2095 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/post_chart_results_json_body.py
--rw-r--r--   0        0        0     2540 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/project_member_profile.py
--rw-r--r--   0        0        0      260 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/project_member_role.py
--rw-r--r--   0        0        0     1294 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/record_string_any.py
--rw-r--r--   0        0        0      193 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_item_type.py
--rw-r--r--   0        0        0      150 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_item_type_chart.py
--rw-r--r--   0        0        0      162 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_item_type_dashboard.py
--rw-r--r--   0        0        0      150 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_item_type_space.py
--rw-r--r--   0        0        0     2093 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_space_item.py
--rw-r--r--   0        0        0     3903 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/resource_view_space_item_data.py
--rw-r--r--   0        0        0     5334 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/run_query_request.py
--rw-r--r--   0        0        0     1933 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/run_query_request_filters.py
--rw-r--r--   0        0        0     1661 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduled_jobs.py
--rw-r--r--   0        0        0     4958 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_base.py
--rw-r--r--   0        0        0     2484 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_csv_options.py
--rw-r--r--   0        0        0      170 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_csv_options_limit_type_1.py
--rw-r--r--   0        0        0     2685 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_email_target.py
--rw-r--r--   0        0        0      156 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_format.py
--rw-r--r--   0        0        0     1272 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_image_options.py
--rw-r--r--   0        0        0      223 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_job_status.py
--rw-r--r--   0        0        0     5049 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_log.py
--rw-r--r--   0        0        0      167 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_log_target_type.py
--rw-r--r--   0        0        0      443 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_log_task.py
--rw-r--r--   0        0        0     2665 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/scheduler_slack_target.py
--rw-r--r--   0        0        0     3505 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/share_url.py
--rw-r--r--   0        0        0     1553 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/slack_channel.py
--rw-r--r--   0        0        0     1658 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/sort_field.py
--rw-r--r--   0        0        0     2115 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/space_share.py
--rw-r--r--   0        0        0     2480 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/space_summary.py
--rw-r--r--   0        0        0     2119 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/table_calculation.py
--rw-r--r--   0        0        0     2350 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/update_pinned_item_order.py
--rw-r--r--   0        0        0     1582 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/update_project_member.py
--rw-r--r--   0        0        0     1173 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/updated_by_user.py
--rw-r--r--   0        0        0     1993 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/user_allowed_organization.py
--rw-r--r--   0        0        0     1964 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validate_project_json_body.py
--rw-r--r--   0        0        0     6205 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_error_chart_response.py
--rw-r--r--   0        0        0     5966 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_error_dashboard_response.py
--rw-r--r--   0        0        0      260 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_error_type.py
--rw-r--r--   0        0        0     3709 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_response_base.py
--rw-r--r--   0        0        0      193 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/validation_source_type.py
--rw-r--r--   0        0        0     2633 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/models/view_statistics.py
--rw-r--r--   0        0        0       26 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/py.typed
--rw-r--r--   0        0        0     1101 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/lightdash_client/types.py
--rw-r--r--   0        0        0     1624 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/pyproject.toml
--rw-r--r--   0        0        0      830 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/setup.py
--rw-r--r--   0        0        0      796 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/tests/__init__.py
--rw-r--r--   0        0        0      908 2023-06-14 04:54:50.000000 lightdash_client_python-0.611.0/tests/test_dummy.py
--rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.611.0/PKG-INFO
+-rw-r--r--   0        0        0      804 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1849 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2335 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1115 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3078 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.gitignore
+-rw-r--r--   0        0        0     1040 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.openapi-generator-ignore
+-rw-r--r--   0        0        0     6821 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.openapi-generator/FILES
+-rw-r--r--   0        0        0        6 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.openapi-generator/VERSION
+-rw-r--r--   0        0        0     1266 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14088 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.pylintrc
+-rw-r--r--   0        0        0      150 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.pypirc
+-rw-r--r--   0        0        0        8 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.python-version
+-rw-r--r--   0        0        0       32 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/.style.yapf
+-rw-r--r--   0        0        0    11357 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/LICENSE
+-rw-r--r--   0        0        0      717 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/Makefile
+-rw-r--r--   0        0        0     3258 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/README.md
+-rwxr-xr-x   0        0        0     1121 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/clean.sh
+-rw-r--r--   0        0        0     2115 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/generate_clients.sh
+-rw-r--r--   0        0        0      974 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/lint.sh
+-rw-r--r--   0        0        0      211 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/openapi-python-client.yml
+-rwxr-xr-x   0        0        0     1391 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/publish.sh
+-rw-r--r--   0        0        0      152 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/schemas/README.md
+-rw-r--r--   0        0        0     1249 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/schemas/download.sh
+-rw-r--r--   0        0        0   200027 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/schemas/swagger.json
+-rwxr-xr-x   0        0        0     1023 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/setup.sh
+-rwxr-xr-x   0        0        0      958 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/dev/test_python.sh
+-rw-r--r--   0        0        0      201 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/charts/__init__.py
+-rw-r--r--   0        0        0     4680 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/charts/post_chart_results.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/content/__init__.py
+-rw-r--r--   0        0        0     4483 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/content/get_pinned_items.py
+-rw-r--r--   0        0        0     5511 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/content/update_pinned_items_order.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exploring/__init__.py
+-rw-r--r--   0        0        0     5017 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exploring/post_run_query.py
+-rw-r--r--   0        0        0     5095 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exploring/post_run_underlying_data_query.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exports/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/exports/get_csv_url.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/__init__.py
+-rw-r--r--   0        0        0     4403 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     2743 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4847 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     3651 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_slack_channels.py
+-rw-r--r--   0        0        0     2734 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/__init__.py
+-rw-r--r--   0        0        0     2573 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/create_email_one_time_passcode.py
+-rw-r--r--   0        0        0     3501 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/delete_me.py
+-rw-r--r--   0        0        0     3021 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/get_email_verification_status.py
+-rw-r--r--   0        0        0     4793 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/join_organization.py
+-rw-r--r--   0        0        0     4349 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/my_account/list_my_available_organizations.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/__init__.py
+-rw-r--r--   0        0        0     4634 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/create_group_in_organization.py
+-rw-r--r--   0        0        0     4256 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/delete_my_organization.py
+-rw-r--r--   0        0        0     4057 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/delete_organization_member.py
+-rw-r--r--   0        0        0     3589 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/get_my_organization.py
+-rw-r--r--   0        0        0     3739 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_groups_in_organization.py
+-rw-r--r--   0        0        0     3983 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_organization_email_domains.py
+-rw-r--r--   0        0        0     3859 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_organization_members.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     5756 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/get_latest_validation_results.py
+-rw-r--r--   0        0        0     4187 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/list_charts_in_project.py
+-rw-r--r--   0        0        0     4187 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/list_spaces_in_project.py
+-rw-r--r--   0        0        0     6428 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/projects/validate_project.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/__init__.py
+-rw-r--r--   0        0        0     2984 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/create_space_in_project.py
+-rw-r--r--   0        0        0     4928 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/get_project_access_list.py
+-rw-r--r--   0        0        0     4648 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
+-rw-r--r--   0        0        0     4425 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
+-rw-r--r--   0        0        0     4794 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
+-rw-r--r--   0        0        0     5026 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/update_project_access_for_user.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/__init__.py
+-rw-r--r--   0        0        0     4176 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/delete_scheduler.py
+-rw-r--r--   0        0        0     4147 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduled_jobs.py
+-rw-r--r--   0        0        0     2633 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler.py
+-rw-r--r--   0        0        0     4201 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler_job_status.py
+-rw-r--r--   0        0        0     2620 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler_logs.py
+-rw-r--r--   0        0        0     2919 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/schedulers/update_scheduler.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/share_links/__init__.py
+-rw-r--r--   0        0        0     3960 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/share_links/get_share_url.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/spaces/__init__.py
+-rw-r--r--   0        0        0     4429 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/spaces/delete_space.py
+-rw-r--r--   0        0        0     2881 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/spaces/get_space.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/ssh_keypairs/__init__.py
+-rw-r--r--   0        0        0     3542 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/__init__.py
+-rw-r--r--   0        0        0     4365 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/add_user_to_group.py
+-rw-r--r--   0        0        0     3927 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/delete_group.py
+-rw-r--r--   0        0        0     3949 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/get_group.py
+-rw-r--r--   0        0        0     4073 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/get_group_members.py
+-rw-r--r--   0        0        0     4348 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/api/user_groups/remove_user_from_group.py
+-rw-r--r--   0        0        0     2906 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/client.py
+-rw-r--r--   0        0        0      470 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/errors.py
+-rw-r--r--   0        0        0    15782 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/__init__.py
+-rw-r--r--   0        0        0     4166 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/additional_metric.py
+-rw-r--r--   0        0        0     2422 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/allowed_email_domains.py
+-rw-r--r--   0        0        0     2410 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_chart_summary_list_response.py
+-rw-r--r--   0        0        0      152 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_chart_summary_list_response_status.py
+-rw-r--r--   0        0        0     2106 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response.py
+-rw-r--r--   0        0        0     1652 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response_results.py
+-rw-r--r--   0        0        0      142 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response_status.py
+-rw-r--r--   0        0        0     2254 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0      143 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_metrics_status.py
+-rw-r--r--   0        0        0     2119 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
+-rw-r--r--   0        0        0      157 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
+-rw-r--r--   0        0        0      147 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_email_status_response_status.py
+-rw-r--r--   0        0        0     2139 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload.py
+-rw-r--r--   0        0        0     2386 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload_error.py
+-rw-r--r--   0        0        0      146 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload_status.py
+-rw-r--r--   0        0        0     2285 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_list_response.py
+-rw-r--r--   0        0        0      145 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_list_response_status.py
+-rw-r--r--   0        0        0     2359 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_members_response.py
+-rw-r--r--   0        0        0      148 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_members_response_status.py
+-rw-r--r--   0        0        0     1951 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_response.py
+-rw-r--r--   0        0        0      141 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_group_response_status.py
+-rw-r--r--   0        0        0     2208 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response.py
+-rw-r--r--   0        0        0     1548 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response_results.py
+-rw-r--r--   0        0        0      148 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response_status.py
+-rw-r--r--   0        0        0     2157 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response.py
+-rw-r--r--   0        0        0     1535 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response_results.py
+-rw-r--r--   0        0        0      145 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response_status.py
+-rw-r--r--   0        0        0     2019 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization.py
+-rw-r--r--   0        0        0     2241 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_allowed_email_domains.py
+-rw-r--r--   0        0        0      159 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_allowed_email_domains_status.py
+-rw-r--r--   0        0        0     2270 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profile.py
+-rw-r--r--   0        0        0      153 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profile_status.py
+-rw-r--r--   0        0        0     2519 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profiles.py
+-rw-r--r--   0        0        0      154 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profiles_status.py
+-rw-r--r--   0        0        0      140 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_organization_status.py
+-rw-r--r--   0        0        0     4825 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_pinned_items.py
+-rw-r--r--   0        0        0      139 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_pinned_items_status.py
+-rw-r--r--   0        0        0     2478 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_project_access_list_response.py
+-rw-r--r--   0        0        0      153 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_project_access_list_response_status.py
+-rw-r--r--   0        0        0     2140 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response.py
+-rw-r--r--   0        0        0     2051 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response_results.py
+-rw-r--r--   0        0        0      144 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response_status.py
+-rw-r--r--   0        0        0     2383 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_scheduled_jobs_response.py
+-rw-r--r--   0        0        0      149 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_scheduled_jobs_response_status.py
+-rw-r--r--   0        0        0      155 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_scheduler_and_targets_response_status.py
+-rw-r--r--   0        0        0      149 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_scheduler_logs_response_status.py
+-rw-r--r--   0        0        0     2129 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_share_response.py
+-rw-r--r--   0        0        0      141 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_share_response_status.py
+-rw-r--r--   0        0        0     2376 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_slack_channels_response.py
+-rw-r--r--   0        0        0      149 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_slack_channels_response_status.py
+-rw-r--r--   0        0        0      141 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_space_response_status.py
+-rw-r--r--   0        0        0     2410 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_space_summary_list_response.py
+-rw-r--r--   0        0        0      152 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_space_summary_list_response_status.py
+-rw-r--r--   0        0        0     2208 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_ssh_key_pair_response.py
+-rw-r--r--   0        0        0      146 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_ssh_key_pair_response_status.py
+-rw-r--r--   0        0        0     1937 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_success_empty.py
+-rw-r--r--   0        0        0      140 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_success_empty_status.py
+-rw-r--r--   0        0        0     2569 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_user_allowed_organizations_response.py
+-rw-r--r--   0        0        0      160 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_user_allowed_organizations_response_status.py
+-rw-r--r--   0        0        0     4732 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_validate_response.py
+-rw-r--r--   0        0        0      144 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_validate_response_status.py
+-rw-r--r--   0        0        0     1737 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_validation_dismiss_response.py
+-rw-r--r--   0        0        0      153 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/api_validation_dismiss_response_status.py
+-rw-r--r--   0        0        0      316 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/chart_kind.py
+-rw-r--r--   0        0        0     3776 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/chart_summary.py
+-rw-r--r--   0        0        0      192 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/chart_type.py
+-rw-r--r--   0        0        0      220 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/compact.py
+-rw-r--r--   0        0        0      272 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/compact_or_alias_type_1.py
+-rw-r--r--   0        0        0     1937 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/create_project_member.py
+-rw-r--r--   0        0        0     2646 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/create_space.py
+-rw-r--r--   0        0        0     2229 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
+-rw-r--r--   0        0        0     2494 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/dbt_cloud_metric.py
+-rw-r--r--   0        0        0     2051 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/delete_scheduler_response_201.py
+-rw-r--r--   0        0        0      151 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/delete_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     2003 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/email_one_time_password.py
+-rw-r--r--   0        0        0     2749 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/email_one_time_password_expiring.py
+-rw-r--r--   0        0        0     2458 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/email_status.py
+-rw-r--r--   0        0        0     1664 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/filter_group_response_type_0.py
+-rw-r--r--   0        0        0     1674 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/filter_group_response_type_1.py
+-rw-r--r--   0        0        0     4615 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/filters.py
+-rw-r--r--   0        0        0     2247 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/group.py
+-rw-r--r--   0        0        0     2163 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/group_member.py
+-rw-r--r--   0        0        0     4963 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/metric_query_response.py
+-rw-r--r--   0        0        0      383 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/metric_type.py
+-rw-r--r--   0        0        0     2812 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/organization.py
+-rw-r--r--   0        0        0     3539 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/organization_member_profile.py
+-rw-r--r--   0        0        0      287 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/organization_member_role.py
+-rw-r--r--   0        0        0     2377 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
+-rw-r--r--   0        0        0     2120 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/partial_pick_organization_member_profile_role.py
+-rw-r--r--   0        0        0     2628 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/partial_pick_space_is_private_or_access.py
+-rw-r--r--   0        0        0     2493 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0     1841 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
+-rw-r--r--   0        0        0     1565 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_create_group_name.py
+-rw-r--r--   0        0        0     6625 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1532 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_group_name.py
+-rw-r--r--   0        0        0     1566 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_organization_name.py
+-rw-r--r--   0        0        0     2016 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     3781 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
+-rw-r--r--   0        0        0     4585 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1757 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_share_url_path_or_params.py
+-rw-r--r--   0        0        0     1502 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_name.py
+-rw-r--r--   0        0        0     1768 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_name_or_is_private.py
+-rw-r--r--   0        0        0     2609 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
+-rw-r--r--   0        0        0     3420 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
+-rw-r--r--   0        0        0     1601 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_space_share_user_uuid.py
+-rw-r--r--   0        0        0     1619 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_ssh_key_pair_public_key.py
+-rw-r--r--   0        0        0     3860 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
+-rw-r--r--   0        0        0     2266 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
+-rw-r--r--   0        0        0     2095 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/post_chart_results_json_body.py
+-rw-r--r--   0        0        0     2540 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/project_member_profile.py
+-rw-r--r--   0        0        0      260 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/project_member_role.py
+-rw-r--r--   0        0        0     1294 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/record_string_any.py
+-rw-r--r--   0        0        0      193 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_item_type.py
+-rw-r--r--   0        0        0      150 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_item_type_chart.py
+-rw-r--r--   0        0        0      162 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_item_type_dashboard.py
+-rw-r--r--   0        0        0      150 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_item_type_space.py
+-rw-r--r--   0        0        0     2093 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_space_item.py
+-rw-r--r--   0        0        0     3903 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/resource_view_space_item_data.py
+-rw-r--r--   0        0        0     5334 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/run_query_request.py
+-rw-r--r--   0        0        0     1933 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/run_query_request_filters.py
+-rw-r--r--   0        0        0     1661 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduled_jobs.py
+-rw-r--r--   0        0        0     4958 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_base.py
+-rw-r--r--   0        0        0     2484 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_csv_options.py
+-rw-r--r--   0        0        0      170 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_csv_options_limit_type_1.py
+-rw-r--r--   0        0        0     2685 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_email_target.py
+-rw-r--r--   0        0        0      156 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_format.py
+-rw-r--r--   0        0        0     1272 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_image_options.py
+-rw-r--r--   0        0        0      223 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_job_status.py
+-rw-r--r--   0        0        0     5049 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_log.py
+-rw-r--r--   0        0        0      167 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_log_target_type.py
+-rw-r--r--   0        0        0      443 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_log_task.py
+-rw-r--r--   0        0        0     2665 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/scheduler_slack_target.py
+-rw-r--r--   0        0        0     3505 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/share_url.py
+-rw-r--r--   0        0        0     1553 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/slack_channel.py
+-rw-r--r--   0        0        0     1658 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/sort_field.py
+-rw-r--r--   0        0        0     2115 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/space_share.py
+-rw-r--r--   0        0        0     2480 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/space_summary.py
+-rw-r--r--   0        0        0     2119 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/table_calculation.py
+-rw-r--r--   0        0        0     2350 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/update_pinned_item_order.py
+-rw-r--r--   0        0        0     1582 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/update_project_member.py
+-rw-r--r--   0        0        0     1173 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/updated_by_user.py
+-rw-r--r--   0        0        0     1993 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/user_allowed_organization.py
+-rw-r--r--   0        0        0     1964 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validate_project_json_body.py
+-rw-r--r--   0        0        0     6492 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_error_chart_response.py
+-rw-r--r--   0        0        0     5966 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_error_dashboard_response.py
+-rw-r--r--   0        0        0      260 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_error_type.py
+-rw-r--r--   0        0        0     3709 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_response_base.py
+-rw-r--r--   0        0        0      193 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/validation_source_type.py
+-rw-r--r--   0        0        0     2633 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/models/view_statistics.py
+-rw-r--r--   0        0        0       26 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/py.typed
+-rw-r--r--   0        0        0     1101 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/lightdash_client/types.py
+-rw-r--r--   0        0        0     1624 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/setup.py
+-rw-r--r--   0        0        0      796 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/tests/__init__.py
+-rw-r--r--   0        0        0      908 2023-06-15 08:00:02.000000 lightdash_client_python-0.613.2/tests/test_dummy.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.613.2/PKG-INFO
```

### Comparing `lightdash_client_python-0.611.0/.github/CODEOWNERS` & `lightdash_client_python-0.613.2/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/.github/workflows/publish.yml` & `lightdash_client_python-0.613.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/.github/workflows/test-publish.yml` & `lightdash_client_python-0.613.2/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/.github/workflows/test.yml` & `lightdash_client_python-0.613.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/.gitignore` & `lightdash_client_python-0.613.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/.openapi-generator-ignore` & `lightdash_client_python-0.613.2/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/.openapi-generator/FILES` & `lightdash_client_python-0.613.2/.openapi-generator/FILES`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/.pre-commit-config.yaml` & `lightdash_client_python-0.613.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/.pylintrc` & `lightdash_client_python-0.613.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/LICENSE` & `lightdash_client_python-0.613.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/Makefile` & `lightdash_client_python-0.613.2/Makefile`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/README.md` & `lightdash_client_python-0.613.2/README.md`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/dev/clean.sh` & `lightdash_client_python-0.613.2/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/dev/generate_clients.sh` & `lightdash_client_python-0.613.2/dev/generate_clients.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/dev/lint.sh` & `lightdash_client_python-0.613.2/dev/lint.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/dev/publish.sh` & `lightdash_client_python-0.613.2/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/dev/schemas/swagger.json` & `lightdash_client_python-0.613.2/dev/schemas/swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916231373501782%*

 * *Differences: {"'components'": "{'schemas': {'ValidationErrorChartResponse': {'allOf': {1: {'properties': "*

 * *                 "{'chartName': OrderedDict([('type', 'string')])}}}}}}",*

 * * "'info'": "{'version': '0.613.1'}",*

 * * "'paths'": "{'/api/v1/projects/{projectUuid}/spaces/{spaceUuid}/share/{userUuid}': {'delete': "*

 * *            "{'operationId': 'RevokeSpaceAccessForUser'}}}"}*

```diff
@@ -2841,14 +2841,17 @@
             "ValidationErrorChartResponse": {
                 "allOf": [
                     {
                         "$ref": "#/components/schemas/ValidationResponseBase"
                     },
                     {
                         "properties": {
+                            "chartName": {
+                                "type": "string"
+                            },
                             "chartType": {
                                 "$ref": "#/components/schemas/ChartKind"
                             },
                             "chartUuid": {
                                 "type": "string"
                             },
                             "chartViews": {
@@ -3044,15 +3047,15 @@
             "url": "https://docs.lightdash.com/help-and-contact/contact/contact_info/"
         },
         "description": "Open API documentation for all public Lightdash API endpoints",
         "license": {
             "name": "MIT"
         },
         "title": "Lightdash API",
-        "version": "0.605.0"
+        "version": "0.613.1"
     },
     "openapi": "3.0.0",
     "paths": {
         "/api/v1/csv/{jobId}": {
             "get": {
                 "description": "Get a Csv",
                 "operationId": "getCsvUrl",
@@ -4794,15 +4797,15 @@
                     "Spaces"
                 ]
             }
         },
         "/api/v1/projects/{projectUuid}/spaces/{spaceUuid}/share/{userUuid}": {
             "delete": {
                 "description": "Remove a user's access to a space",
-                "operationId": "RevokeProjectAccessForUser",
+                "operationId": "RevokeSpaceAccessForUser",
                 "parameters": [
                     {
                         "description": "The uuid of the space's parent project",
                         "in": "path",
                         "name": "projectUuid",
                         "required": true,
                         "schema": {
```

### Comparing `lightdash_client_python-0.611.0/dev/setup.sh` & `lightdash_client_python-0.613.2/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/dev/test_python.sh` & `lightdash_client_python-0.613.2/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/charts/post_chart_results.py` & `lightdash_client_python-0.613.2/lightdash_client/api/charts/post_chart_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/content/get_pinned_items.py` & `lightdash_client_python-0.613.2/lightdash_client/api/content/get_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/content/update_pinned_items_order.py` & `lightdash_client_python-0.613.2/lightdash_client/api/content/update_pinned_items_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/exploring/post_run_query.py` & `lightdash_client_python-0.613.2/lightdash_client/api/exploring/post_run_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/exploring/post_run_underlying_data_query.py` & `lightdash_client_python-0.613.2/lightdash_client/api/exploring/post_run_underlying_data_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/exports/get_csv_url.py` & `lightdash_client_python-0.613.2/lightdash_client/api/exports/get_csv_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.613.2/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py` & `lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/integrations/get_slack_channels.py` & `lightdash_client_python-0.613.2/lightdash_client/api/integrations/get_slack_channels.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.613.2/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/my_account/create_email_one_time_passcode.py` & `lightdash_client_python-0.613.2/lightdash_client/api/my_account/create_email_one_time_passcode.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/my_account/delete_me.py` & `lightdash_client_python-0.613.2/lightdash_client/api/my_account/delete_me.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/my_account/get_email_verification_status.py` & `lightdash_client_python-0.613.2/lightdash_client/api/my_account/get_email_verification_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/my_account/join_organization.py` & `lightdash_client_python-0.613.2/lightdash_client/api/my_account/join_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/my_account/list_my_available_organizations.py` & `lightdash_client_python-0.613.2/lightdash_client/api/my_account/list_my_available_organizations.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/organizations/create_group_in_organization.py` & `lightdash_client_python-0.613.2/lightdash_client/api/organizations/create_group_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/organizations/delete_my_organization.py` & `lightdash_client_python-0.613.2/lightdash_client/api/organizations/delete_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/organizations/delete_organization_member.py` & `lightdash_client_python-0.613.2/lightdash_client/api/organizations/delete_organization_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/organizations/get_my_organization.py` & `lightdash_client_python-0.613.2/lightdash_client/api/organizations/get_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_groups_in_organization.py` & `lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_groups_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_organization_email_domains.py` & `lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_organization_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/organizations/list_organization_members.py` & `lightdash_client_python-0.613.2/lightdash_client/api/organizations/list_organization_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/projects/get_latest_validation_results.py` & `lightdash_client_python-0.613.2/lightdash_client/api/projects/get_latest_validation_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/projects/list_charts_in_project.py` & `lightdash_client_python-0.613.2/lightdash_client/api/projects/list_charts_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/projects/list_spaces_in_project.py` & `lightdash_client_python-0.613.2/lightdash_client/api/projects/list_spaces_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/projects/validate_project.py` & `lightdash_client_python-0.613.2/lightdash_client/api/projects/validate_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/create_space_in_project.py` & `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/create_space_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/get_project_access_list.py` & `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/get_project_access_list.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/grant_project_access_to_user.py` & `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/grant_project_access_to_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py` & `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/roles_permissions/update_project_access_for_user.py` & `lightdash_client_python-0.613.2/lightdash_client/api/roles_permissions/update_project_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/delete_scheduler.py` & `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/delete_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduled_jobs.py` & `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler.py` & `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler_job_status.py` & `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler_job_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/get_scheduler_logs.py` & `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/get_scheduler_logs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/schedulers/update_scheduler.py` & `lightdash_client_python-0.613.2/lightdash_client/api/schedulers/update_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/share_links/get_share_url.py` & `lightdash_client_python-0.613.2/lightdash_client/api/share_links/get_share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/spaces/delete_space.py` & `lightdash_client_python-0.613.2/lightdash_client/api/spaces/delete_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/spaces/get_space.py` & `lightdash_client_python-0.613.2/lightdash_client/api/spaces/get_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py` & `lightdash_client_python-0.613.2/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/user_groups/add_user_to_group.py` & `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/user_groups/delete_group.py` & `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/delete_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/user_groups/get_group.py` & `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/get_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/user_groups/get_group_members.py` & `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/get_group_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/api/user_groups/remove_user_from_group.py` & `lightdash_client_python-0.613.2/lightdash_client/api/user_groups/remove_user_from_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/client.py` & `lightdash_client_python-0.613.2/lightdash_client/client.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/__init__.py` & `lightdash_client_python-0.613.2/lightdash_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/additional_metric.py` & `lightdash_client_python-0.613.2/lightdash_client/models/additional_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/allowed_email_domains.py` & `lightdash_client_python-0.613.2/lightdash_client/models/allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_chart_summary_list_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_chart_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_csv_url_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_csv_url_response_results.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_csv_url_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_metrics.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_dbt_cloud_settings_delete_success.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_error_payload.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_error_payload_error.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_error_payload_error.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_group_list_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_group_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_group_members_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_group_members_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_group_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_group_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_job_scheduled_response_results.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_job_scheduled_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_job_status_response_results.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_job_status_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_organization.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_organization_allowed_email_domains.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_organization_allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profile.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_organization_member_profiles.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_organization_member_profiles.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_pinned_items.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_project_access_list_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_project_access_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_run_query_response_results.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_run_query_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_scheduled_jobs_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_scheduled_jobs_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_share_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_share_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_slack_channels_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_slack_channels_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_space_summary_list_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_space_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_ssh_key_pair_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_ssh_key_pair_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_success_empty.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_success_empty.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_user_allowed_organizations_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_user_allowed_organizations_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_validate_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_validate_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/api_validation_dismiss_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/api_validation_dismiss_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/chart_summary.py` & `lightdash_client_python-0.613.2/lightdash_client/models/chart_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/create_project_member.py` & `lightdash_client_python-0.613.2/lightdash_client/models/create_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/create_space.py` & `lightdash_client_python-0.613.2/lightdash_client/models/create_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/dbt_cloud_metadata_response_metrics.py` & `lightdash_client_python-0.613.2/lightdash_client/models/dbt_cloud_metadata_response_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/dbt_cloud_metric.py` & `lightdash_client_python-0.613.2/lightdash_client/models/dbt_cloud_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/delete_scheduler_response_201.py` & `lightdash_client_python-0.613.2/lightdash_client/models/delete_scheduler_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/email_one_time_password.py` & `lightdash_client_python-0.613.2/lightdash_client/models/email_one_time_password.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/email_one_time_password_expiring.py` & `lightdash_client_python-0.613.2/lightdash_client/models/email_one_time_password_expiring.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/email_status.py` & `lightdash_client_python-0.613.2/lightdash_client/models/email_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/filter_group_response_type_0.py` & `lightdash_client_python-0.613.2/lightdash_client/models/filter_group_response_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/filter_group_response_type_1.py` & `lightdash_client_python-0.613.2/lightdash_client/models/filter_group_response_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/filters.py` & `lightdash_client_python-0.613.2/lightdash_client/models/filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/group.py` & `lightdash_client_python-0.613.2/lightdash_client/models/group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/group_member.py` & `lightdash_client_python-0.613.2/lightdash_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/metric_query_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/metric_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/organization.py` & `lightdash_client_python-0.613.2/lightdash_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/organization_member_profile.py` & `lightdash_client_python-0.613.2/lightdash_client/models/organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py` & `lightdash_client_python-0.613.2/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/partial_pick_organization_member_profile_role.py` & `lightdash_client_python-0.613.2/lightdash_client/models/partial_pick_organization_member_profile_role.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/partial_pick_space_is_private_or_access.py` & `lightdash_client_python-0.613.2/lightdash_client/models/partial_pick_space_is_private_or_access.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_create_group_name.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_create_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_group_name.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_organization_name.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_organization_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_share_url_path_or_params.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_share_url_path_or_params.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_space_name.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_space_name_or_is_private.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_name_or_is_private.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_space_share_user_uuid.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_space_share_user_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_ssh_key_pair_public_key.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_ssh_key_pair_public_key.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py` & `lightdash_client_python-0.613.2/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/post_chart_results_json_body.py` & `lightdash_client_python-0.613.2/lightdash_client/models/post_chart_results_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/project_member_profile.py` & `lightdash_client_python-0.613.2/lightdash_client/models/project_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/record_string_any.py` & `lightdash_client_python-0.613.2/lightdash_client/models/record_string_any.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/resource_view_space_item.py` & `lightdash_client_python-0.613.2/lightdash_client/models/resource_view_space_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/resource_view_space_item_data.py` & `lightdash_client_python-0.613.2/lightdash_client/models/resource_view_space_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/run_query_request.py` & `lightdash_client_python-0.613.2/lightdash_client/models/run_query_request.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/run_query_request_filters.py` & `lightdash_client_python-0.613.2/lightdash_client/models/run_query_request_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/scheduled_jobs.py` & `lightdash_client_python-0.613.2/lightdash_client/models/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/scheduler_base.py` & `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/scheduler_csv_options.py` & `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_csv_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/scheduler_email_target.py` & `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_email_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/scheduler_image_options.py` & `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_image_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/scheduler_log.py` & `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_log.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/scheduler_slack_target.py` & `lightdash_client_python-0.613.2/lightdash_client/models/scheduler_slack_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/share_url.py` & `lightdash_client_python-0.613.2/lightdash_client/models/share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/slack_channel.py` & `lightdash_client_python-0.613.2/lightdash_client/models/slack_channel.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/sort_field.py` & `lightdash_client_python-0.613.2/lightdash_client/models/sort_field.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/space_share.py` & `lightdash_client_python-0.613.2/lightdash_client/models/space_share.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/space_summary.py` & `lightdash_client_python-0.613.2/lightdash_client/models/space_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/table_calculation.py` & `lightdash_client_python-0.613.2/lightdash_client/models/table_calculation.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/update_pinned_item_order.py` & `lightdash_client_python-0.613.2/lightdash_client/models/update_pinned_item_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/update_project_member.py` & `lightdash_client_python-0.613.2/lightdash_client/models/update_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/updated_by_user.py` & `lightdash_client_python-0.613.2/lightdash_client/models/updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/user_allowed_organization.py` & `lightdash_client_python-0.613.2/lightdash_client/models/user_allowed_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/validate_project_json_body.py` & `lightdash_client_python-0.613.2/lightdash_client/models/validate_project_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/validation_error_chart_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/validation_error_chart_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         error (str):
         name (str):
         created_at (datetime.datetime):
         validation_id (float):
         chart_views (float):
         source (Union[Unset, ValidationSourceType]):
         space_uuid (Union[Unset, str]):
+        chart_name (Union[Unset, str]):
         last_updated_at (Union[Unset, datetime.datetime]):
         last_updated_by (Union[Unset, str]):
         field_name (Union[Unset, str]):
         chart_type (Union[Unset, ChartKind]):
         chart_uuid (Union[Unset, str]):
     """
 
@@ -43,14 +44,15 @@
     error: str
     name: str
     created_at: datetime.datetime
     validation_id: float
     chart_views: float
     source: Union[Unset, ValidationSourceType] = UNSET
     space_uuid: Union[Unset, str] = UNSET
+    chart_name: Union[Unset, str] = UNSET
     last_updated_at: Union[Unset, datetime.datetime] = UNSET
     last_updated_by: Union[Unset, str] = UNSET
     field_name: Union[Unset, str] = UNSET
     chart_type: Union[Unset, ChartKind] = UNSET
     chart_uuid: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -65,14 +67,15 @@
         validation_id = self.validation_id
         chart_views = self.chart_views
         source: Union[Unset, str] = UNSET
         if not isinstance(self.source, Unset):
             source = self.source.value
 
         space_uuid = self.space_uuid
+        chart_name = self.chart_name
         last_updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.last_updated_at, Unset):
             last_updated_at = self.last_updated_at.isoformat()
 
         last_updated_by = self.last_updated_by
         field_name = self.field_name
         chart_type: Union[Unset, str] = UNSET
@@ -94,14 +97,16 @@
                 "chartViews": chart_views,
             }
         )
         if source is not UNSET:
             field_dict["source"] = source
         if space_uuid is not UNSET:
             field_dict["spaceUuid"] = space_uuid
+        if chart_name is not UNSET:
+            field_dict["chartName"] = chart_name
         if last_updated_at is not UNSET:
             field_dict["lastUpdatedAt"] = last_updated_at
         if last_updated_by is not UNSET:
             field_dict["lastUpdatedBy"] = last_updated_by
         if field_name is not UNSET:
             field_dict["fieldName"] = field_name
         if chart_type is not UNSET:
@@ -133,14 +138,16 @@
         if isinstance(_source, Unset):
             source = UNSET
         else:
             source = ValidationSourceType(_source)
 
         space_uuid = d.pop("spaceUuid", UNSET)
 
+        chart_name = d.pop("chartName", UNSET)
+
         _last_updated_at = d.pop("lastUpdatedAt", UNSET)
         last_updated_at: Union[Unset, datetime.datetime]
         if isinstance(_last_updated_at, Unset):
             last_updated_at = UNSET
         else:
             last_updated_at = isoparse(_last_updated_at)
 
@@ -163,14 +170,15 @@
             error=error,
             name=name,
             created_at=created_at,
             validation_id=validation_id,
             chart_views=chart_views,
             source=source,
             space_uuid=space_uuid,
+            chart_name=chart_name,
             last_updated_at=last_updated_at,
             last_updated_by=last_updated_by,
             field_name=field_name,
             chart_type=chart_type,
             chart_uuid=chart_uuid,
         )
```

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/validation_error_dashboard_response.py` & `lightdash_client_python-0.613.2/lightdash_client/models/validation_error_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/validation_response_base.py` & `lightdash_client_python-0.613.2/lightdash_client/models/validation_response_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/models/view_statistics.py` & `lightdash_client_python-0.613.2/lightdash_client/models/view_statistics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/lightdash_client/types.py` & `lightdash_client_python-0.613.2/lightdash_client/types.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/pyproject.toml` & `lightdash_client_python-0.613.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/setup.py` & `lightdash_client_python-0.613.2/setup.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/tests/__init__.py` & `lightdash_client_python-0.613.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/tests/test_dummy.py` & `lightdash_client_python-0.613.2/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.611.0/PKG-INFO` & `lightdash_client_python-0.613.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-client-python
-Version: 0.611.0
+Version: 0.613.2
 Summary: A client library for accessing Lightdash API 
 Author: yu-iskw
 Requires-Python: >=3.8.0,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

