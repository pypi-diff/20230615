# Comparing `tmp/kiln_connect-1.0.0.dev6.tar.gz` & `tmp/kiln_connect-1.0.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiln_connect-1.0.0.dev6.tar", max compression
+gzip compressed data, was "kiln_connect-1.0.0.dev7.tar", max compression
```

## Comparing `kiln_connect-1.0.0.dev6.tar` & `kiln_connect-1.0.0.dev7.tar`

### file list

```diff
@@ -1,256 +1,360 @@
--rw-r--r--   0        0        0     5728 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev6/docs/README.md
--rw-r--r--   0        0        0        0 2023-02-14 16:33:38.709950 kiln_connect-1.0.0.dev6/kiln_cli/__init__.py
--rw-r--r--   0        0        0     4536 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev6/kiln_cli/accounts.py
--rw-r--r--   0        0        0     2472 2023-04-24 06:41:57.416792 kiln_connect-1.0.0.dev6/kiln_cli/atom.py
--rw-r--r--   0        0        0     6670 2023-04-06 15:53:36.351598 kiln_connect-1.0.0.dev6/kiln_cli/eth.py
--rw-r--r--   0        0        0      410 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_cli/main.py
--rwxr-xr-x   0        0        0    10741 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_cli/sol.py
--rw-r--r--   0        0        0    10177 2023-04-24 06:41:57.416792 kiln_connect-1.0.0.dev6/kiln_cli/xtz.py
--rw-r--r--   0        0        0      155 2023-03-03 17:16:30.658551 kiln_connect-1.0.0.dev6/kiln_connect/__init__.py
--rw-r--r--   0        0        0      535 2023-03-08 16:23:14.337182 kiln_connect-1.0.0.dev6/kiln_connect/accounts.py
--rw-r--r--   0        0        0      641 2023-04-24 06:41:57.416792 kiln_connect-1.0.0.dev6/kiln_connect/atom.py
--rw-r--r--   0        0        0      942 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev6/kiln_connect/errors.py
--rw-r--r--   0        0        0     4144 2023-04-14 03:37:21.881892 kiln_connect-1.0.0.dev6/kiln_connect/eth.py
--rw-r--r--   0        0        0     5301 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/integrations.py
--rw-r--r--   0        0        0     3649 2023-04-17 13:51:44.551380 kiln_connect-1.0.0.dev6/kiln_connect/kiln_connect.py
--rw-r--r--   0        0        0    12202 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/__init__.py
--rw-r--r--   0        0        0      394 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    32819 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/accounts_api.py
--rw-r--r--   0        0        0    21212 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/atom_api.py
--rw-r--r--   0        0        0    84284 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/eth_api.py
--rw-r--r--   0        0        0   104060 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/sol_api.py
--rw-r--r--   0        0        0    66804 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/xtz_api.py
--rw-r--r--   0        0        0    30218 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api_client.py
--rw-r--r--   0        0        0    17494 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/configuration.py
--rw-r--r--   0        0        0     5713 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/exceptions.py
--rw-r--r--   0        0        0    11300 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/__init__.py
--rw-r--r--   0        0        0     3006 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account.py
--rw-r--r--   0        0        0     2782 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_payload.py
--rw-r--r--   0        0        0     4028 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio.py
--rw-r--r--   0        0        0     4878 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py
--rw-r--r--   0        0        0     3019 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py
--rw-r--r--   0        0        0     3016 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py
--rw-r--r--   0        0        0     3478 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/atom_reward.py
--rw-r--r--   0        0        0     4849 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/atom_stake.py
--rw-r--r--   0        0        0     3245 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/core_stake.py
--rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2639 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_broadcasted_tx.py
--rw-r--r--   0        0        0     3090 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2910 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_kiln_stats.py
--rw-r--r--   0        0        0     2971 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py
--rw-r--r--   0        0        0     3028 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_network_stats.py
--rw-r--r--   0        0        0     3485 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py
--rw-r--r--   0        0        0     4582 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_deposit.py
--rw-r--r--   0        0        0     3820 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_execution_reward.py
--rw-r--r--   0        0        0     3522 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py
--rw-r--r--   0        0        0     4456 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py
--rw-r--r--   0        0        0     3376 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_payload.py
--rw-r--r--   0        0        0     3042 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py
--rw-r--r--   0        0        0     3846 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_reward.py
--rw-r--r--   0        0        0     2662 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_signed_tx.py
--rw-r--r--   0        0        0     7278 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_stake.py
--rw-r--r--   0        0        0     4514 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_unsigned_tx.py
--rw-r--r--   0        0        0     3024 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status.py
--rw-r--r--   0        0        0     5288 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status_receipt.py
--rw-r--r--   0        0        0     3681 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py
--rw-r--r--   0        0        0     2972 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_account_portfolio200_response.py
--rw-r--r--   0        0        0     3064 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_accounts200_response.py
--rw-r--r--   0        0        0     3098 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_atom_rewards200_response.py
--rw-r--r--   0        0        0     3087 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_atom_stakes200_response.py
--rw-r--r--   0        0        0     2929 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py
--rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py
--rw-r--r--   0        0        0     3220 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_operations200_response.py
--rw-r--r--   0        0        0     7941 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py
--rw-r--r--   0        0        0     3087 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_rewards200_response.py
--rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_stakes200_response.py
--rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py
--rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py
--rw-r--r--   0        0        0     3220 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_operations200_response.py
--rw-r--r--   0        0        0    13955 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_operations200_response_data_inner.py
--rw-r--r--   0        0        0     3187 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_rewards200_response.py
--rw-r--r--   0        0        0     5115 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_stakes200_response.py
--rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py
--rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py
--rw-r--r--   0        0        0     3220 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_operations200_response.py
--rw-r--r--   0        0        0     8863 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_operations200_response_data_inner.py
--rw-r--r--   0        0        0     3187 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py
--rw-r--r--   0        0        0     5085 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py
--rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py
--rw-r--r--   0        0        0     2879 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_account201_response.py
--rw-r--r--   0        0        0     2966 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2959 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_keys201_response.py
--rw-r--r--   0        0        0     5501 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py
--rw-r--r--   0        0        0     2932 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py
--rw-r--r--   0        0        0     2926 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py
--rw-r--r--   0        0        0     2958 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2940 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py
--rw-r--r--   0        0        0     2914 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py
--rw-r--r--   0        0        0     2902 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_stakes201_response.py
--rw-r--r--   0        0        0     2966 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2932 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py
--rw-r--r--   0        0        0     2926 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py
--rw-r--r--   0        0        0     2572 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_broadcast_tx.py
--rw-r--r--   0        0        0     2607 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2816 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py
--rw-r--r--   0        0        0     3015 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py
--rw-r--r--   0        0        0     3025 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_network_stats.py
--rw-r--r--   0        0        0     4048 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_create_account.py
--rw-r--r--   0        0        0     4104 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_create_account_with_seed.py
--rw-r--r--   0        0        0     3866 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_deactivate.py
--rw-r--r--   0        0        0     4037 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_delegate.py
--rw-r--r--   0        0        0     4064 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_merge.py
--rw-r--r--   0        0        0     4244 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_redelegate.py
--rw-r--r--   0        0        0     4313 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_split.py
--rw-r--r--   0        0        0     4218 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_withdraw.py
--rw-r--r--   0        0        0     3299 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_post_stakes_payload.py
--rw-r--r--   0        0        0     3072 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py
--rw-r--r--   0        0        0     2765 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py
--rw-r--r--   0        0        0     2617 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_prepared_tx.py
--rw-r--r--   0        0        0     3142 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_reward_by_day.py
--rw-r--r--   0        0        0     3317 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_reward_by_epoch.py
--rw-r--r--   0        0        0     3070 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py
--rw-r--r--   0        0        0     4916 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake.py
--rw-r--r--   0        0        0     2734 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake_tx.py
--rw-r--r--   0        0        0     3095 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake_tx_payload.py
--rw-r--r--   0        0        0     2996 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py
--rw-r--r--   0        0        0     2705 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/soltx_status.py
--rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2639 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py
--rw-r--r--   0        0        0     2984 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2664 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py
--rw-r--r--   0        0        0     3294 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_cycle_reward.py
--rw-r--r--   0        0        0     3130 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_daily_reward.py
--rw-r--r--   0        0        0     3522 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_network_stats.py
--rw-r--r--   0        0        0     3415 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_activation.py
--rw-r--r--   0        0        0     4022 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_delegate.py
--rw-r--r--   0        0        0     4212 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_payment.py
--rw-r--r--   0        0        0     3903 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_undelegate.py
--rw-r--r--   0        0        0     2832 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py
--rw-r--r--   0        0        0     2662 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_signed_tx.py
--rw-r--r--   0        0        0     5809 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_stake.py
--rw-r--r--   0        0        0     2871 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_unsigned_tx.py
--rw-r--r--   0        0        0     3024 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtztx_status.py
--rw-r--r--   0        0        0     3193 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtztx_status_receipt.py
--rw-r--r--   0        0        0    13289 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/rest.py
--rw-r--r--   0        0        0        0 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/__init__.py
--rw-r--r--   0        0        0     2257 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account.py
--rw-r--r--   0        0        0     2283 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_payload.py
--rw-r--r--   0        0        0     3364 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio.py
--rw-r--r--   0        0        0     3074 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py
--rw-r--r--   0        0        0     2552 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py
--rw-r--r--   0        0        0     2552 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py
--rw-r--r--   0        0        0     2053 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_accounts_api.py
--rw-r--r--   0        0        0     1632 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_api.py
--rw-r--r--   0        0        0     2284 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_reward.py
--rw-r--r--   0        0        0     2624 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_stake.py
--rw-r--r--   0        0        0     2719 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_core_stake.py
--rw-r--r--   0        0        0     2949 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_api.py
--rw-r--r--   0        0        0     2414 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2252 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py
--rw-r--r--   0        0        0     2620 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2337 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_kiln_stats.py
--rw-r--r--   0        0        0     2310 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py
--rw-r--r--   0        0        0     2273 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_network_stats.py
--rw-r--r--   0        0        0     2735 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py
--rw-r--r--   0        0        0     3049 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_deposit.py
--rw-r--r--   0        0        0     2791 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py
--rw-r--r--   0        0        0     2875 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py
--rw-r--r--   0        0        0     3182 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py
--rw-r--r--   0        0        0     2587 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py
--rw-r--r--   0        0        0     2809 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py
--rw-r--r--   0        0        0     2432 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_reward.py
--rw-r--r--   0        0        0     2201 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_signed_tx.py
--rw-r--r--   0        0        0     3015 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_stake.py
--rw-r--r--   0        0        0     4064 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py
--rw-r--r--   0        0        0     3737 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status.py
--rw-r--r--   0        0        0     3576 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py
--rw-r--r--   0        0        0     2650 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py
--rw-r--r--   0        0        0     3709 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py
--rw-r--r--   0        0        0     2595 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_accounts200_response.py
--rw-r--r--   0        0        0     2625 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_atom_rewards200_response.py
--rw-r--r--   0        0        0     3007 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_atom_stakes200_response.py
--rw-r--r--   0        0        0     2615 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py
--rw-r--r--   0        0        0     2553 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py
--rw-r--r--   0        0        0     2363 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py
--rw-r--r--   0        0        0     3451 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py
--rw-r--r--   0        0        0     2803 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py
--rw-r--r--   0        0        0     3444 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py
--rw-r--r--   0        0        0     4114 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py
--rw-r--r--   0        0        0     2550 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py
--rw-r--r--   0        0        0     2363 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_operations200_response.py
--rw-r--r--   0        0        0     3163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_operations200_response_data_inner.py
--rw-r--r--   0        0        0     2327 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py
--rw-r--r--   0        0        0     2706 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3093 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py
--rw-r--r--   0        0        0     2480 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py
--rw-r--r--   0        0        0     2650 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py
--rw-r--r--   0        0        0     2363 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_operations200_response.py
--rw-r--r--   0        0        0     2967 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_operations200_response_data_inner.py
--rw-r--r--   0        0        0     2327 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py
--rw-r--r--   0        0        0     2779 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3071 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py
--rw-r--r--   0        0        0     2877 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py
--rw-r--r--   0        0        0     2535 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_account201_response.py
--rw-r--r--   0        0        0     2514 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2259 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py
--rw-r--r--   0        0        0     2899 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py
--rw-r--r--   0        0        0     2489 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py
--rw-r--r--   0        0        0     4344 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py
--rw-r--r--   0        0        0     2444 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2431 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py
--rw-r--r--   0        0        0     2447 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py
--rw-r--r--   0        0        0     2746 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py
--rw-r--r--   0        0        0     2499 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2489 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py
--rw-r--r--   0        0        0     2581 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py
--rw-r--r--   0        0        0     3493 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_api.py
--rw-r--r--   0        0        0     2162 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py
--rw-r--r--   0        0        0     2290 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2599 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py
--rw-r--r--   0        0        0     2750 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py
--rw-r--r--   0        0        0     2270 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_network_stats.py
--rw-r--r--   0        0        0     2792 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_create_account.py
--rw-r--r--   0        0        0     2873 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_create_account_with_seed.py
--rw-r--r--   0        0        0     2687 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_deactivate.py
--rw-r--r--   0        0        0     2741 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_delegate.py
--rw-r--r--   0        0        0     2644 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_merge.py
--rw-r--r--   0        0        0     2786 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_redelegate.py
--rw-r--r--   0        0        0     2740 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_split.py
--rw-r--r--   0        0        0     2788 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_withdraw.py
--rw-r--r--   0        0        0     2953 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py
--rw-r--r--   0        0        0     2451 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py
--rw-r--r--   0        0        0     2439 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py
--rw-r--r--   0        0        0     2163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_prepared_tx.py
--rw-r--r--   0        0        0     2363 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_reward_by_day.py
--rw-r--r--   0        0        0     2379 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py
--rw-r--r--   0        0        0     2773 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py
--rw-r--r--   0        0        0     2688 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake.py
--rw-r--r--   0        0        0     2169 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake_tx.py
--rw-r--r--   0        0        0     2739 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py
--rw-r--r--   0        0        0     2630 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py
--rw-r--r--   0        0        0     2163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_soltx_status.py
--rw-r--r--   0        0        0     2684 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_api.py
--rw-r--r--   0        0        0     2414 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2237 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py
--rw-r--r--   0        0        0     2646 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2388 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py
--rw-r--r--   0        0        0     2426 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py
--rw-r--r--   0        0        0     2374 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_daily_reward.py
--rw-r--r--   0        0        0     2362 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_network_stats.py
--rw-r--r--   0        0        0     2494 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_activation.py
--rw-r--r--   0        0        0     2668 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_delegate.py
--rw-r--r--   0        0        0     2727 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_payment.py
--rw-r--r--   0        0        0     2658 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_undelegate.py
--rw-r--r--   0        0        0     2601 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py
--rw-r--r--   0        0        0     2201 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_signed_tx.py
--rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_stake.py
--rw-r--r--   0        0        0     2333 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py
--rw-r--r--   0        0        0     2580 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtztx_status.py
--rw-r--r--   0        0        0     2502 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py
--rw-r--r--   0        0        0     6471 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/sol.py
--rw-r--r--   0        0        0      451 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/utils.py
--rw-r--r--   0        0        0     4442 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev6/kiln_connect/xtz.py
--rw-r--r--   0        0        0     1011 2023-04-24 06:43:22.622507 kiln_connect-1.0.0.dev6/pyproject.toml
--rw-r--r--   0        0        0     6658 1970-01-01 00:00:00.000000 kiln_connect-1.0.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0     5728 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev7/docs/README.md
+-rw-r--r--   0        0        0        0 2023-02-14 16:33:38.709950 kiln_connect-1.0.0.dev7/kiln_cli/__init__.py
+-rw-r--r--   0        0        0     4536 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev7/kiln_cli/accounts.py
+-rw-r--r--   0        0        0     2472 2023-06-15 12:34:11.217420 kiln_connect-1.0.0.dev7/kiln_cli/atom.py
+-rw-r--r--   0        0        0     6670 2023-06-15 12:33:20.467919 kiln_connect-1.0.0.dev7/kiln_cli/eth.py
+-rw-r--r--   0        0        0      462 2023-06-15 12:53:47.129328 kiln_connect-1.0.0.dev7/kiln_cli/main.py
+-rw-r--r--   0        0        0     4167 2023-06-15 12:53:47.129328 kiln_connect-1.0.0.dev7/kiln_cli/matic.py
+-rwxr-xr-x   0        0        0    10741 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev7/kiln_cli/sol.py
+-rw-r--r--   0        0        0    10178 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_cli/xtz.py
+-rw-r--r--   0        0        0      155 2023-03-03 17:16:30.658551 kiln_connect-1.0.0.dev7/kiln_connect/__init__.py
+-rw-r--r--   0        0        0      535 2023-03-08 16:23:14.337182 kiln_connect-1.0.0.dev7/kiln_connect/accounts.py
+-rw-r--r--   0        0        0      641 2023-06-15 12:34:11.220754 kiln_connect-1.0.0.dev7/kiln_connect/atom.py
+-rw-r--r--   0        0        0      942 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev7/kiln_connect/errors.py
+-rw-r--r--   0        0        0     4144 2023-04-14 03:37:21.881892 kiln_connect-1.0.0.dev7/kiln_connect/eth.py
+-rw-r--r--   0        0        0     5321 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/integrations.py
+-rw-r--r--   0        0        0     3839 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/kiln_connect.py
+-rw-r--r--   0        0        0     8280 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/matic.py
+-rw-r--r--   0        0        0    17103 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/__init__.py
+-rw-r--r--   0        0        0      595 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    38723 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/accounts_api.py
+-rw-r--r--   0        0        0    42634 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/ada_api.py
+-rw-r--r--   0        0        0    75017 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/atom_api.py
+-rw-r--r--   0        0        0    97577 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/eth_api.py
+-rw-r--r--   0        0        0    65454 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/matic_api.py
+-rw-r--r--   0        0        0     7979 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/organizations_api.py
+-rw-r--r--   0        0        0   104060 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/sol_api.py
+-rw-r--r--   0        0        0    73771 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/xtz_api.py
+-rw-r--r--   0        0        0    30218 2023-06-15 12:44:20.274755 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api_client.py
+-rw-r--r--   0        0        0    17494 2023-06-15 12:44:20.274755 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/configuration.py
+-rw-r--r--   0        0        0     5713 2023-06-15 12:44:20.274755 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/exceptions.py
+-rw-r--r--   0        0        0    16000 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0     3006 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/account.py
+-rw-r--r--   0        0        0     2782 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/account_payload.py
+-rw-r--r--   0        0        0     2666 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2928 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2664 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_craft_unstake_tx_payload.py
+-rw-r--r--   0        0        0     3037 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_craft_withdraw_rewards_tx_payload.py
+-rw-r--r--   0        0        0     3504 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2944 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_prepare_tx_payload_signed_messages_inner.py
+-rw-r--r--   0        0        0     2662 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_signed_tx.py
+-rw-r--r--   0        0        0     3047 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_unsigned_tx.py
+-rw-r--r--   0        0        0     2590 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/adatx_hash.py
+-rw-r--r--   0        0        0     2861 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/adatx_status.py
+-rw-r--r--   0        0        0     2680 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     3122 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     3029 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_craft_unstake_tx_payload.py
+-rw-r--r--   0        0        0     2895 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_craft_withdraw_rewards_tx_payload.py
+-rw-r--r--   0        0        0     3391 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_network_stats.py
+-rw-r--r--   0        0        0     3131 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_prepare_tx_payload.py
+-rw-r--r--   0        0        0     3478 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_reward.py
+-rw-r--r--   0        0        0     2676 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_signed_tx.py
+-rw-r--r--   0        0        0     4849 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_stake.py
+-rw-r--r--   0        0        0     3486 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_unsigned_tx.py
+-rw-r--r--   0        0        0     2597 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atomtx_hash.py
+-rw-r--r--   0        0        0     2947 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atomtx_status.py
+-rw-r--r--   0        0        0     3245 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/core_stake.py
+-rw-r--r--   0        0        0     2666 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2639 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_broadcasted_tx.py
+-rw-r--r--   0        0        0     3090 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     3360 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_exit_message.py
+-rw-r--r--   0        0        0     2910 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_kiln_stats.py
+-rw-r--r--   0        0        0     2971 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py
+-rw-r--r--   0        0        0     3860 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_network_stats.py
+-rw-r--r--   0        0        0     3691 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py
+-rw-r--r--   0        0        0     4795 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_operation_deposit.py
+-rw-r--r--   0        0        0     4026 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_operation_execution_reward.py
+-rw-r--r--   0        0        0     3522 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py
+-rw-r--r--   0        0        0     4456 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py
+-rw-r--r--   0        0        0     3376 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_post_keys_payload.py
+-rw-r--r--   0        0        0     3042 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py
+-rw-r--r--   0        0        0     3846 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_reward.py
+-rw-r--r--   0        0        0     2662 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_signed_tx.py
+-rw-r--r--   0        0        0     8128 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_stake.py
+-rw-r--r--   0        0        0     4514 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_unsigned_tx.py
+-rw-r--r--   0        0        0     2902 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ethtx_status.py
+-rw-r--r--   0        0        0     2943 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_account_portfolio200_response.py
+-rw-r--r--   0        0        0     3064 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_accounts200_response.py
+-rw-r--r--   0        0        0     2917 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_ada_tx_status200_response.py
+-rw-r--r--   0        0        0     2973 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_atom_network_stats200_response.py
+-rw-r--r--   0        0        0     3098 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_atom_rewards200_response.py
+-rw-r--r--   0        0        0     3087 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_atom_stakes200_response.py
+-rw-r--r--   0        0        0     2928 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_atom_tx_status200_response.py
+-rw-r--r--   0        0        0     2929 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py
+-rw-r--r--   0        0        0     2962 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py
+-rw-r--r--   0        0        0     3220 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_operations200_response.py
+-rw-r--r--   0        0        0     5653 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     3087 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_rewards200_response.py
+-rw-r--r--   0        0        0     3076 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_stakes200_response.py
+-rw-r--r--   0        0        0     2917 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py
+-rw-r--r--   0        0        0     3115 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_exit_message200_response.py
+-rw-r--r--   0        0        0     2939 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_matic_tx_status200_response.py
+-rw-r--r--   0        0        0     2962 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py
+-rw-r--r--   0        0        0     3220 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_operations200_response.py
+-rw-r--r--   0        0        0     9508 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     3187 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_rewards200_response.py
+-rw-r--r--   0        0        0     4493 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3076 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_stakes200_response.py
+-rw-r--r--   0        0        0     2917 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py
+-rw-r--r--   0        0        0     2962 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py
+-rw-r--r--   0        0        0     3220 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_operations200_response.py
+-rw-r--r--   0        0        0     6256 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     3187 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py
+-rw-r--r--   0        0        0     4467 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3076 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py
+-rw-r--r--   0        0        0     2917 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py
+-rw-r--r--   0        0        0     2680 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2653 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_broadcasted_tx.py
+-rw-r--r--   0        0        0     3059 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_craft_approve_tx_payload.py
+-rw-r--r--   0        0        0     3223 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_craft_buy_voucher_tx_payload.py
+-rw-r--r--   0        0        0     2955 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_craft_restake_rewards_tx_payload.py
+-rw-r--r--   0        0        0     3082 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_craft_sell_voucher_tx_payload.py
+-rw-r--r--   0        0        0     2983 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_craft_unstake_claim_tokens_tx_payload.py
+-rw-r--r--   0        0        0     2962 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_craft_withdraw_rewards_tx_payload.py
+-rw-r--r--   0        0        0     3056 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2676 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_signed_tx.py
+-rw-r--r--   0        0        0     2885 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_unsigned_tx.py
+-rw-r--r--   0        0        0     2916 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matictx_status.py
+-rw-r--r--   0        0        0     3950 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/portfolio.py
+-rw-r--r--   0        0        0     4771 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/portfolio_protocols_inner.py
+-rw-r--r--   0        0        0     2970 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/portfolio_protocols_inner_total_balance.py
+-rw-r--r--   0        0        0     2967 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/portfolio_protocols_inner_total_rewards.py
+-rw-r--r--   0        0        0     2879 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_account201_response.py
+-rw-r--r--   0        0        0     2937 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_ada_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2932 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_ada_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2926 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_ada_stake_tx201_response.py
+-rw-r--r--   0        0        0     2948 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_atom_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2943 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_atom_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2937 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_atom_stake_tx201_response.py
+-rw-r--r--   0        0        0     3310 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_atom_stakes_payload.py
+-rw-r--r--   0        0        0     2931 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_atom_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     2966 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2959 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_keys201_response.py
+-rw-r--r--   0        0        0     4787 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py
+-rw-r--r--   0        0        0     2932 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2926 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py
+-rw-r--r--   0        0        0     2902 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_stakes201_response.py
+-rw-r--r--   0        0        0     3299 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_stakes_payload.py
+-rw-r--r--   0        0        0     2745 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     2962 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_matic_approve_tx201_response.py
+-rw-r--r--   0        0        0     2988 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_matic_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2954 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_matic_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2958 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2940 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2914 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py
+-rw-r--r--   0        0        0     2966 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2932 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2926 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py
+-rw-r--r--   0        0        0     2625 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_broadcast_tx.py
+-rw-r--r--   0        0        0     2667 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2816 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py
+-rw-r--r--   0        0        0     3015 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py
+-rw-r--r--   0        0        0     3025 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_network_stats.py
+-rw-r--r--   0        0        0     4048 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_create_account.py
+-rw-r--r--   0        0        0     4104 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_create_account_with_seed.py
+-rw-r--r--   0        0        0     3866 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_deactivate.py
+-rw-r--r--   0        0        0     4037 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_delegate.py
+-rw-r--r--   0        0        0     4064 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_merge.py
+-rw-r--r--   0        0        0     4244 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_redelegate.py
+-rw-r--r--   0        0        0     4313 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_split.py
+-rw-r--r--   0        0        0     4218 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_withdraw.py
+-rw-r--r--   0        0        0     3299 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_post_stakes_payload.py
+-rw-r--r--   0        0        0     3072 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     2872 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2677 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_prepared_tx.py
+-rw-r--r--   0        0        0     3142 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_reward_by_day.py
+-rw-r--r--   0        0        0     3317 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_reward_by_epoch.py
+-rw-r--r--   0        0        0     3070 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py
+-rw-r--r--   0        0        0     4916 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_stake.py
+-rw-r--r--   0        0        0     3228 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_stake_tx.py
+-rw-r--r--   0        0        0     3278 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_stake_tx_payload.py
+-rw-r--r--   0        0        0     2996 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py
+-rw-r--r--   0        0        0     2922 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/soltx_status.py
+-rw-r--r--   0        0        0     2666 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2639 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py
+-rw-r--r--   0        0        0     2959 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2664 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py
+-rw-r--r--   0        0        0     3294 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_cycle_reward.py
+-rw-r--r--   0        0        0     3130 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_daily_reward.py
+-rw-r--r--   0        0        0     3522 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_network_stats.py
+-rw-r--r--   0        0        0     3415 2023-06-15 12:44:20.268088 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_operation_activation.py
+-rw-r--r--   0        0        0     4022 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_operation_delegate.py
+-rw-r--r--   0        0        0     4212 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_operation_payment.py
+-rw-r--r--   0        0        0     3903 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_operation_undelegate.py
+-rw-r--r--   0        0        0     2832 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2662 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_signed_tx.py
+-rw-r--r--   0        0        0     5809 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_stake.py
+-rw-r--r--   0        0        0     3172 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_unsigned_tx.py
+-rw-r--r--   0        0        0     2870 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtztx_status.py
+-rw-r--r--   0        0        0    13289 2023-06-15 12:44:20.274755 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/rest.py
+-rw-r--r--   0        0        0        0 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/__init__.py
+-rw-r--r--   0        0        0     2257 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_account.py
+-rw-r--r--   0        0        0     2283 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_account_payload.py
+-rw-r--r--   0        0        0     2185 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_accounts_api.py
+-rw-r--r--   0        0        0     2303 2023-06-15 12:53:47.132661 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_api.py
+-rw-r--r--   0        0        0     5550 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2808 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2520 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_craft_unstake_tx_payload.py
+-rw-r--r--   0        0        0     2664 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_craft_withdraw_rewards_tx_payload.py
+-rw-r--r--   0        0        0     6109 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2490 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_prepare_tx_payload_signed_messages_inner.py
+-rw-r--r--   0        0        0     2591 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_signed_tx.py
+-rw-r--r--   0        0        0     2846 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_unsigned_tx.py
+-rw-r--r--   0        0        0     2164 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_adatx_hash.py
+-rw-r--r--   0        0        0     2755 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_adatx_status.py
+-rw-r--r--   0        0        0     2886 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_api.py
+-rw-r--r--   0        0        0     3642 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2863 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2688 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_craft_unstake_tx_payload.py
+-rw-r--r--   0        0        0     2725 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_craft_withdraw_rewards_tx_payload.py
+-rw-r--r--   0        0        0     2377 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_network_stats.py
+-rw-r--r--   0        0        0     4105 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2284 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_reward.py
+-rw-r--r--   0        0        0     2821 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_signed_tx.py
+-rw-r--r--   0        0        0     2624 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_stake.py
+-rw-r--r--   0        0        0     3387 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_unsigned_tx.py
+-rw-r--r--   0        0        0     2176 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atomtx_hash.py
+-rw-r--r--   0        0        0     9562 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atomtx_status.py
+-rw-r--r--   0        0        0     2719 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_core_stake.py
+-rw-r--r--   0        0        0     3231 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_api.py
+-rw-r--r--   0        0        0     2414 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2252 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py
+-rw-r--r--   0        0        0     2620 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     3088 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_exit_message.py
+-rw-r--r--   0        0        0     2337 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_kiln_stats.py
+-rw-r--r--   0        0        0     2310 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py
+-rw-r--r--   0        0        0     2445 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_network_stats.py
+-rw-r--r--   0        0        0     2773 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py
+-rw-r--r--   0        0        0     3087 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_operation_deposit.py
+-rw-r--r--   0        0        0     2829 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py
+-rw-r--r--   0        0        0     2875 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py
+-rw-r--r--   0        0        0     3182 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py
+-rw-r--r--   0        0        0     2587 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py
+-rw-r--r--   0        0        0     2809 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2432 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_reward.py
+-rw-r--r--   0        0        0     2201 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_signed_tx.py
+-rw-r--r--   0        0        0     3142 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_stake.py
+-rw-r--r--   0        0        0     4064 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py
+-rw-r--r--   0        0        0     5562 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ethtx_status.py
+-rw-r--r--   0        0        0     3649 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py
+-rw-r--r--   0        0        0     2595 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_accounts200_response.py
+-rw-r--r--   0        0        0     3024 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_ada_tx_status200_response.py
+-rw-r--r--   0        0        0     2667 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_atom_network_stats200_response.py
+-rw-r--r--   0        0        0     2625 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_atom_rewards200_response.py
+-rw-r--r--   0        0        0     3007 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_atom_stakes200_response.py
+-rw-r--r--   0        0        0     9833 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_atom_tx_status200_response.py
+-rw-r--r--   0        0        0     2615 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py
+-rw-r--r--   0        0        0     2737 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py
+-rw-r--r--   0        0        0     2363 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py
+-rw-r--r--   0        0        0     3489 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     2803 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py
+-rw-r--r--   0        0        0     3595 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py
+-rw-r--r--   0        0        0     5831 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py
+-rw-r--r--   0        0        0     3392 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_exit_message200_response.py
+-rw-r--r--   0        0        0     5859 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_matic_tx_status200_response.py
+-rw-r--r--   0        0        0     2550 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py
+-rw-r--r--   0        0        0     2363 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_operations200_response.py
+-rw-r--r--   0        0        0     3163 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     2327 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py
+-rw-r--r--   0        0        0     2706 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3093 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py
+-rw-r--r--   0        0        0     4900 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py
+-rw-r--r--   0        0        0     2650 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py
+-rw-r--r--   0        0        0     2363 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_operations200_response.py
+-rw-r--r--   0        0        0     2967 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     2327 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py
+-rw-r--r--   0        0        0     2779 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3071 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py
+-rw-r--r--   0        0        0     7615 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py
+-rw-r--r--   0        0        0     2909 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_api.py
+-rw-r--r--   0        0        0     2438 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2276 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_broadcasted_tx.py
+-rw-r--r--   0        0        0     2623 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_craft_approve_tx_payload.py
+-rw-r--r--   0        0        0     2895 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_craft_buy_voucher_tx_payload.py
+-rw-r--r--   0        0        0     2697 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_craft_restake_rewards_tx_payload.py
+-rw-r--r--   0        0        0     2768 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_craft_sell_voucher_tx_payload.py
+-rw-r--r--   0        0        0     2747 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_craft_unstake_claim_tokens_tx_payload.py
+-rw-r--r--   0        0        0     2709 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_craft_withdraw_rewards_tx_payload.py
+-rw-r--r--   0        0        0     2833 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2225 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_signed_tx.py
+-rw-r--r--   0        0        0     2357 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_unsigned_tx.py
+-rw-r--r--   0        0        0     5586 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matictx_status.py
+-rw-r--r--   0        0        0     1588 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_organizations_api.py
+-rw-r--r--   0        0        0     3233 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_portfolio.py
+-rw-r--r--   0        0        0     2958 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_portfolio_protocols_inner.py
+-rw-r--r--   0        0        0     2466 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_portfolio_protocols_inner_total_balance.py
+-rw-r--r--   0        0        0     2466 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_portfolio_protocols_inner_total_rewards.py
+-rw-r--r--   0        0        0     2535 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_account201_response.py
+-rw-r--r--   0        0        0     2497 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_ada_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2879 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_ada_prepare_tx201_response.py
+-rw-r--r--   0        0        0     3098 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_ada_stake_tx201_response.py
+-rw-r--r--   0        0        0     2511 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_atom_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     3111 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_atom_prepare_tx201_response.py
+-rw-r--r--   0        0        0     3653 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_atom_stake_tx201_response.py
+-rw-r--r--   0        0        0     3081 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_atom_stakes_payload.py
+-rw-r--r--   0        0        0     2519 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_atom_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     2514 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2259 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py
+-rw-r--r--   0        0        0     2899 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py
+-rw-r--r--   0        0        0     2489 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py
+-rw-r--r--   0        0        0     4344 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py
+-rw-r--r--   0        0        0     2746 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_stakes201_response.py
+-rw-r--r--   0        0        0     2979 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_stakes_payload.py
+-rw-r--r--   0        0        0     2472 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     2633 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_matic_approve_tx201_response.py
+-rw-r--r--   0        0        0     2542 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_matic_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2517 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_matic_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2531 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     4061 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py
+-rw-r--r--   0        0        0     6566 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py
+-rw-r--r--   0        0        0     2499 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2489 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2995 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py
+-rw-r--r--   0        0        0     3493 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_api.py
+-rw-r--r--   0        0        0     2249 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py
+-rw-r--r--   0        0        0     5550 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2599 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py
+-rw-r--r--   0        0        0     2750 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py
+-rw-r--r--   0        0        0     2270 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_network_stats.py
+-rw-r--r--   0        0        0     2792 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_create_account.py
+-rw-r--r--   0        0        0     2873 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_create_account_with_seed.py
+-rw-r--r--   0        0        0     2687 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_deactivate.py
+-rw-r--r--   0        0        0     2741 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_delegate.py
+-rw-r--r--   0        0        0     2644 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_merge.py
+-rw-r--r--   0        0        0     2786 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_redelegate.py
+-rw-r--r--   0        0        0     2740 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_split.py
+-rw-r--r--   0        0        0     2788 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_withdraw.py
+-rw-r--r--   0        0        0     2953 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py
+-rw-r--r--   0        0        0     2451 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     5829 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py
+-rw-r--r--   0        0        0     3793 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_prepared_tx.py
+-rw-r--r--   0        0        0     2363 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_reward_by_day.py
+-rw-r--r--   0        0        0     2379 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py
+-rw-r--r--   0        0        0     2773 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py
+-rw-r--r--   0        0        0     2688 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_stake.py
+-rw-r--r--   0        0        0     6284 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_stake_tx.py
+-rw-r--r--   0        0        0     2781 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py
+-rw-r--r--   0        0        0     2630 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py
+-rw-r--r--   0        0        0     4631 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_soltx_status.py
+-rw-r--r--   0        0        0     2824 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_api.py
+-rw-r--r--   0        0        0     2414 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2237 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py
+-rw-r--r--   0        0        0     2646 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2388 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py
+-rw-r--r--   0        0        0     2426 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py
+-rw-r--r--   0        0        0     2374 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_daily_reward.py
+-rw-r--r--   0        0        0     2362 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_network_stats.py
+-rw-r--r--   0        0        0     2494 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_operation_activation.py
+-rw-r--r--   0        0        0     2668 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_operation_delegate.py
+-rw-r--r--   0        0        0     2727 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_operation_payment.py
+-rw-r--r--   0        0        0     2658 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_operation_undelegate.py
+-rw-r--r--   0        0        0     2601 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2201 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_signed_tx.py
+-rw-r--r--   0        0        0     2666 2023-06-15 12:44:20.271421 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_stake.py
+-rw-r--r--   0        0        0     2743 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py
+-rw-r--r--   0        0        0     7346 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtztx_status.py
+-rw-r--r--   0        0        0     6471 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev7/kiln_connect/sol.py
+-rw-r--r--   0        0        0      566 2023-06-15 12:53:47.135995 kiln_connect-1.0.0.dev7/kiln_connect/utils.py
+-rw-r--r--   0        0        0     4442 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev7/kiln_connect/xtz.py
+-rw-r--r--   0        0        0     1011 2023-06-15 12:55:39.731787 kiln_connect-1.0.0.dev7/pyproject.toml
+-rw-r--r--   0        0        0     6658 1970-01-01 00:00:00.000000 kiln_connect-1.0.0.dev7/PKG-INFO
```

### Comparing `kiln_connect-1.0.0.dev6/docs/README.md` & `kiln_connect-1.0.0.dev7/docs/README.md`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_cli/accounts.py` & `kiln_connect-1.0.0.dev7/kiln_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_cli/atom.py` & `kiln_connect-1.0.0.dev7/kiln_cli/atom.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_cli/eth.py` & `kiln_connect-1.0.0.dev7/kiln_cli/eth.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_cli/sol.py` & `kiln_connect-1.0.0.dev7/kiln_cli/sol.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_cli/xtz.py` & `kiln_connect-1.0.0.dev7/kiln_cli/xtz.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -263,8 +263,8 @@
                     str(pretty_mutez_to_tez(operation.actual_instance.operation_gas_used)),
                     pretty_mutez_to_tez(operation.actual_instance.baker_fee),
                     str(operation.actual_instance.block),
                     str(pretty_mutez_to_tez(operation.actual_instance.amount)),
                     "n/a"
                 )
             
-        console.print(table)
+        console.print(table)
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/accounts.py` & `kiln_connect-1.0.0.dev7/kiln_connect/accounts.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/atom.py` & `kiln_connect-1.0.0.dev7/kiln_connect/atom.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/errors.py` & `kiln_connect-1.0.0.dev7/kiln_connect/errors.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/eth.py` & `kiln_connect-1.0.0.dev7/kiln_connect/eth.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/integrations.py` & `kiln_connect-1.0.0.dev7/kiln_connect/integrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     parameters: dict
 
 
 class Asset(str, Enum):
     eth = "eth"
     xtz = "xtz"
     sol = "sol"
+    matic = "matic"
 
 
 class FireblocksIntegration:
     """Handles the Fireblocks integration.
     """
 
     def __init__(self, config: IntegrationConfig):
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/kiln_connect.py` & `kiln_connect-1.0.0.dev7/kiln_connect/kiln_connect.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from dataclasses import dataclass
 
 from kiln_connect.openapi_client import ApiClient, Configuration
 
 from .atom import ATOM
 from .eth import ETH
+from .matic import MATIC
 from .sol import SOL
 from .xtz import XTZ
 from .accounts import Accounts
 from .errors import (
     KilnInvalidEnvError,
     KilnError  # noqa: F401
 )
@@ -40,21 +41,23 @@
         if fireblocks_api_token:
             assets = {}
 
             if env in ("devnet", "testnet"): 
                     assets = {
                         Asset.eth: "ETH_TEST3",
                         Asset.xtz: "XTZ_TEST",
-                        Asset.sol: "SOL_TEST"
+                        Asset.sol: "SOL_TEST",
+                        Asset.matic: "MATIC_POLYGON_MUMBAI"
                     }
             elif env == "mainnet":
                     assets = {
                         Asset.eth: "ETH",
                         Asset.xtz: "XTZ",
-                        Asset.sol: "SOL"
+                        Asset.sol: "SOL",
+                        Asset.matic: "MATIC"
                     }
 
             fireblocks_raw_key_path = os.getenv("FIREBLOCKS_RAW_KEY_PATH")
             fireblocks_vault_account_id = os.getenv(
                 "FIREBLOCKS_VAULT_ACCOUNT_ID")
             integration_configs.append(IntegrationConfig(
                 name="fireblocks",
@@ -105,14 +108,15 @@
 
         self._integrations = Integrations(config.integrations)
 
         self.xtz = XTZ(self._api, self._integrations)
         self.eth = ETH(self._api, self._integrations)
         self.sol = SOL(self._api, self._integrations)
         self.atom = ATOM(self._api, self._integrations)
+        self.matic = MATIC(self._api, self._integrations)
         self.accounts = Accounts(self._api, self._integrations)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/__init__.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,137 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Kiln API Docs (dev)
 
     This API provides reporting staking data on various protocols as well as network wide data, staking transaction crafting features and so on. In order to use it, you should first get an API token from your Kiln dashboard (applications section). If you don't have access to our dashboard, please get in touch at hello@kiln.fi. Once you have your API token, you can set it as a bearer token in your request headers.  ### Backward Compatibility  This is an experimental specification used for development and testing, do not rely on what is here unless you know the implications.  The official Kiln API specification following backward compatible changes can be found [here](/).  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: contact@kiln.fi
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.0"
-
-# import apis into sdk package
-from kiln_connect.openapi_client.api.accounts_api import AccountsApi
-from kiln_connect.openapi_client.api.atom_api import AtomApi
-from kiln_connect.openapi_client.api.eth_api import EthApi
-from kiln_connect.openapi_client.api.sol_api import SolApi
-from kiln_connect.openapi_client.api.xtz_api import XtzApi
-
-# import ApiClient
-from kiln_connect.openapi_client.api_client import ApiClient
-from kiln_connect.openapi_client.configuration import Configuration
-from kiln_connect.openapi_client.exceptions import OpenApiException
-from kiln_connect.openapi_client.exceptions import ApiTypeError
-from kiln_connect.openapi_client.exceptions import ApiValueError
-from kiln_connect.openapi_client.exceptions import ApiKeyError
-from kiln_connect.openapi_client.exceptions import ApiAttributeError
-from kiln_connect.openapi_client.exceptions import ApiException
-# import models into sdk package
+# import models into model package
+from kiln_connect.openapi_client.models.ada_broadcast_tx_payload import ADABroadcastTxPayload
+from kiln_connect.openapi_client.models.ada_craft_stake_tx_payload import ADACraftStakeTxPayload
+from kiln_connect.openapi_client.models.ada_craft_unstake_tx_payload import ADACraftUnstakeTxPayload
+from kiln_connect.openapi_client.models.ada_craft_withdraw_rewards_tx_payload import ADACraftWithdrawRewardsTxPayload
+from kiln_connect.openapi_client.models.ada_prepare_tx_payload import ADAPrepareTxPayload
+from kiln_connect.openapi_client.models.ada_prepare_tx_payload_signed_messages_inner import ADAPrepareTxPayloadSignedMessagesInner
+from kiln_connect.openapi_client.models.ada_signed_tx import ADASignedTx
+from kiln_connect.openapi_client.models.adatx_hash import ADATxHash
+from kiln_connect.openapi_client.models.adatx_status import ADATxStatus
+from kiln_connect.openapi_client.models.ada_unsigned_tx import ADAUnsignedTx
+from kiln_connect.openapi_client.models.atom_broadcast_tx_payload import ATOMBroadcastTxPayload
+from kiln_connect.openapi_client.models.atom_craft_stake_tx_payload import ATOMCraftStakeTxPayload
+from kiln_connect.openapi_client.models.atom_craft_unstake_tx_payload import ATOMCraftUnstakeTxPayload
+from kiln_connect.openapi_client.models.atom_craft_withdraw_rewards_tx_payload import ATOMCraftWithdrawRewardsTxPayload
+from kiln_connect.openapi_client.models.atom_network_stats import ATOMNetworkStats
+from kiln_connect.openapi_client.models.atom_prepare_tx_payload import ATOMPrepareTxPayload
 from kiln_connect.openapi_client.models.atom_reward import ATOMReward
+from kiln_connect.openapi_client.models.atom_signed_tx import ATOMSignedTx
 from kiln_connect.openapi_client.models.atom_stake import ATOMStake
+from kiln_connect.openapi_client.models.atomtx_hash import ATOMTxHash
+from kiln_connect.openapi_client.models.atomtx_status import ATOMTxStatus
+from kiln_connect.openapi_client.models.atom_unsigned_tx import ATOMUnsignedTx
 from kiln_connect.openapi_client.models.account import Account
 from kiln_connect.openapi_client.models.account_payload import AccountPayload
-from kiln_connect.openapi_client.models.account_portfolio import AccountPortfolio
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner import AccountPortfolioProtocolsInner
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance import AccountPortfolioProtocolsInnerTotalBalance
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards import AccountPortfolioProtocolsInnerTotalRewards
 from kiln_connect.openapi_client.models.core_stake import CoreStake
 from kiln_connect.openapi_client.models.eth_broadcast_tx_payload import ETHBroadcastTxPayload
 from kiln_connect.openapi_client.models.eth_broadcasted_tx import ETHBroadcastedTx
 from kiln_connect.openapi_client.models.eth_craft_stake_tx_payload import ETHCraftStakeTxPayload
+from kiln_connect.openapi_client.models.eth_exit_message import ETHExitMessage
 from kiln_connect.openapi_client.models.eth_kiln_stats import ETHKilnStats
 from kiln_connect.openapi_client.models.eth_kiln_stats_gross_apy import ETHKilnStatsGrossApy
 from kiln_connect.openapi_client.models.eth_network_stats import ETHNetworkStats
 from kiln_connect.openapi_client.models.eth_operation_consensus_withdrawal import ETHOperationConsensusWithdrawal
 from kiln_connect.openapi_client.models.eth_operation_deposit import ETHOperationDeposit
 from kiln_connect.openapi_client.models.eth_operation_execution_reward import ETHOperationExecutionReward
 from kiln_connect.openapi_client.models.eth_post_keys_batch_response import ETHPostKeysBatchResponse
 from kiln_connect.openapi_client.models.eth_post_keys_cli_response_inner import ETHPostKeysCliResponseInner
 from kiln_connect.openapi_client.models.eth_post_keys_payload import ETHPostKeysPayload
 from kiln_connect.openapi_client.models.eth_prepare_tx_payload import ETHPrepareTxPayload
 from kiln_connect.openapi_client.models.eth_reward import ETHReward
 from kiln_connect.openapi_client.models.eth_signed_tx import ETHSignedTx
 from kiln_connect.openapi_client.models.eth_stake import ETHStake
 from kiln_connect.openapi_client.models.ethtx_status import ETHTxStatus
-from kiln_connect.openapi_client.models.ethtx_status_receipt import ETHTxStatusReceipt
-from kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner import ETHTxStatusReceiptLogsInner
 from kiln_connect.openapi_client.models.eth_unsigned_tx import ETHUnsignedTx
 from kiln_connect.openapi_client.models.get_account_portfolio200_response import GetAccountPortfolio200Response
 from kiln_connect.openapi_client.models.get_accounts200_response import GetAccounts200Response
+from kiln_connect.openapi_client.models.get_ada_tx_status200_response import GetAdaTxStatus200Response
+from kiln_connect.openapi_client.models.get_atom_network_stats200_response import GetAtomNetworkStats200Response
 from kiln_connect.openapi_client.models.get_atom_rewards200_response import GetAtomRewards200Response
 from kiln_connect.openapi_client.models.get_atom_stakes200_response import GetAtomStakes200Response
+from kiln_connect.openapi_client.models.get_atom_tx_status200_response import GetAtomTxStatus200Response
 from kiln_connect.openapi_client.models.get_eth_kiln_stats200_response import GetEthKilnStats200Response
 from kiln_connect.openapi_client.models.get_eth_network_stats200_response import GetEthNetworkStats200Response
 from kiln_connect.openapi_client.models.get_eth_operations200_response import GetEthOperations200Response
 from kiln_connect.openapi_client.models.get_eth_operations200_response_data_inner import GetEthOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_eth_rewards200_response import GetEthRewards200Response
 from kiln_connect.openapi_client.models.get_eth_stakes200_response import GetEthStakes200Response
 from kiln_connect.openapi_client.models.get_eth_tx_status200_response import GetEthTxStatus200Response
+from kiln_connect.openapi_client.models.get_exit_message200_response import GetExitMessage200Response
+from kiln_connect.openapi_client.models.get_matic_tx_status200_response import GetMaticTxStatus200Response
 from kiln_connect.openapi_client.models.get_sol_network_stats200_response import GetSolNetworkStats200Response
 from kiln_connect.openapi_client.models.get_sol_operations200_response import GetSolOperations200Response
 from kiln_connect.openapi_client.models.get_sol_operations200_response_data_inner import GetSolOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response
 from kiln_connect.openapi_client.models.get_sol_rewards200_response_data_inner import GetSolRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_stakes200_response import GetSolStakes200Response
 from kiln_connect.openapi_client.models.get_sol_tx_status200_response import GetSolTxStatus200Response
 from kiln_connect.openapi_client.models.get_xtz_network_stats200_response import GetXtzNetworkStats200Response
 from kiln_connect.openapi_client.models.get_xtz_operations200_response import GetXtzOperations200Response
 from kiln_connect.openapi_client.models.get_xtz_operations200_response_data_inner import GetXtzOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response import GetXtzRewards200Response
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner import GetXtzRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_xtz_stakes200_response import GetXtzStakes200Response
 from kiln_connect.openapi_client.models.get_xtz_tx_status200_response import GetXtzTxStatus200Response
+from kiln_connect.openapi_client.models.matic_broadcast_tx_payload import MATICBroadcastTxPayload
+from kiln_connect.openapi_client.models.matic_broadcasted_tx import MATICBroadcastedTx
+from kiln_connect.openapi_client.models.matic_craft_approve_tx_payload import MATICCraftApproveTxPayload
+from kiln_connect.openapi_client.models.matic_craft_buy_voucher_tx_payload import MATICCraftBuyVoucherTxPayload
+from kiln_connect.openapi_client.models.matic_craft_restake_rewards_tx_payload import MATICCraftRestakeRewardsTxPayload
+from kiln_connect.openapi_client.models.matic_craft_sell_voucher_tx_payload import MATICCraftSellVoucherTxPayload
+from kiln_connect.openapi_client.models.matic_craft_unstake_claim_tokens_tx_payload import MATICCraftUnstakeClaimTokensTxPayload
+from kiln_connect.openapi_client.models.matic_craft_withdraw_rewards_tx_payload import MATICCraftWithdrawRewardsTxPayload
+from kiln_connect.openapi_client.models.matic_prepare_tx_payload import MATICPrepareTxPayload
+from kiln_connect.openapi_client.models.matic_signed_tx import MATICSignedTx
+from kiln_connect.openapi_client.models.matictx_status import MATICTxStatus
+from kiln_connect.openapi_client.models.matic_unsigned_tx import MATICUnsignedTx
+from kiln_connect.openapi_client.models.portfolio import Portfolio
+from kiln_connect.openapi_client.models.portfolio_protocols_inner import PortfolioProtocolsInner
+from kiln_connect.openapi_client.models.portfolio_protocols_inner_total_balance import PortfolioProtocolsInnerTotalBalance
+from kiln_connect.openapi_client.models.portfolio_protocols_inner_total_rewards import PortfolioProtocolsInnerTotalRewards
+from kiln_connect.openapi_client.models.post_atom_stakes_payload import PostATOMStakesPayload
+from kiln_connect.openapi_client.models.post_atom_stakes_payload_stakes_inner import PostATOMStakesPayloadStakesInner
 from kiln_connect.openapi_client.models.post_account201_response import PostAccount201Response
+from kiln_connect.openapi_client.models.post_ada_broadcast_tx201_response import PostAdaBroadcastTx201Response
+from kiln_connect.openapi_client.models.post_ada_prepare_tx201_response import PostAdaPrepareTx201Response
+from kiln_connect.openapi_client.models.post_ada_stake_tx201_response import PostAdaStakeTx201Response
+from kiln_connect.openapi_client.models.post_atom_broadcast_tx201_response import PostAtomBroadcastTx201Response
+from kiln_connect.openapi_client.models.post_atom_prepare_tx201_response import PostAtomPrepareTx201Response
+from kiln_connect.openapi_client.models.post_atom_stake_tx201_response import PostAtomStakeTx201Response
+from kiln_connect.openapi_client.models.post_eth_stakes_payload import PostETHStakesPayload
+from kiln_connect.openapi_client.models.post_eth_stakes_payload_stakes_inner import PostETHStakesPayloadStakesInner
 from kiln_connect.openapi_client.models.post_eth_broadcast_tx201_response import PostEthBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_eth_keys201_response import PostEthKeys201Response
 from kiln_connect.openapi_client.models.post_eth_keys201_response_data import PostEthKeys201ResponseData
 from kiln_connect.openapi_client.models.post_eth_prepare_tx201_response import PostEthPrepareTx201Response
 from kiln_connect.openapi_client.models.post_eth_stake_tx201_response import PostEthStakeTx201Response
+from kiln_connect.openapi_client.models.post_eth_stakes201_response import PostEthStakes201Response
+from kiln_connect.openapi_client.models.post_matic_approve_tx201_response import PostMaticApproveTx201Response
+from kiln_connect.openapi_client.models.post_matic_broadcast_tx201_response import PostMaticBroadcastTx201Response
+from kiln_connect.openapi_client.models.post_matic_prepare_tx201_response import PostMaticPrepareTx201Response
 from kiln_connect.openapi_client.models.post_sol_broadcast_tx201_response import PostSolBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_sol_prepare_tx201_response import PostSolPrepareTx201Response
 from kiln_connect.openapi_client.models.post_sol_stake_tx201_response import PostSolStakeTx201Response
-from kiln_connect.openapi_client.models.post_sol_stakes201_response import PostSolStakes201Response
 from kiln_connect.openapi_client.models.post_xtz_broadcast_tx201_response import PostXtzBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_xtz_prepare_tx201_response import PostXtzPrepareTx201Response
 from kiln_connect.openapi_client.models.post_xtz_stake_tx201_response import PostXtzStakeTx201Response
 from kiln_connect.openapi_client.models.sol_broadcast_tx import SOLBroadcastTx
 from kiln_connect.openapi_client.models.sol_broadcast_tx_payload import SOLBroadcastTxPayload
 from kiln_connect.openapi_client.models.sol_deactivate_stake_tx_payload import SOLDeactivateStakeTxPayload
 from kiln_connect.openapi_client.models.sol_merge_stakes_tx_payload import SOLMergeStakesTxPayload
@@ -137,9 +167,8 @@
 from kiln_connect.openapi_client.models.xtz_operation_delegate import XTZOperationDelegate
 from kiln_connect.openapi_client.models.xtz_operation_payment import XTZOperationPayment
 from kiln_connect.openapi_client.models.xtz_operation_undelegate import XTZOperationUndelegate
 from kiln_connect.openapi_client.models.xtz_prepare_tx_payload import XTZPrepareTxPayload
 from kiln_connect.openapi_client.models.xtz_signed_tx import XTZSignedTx
 from kiln_connect.openapi_client.models.xtz_stake import XTZStake
 from kiln_connect.openapi_client.models.xtztx_status import XTZTxStatus
-from kiln_connect.openapi_client.models.xtztx_status_receipt import XTZTxStatusReceipt
 from kiln_connect.openapi_client.models.xtz_unsigned_tx import XTZUnsignedTx
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/accounts_api.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/accounts_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,159 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
+    def delete_account(self, id : Annotated[StrictStr, Field(..., description="Account id")], **kwargs) -> PostAccount201Response:  # noqa: E501
+        """Account  # noqa: E501
+
+        Delete an account in your organization  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_account(id, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Account id (required)
+        :type id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: PostAccount201Response
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_account_with_http_info(id, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def delete_account_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Account id")], **kwargs):  # noqa: E501
+        """Account  # noqa: E501
+
+        Delete an account in your organization  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_account_with_http_info(id, async_req=True)
+        >>> result = thread.get()
+
+        :param id: Account id (required)
+        :type id: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(PostAccount201Response, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'id'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_account" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['bearerAuth']  # noqa: E501
+
+        _response_types_map = {
+            '200': "PostAccount201Response",
+            '401': None,
+            '500': None,
+        }
+
+        return self.api_client.call_api(
+            '/v1/accounts/{id}', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def get_account(self, id : Annotated[StrictStr, Field(..., description="Account id")], **kwargs) -> PostAccount201Response:  # noqa: E501
         """Account  # noqa: E501
 
         Retrieve an account in your organization  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/eth_api.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/eth_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,35 @@
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from datetime import date
 
-from pydantic import Field, StrictStr, conlist
+from pydantic import Field, StrictInt, StrictStr, conlist
 
 from typing import Optional
 
 from kiln_connect.openapi_client.models.eth_broadcast_tx_payload import ETHBroadcastTxPayload
 from kiln_connect.openapi_client.models.eth_craft_stake_tx_payload import ETHCraftStakeTxPayload
 from kiln_connect.openapi_client.models.eth_post_keys_payload import ETHPostKeysPayload
 from kiln_connect.openapi_client.models.eth_prepare_tx_payload import ETHPrepareTxPayload
 from kiln_connect.openapi_client.models.get_eth_kiln_stats200_response import GetEthKilnStats200Response
 from kiln_connect.openapi_client.models.get_eth_network_stats200_response import GetEthNetworkStats200Response
 from kiln_connect.openapi_client.models.get_eth_operations200_response import GetEthOperations200Response
 from kiln_connect.openapi_client.models.get_eth_rewards200_response import GetEthRewards200Response
 from kiln_connect.openapi_client.models.get_eth_stakes200_response import GetEthStakes200Response
 from kiln_connect.openapi_client.models.get_eth_tx_status200_response import GetEthTxStatus200Response
+from kiln_connect.openapi_client.models.get_exit_message200_response import GetExitMessage200Response
+from kiln_connect.openapi_client.models.post_eth_stakes_payload import PostETHStakesPayload
 from kiln_connect.openapi_client.models.post_eth_broadcast_tx201_response import PostEthBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_eth_keys201_response import PostEthKeys201Response
 from kiln_connect.openapi_client.models.post_eth_prepare_tx201_response import PostEthPrepareTx201Response
 from kiln_connect.openapi_client.models.post_eth_stake_tx201_response import PostEthStakeTx201Response
+from kiln_connect.openapi_client.models.post_eth_stakes201_response import PostEthStakes201Response
 
 from kiln_connect.openapi_client.api_client import ApiClient
 from kiln_connect.openapi_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
@@ -331,15 +334,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_eth_operations(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(float)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> GetEthOperations200Response:  # noqa: E501
+    def get_eth_operations(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(StrictInt)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> GetEthOperations200Response:  # noqa: E501
         """Operations  # noqa: E501
 
         Get the operations of Ethereum stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_eth_operations(validators, wallets, proxies, validator_indexes, accounts, async_req=True)
@@ -348,15 +351,15 @@
         :param validators: Comma-separated list of validators addresses
         :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param proxies: Comma-separated list of proxy-contract addresses
         :type proxies: List[str]
         :param validator_indexes: Comma-separated list of validators' consensus layer indexes
-        :type validator_indexes: List[float]
+        :type validator_indexes: List[int]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -370,15 +373,15 @@
                  returns the request thread.
         :rtype: GetEthOperations200Response
         """
         kwargs['_return_http_data_only'] = True
         return self.get_eth_operations_with_http_info(validators, wallets, proxies, validator_indexes, accounts, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_eth_operations_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(float)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
+    def get_eth_operations_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(StrictInt)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
         """Operations  # noqa: E501
 
         Get the operations of Ethereum stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_eth_operations_with_http_info(validators, wallets, proxies, validator_indexes, accounts, async_req=True)
@@ -387,15 +390,15 @@
         :param validators: Comma-separated list of validators addresses
         :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param proxies: Comma-separated list of proxy-contract addresses
         :type proxies: List[str]
         :param validator_indexes: Comma-separated list of validators' consensus layer indexes
-        :type validator_indexes: List[float]
+        :type validator_indexes: List[int]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -673,15 +676,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_eth_rewards(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(float)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, start_date : Annotated[Optional[date], Field(description="Get rewards from this date (YYYY-MM-DD)")] = None, end_date : Annotated[Optional[date], Field(description="Get rewards to this date (YYYY-MM-DD)")] = None, **kwargs) -> GetEthRewards200Response:  # noqa: E501
+    def get_eth_rewards(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(StrictInt)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, start_date : Annotated[Optional[date], Field(description="Get rewards from this date (YYYY-MM-DD)")] = None, end_date : Annotated[Optional[date], Field(description="Get rewards to this date (YYYY-MM-DD)")] = None, **kwargs) -> GetEthRewards200Response:  # noqa: E501
         """Rewards  # noqa: E501
 
         Get historical rewards by day of Ethereum stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_eth_rewards(validators, wallets, proxies, validator_indexes, accounts, start_date, end_date, async_req=True)
@@ -690,15 +693,15 @@
         :param validators: Comma-separated list of validators addresses
         :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param proxies: Comma-separated list of proxy-contract addresses
         :type proxies: List[str]
         :param validator_indexes: Comma-separated list of validators' consensus layer indexes
-        :type validator_indexes: List[float]
+        :type validator_indexes: List[int]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param start_date: Get rewards from this date (YYYY-MM-DD)
         :type start_date: date
         :param end_date: Get rewards to this date (YYYY-MM-DD)
         :type end_date: date
         :param async_req: Whether to execute the request asynchronously.
@@ -716,15 +719,15 @@
                  returns the request thread.
         :rtype: GetEthRewards200Response
         """
         kwargs['_return_http_data_only'] = True
         return self.get_eth_rewards_with_http_info(validators, wallets, proxies, validator_indexes, accounts, start_date, end_date, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_eth_rewards_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(float)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, start_date : Annotated[Optional[date], Field(description="Get rewards from this date (YYYY-MM-DD)")] = None, end_date : Annotated[Optional[date], Field(description="Get rewards to this date (YYYY-MM-DD)")] = None, **kwargs):  # noqa: E501
+    def get_eth_rewards_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(StrictInt)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, start_date : Annotated[Optional[date], Field(description="Get rewards from this date (YYYY-MM-DD)")] = None, end_date : Annotated[Optional[date], Field(description="Get rewards to this date (YYYY-MM-DD)")] = None, **kwargs):  # noqa: E501
         """Rewards  # noqa: E501
 
         Get historical rewards by day of Ethereum stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_eth_rewards_with_http_info(validators, wallets, proxies, validator_indexes, accounts, start_date, end_date, async_req=True)
@@ -733,15 +736,15 @@
         :param validators: Comma-separated list of validators addresses
         :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param proxies: Comma-separated list of proxy-contract addresses
         :type proxies: List[str]
         :param validator_indexes: Comma-separated list of validators' consensus layer indexes
-        :type validator_indexes: List[float]
+        :type validator_indexes: List[int]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param start_date: Get rewards from this date (YYYY-MM-DD)
         :type start_date: date
         :param end_date: Get rewards to this date (YYYY-MM-DD)
         :type end_date: date
         :param async_req: Whether to execute the request asynchronously.
@@ -866,15 +869,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_eth_stakes(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(float)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> GetEthStakes200Response:  # noqa: E501
+    def get_eth_stakes(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(StrictInt)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> GetEthStakes200Response:  # noqa: E501
         """Stakes  # noqa: E501
 
         Get the status of Ethereum stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_eth_stakes(validators, wallets, proxies, validator_indexes, accounts, async_req=True)
@@ -883,15 +886,15 @@
         :param validators: Comma-separated list of validators addresses
         :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param proxies: Comma-separated list of proxy-contract addresses
         :type proxies: List[str]
         :param validator_indexes: Comma-separated list of validators' consensus layer indexes
-        :type validator_indexes: List[float]
+        :type validator_indexes: List[int]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -905,15 +908,15 @@
                  returns the request thread.
         :rtype: GetEthStakes200Response
         """
         kwargs['_return_http_data_only'] = True
         return self.get_eth_stakes_with_http_info(validators, wallets, proxies, validator_indexes, accounts, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_eth_stakes_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(float)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
+    def get_eth_stakes_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, proxies : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of proxy-contract addresses")] = None, validator_indexes : Annotated[Optional[conlist(StrictInt)], Field(description="Comma-separated list of validators' consensus layer indexes")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
         """Stakes  # noqa: E501
 
         Get the status of Ethereum stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_eth_stakes_with_http_info(validators, wallets, proxies, validator_indexes, accounts, async_req=True)
@@ -922,15 +925,15 @@
         :param validators: Comma-separated list of validators addresses
         :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param proxies: Comma-separated list of proxy-contract addresses
         :type proxies: List[str]
         :param validator_indexes: Comma-separated list of validators' consensus layer indexes
-        :type validator_indexes: List[float]
+        :type validator_indexes: List[int]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1191,14 +1194,162 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def get_exit_message(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, **kwargs) -> GetExitMessage200Response:  # noqa: E501
+        """Exit Messages  # noqa: E501
+
+        Get encrypted exit message for a validator  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_exit_message(validators, async_req=True)
+        >>> result = thread.get()
+
+        :param validators: Comma-separated list of validators addresses
+        :type validators: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GetExitMessage200Response
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_exit_message_with_http_info(validators, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_exit_message_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, **kwargs):  # noqa: E501
+        """Exit Messages  # noqa: E501
+
+        Get encrypted exit message for a validator  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_exit_message_with_http_info(validators, async_req=True)
+        >>> result = thread.get()
+
+        :param validators: Comma-separated list of validators addresses
+        :type validators: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GetExitMessage200Response, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'validators'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_exit_message" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('validators') is not None:  # noqa: E501
+            _query_params.append(('validators', _params['validators']))
+            _collection_formats['validators'] = 'csv'
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json; charset=utf-8'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['bearerAuth']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GetExitMessage200Response",
+            '400': None,
+            '404': None,
+            '401': None,
+            '500': None,
+        }
+
+        return self.api_client.call_api(
+            '/v1/eth/exit-messages', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def post_eth_broadcast_tx(self, eth_broadcast_tx_payload : Annotated[ETHBroadcastTxPayload, Field(..., description="Transaction to broadcast")], **kwargs) -> PostEthBroadcastTx201Response:  # noqa: E501
         """Broadcast Transaction  # noqa: E501
 
         Broadcasts a signed Ethereum transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
@@ -1794,14 +1945,167 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def post_eth_stakes(self, post_eth_stakes_payload : Annotated[PostETHStakesPayload, Field(..., description="Stakes to create")], **kwargs) -> PostEthStakes201Response:  # noqa: E501
+        """Create stakes  # noqa: E501
+
+        Link ETH stakes to a Kiln account  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.post_eth_stakes(post_eth_stakes_payload, async_req=True)
+        >>> result = thread.get()
+
+        :param post_eth_stakes_payload: Stakes to create (required)
+        :type post_eth_stakes_payload: PostETHStakesPayload
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: PostEthStakes201Response
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.post_eth_stakes_with_http_info(post_eth_stakes_payload, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def post_eth_stakes_with_http_info(self, post_eth_stakes_payload : Annotated[PostETHStakesPayload, Field(..., description="Stakes to create")], **kwargs):  # noqa: E501
+        """Create stakes  # noqa: E501
+
+        Link ETH stakes to a Kiln account  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.post_eth_stakes_with_http_info(post_eth_stakes_payload, async_req=True)
+        >>> result = thread.get()
+
+        :param post_eth_stakes_payload: Stakes to create (required)
+        :type post_eth_stakes_payload: PostETHStakesPayload
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(PostEthStakes201Response, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'post_eth_stakes_payload'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method post_eth_stakes" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['post_eth_stakes_payload']:
+            _body_params = _params['post_eth_stakes_payload']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json; charset=utf-8'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json; charset=utf-8']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['bearerAuth']  # noqa: E501
+
+        _response_types_map = {
+            '201': "PostEthStakes201Response",
+            '400': None,
+            '401': None,
+            '500': None,
+        }
+
+        return self.api_client.call_api(
+            '/v1/eth/stakes', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/sol_api.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/sol_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 from typing import Optional
 
 from kiln_connect.openapi_client.models.get_sol_network_stats200_response import GetSolNetworkStats200Response
 from kiln_connect.openapi_client.models.get_sol_operations200_response import GetSolOperations200Response
 from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response
 from kiln_connect.openapi_client.models.get_sol_stakes200_response import GetSolStakes200Response
 from kiln_connect.openapi_client.models.get_sol_tx_status200_response import GetSolTxStatus200Response
+from kiln_connect.openapi_client.models.post_eth_stakes201_response import PostEthStakes201Response
 from kiln_connect.openapi_client.models.post_sol_broadcast_tx201_response import PostSolBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_sol_prepare_tx201_response import PostSolPrepareTx201Response
 from kiln_connect.openapi_client.models.post_sol_stake_tx201_response import PostSolStakeTx201Response
-from kiln_connect.openapi_client.models.post_sol_stakes201_response import PostSolStakes201Response
 from kiln_connect.openapi_client.models.sol_broadcast_tx_payload import SOLBroadcastTxPayload
 from kiln_connect.openapi_client.models.sol_deactivate_stake_tx_payload import SOLDeactivateStakeTxPayload
 from kiln_connect.openapi_client.models.sol_merge_stakes_tx_payload import SOLMergeStakesTxPayload
 from kiln_connect.openapi_client.models.sol_post_stakes_payload import SOLPostStakesPayload
 from kiln_connect.openapi_client.models.sol_prepare_tx_payload import SOLPrepareTxPayload
 from kiln_connect.openapi_client.models.sol_split_stake_tx_payload import SOLSplitStakeTxPayload
 from kiln_connect.openapi_client.models.sol_stake_tx_payload import SOLStakeTxPayload
@@ -1954,15 +1954,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def post_sol_stakes(self, sol_post_stakes_payload : Annotated[SOLPostStakesPayload, Field(..., description="Stakes to create")], **kwargs) -> PostSolStakes201Response:  # noqa: E501
+    def post_sol_stakes(self, sol_post_stakes_payload : Annotated[SOLPostStakesPayload, Field(..., description="Stakes to create")], **kwargs) -> PostEthStakes201Response:  # noqa: E501
         """Create stakes  # noqa: E501
 
         Create Solana stakes and linked them to a Kiln account  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.post_sol_stakes(sol_post_stakes_payload, async_req=True)
@@ -1979,15 +1979,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PostSolStakes201Response
+        :rtype: PostEthStakes201Response
         """
         kwargs['_return_http_data_only'] = True
         return self.post_sol_stakes_with_http_info(sol_post_stakes_payload, **kwargs)  # noqa: E501
 
     @validate_arguments
     def post_sol_stakes_with_http_info(self, sol_post_stakes_payload : Annotated[SOLPostStakesPayload, Field(..., description="Stakes to create")], **kwargs):  # noqa: E501
         """Create stakes  # noqa: E501
@@ -2018,15 +2018,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PostSolStakes201Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PostEthStakes201Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'sol_post_stakes_payload'
         ]
@@ -2083,15 +2083,15 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '201': "PostSolStakes201Response",
+            '201': "PostEthStakes201Response",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
             '/v1/sol/stakes', 'POST',
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/xtz_api.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api/xtz_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -346,14 +346,169 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def get_xtz_reports(self, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> bytearray:  # noqa: E501
+        """Excel Reports  # noqa: E501
+
+        Generates an Excel report sheet for your stakes and rewards  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_xtz_reports(wallets, accounts, async_req=True)
+        >>> result = thread.get()
+
+        :param wallets: Comma-separated list of wallets addresses
+        :type wallets: List[str]
+        :param accounts: Comma-separated list of Kiln accounts identifiers
+        :type accounts: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: bytearray
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_xtz_reports_with_http_info(wallets, accounts, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_xtz_reports_with_http_info(self, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
+        """Excel Reports  # noqa: E501
+
+        Generates an Excel report sheet for your stakes and rewards  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_xtz_reports_with_http_info(wallets, accounts, async_req=True)
+        >>> result = thread.get()
+
+        :param wallets: Comma-separated list of wallets addresses
+        :type wallets: List[str]
+        :param accounts: Comma-separated list of Kiln accounts identifiers
+        :type accounts: List[str]
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(bytearray, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'wallets',
+            'accounts'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_xtz_reports" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('wallets') is not None:  # noqa: E501
+            _query_params.append(('wallets', _params['wallets']))
+            _collection_formats['wallets'] = 'csv'
+        if _params.get('accounts') is not None:  # noqa: E501
+            _query_params.append(('accounts', _params['accounts']))
+            _collection_formats['accounts'] = 'csv'
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/octet-stream'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['bearerAuth']  # noqa: E501
+
+        _response_types_map = {
+            '200': "bytearray",
+            '400': None,
+            '401': None,
+            '500': None,
+        }
+
+        return self.api_client.call_api(
+            '/v1/xtz/reports', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def get_xtz_rewards(self, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, format : Annotated[Optional[StrictStr], Field(description="The format of the response. Defaults to daily")] = None, start_date : Annotated[Optional[date], Field(description="Get rewards from this date (YYYY-MM-DD)")] = None, end_date : Annotated[Optional[date], Field(description="Get rewards to this date (YYYY-MM-DD)")] = None, start_cycle : Annotated[Optional[float], Field(description="The cycle from which we want to fetch rewards. Must be used with format=cycle")] = None, end_cycle : Annotated[Optional[float], Field(description="The cycle until which we want to fetch rewards. Must be used with format=cycle")] = None, **kwargs) -> GetXtzRewards200Response:  # noqa: E501
         """Rewards  # noqa: E501
 
         Get historical rewards of Tezos stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api_client.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/configuration.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/exceptions.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/__init__.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,159 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     Kiln API Docs (dev)
 
     This API provides reporting staking data on various protocols as well as network wide data, staking transaction crafting features and so on. In order to use it, you should first get an API token from your Kiln dashboard (applications section). If you don't have access to our dashboard, please get in touch at hello@kiln.fi. Once you have your API token, you can set it as a bearer token in your request headers.  ### Backward Compatibility  This is an experimental specification used for development and testing, do not rely on what is here unless you know the implications.  The official Kiln API specification following backward compatible changes can be found [here](/).  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: contact@kiln.fi
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-# import models into model package
+__version__ = "1.0.0"
+
+# import apis into sdk package
+from kiln_connect.openapi_client.api.accounts_api import AccountsApi
+from kiln_connect.openapi_client.api.ada_api import AdaApi
+from kiln_connect.openapi_client.api.atom_api import AtomApi
+from kiln_connect.openapi_client.api.eth_api import EthApi
+from kiln_connect.openapi_client.api.matic_api import MaticApi
+from kiln_connect.openapi_client.api.organizations_api import OrganizationsApi
+from kiln_connect.openapi_client.api.sol_api import SolApi
+from kiln_connect.openapi_client.api.xtz_api import XtzApi
+
+# import ApiClient
+from kiln_connect.openapi_client.api_client import ApiClient
+from kiln_connect.openapi_client.configuration import Configuration
+from kiln_connect.openapi_client.exceptions import OpenApiException
+from kiln_connect.openapi_client.exceptions import ApiTypeError
+from kiln_connect.openapi_client.exceptions import ApiValueError
+from kiln_connect.openapi_client.exceptions import ApiKeyError
+from kiln_connect.openapi_client.exceptions import ApiAttributeError
+from kiln_connect.openapi_client.exceptions import ApiException
+# import models into sdk package
+from kiln_connect.openapi_client.models.ada_broadcast_tx_payload import ADABroadcastTxPayload
+from kiln_connect.openapi_client.models.ada_craft_stake_tx_payload import ADACraftStakeTxPayload
+from kiln_connect.openapi_client.models.ada_craft_unstake_tx_payload import ADACraftUnstakeTxPayload
+from kiln_connect.openapi_client.models.ada_craft_withdraw_rewards_tx_payload import ADACraftWithdrawRewardsTxPayload
+from kiln_connect.openapi_client.models.ada_prepare_tx_payload import ADAPrepareTxPayload
+from kiln_connect.openapi_client.models.ada_prepare_tx_payload_signed_messages_inner import ADAPrepareTxPayloadSignedMessagesInner
+from kiln_connect.openapi_client.models.ada_signed_tx import ADASignedTx
+from kiln_connect.openapi_client.models.adatx_hash import ADATxHash
+from kiln_connect.openapi_client.models.adatx_status import ADATxStatus
+from kiln_connect.openapi_client.models.ada_unsigned_tx import ADAUnsignedTx
+from kiln_connect.openapi_client.models.atom_broadcast_tx_payload import ATOMBroadcastTxPayload
+from kiln_connect.openapi_client.models.atom_craft_stake_tx_payload import ATOMCraftStakeTxPayload
+from kiln_connect.openapi_client.models.atom_craft_unstake_tx_payload import ATOMCraftUnstakeTxPayload
+from kiln_connect.openapi_client.models.atom_craft_withdraw_rewards_tx_payload import ATOMCraftWithdrawRewardsTxPayload
+from kiln_connect.openapi_client.models.atom_network_stats import ATOMNetworkStats
+from kiln_connect.openapi_client.models.atom_prepare_tx_payload import ATOMPrepareTxPayload
 from kiln_connect.openapi_client.models.atom_reward import ATOMReward
+from kiln_connect.openapi_client.models.atom_signed_tx import ATOMSignedTx
 from kiln_connect.openapi_client.models.atom_stake import ATOMStake
+from kiln_connect.openapi_client.models.atomtx_hash import ATOMTxHash
+from kiln_connect.openapi_client.models.atomtx_status import ATOMTxStatus
+from kiln_connect.openapi_client.models.atom_unsigned_tx import ATOMUnsignedTx
 from kiln_connect.openapi_client.models.account import Account
 from kiln_connect.openapi_client.models.account_payload import AccountPayload
-from kiln_connect.openapi_client.models.account_portfolio import AccountPortfolio
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner import AccountPortfolioProtocolsInner
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance import AccountPortfolioProtocolsInnerTotalBalance
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards import AccountPortfolioProtocolsInnerTotalRewards
 from kiln_connect.openapi_client.models.core_stake import CoreStake
 from kiln_connect.openapi_client.models.eth_broadcast_tx_payload import ETHBroadcastTxPayload
 from kiln_connect.openapi_client.models.eth_broadcasted_tx import ETHBroadcastedTx
 from kiln_connect.openapi_client.models.eth_craft_stake_tx_payload import ETHCraftStakeTxPayload
+from kiln_connect.openapi_client.models.eth_exit_message import ETHExitMessage
 from kiln_connect.openapi_client.models.eth_kiln_stats import ETHKilnStats
 from kiln_connect.openapi_client.models.eth_kiln_stats_gross_apy import ETHKilnStatsGrossApy
 from kiln_connect.openapi_client.models.eth_network_stats import ETHNetworkStats
 from kiln_connect.openapi_client.models.eth_operation_consensus_withdrawal import ETHOperationConsensusWithdrawal
 from kiln_connect.openapi_client.models.eth_operation_deposit import ETHOperationDeposit
 from kiln_connect.openapi_client.models.eth_operation_execution_reward import ETHOperationExecutionReward
 from kiln_connect.openapi_client.models.eth_post_keys_batch_response import ETHPostKeysBatchResponse
 from kiln_connect.openapi_client.models.eth_post_keys_cli_response_inner import ETHPostKeysCliResponseInner
 from kiln_connect.openapi_client.models.eth_post_keys_payload import ETHPostKeysPayload
 from kiln_connect.openapi_client.models.eth_prepare_tx_payload import ETHPrepareTxPayload
 from kiln_connect.openapi_client.models.eth_reward import ETHReward
 from kiln_connect.openapi_client.models.eth_signed_tx import ETHSignedTx
 from kiln_connect.openapi_client.models.eth_stake import ETHStake
 from kiln_connect.openapi_client.models.ethtx_status import ETHTxStatus
-from kiln_connect.openapi_client.models.ethtx_status_receipt import ETHTxStatusReceipt
-from kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner import ETHTxStatusReceiptLogsInner
 from kiln_connect.openapi_client.models.eth_unsigned_tx import ETHUnsignedTx
 from kiln_connect.openapi_client.models.get_account_portfolio200_response import GetAccountPortfolio200Response
 from kiln_connect.openapi_client.models.get_accounts200_response import GetAccounts200Response
+from kiln_connect.openapi_client.models.get_ada_tx_status200_response import GetAdaTxStatus200Response
+from kiln_connect.openapi_client.models.get_atom_network_stats200_response import GetAtomNetworkStats200Response
 from kiln_connect.openapi_client.models.get_atom_rewards200_response import GetAtomRewards200Response
 from kiln_connect.openapi_client.models.get_atom_stakes200_response import GetAtomStakes200Response
+from kiln_connect.openapi_client.models.get_atom_tx_status200_response import GetAtomTxStatus200Response
 from kiln_connect.openapi_client.models.get_eth_kiln_stats200_response import GetEthKilnStats200Response
 from kiln_connect.openapi_client.models.get_eth_network_stats200_response import GetEthNetworkStats200Response
 from kiln_connect.openapi_client.models.get_eth_operations200_response import GetEthOperations200Response
 from kiln_connect.openapi_client.models.get_eth_operations200_response_data_inner import GetEthOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_eth_rewards200_response import GetEthRewards200Response
 from kiln_connect.openapi_client.models.get_eth_stakes200_response import GetEthStakes200Response
 from kiln_connect.openapi_client.models.get_eth_tx_status200_response import GetEthTxStatus200Response
+from kiln_connect.openapi_client.models.get_exit_message200_response import GetExitMessage200Response
+from kiln_connect.openapi_client.models.get_matic_tx_status200_response import GetMaticTxStatus200Response
 from kiln_connect.openapi_client.models.get_sol_network_stats200_response import GetSolNetworkStats200Response
 from kiln_connect.openapi_client.models.get_sol_operations200_response import GetSolOperations200Response
 from kiln_connect.openapi_client.models.get_sol_operations200_response_data_inner import GetSolOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response
 from kiln_connect.openapi_client.models.get_sol_rewards200_response_data_inner import GetSolRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_stakes200_response import GetSolStakes200Response
 from kiln_connect.openapi_client.models.get_sol_tx_status200_response import GetSolTxStatus200Response
 from kiln_connect.openapi_client.models.get_xtz_network_stats200_response import GetXtzNetworkStats200Response
 from kiln_connect.openapi_client.models.get_xtz_operations200_response import GetXtzOperations200Response
 from kiln_connect.openapi_client.models.get_xtz_operations200_response_data_inner import GetXtzOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response import GetXtzRewards200Response
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner import GetXtzRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_xtz_stakes200_response import GetXtzStakes200Response
 from kiln_connect.openapi_client.models.get_xtz_tx_status200_response import GetXtzTxStatus200Response
+from kiln_connect.openapi_client.models.matic_broadcast_tx_payload import MATICBroadcastTxPayload
+from kiln_connect.openapi_client.models.matic_broadcasted_tx import MATICBroadcastedTx
+from kiln_connect.openapi_client.models.matic_craft_approve_tx_payload import MATICCraftApproveTxPayload
+from kiln_connect.openapi_client.models.matic_craft_buy_voucher_tx_payload import MATICCraftBuyVoucherTxPayload
+from kiln_connect.openapi_client.models.matic_craft_restake_rewards_tx_payload import MATICCraftRestakeRewardsTxPayload
+from kiln_connect.openapi_client.models.matic_craft_sell_voucher_tx_payload import MATICCraftSellVoucherTxPayload
+from kiln_connect.openapi_client.models.matic_craft_unstake_claim_tokens_tx_payload import MATICCraftUnstakeClaimTokensTxPayload
+from kiln_connect.openapi_client.models.matic_craft_withdraw_rewards_tx_payload import MATICCraftWithdrawRewardsTxPayload
+from kiln_connect.openapi_client.models.matic_prepare_tx_payload import MATICPrepareTxPayload
+from kiln_connect.openapi_client.models.matic_signed_tx import MATICSignedTx
+from kiln_connect.openapi_client.models.matictx_status import MATICTxStatus
+from kiln_connect.openapi_client.models.matic_unsigned_tx import MATICUnsignedTx
+from kiln_connect.openapi_client.models.portfolio import Portfolio
+from kiln_connect.openapi_client.models.portfolio_protocols_inner import PortfolioProtocolsInner
+from kiln_connect.openapi_client.models.portfolio_protocols_inner_total_balance import PortfolioProtocolsInnerTotalBalance
+from kiln_connect.openapi_client.models.portfolio_protocols_inner_total_rewards import PortfolioProtocolsInnerTotalRewards
+from kiln_connect.openapi_client.models.post_atom_stakes_payload import PostATOMStakesPayload
+from kiln_connect.openapi_client.models.post_atom_stakes_payload_stakes_inner import PostATOMStakesPayloadStakesInner
 from kiln_connect.openapi_client.models.post_account201_response import PostAccount201Response
+from kiln_connect.openapi_client.models.post_ada_broadcast_tx201_response import PostAdaBroadcastTx201Response
+from kiln_connect.openapi_client.models.post_ada_prepare_tx201_response import PostAdaPrepareTx201Response
+from kiln_connect.openapi_client.models.post_ada_stake_tx201_response import PostAdaStakeTx201Response
+from kiln_connect.openapi_client.models.post_atom_broadcast_tx201_response import PostAtomBroadcastTx201Response
+from kiln_connect.openapi_client.models.post_atom_prepare_tx201_response import PostAtomPrepareTx201Response
+from kiln_connect.openapi_client.models.post_atom_stake_tx201_response import PostAtomStakeTx201Response
+from kiln_connect.openapi_client.models.post_eth_stakes_payload import PostETHStakesPayload
+from kiln_connect.openapi_client.models.post_eth_stakes_payload_stakes_inner import PostETHStakesPayloadStakesInner
 from kiln_connect.openapi_client.models.post_eth_broadcast_tx201_response import PostEthBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_eth_keys201_response import PostEthKeys201Response
 from kiln_connect.openapi_client.models.post_eth_keys201_response_data import PostEthKeys201ResponseData
 from kiln_connect.openapi_client.models.post_eth_prepare_tx201_response import PostEthPrepareTx201Response
 from kiln_connect.openapi_client.models.post_eth_stake_tx201_response import PostEthStakeTx201Response
+from kiln_connect.openapi_client.models.post_eth_stakes201_response import PostEthStakes201Response
+from kiln_connect.openapi_client.models.post_matic_approve_tx201_response import PostMaticApproveTx201Response
+from kiln_connect.openapi_client.models.post_matic_broadcast_tx201_response import PostMaticBroadcastTx201Response
+from kiln_connect.openapi_client.models.post_matic_prepare_tx201_response import PostMaticPrepareTx201Response
 from kiln_connect.openapi_client.models.post_sol_broadcast_tx201_response import PostSolBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_sol_prepare_tx201_response import PostSolPrepareTx201Response
 from kiln_connect.openapi_client.models.post_sol_stake_tx201_response import PostSolStakeTx201Response
-from kiln_connect.openapi_client.models.post_sol_stakes201_response import PostSolStakes201Response
 from kiln_connect.openapi_client.models.post_xtz_broadcast_tx201_response import PostXtzBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_xtz_prepare_tx201_response import PostXtzPrepareTx201Response
 from kiln_connect.openapi_client.models.post_xtz_stake_tx201_response import PostXtzStakeTx201Response
 from kiln_connect.openapi_client.models.sol_broadcast_tx import SOLBroadcastTx
 from kiln_connect.openapi_client.models.sol_broadcast_tx_payload import SOLBroadcastTxPayload
 from kiln_connect.openapi_client.models.sol_deactivate_stake_tx_payload import SOLDeactivateStakeTxPayload
 from kiln_connect.openapi_client.models.sol_merge_stakes_tx_payload import SOLMergeStakesTxPayload
@@ -118,9 +189,8 @@
 from kiln_connect.openapi_client.models.xtz_operation_delegate import XTZOperationDelegate
 from kiln_connect.openapi_client.models.xtz_operation_payment import XTZOperationPayment
 from kiln_connect.openapi_client.models.xtz_operation_undelegate import XTZOperationUndelegate
 from kiln_connect.openapi_client.models.xtz_prepare_tx_payload import XTZPrepareTxPayload
 from kiln_connect.openapi_client.models.xtz_signed_tx import XTZSignedTx
 from kiln_connect.openapi_client.models.xtz_stake import XTZStake
 from kiln_connect.openapi_client.models.xtztx_status import XTZTxStatus
-from kiln_connect.openapi_client.models.xtztx_status_receipt import XTZTxStatusReceipt
 from kiln_connect.openapi_client.models.xtz_unsigned_tx import XTZUnsignedTx
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/account_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/portfolio.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictInt, conlist
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner import AccountPortfolioProtocolsInner
+from kiln_connect.openapi_client.models.portfolio_protocols_inner import PortfolioProtocolsInner
 
-class AccountPortfolio(BaseModel):
+class Portfolio(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     total_balance_usd: Optional[float] = Field(None, description="Total USD balance of all the account's stakes")
     total_rewards_usd: Optional[float] = Field(None, description="Total USD of rewards earned from all the account's stakes")
     total_stakes: Optional[StrictInt] = Field(None, description="Total number of stakes")
     total_active_stakes: Optional[StrictInt] = Field(None, description="Total number of stakes actively collecting rewards")
-    protocols: Optional[conlist(AccountPortfolioProtocolsInner)] = Field(None, description="List of protocols staked within the account")
+    protocols: Optional[conlist(PortfolioProtocolsInner)] = Field(None, description="List of protocols staked within the account")
     __properties = ["total_balance_usd", "total_rewards_usd", "total_stakes", "total_active_stakes", "protocols"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -44,16 +44,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AccountPortfolio:
-        """Create an instance of AccountPortfolio from a JSON string"""
+    def from_json(cls, json_str: str) -> Portfolio:
+        """Create an instance of Portfolio from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -64,24 +64,24 @@
             for _item in self.protocols:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['protocols'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AccountPortfolio:
-        """Create an instance of AccountPortfolio from a dict"""
+    def from_dict(cls, obj: dict) -> Portfolio:
+        """Create an instance of Portfolio from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AccountPortfolio.parse_obj(obj)
+            return Portfolio.parse_obj(obj)
 
-        _obj = AccountPortfolio.parse_obj({
+        _obj = Portfolio.parse_obj({
             "total_balance_usd": obj.get("total_balance_usd"),
             "total_rewards_usd": obj.get("total_rewards_usd"),
             "total_stakes": obj.get("total_stakes"),
             "total_active_stakes": obj.get("total_active_stakes"),
-            "protocols": [AccountPortfolioProtocolsInner.from_dict(_item) for _item in obj.get("protocols")] if obj.get("protocols") is not None else None
+            "protocols": [PortfolioProtocolsInner.from_dict(_item) for _item in obj.get("protocols")] if obj.get("protocols") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/portfolio_protocols_inner.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr, confloat
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance import AccountPortfolioProtocolsInnerTotalBalance
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards import AccountPortfolioProtocolsInnerTotalRewards
+from kiln_connect.openapi_client.models.portfolio_protocols_inner_total_balance import PortfolioProtocolsInnerTotalBalance
+from kiln_connect.openapi_client.models.portfolio_protocols_inner_total_rewards import PortfolioProtocolsInnerTotalRewards
 
-class AccountPortfolioProtocolsInner(BaseModel):
+class PortfolioProtocolsInner(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     token: Optional[StrictStr] = Field(None, description="Token name")
     name: Optional[StrictStr] = Field(None, description="Protocol name")
     total_stakes: Optional[StrictInt] = Field(None, description="Total number of stakes for this protocol")
     total_active_stakes: Optional[StrictInt] = Field(None, description="Total number of stakes actively collecting rewards for this protocol")
-    total_balance: Optional[AccountPortfolioProtocolsInnerTotalBalance] = None
-    total_rewards: Optional[AccountPortfolioProtocolsInnerTotalRewards] = None
+    total_balance: Optional[PortfolioProtocolsInnerTotalBalance] = None
+    total_rewards: Optional[PortfolioProtocolsInnerTotalRewards] = None
     balance_share_percent: Optional[confloat(le=100, ge=0)] = Field(None, description="Protocol share of the total balance")
     rewards_share_percent: Optional[confloat(le=100, ge=0)] = Field(None, description="Protocol share of the total rewards earned")
     __properties = ["token", "name", "total_stakes", "total_active_stakes", "total_balance", "total_rewards", "balance_share_percent", "rewards_share_percent"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
@@ -48,16 +48,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AccountPortfolioProtocolsInner:
-        """Create an instance of AccountPortfolioProtocolsInner from a JSON string"""
+    def from_json(cls, json_str: str) -> PortfolioProtocolsInner:
+        """Create an instance of PortfolioProtocolsInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -67,27 +67,27 @@
             _dict['total_balance'] = self.total_balance.to_dict()
         # override the default output from pydantic by calling `to_dict()` of total_rewards
         if self.total_rewards:
             _dict['total_rewards'] = self.total_rewards.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AccountPortfolioProtocolsInner:
-        """Create an instance of AccountPortfolioProtocolsInner from a dict"""
+    def from_dict(cls, obj: dict) -> PortfolioProtocolsInner:
+        """Create an instance of PortfolioProtocolsInner from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AccountPortfolioProtocolsInner.parse_obj(obj)
+            return PortfolioProtocolsInner.parse_obj(obj)
 
-        _obj = AccountPortfolioProtocolsInner.parse_obj({
+        _obj = PortfolioProtocolsInner.parse_obj({
             "token": obj.get("token"),
             "name": obj.get("name"),
             "total_stakes": obj.get("total_stakes"),
             "total_active_stakes": obj.get("total_active_stakes"),
-            "total_balance": AccountPortfolioProtocolsInnerTotalBalance.from_dict(obj.get("total_balance")) if obj.get("total_balance") is not None else None,
-            "total_rewards": AccountPortfolioProtocolsInnerTotalRewards.from_dict(obj.get("total_rewards")) if obj.get("total_rewards") is not None else None,
+            "total_balance": PortfolioProtocolsInnerTotalBalance.from_dict(obj.get("total_balance")) if obj.get("total_balance") is not None else None,
+            "total_rewards": PortfolioProtocolsInnerTotalRewards.from_dict(obj.get("total_rewards")) if obj.get("total_rewards") is not None else None,
             "balance_share_percent": obj.get("balance_share_percent"),
             "rewards_share_percent": obj.get("rewards_share_percent")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/portfolio_protocols_inner_total_balance.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field
 
-class AccountPortfolioProtocolsInnerTotalBalance(BaseModel):
+class PortfolioProtocolsInnerTotalBalance(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     amount_usd: Optional[float] = Field(None, description="Total USD balance of stakes for this protocol")
     amount: Optional[float] = Field(None, description="Total balance of stakes in the native protocol token for this protocol")
@@ -40,34 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AccountPortfolioProtocolsInnerTotalBalance:
-        """Create an instance of AccountPortfolioProtocolsInnerTotalBalance from a JSON string"""
+    def from_json(cls, json_str: str) -> PortfolioProtocolsInnerTotalBalance:
+        """Create an instance of PortfolioProtocolsInnerTotalBalance from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AccountPortfolioProtocolsInnerTotalBalance:
-        """Create an instance of AccountPortfolioProtocolsInnerTotalBalance from a dict"""
+    def from_dict(cls, obj: dict) -> PortfolioProtocolsInnerTotalBalance:
+        """Create an instance of PortfolioProtocolsInnerTotalBalance from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AccountPortfolioProtocolsInnerTotalBalance.parse_obj(obj)
+            return PortfolioProtocolsInnerTotalBalance.parse_obj(obj)
 
-        _obj = AccountPortfolioProtocolsInnerTotalBalance.parse_obj({
+        _obj = PortfolioProtocolsInnerTotalBalance.parse_obj({
             "amount_usd": obj.get("amount_usd"),
             "amount": obj.get("amount")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/portfolio_protocols_inner_total_rewards.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field
 
-class AccountPortfolioProtocolsInnerTotalRewards(BaseModel):
+class PortfolioProtocolsInnerTotalRewards(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     amount_usd: Optional[float] = Field(None, description="Total USD of rewards earned for this protocol")
     amount: Optional[float] = Field(None, description="Total rewards earned in the native protocol token for this protocol")
@@ -40,34 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> AccountPortfolioProtocolsInnerTotalRewards:
-        """Create an instance of AccountPortfolioProtocolsInnerTotalRewards from a JSON string"""
+    def from_json(cls, json_str: str) -> PortfolioProtocolsInnerTotalRewards:
+        """Create an instance of PortfolioProtocolsInnerTotalRewards from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> AccountPortfolioProtocolsInnerTotalRewards:
-        """Create an instance of AccountPortfolioProtocolsInnerTotalRewards from a dict"""
+    def from_dict(cls, obj: dict) -> PortfolioProtocolsInnerTotalRewards:
+        """Create an instance of PortfolioProtocolsInnerTotalRewards from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return AccountPortfolioProtocolsInnerTotalRewards.parse_obj(obj)
+            return PortfolioProtocolsInnerTotalRewards.parse_obj(obj)
 
-        _obj = AccountPortfolioProtocolsInnerTotalRewards.parse_obj({
+        _obj = PortfolioProtocolsInnerTotalRewards.parse_obj({
             "amount_usd": obj.get("amount_usd"),
             "amount": obj.get("amount")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/atom_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/atom_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/core_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/core_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_broadcasted_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_kiln_stats.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_kiln_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_network_stats.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_network_stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,59 +17,59 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field
 
-class ETHNetworkStats(BaseModel):
+class SOLNetworkStats(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     network_gross_apy: Optional[float] = Field(None, description="Gross annual percentage yield")
-    supply_staked_percent: Optional[float] = Field(None, description="Supply of Ethereum currently staked")
-    eth_price_usd: Optional[float] = Field(None, description="Price of Ethereum in USD")
-    __properties = ["network_gross_apy", "supply_staked_percent", "eth_price_usd"]
+    supply_staked_percent: Optional[float] = Field(None, description="Supply of Solana currently staked")
+    nb_validators: Optional[float] = Field(None, description="Number of active stakes")
+    __properties = ["network_gross_apy", "supply_staked_percent", "nb_validators"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ETHNetworkStats:
-        """Create an instance of ETHNetworkStats from a JSON string"""
+    def from_json(cls, json_str: str) -> SOLNetworkStats:
+        """Create an instance of SOLNetworkStats from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ETHNetworkStats:
-        """Create an instance of ETHNetworkStats from a dict"""
+    def from_dict(cls, obj: dict) -> SOLNetworkStats:
+        """Create an instance of SOLNetworkStats from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ETHNetworkStats.parse_obj(obj)
+            return SOLNetworkStats.parse_obj(obj)
 
-        _obj = ETHNetworkStats.parse_obj({
+        _obj = SOLNetworkStats.parse_obj({
             "network_gross_apy": obj.get("network_gross_apy"),
             "supply_staked_percent": obj.get("supply_staked_percent"),
-            "eth_price_usd": obj.get("eth_price_usd")
+            "nb_validators": obj.get("nb_validators")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictInt, StrictStr, conint
 
 class ETHOperationConsensusWithdrawal(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     type: Optional[StrictStr] = None
     time: Optional[datetime] = Field(None, description="Time of the operation")
     validator_address: Optional[StrictStr] = Field(None, description="Validator address of the operation")
+    validator_index: Optional[conint(strict=True, ge=1)] = Field(None, description="Validator's consensus layer index")
     block: Optional[StrictInt] = Field(None, description="Block number of the reward")
     fee_recipient: Optional[StrictStr] = Field(None, description="Fee recipient of the reward")
     amount: Optional[StrictStr] = Field(None, description="Amount in WEI of the reward")
-    __properties = ["type", "time", "validator_address", "block", "fee_recipient", "amount"]
+    __properties = ["type", "time", "validator_address", "validator_index", "block", "fee_recipient", "amount"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -69,13 +70,14 @@
         if type(obj) is not dict:
             return ETHOperationConsensusWithdrawal.parse_obj(obj)
 
         _obj = ETHOperationConsensusWithdrawal.parse_obj({
             "type": obj.get("type"),
             "time": obj.get("time"),
             "validator_address": obj.get("validator_address"),
+            "validator_index": obj.get("validator_index"),
             "block": obj.get("block"),
             "fee_recipient": obj.get("fee_recipient"),
             "amount": obj.get("amount")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_deposit.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_operation_deposit.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,35 +15,36 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist
+from pydantic import BaseModel, Field, StrictInt, StrictStr, conint, conlist
 
 class ETHOperationDeposit(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     type: Optional[StrictStr] = Field(None, description="type of the operation")
     time: Optional[datetime] = Field(None, description="Time of the operation")
     validator_address: Optional[StrictStr] = Field(None, description="Validator address of the operation")
+    validator_index: Optional[conint(strict=True, ge=1)] = Field(None, description="Index of the public key of the validator")
     tx_hash: Optional[StrictStr] = Field(None, description="Hash of the transaction")
     tx_sender: Optional[StrictStr] = Field(None, description="Address of the sender of the transaction")
     tx_gas_used: Optional[StrictStr] = Field(None, description="Gas used by the transaction in WEI")
     tx_effective_gas_price: Optional[StrictStr] = Field(None, description="Effective gas price used for this TX in WEI")
     proxies: Optional[conlist(StrictStr)] = Field(None, description="Ordered list of smart-contracts in the calling chain")
     block: Optional[StrictInt] = Field(None, description="Block number containing the transaction")
     block_base_fee: Optional[StrictStr] = Field(None, description="Base fee used for this block in WEI")
     withdrawal_credentials: Optional[StrictStr] = Field(None, description="Withdrawal credentials of the deposit")
     amount: Optional[StrictStr] = Field(None, description="Amount in WEI of the deposit transaction")
-    __properties = ["type", "time", "validator_address", "tx_hash", "tx_sender", "tx_gas_used", "tx_effective_gas_price", "proxies", "block", "block_base_fee", "withdrawal_credentials", "amount"]
+    __properties = ["type", "time", "validator_address", "validator_index", "tx_hash", "tx_sender", "tx_gas_used", "tx_effective_gas_price", "proxies", "block", "block_base_fee", "withdrawal_credentials", "amount"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -75,14 +76,15 @@
         if type(obj) is not dict:
             return ETHOperationDeposit.parse_obj(obj)
 
         _obj = ETHOperationDeposit.parse_obj({
             "type": obj.get("type"),
             "time": obj.get("time"),
             "validator_address": obj.get("validator_address"),
+            "validator_index": obj.get("validator_index"),
             "tx_hash": obj.get("tx_hash"),
             "tx_sender": obj.get("tx_sender"),
             "tx_gas_used": obj.get("tx_gas_used"),
             "tx_effective_gas_price": obj.get("tx_effective_gas_price"),
             "proxies": obj.get("proxies"),
             "block": obj.get("block"),
             "block_base_fee": obj.get("block_base_fee"),
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_execution_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_operation_execution_reward.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,30 +15,31 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictInt, StrictStr, conint
 
 class ETHOperationExecutionReward(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     type: Optional[StrictStr] = None
     time: Optional[datetime] = Field(None, description="Time of the operation")
     validator_address: Optional[StrictStr] = Field(None, description="Validator address of the operation")
+    validator_index: Optional[conint(strict=True, ge=1)] = Field(None, description="Validator's consensus layer index")
     block: Optional[StrictInt] = Field(None, description="Block number of the reward")
     fee_recipient: Optional[StrictStr] = Field(None, description="Fee recipient of the reward")
     mev_payout_tx_hash: Optional[StrictStr] = Field(None, description="Hash of the MEV payout transaction if appliable")
     amount: Optional[StrictStr] = Field(None, description="Amount in WEI of the reward")
-    __properties = ["type", "time", "validator_address", "block", "fee_recipient", "mev_payout_tx_hash", "amount"]
+    __properties = ["type", "time", "validator_address", "validator_index", "block", "fee_recipient", "mev_payout_tx_hash", "amount"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -74,14 +75,15 @@
         if type(obj) is not dict:
             return ETHOperationExecutionReward.parse_obj(obj)
 
         _obj = ETHOperationExecutionReward.parse_obj({
             "type": obj.get("type"),
             "time": obj.get("time"),
             "validator_address": obj.get("validator_address"),
+            "validator_index": obj.get("validator_index"),
             "block": obj.get("block"),
             "fee_recipient": obj.get("fee_recipient"),
             "mev_payout_tx_hash": obj.get("mev_payout_tx_hash"),
             "amount": obj.get("amount")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_post_keys_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_signed_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_stake.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,38 +15,41 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conint
 
 class ETHStake(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     validator_address: Optional[StrictStr] = Field(None, description="Public key of the validator")
+    validator_index: Optional[conint(strict=True, ge=1)] = Field(None, description="Validator's consensus layer index")
     state: Optional[StrictStr] = Field(None, description="State of the Ethereum stake as seen be the consensus layer")
     activated_at: Optional[datetime] = Field(None, description="Date of activation on the Ethereum consensus layer")
     activated_epoch: Optional[StrictInt] = Field(None, description="Epoch of activation on the Ethereum consensus layer")
+    delegated_at: Optional[datetime] = Field(None, description="Timestamp of the block at which the corresponding staking transaction was executed")
     delegated_block: Optional[StrictInt] = Field(None, description="Block at which the corresponding staking transaction was executed")
     deposit_tx_sender: Optional[StrictStr] = Field(None, description="Address of the sender of the first deposit transaction")
     execution_fee_recipient: Optional[StrictStr] = Field(None, description="Address of the last recipient of an execution reward")
     withdrawal_credentials: Optional[StrictStr] = Field(None, description="Ethereum withdrawal credentials")
     effective_balance: Optional[StrictStr] = Field(None, description="Effective balance in WEI of the stake as seen by the Ethereum consensus layer")
     balance: Optional[StrictStr] = Field(None, description="Current balance in WEI on the Ethereum consensus layer")
     consensus_rewards: Optional[StrictStr] = Field(None, description="Sum of consensus rewards in WEI earned by this stake")
     execution_rewards: Optional[StrictStr] = Field(None, description="Sum of execution rewards in WEI earned by this stake")
     rewards: Optional[StrictStr] = Field(None, description="Sum of consensus and execution rewards in WEI earned by this stake")
     gross_apy: Optional[float] = Field(None, description="Gross annual percentage yield")
+    is_kiln: Optional[StrictBool] = Field(None, description="Whether this stake is managed by Kiln")
     updated_at: Optional[datetime] = Field(None, description="Last date this data was updated")
-    __properties = ["validator_address", "state", "activated_at", "activated_epoch", "delegated_block", "deposit_tx_sender", "execution_fee_recipient", "withdrawal_credentials", "effective_balance", "balance", "consensus_rewards", "execution_rewards", "rewards", "gross_apy", "updated_at"]
+    __properties = ["validator_address", "validator_index", "state", "activated_at", "activated_epoch", "delegated_at", "delegated_block", "deposit_tx_sender", "execution_fee_recipient", "withdrawal_credentials", "effective_balance", "balance", "consensus_rewards", "execution_rewards", "rewards", "gross_apy", "is_kiln", "updated_at"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -71,14 +74,18 @@
         if self.activated_at is None:
             _dict['activated_at'] = None
 
         # set to None if activated_epoch (nullable) is None
         if self.activated_epoch is None:
             _dict['activated_epoch'] = None
 
+        # set to None if delegated_at (nullable) is None
+        if self.delegated_at is None:
+            _dict['delegated_at'] = None
+
         # set to None if delegated_block (nullable) is None
         if self.delegated_block is None:
             _dict['delegated_block'] = None
 
         # set to None if deposit_tx_sender (nullable) is None
         if self.deposit_tx_sender is None:
             _dict['deposit_tx_sender'] = None
@@ -111,14 +118,18 @@
         if self.rewards is None:
             _dict['rewards'] = None
 
         # set to None if gross_apy (nullable) is None
         if self.gross_apy is None:
             _dict['gross_apy'] = None
 
+        # set to None if is_kiln (nullable) is None
+        if self.is_kiln is None:
+            _dict['is_kiln'] = None
+
         # set to None if updated_at (nullable) is None
         if self.updated_at is None:
             _dict['updated_at'] = None
 
         return _dict
 
     @classmethod
@@ -128,24 +139,27 @@
             return None
 
         if type(obj) is not dict:
             return ETHStake.parse_obj(obj)
 
         _obj = ETHStake.parse_obj({
             "validator_address": obj.get("validator_address"),
+            "validator_index": obj.get("validator_index"),
             "state": obj.get("state"),
             "activated_at": obj.get("activated_at"),
             "activated_epoch": obj.get("activated_epoch"),
+            "delegated_at": obj.get("delegated_at"),
             "delegated_block": obj.get("delegated_block"),
             "deposit_tx_sender": obj.get("deposit_tx_sender"),
             "execution_fee_recipient": obj.get("execution_fee_recipient"),
             "withdrawal_credentials": obj.get("withdrawal_credentials"),
             "effective_balance": obj.get("effective_balance"),
             "balance": obj.get("balance"),
             "consensus_rewards": obj.get("consensus_rewards"),
             "execution_rewards": obj.get("execution_rewards"),
             "rewards": obj.get("rewards"),
             "gross_apy": obj.get("gross_apy"),
+            "is_kiln": obj.get("is_kiln"),
             "updated_at": obj.get("updated_at")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_unsigned_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/eth_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atomtx_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Any, Dict, Optional
 from pydantic import BaseModel, Field, StrictStr
-from kiln_connect.openapi_client.models.ethtx_status_receipt import ETHTxStatusReceipt
 
-class ETHTxStatus(BaseModel):
+class ATOMTxStatus(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     status: Optional[StrictStr] = Field(None, description="Transaction status")
-    receipt: Optional[ETHTxStatusReceipt] = None
+    receipt: Optional[Dict[str, Any]] = Field(None, description="Transaction receipt. Only present if status is success. Object shape can be found [here](https://github.com/cosmos/cosmjs/blob/e8e65aa0c145616ccb58625c32bffe08b46ff574/packages/stargate/src/stargateclient.ts#L67)")
     __properties = ["status", "receipt"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -41,37 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ETHTxStatus:
-        """Create an instance of ETHTxStatus from a JSON string"""
+    def from_json(cls, json_str: str) -> ATOMTxStatus:
+        """Create an instance of ATOMTxStatus from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of receipt
-        if self.receipt:
-            _dict['receipt'] = self.receipt.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ETHTxStatus:
-        """Create an instance of ETHTxStatus from a dict"""
+    def from_dict(cls, obj: dict) -> ATOMTxStatus:
+        """Create an instance of ATOMTxStatus from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ETHTxStatus.parse_obj(obj)
+            return ATOMTxStatus.parse_obj(obj)
 
-        _obj = ETHTxStatus.parse_obj({
+        _obj = ATOMTxStatus.parse_obj({
             "status": obj.get("status"),
-            "receipt": ETHTxStatusReceipt.from_dict(obj.get("receipt")) if obj.get("receipt") is not None else None
+            "receipt": obj.get("receipt")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status_receipt.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_operation_payment.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,93 +13,77 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
+from datetime import datetime
+from typing import Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist
-from kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner import ETHTxStatusReceiptLogsInner
-
-class ETHTxStatusReceipt(BaseModel):
+class XTZOperationPayment(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    status: Optional[StrictBool] = Field(None, description="True if transaction has been confirmed")
-    transaction_hash: Optional[StrictStr] = Field(None, alias="transactionHash", description="Transaction hash")
-    transaction_index: Optional[float] = Field(None, alias="transactionIndex", description="Transaction index")
-    block_hash: Optional[StrictStr] = Field(None, alias="blockHash", description="Block hash")
-    block_number: Optional[float] = Field(None, alias="blockNumber", description="Block number")
-    var_from: Optional[StrictStr] = Field(None, alias="from", description="Transaction from address")
-    to: Optional[StrictStr] = Field(None, description="Transaction to address")
-    contract_address: Optional[StrictStr] = Field(None, alias="contractAddress", description="Contract address called")
-    cumulative_gas_used: Optional[float] = Field(None, alias="cumulativeGasUsed", description="Cumulative gas used")
-    gas_used: Optional[float] = Field(None, alias="gasUsed", description="Gas used")
-    effective_gas_price: Optional[float] = Field(None, alias="effectiveGasPrice", description="Gas price")
-    logs: Optional[conlist(ETHTxStatusReceiptLogsInner)] = Field(None, description="Transaction logs")
-    logs_bloom: Optional[StrictStr] = Field(None, alias="logsBloom")
-    events: Optional[Dict[str, Any]] = None
-    __properties = ["status", "transactionHash", "transactionIndex", "blockHash", "blockNumber", "from", "to", "contractAddress", "cumulativeGasUsed", "gasUsed", "effectiveGasPrice", "logs", "logsBloom", "events"]
+    type: Optional[StrictStr] = Field(None, description="Type of the operation")
+    var_date: Optional[datetime] = Field(None, alias="date", description="When did the operation occur in an RFC3339 format")
+    staker_address: Optional[StrictStr] = Field(None, description="The wallet address for the stake")
+    baker_address: Optional[StrictStr] = Field(None, description="The baker address to which the wallet is staked")
+    sender_address: Optional[StrictStr] = Field(None, description="The address that executed the payment")
+    operation: Optional[StrictStr] = Field(None, description="The operation hash")
+    operation_gas_used: Optional[StrictStr] = Field(None, description="The operation gas used if any")
+    baker_fee: Optional[StrictStr] = Field(None, description="The operation baker fee if applicable")
+    block: Optional[StrictInt] = Field(None, description="The block number in which the operation was included")
+    amount: Optional[StrictStr] = Field(None, description="The reward amount that was paid out")
+    __properties = ["type", "date", "staker_address", "baker_address", "sender_address", "operation", "operation_gas_used", "baker_fee", "block", "amount"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ETHTxStatusReceipt:
-        """Create an instance of ETHTxStatusReceipt from a JSON string"""
+    def from_json(cls, json_str: str) -> XTZOperationPayment:
+        """Create an instance of XTZOperationPayment from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in logs (list)
-        _items = []
-        if self.logs:
-            for _item in self.logs:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['logs'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ETHTxStatusReceipt:
-        """Create an instance of ETHTxStatusReceipt from a dict"""
+    def from_dict(cls, obj: dict) -> XTZOperationPayment:
+        """Create an instance of XTZOperationPayment from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ETHTxStatusReceipt.parse_obj(obj)
+            return XTZOperationPayment.parse_obj(obj)
 
-        _obj = ETHTxStatusReceipt.parse_obj({
-            "status": obj.get("status"),
-            "transaction_hash": obj.get("transactionHash"),
-            "transaction_index": obj.get("transactionIndex"),
-            "block_hash": obj.get("blockHash"),
-            "block_number": obj.get("blockNumber"),
-            "var_from": obj.get("from"),
-            "to": obj.get("to"),
-            "contract_address": obj.get("contractAddress"),
-            "cumulative_gas_used": obj.get("cumulativeGasUsed"),
-            "gas_used": obj.get("gasUsed"),
-            "effective_gas_price": obj.get("effectiveGasPrice"),
-            "logs": [ETHTxStatusReceiptLogsInner.from_dict(_item) for _item in obj.get("logs")] if obj.get("logs") is not None else None,
-            "logs_bloom": obj.get("logsBloom"),
-            "events": obj.get("events")
+        _obj = XTZOperationPayment.parse_obj({
+            "type": obj.get("type"),
+            "var_date": obj.get("date"),
+            "staker_address": obj.get("staker_address"),
+            "baker_address": obj.get("baker_address"),
+            "sender_address": obj.get("sender_address"),
+            "operation": obj.get("operation"),
+            "operation_gas_used": obj.get("operation_gas_used"),
+            "baker_fee": obj.get("baker_fee"),
+            "block": obj.get("block"),
+            "amount": obj.get("amount")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_operation_activation.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,75 +13,67 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
+from datetime import datetime
+from typing import Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist
-
-class ETHTxStatusReceiptLogsInner(BaseModel):
+class XTZOperationActivation(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    address: Optional[StrictStr] = None
-    data: Optional[StrictStr] = None
-    topics: Optional[conlist(StrictStr)] = None
-    log_index: Optional[float] = Field(None, alias="logIndex")
-    transaction_index: Optional[float] = Field(None, alias="transactionIndex")
-    transaction_hash: Optional[StrictStr] = Field(None, alias="transactionHash")
-    block_hash: Optional[StrictStr] = Field(None, alias="blockHash")
-    block_number: Optional[float] = Field(None, alias="blockNumber")
-    removed: Optional[StrictBool] = None
-    __properties = ["address", "data", "topics", "logIndex", "transactionIndex", "transactionHash", "blockHash", "blockNumber", "removed"]
+    type: Optional[StrictStr] = Field(None, description="Type of the operation")
+    var_date: Optional[datetime] = Field(None, alias="date", description="When did the operation occur in an RFC3339 format")
+    staker_address: Optional[StrictStr] = Field(None, description="The wallet address for the stake")
+    baker_address: Optional[StrictStr] = Field(None, description="The baker address to which the wallet is staked")
+    cycle: Optional[StrictInt] = Field(None, description="The cycle at which the stake was active and started earning")
+    __properties = ["type", "date", "staker_address", "baker_address", "cycle"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ETHTxStatusReceiptLogsInner:
-        """Create an instance of ETHTxStatusReceiptLogsInner from a JSON string"""
+    def from_json(cls, json_str: str) -> XTZOperationActivation:
+        """Create an instance of XTZOperationActivation from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ETHTxStatusReceiptLogsInner:
-        """Create an instance of ETHTxStatusReceiptLogsInner from a dict"""
+    def from_dict(cls, obj: dict) -> XTZOperationActivation:
+        """Create an instance of XTZOperationActivation from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ETHTxStatusReceiptLogsInner.parse_obj(obj)
+            return XTZOperationActivation.parse_obj(obj)
 
-        _obj = ETHTxStatusReceiptLogsInner.parse_obj({
-            "address": obj.get("address"),
-            "data": obj.get("data"),
-            "topics": obj.get("topics"),
-            "log_index": obj.get("logIndex"),
-            "transaction_index": obj.get("transactionIndex"),
-            "transaction_hash": obj.get("transactionHash"),
-            "block_hash": obj.get("blockHash"),
-            "block_number": obj.get("blockNumber"),
-            "removed": obj.get("removed")
+        _obj = XTZOperationActivation.parse_obj({
+            "type": obj.get("type"),
+            "var_date": obj.get("date"),
+            "staker_address": obj.get("staker_address"),
+            "baker_address": obj.get("baker_address"),
+            "cycle": obj.get("cycle")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_account_portfolio200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_accounts200_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel
-from kiln_connect.openapi_client.models.account_portfolio import AccountPortfolio
+from typing import List, Optional
+from pydantic import BaseModel, conlist
+from kiln_connect.openapi_client.models.account import Account
 
-class GetAccountPortfolio200Response(BaseModel):
+class GetAccounts200Response(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    data: Optional[AccountPortfolio] = None
+    data: Optional[conlist(Account)] = None
     __properties = ["data"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,36 +40,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetAccountPortfolio200Response:
-        """Create an instance of GetAccountPortfolio200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> GetAccounts200Response:
+        """Create an instance of GetAccounts200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of data
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        _items = []
         if self.data:
-            _dict['data'] = self.data.to_dict()
+            for _item in self.data:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetAccountPortfolio200Response:
-        """Create an instance of GetAccountPortfolio200Response from a dict"""
+    def from_dict(cls, obj: dict) -> GetAccounts200Response:
+        """Create an instance of GetAccounts200Response from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GetAccountPortfolio200Response.parse_obj(obj)
+            return GetAccounts200Response.parse_obj(obj)
 
-        _obj = GetAccountPortfolio200Response.parse_obj({
-            "data": AccountPortfolio.from_dict(obj.get("data")) if obj.get("data") is not None else None
+        _obj = GetAccounts200Response.parse_obj({
+            "data": [Account.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_accounts200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_atom_stakes200_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from kiln_connect.openapi_client.models.account import Account
+from kiln_connect.openapi_client.models.atom_stake import ATOMStake
 
-class GetAccounts200Response(BaseModel):
+class GetAtomStakes200Response(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    data: Optional[conlist(Account)] = None
+    data: Optional[conlist(ATOMStake)] = None
     __properties = ["data"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,16 +40,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetAccounts200Response:
-        """Create an instance of GetAccounts200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> GetAtomStakes200Response:
+        """Create an instance of GetAtomStakes200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -60,20 +60,20 @@
             for _item in self.data:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetAccounts200Response:
-        """Create an instance of GetAccounts200Response from a dict"""
+    def from_dict(cls, obj: dict) -> GetAtomStakes200Response:
+        """Create an instance of GetAtomStakes200Response from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GetAccounts200Response.parse_obj(obj)
+            return GetAtomStakes200Response.parse_obj(obj)
 
-        _obj = GetAccounts200Response.parse_obj({
-            "data": [Account.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = GetAtomStakes200Response.parse_obj({
+            "data": [ATOMStake.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_atom_rewards200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_atom_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_atom_stakes200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_stakes200_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from kiln_connect.openapi_client.models.atom_stake import ATOMStake
+from kiln_connect.openapi_client.models.sol_stake import SOLStake
 
-class GetAtomStakes200Response(BaseModel):
+class GetSolStakes200Response(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    data: Optional[conlist(ATOMStake)] = None
+    data: Optional[conlist(SOLStake)] = None
     __properties = ["data"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,16 +40,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetAtomStakes200Response:
-        """Create an instance of GetAtomStakes200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> GetSolStakes200Response:
+        """Create an instance of GetSolStakes200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -60,20 +60,20 @@
             for _item in self.data:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetAtomStakes200Response:
-        """Create an instance of GetAtomStakes200Response from a dict"""
+    def from_dict(cls, obj: dict) -> GetSolStakes200Response:
+        """Create an instance of GetSolStakes200Response from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GetAtomStakes200Response.parse_obj(obj)
+            return GetSolStakes200Response.parse_obj(obj)
 
-        _obj = GetAtomStakes200Response.parse_obj({
-            "data": [ATOMStake.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = GetSolStakes200Response.parse_obj({
+            "data": [SOLStake.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_operations200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_rewards200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_stakes200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_operations200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_operations200_response_data_inner.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,275 +9,177 @@
     Contact: contact@kiln.fi
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
-import json
 import pprint
 import re  # noqa: F401
 
-from typing import Any, List, Optional
+from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
 from kiln_connect.openapi_client.models.sol_operation_create_account import SOLOperationCreateAccount
 from kiln_connect.openapi_client.models.sol_operation_create_account_with_seed import SOLOperationCreateAccountWithSeed
 from kiln_connect.openapi_client.models.sol_operation_deactivate import SOLOperationDeactivate
 from kiln_connect.openapi_client.models.sol_operation_delegate import SOLOperationDelegate
 from kiln_connect.openapi_client.models.sol_operation_merge import SOLOperationMerge
 from kiln_connect.openapi_client.models.sol_operation_redelegate import SOLOperationRedelegate
 from kiln_connect.openapi_client.models.sol_operation_split import SOLOperationSplit
 from kiln_connect.openapi_client.models.sol_operation_withdraw import SOLOperationWithdraw
 from typing import Any, List
 from pydantic import StrictStr, Field
 
-GETSOLOPERATIONS200RESPONSEDATAINNER_ONE_OF_SCHEMAS = ["SOLOperationCreateAccount", "SOLOperationCreateAccountWithSeed", "SOLOperationDeactivate", "SOLOperationDelegate", "SOLOperationMerge", "SOLOperationRedelegate", "SOLOperationSplit", "SOLOperationWithdraw"]
+GETSOLOPERATIONS200RESPONSEDATAINNER_ANY_OF_SCHEMAS = ["SOLOperationCreateAccount", "SOLOperationCreateAccountWithSeed", "SOLOperationDeactivate", "SOLOperationDelegate", "SOLOperationMerge", "SOLOperationRedelegate", "SOLOperationSplit", "SOLOperationWithdraw"]
 
 class GetSolOperations200ResponseDataInner(BaseModel):
-    """
-    GetSolOperations200ResponseDataInner
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
     """
     # data type: SOLOperationCreateAccountWithSeed
-    oneof_schema_1_validator: Optional[SOLOperationCreateAccountWithSeed] = None
+    anyof_schema_1_validator: Optional[SOLOperationCreateAccountWithSeed] = None
     # data type: SOLOperationCreateAccount
-    oneof_schema_2_validator: Optional[SOLOperationCreateAccount] = None
+    anyof_schema_2_validator: Optional[SOLOperationCreateAccount] = None
     # data type: SOLOperationDelegate
-    oneof_schema_3_validator: Optional[SOLOperationDelegate] = None
+    anyof_schema_3_validator: Optional[SOLOperationDelegate] = None
     # data type: SOLOperationDeactivate
-    oneof_schema_4_validator: Optional[SOLOperationDeactivate] = None
+    anyof_schema_4_validator: Optional[SOLOperationDeactivate] = None
     # data type: SOLOperationRedelegate
-    oneof_schema_5_validator: Optional[SOLOperationRedelegate] = None
+    anyof_schema_5_validator: Optional[SOLOperationRedelegate] = None
     # data type: SOLOperationSplit
-    oneof_schema_6_validator: Optional[SOLOperationSplit] = None
+    anyof_schema_6_validator: Optional[SOLOperationSplit] = None
     # data type: SOLOperationWithdraw
-    oneof_schema_7_validator: Optional[SOLOperationWithdraw] = None
+    anyof_schema_7_validator: Optional[SOLOperationWithdraw] = None
     # data type: SOLOperationMerge
-    oneof_schema_8_validator: Optional[SOLOperationMerge] = None
+    anyof_schema_8_validator: Optional[SOLOperationMerge] = None
     actual_instance: Any
-    one_of_schemas: List[str] = Field(GETSOLOPERATIONS200RESPONSEDATAINNER_ONE_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(GETSOLOPERATIONS200RESPONSEDATAINNER_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
     discriminator_value_class_map = {
     }
 
     @validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
-        instance = cls()
+    def actual_instance_must_validate_anyof(cls, v):
         error_messages = []
-        match = 0
         # validate data type: SOLOperationCreateAccountWithSeed
         if type(v) is not SOLOperationCreateAccountWithSeed:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLOperationCreateAccountWithSeed`")
         else:
-            match += 1
+            return v
 
         # validate data type: SOLOperationCreateAccount
         if type(v) is not SOLOperationCreateAccount:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLOperationCreateAccount`")
         else:
-            match += 1
+            return v
 
         # validate data type: SOLOperationDelegate
         if type(v) is not SOLOperationDelegate:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLOperationDelegate`")
         else:
-            match += 1
+            return v
 
         # validate data type: SOLOperationDeactivate
         if type(v) is not SOLOperationDeactivate:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLOperationDeactivate`")
         else:
-            match += 1
+            return v
 
         # validate data type: SOLOperationRedelegate
         if type(v) is not SOLOperationRedelegate:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLOperationRedelegate`")
         else:
-            match += 1
+            return v
 
         # validate data type: SOLOperationSplit
         if type(v) is not SOLOperationSplit:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLOperationSplit`")
         else:
-            match += 1
+            return v
 
         # validate data type: SOLOperationWithdraw
         if type(v) is not SOLOperationWithdraw:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLOperationWithdraw`")
         else:
-            match += 1
+            return v
 
         # validate data type: SOLOperationMerge
         if type(v) is not SOLOperationMerge:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLOperationMerge`")
         else:
-            match += 1
+            return v
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into GetSolOperations200ResponseDataInner with oneOf schemas: SOLOperationCreateAccount, SOLOperationCreateAccountWithSeed, SOLOperationDeactivate, SOLOperationDelegate, SOLOperationMerge, SOLOperationRedelegate, SOLOperationSplit, SOLOperationWithdraw. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into GetSolOperations200ResponseDataInner with oneOf schemas: SOLOperationCreateAccount, SOLOperationCreateAccountWithSeed, SOLOperationDeactivate, SOLOperationDelegate, SOLOperationMerge, SOLOperationRedelegate, SOLOperationSplit, SOLOperationWithdraw. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into GetSolOperations200ResponseDataInner with anyOf schemas: SOLOperationCreateAccount, SOLOperationCreateAccountWithSeed, SOLOperationDeactivate, SOLOperationDelegate, SOLOperationMerge, SOLOperationRedelegate, SOLOperationSplit, SOLOperationWithdraw. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetSolOperations200ResponseDataInner:
-        return cls.from_json(json.dumps(obj))
-
-    @classmethod
     def from_json(cls, json_str: str) -> GetSolOperations200ResponseDataInner:
         """Returns the object represented by the json string"""
         instance = cls()
         error_messages = []
-        match = 0
-
-        # use oneOf discriminator to lookup the data type
-        _data_type = json.loads(json_str).get("type")
-        if not _data_type:
-            raise ValueError("Failed to lookup data type from the field `type` in the input.")
-
-        # check if data type is `SOLOperationCreateAccount`
-        if _data_type == "SOLOperationCreateAccount":
-            instance.actual_instance = SOLOperationCreateAccount.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationCreateAccountWithSeed`
-        if _data_type == "SOLOperationCreateAccountWithSeed":
-            instance.actual_instance = SOLOperationCreateAccountWithSeed.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationDeactivate`
-        if _data_type == "SOLOperationDeactivate":
-            instance.actual_instance = SOLOperationDeactivate.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationDelegate`
-        if _data_type == "SOLOperationDelegate":
-            instance.actual_instance = SOLOperationDelegate.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationMerge`
-        if _data_type == "SOLOperationMerge":
-            instance.actual_instance = SOLOperationMerge.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationRedelegate`
-        if _data_type == "SOLOperationRedelegate":
-            instance.actual_instance = SOLOperationRedelegate.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationSplit`
-        if _data_type == "SOLOperationSplit":
-            instance.actual_instance = SOLOperationSplit.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationWithdraw`
-        if _data_type == "SOLOperationWithdraw":
-            instance.actual_instance = SOLOperationWithdraw.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationCreateAccount`
-        if _data_type == "create_account":
-            instance.actual_instance = SOLOperationCreateAccount.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationCreateAccountWithSeed`
-        if _data_type == "create_account_with_seed":
-            instance.actual_instance = SOLOperationCreateAccountWithSeed.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationDeactivate`
-        if _data_type == "deactivate":
-            instance.actual_instance = SOLOperationDeactivate.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationDelegate`
-        if _data_type == "delegate":
-            instance.actual_instance = SOLOperationDelegate.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationMerge`
-        if _data_type == "merge":
-            instance.actual_instance = SOLOperationMerge.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationRedelegate`
-        if _data_type == "redelegate":
-            instance.actual_instance = SOLOperationRedelegate.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationSplit`
-        if _data_type == "split":
-            instance.actual_instance = SOLOperationSplit.from_json(json_str)
-            return instance
-
-        # check if data type is `SOLOperationWithdraw`
-        if _data_type == "withdraw":
-            instance.actual_instance = SOLOperationWithdraw.from_json(json_str)
-            return instance
-
-        # deserialize data into SOLOperationCreateAccountWithSeed
+        # anyof_schema_1_validator: Optional[SOLOperationCreateAccountWithSeed] = None
         try:
             instance.actual_instance = SOLOperationCreateAccountWithSeed.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into SOLOperationCreateAccount
+             error_messages.append(str(e))
+        # anyof_schema_2_validator: Optional[SOLOperationCreateAccount] = None
         try:
             instance.actual_instance = SOLOperationCreateAccount.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into SOLOperationDelegate
+             error_messages.append(str(e))
+        # anyof_schema_3_validator: Optional[SOLOperationDelegate] = None
         try:
             instance.actual_instance = SOLOperationDelegate.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into SOLOperationDeactivate
+             error_messages.append(str(e))
+        # anyof_schema_4_validator: Optional[SOLOperationDeactivate] = None
         try:
             instance.actual_instance = SOLOperationDeactivate.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into SOLOperationRedelegate
+             error_messages.append(str(e))
+        # anyof_schema_5_validator: Optional[SOLOperationRedelegate] = None
         try:
             instance.actual_instance = SOLOperationRedelegate.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into SOLOperationSplit
+             error_messages.append(str(e))
+        # anyof_schema_6_validator: Optional[SOLOperationSplit] = None
         try:
             instance.actual_instance = SOLOperationSplit.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into SOLOperationWithdraw
+             error_messages.append(str(e))
+        # anyof_schema_7_validator: Optional[SOLOperationWithdraw] = None
         try:
             instance.actual_instance = SOLOperationWithdraw.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into SOLOperationMerge
+             error_messages.append(str(e))
+        # anyof_schema_8_validator: Optional[SOLOperationMerge] = None
         try:
             instance.actual_instance = SOLOperationMerge.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
+             error_messages.append(str(e))
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into GetSolOperations200ResponseDataInner with oneOf schemas: SOLOperationCreateAccount, SOLOperationCreateAccountWithSeed, SOLOperationDeactivate, SOLOperationDelegate, SOLOperationMerge, SOLOperationRedelegate, SOLOperationSplit, SOLOperationWithdraw. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into GetSolOperations200ResponseDataInner with oneOf schemas: SOLOperationCreateAccount, SOLOperationCreateAccountWithSeed, SOLOperationDeactivate, SOLOperationDelegate, SOLOperationMerge, SOLOperationRedelegate, SOLOperationSplit, SOLOperationWithdraw. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into GetSolOperations200ResponseDataInner with anyOf schemas: SOLOperationCreateAccount, SOLOperationCreateAccountWithSeed, SOLOperationDeactivate, SOLOperationDelegate, SOLOperationMerge, SOLOperationRedelegate, SOLOperationSplit, SOLOperationWithdraw. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is not None:
             return self.actual_instance.to_json()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_rewards200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,97 +9,84 @@
     Contact: contact@kiln.fi
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
-import json
 import pprint
 import re  # noqa: F401
 
-from typing import Any, List, Optional
+from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
 from kiln_connect.openapi_client.models.sol_reward_by_day import SOLRewardByDay
 from kiln_connect.openapi_client.models.sol_reward_by_epoch import SOLRewardByEpoch
 from typing import Any, List
 from pydantic import StrictStr, Field
 
-GETSOLREWARDS200RESPONSEDATAINNER_ONE_OF_SCHEMAS = ["SOLRewardByDay", "SOLRewardByEpoch"]
+GETSOLREWARDS200RESPONSEDATAINNER_ANY_OF_SCHEMAS = ["SOLRewardByDay", "SOLRewardByEpoch"]
 
 class GetSolRewards200ResponseDataInner(BaseModel):
-    """
-    GetSolRewards200ResponseDataInner
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
     """
     # data type: SOLRewardByEpoch
-    oneof_schema_1_validator: Optional[SOLRewardByEpoch] = None
+    anyof_schema_1_validator: Optional[SOLRewardByEpoch] = None
     # data type: SOLRewardByDay
-    oneof_schema_2_validator: Optional[SOLRewardByDay] = None
+    anyof_schema_2_validator: Optional[SOLRewardByDay] = None
     actual_instance: Any
-    one_of_schemas: List[str] = Field(GETSOLREWARDS200RESPONSEDATAINNER_ONE_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(GETSOLREWARDS200RESPONSEDATAINNER_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
     @validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
-        instance = cls()
+    def actual_instance_must_validate_anyof(cls, v):
         error_messages = []
-        match = 0
         # validate data type: SOLRewardByEpoch
         if type(v) is not SOLRewardByEpoch:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLRewardByEpoch`")
         else:
-            match += 1
+            return v
 
         # validate data type: SOLRewardByDay
         if type(v) is not SOLRewardByDay:
             error_messages.append(f"Error! Input type `{type(v)}` is not `SOLRewardByDay`")
         else:
-            match += 1
+            return v
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into GetSolRewards200ResponseDataInner with oneOf schemas: SOLRewardByDay, SOLRewardByEpoch. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into GetSolRewards200ResponseDataInner with oneOf schemas: SOLRewardByDay, SOLRewardByEpoch. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into GetSolRewards200ResponseDataInner with anyOf schemas: SOLRewardByDay, SOLRewardByEpoch. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetSolRewards200ResponseDataInner:
-        return cls.from_json(json.dumps(obj))
-
-    @classmethod
     def from_json(cls, json_str: str) -> GetSolRewards200ResponseDataInner:
         """Returns the object represented by the json string"""
         instance = cls()
         error_messages = []
-        match = 0
-
-        # deserialize data into SOLRewardByEpoch
+        # anyof_schema_1_validator: Optional[SOLRewardByEpoch] = None
         try:
             instance.actual_instance = SOLRewardByEpoch.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into SOLRewardByDay
+             error_messages.append(str(e))
+        # anyof_schema_2_validator: Optional[SOLRewardByDay] = None
         try:
             instance.actual_instance = SOLRewardByDay.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
+             error_messages.append(str(e))
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into GetSolRewards200ResponseDataInner with oneOf schemas: SOLRewardByDay, SOLRewardByEpoch. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into GetSolRewards200ResponseDataInner with oneOf schemas: SOLRewardByDay, SOLRewardByEpoch. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into GetSolRewards200ResponseDataInner with anyOf schemas: SOLRewardByDay, SOLRewardByEpoch. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is not None:
             return self.actual_instance.to_json()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_stakes200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, conlist
-from kiln_connect.openapi_client.models.sol_stake import SOLStake
+from kiln_connect.openapi_client.models.xtz_stake import XTZStake
 
-class GetSolStakes200Response(BaseModel):
+class GetXtzStakes200Response(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    data: Optional[conlist(SOLStake)] = None
+    data: Optional[conlist(XTZStake)] = None
     __properties = ["data"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,16 +40,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetSolStakes200Response:
-        """Create an instance of GetSolStakes200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> GetXtzStakes200Response:
+        """Create an instance of GetXtzStakes200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -60,20 +60,20 @@
             for _item in self.data:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetSolStakes200Response:
-        """Create an instance of GetSolStakes200Response from a dict"""
+    def from_dict(cls, obj: dict) -> GetXtzStakes200Response:
+        """Create an instance of GetXtzStakes200Response from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GetSolStakes200Response.parse_obj(obj)
+            return GetXtzStakes200Response.parse_obj(obj)
 
-        _obj = GetSolStakes200Response.parse_obj({
-            "data": [SOLStake.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = GetXtzStakes200Response.parse_obj({
+            "data": [XTZStake.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_operations200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,97 +9,84 @@
     Contact: contact@kiln.fi
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
-import json
 import pprint
 import re  # noqa: F401
 
-from typing import Any, List, Optional
+from typing import Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
 from kiln_connect.openapi_client.models.xtz_cycle_reward import XTZCycleReward
 from kiln_connect.openapi_client.models.xtz_daily_reward import XTZDailyReward
 from typing import Any, List
 from pydantic import StrictStr, Field
 
-GETXTZREWARDS200RESPONSEDATAINNER_ONE_OF_SCHEMAS = ["XTZCycleReward", "XTZDailyReward"]
+GETXTZREWARDS200RESPONSEDATAINNER_ANY_OF_SCHEMAS = ["XTZCycleReward", "XTZDailyReward"]
 
 class GetXtzRewards200ResponseDataInner(BaseModel):
-    """
-    GetXtzRewards200ResponseDataInner
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
     """
     # data type: XTZDailyReward
-    oneof_schema_1_validator: Optional[XTZDailyReward] = None
+    anyof_schema_1_validator: Optional[XTZDailyReward] = None
     # data type: XTZCycleReward
-    oneof_schema_2_validator: Optional[XTZCycleReward] = None
+    anyof_schema_2_validator: Optional[XTZCycleReward] = None
     actual_instance: Any
-    one_of_schemas: List[str] = Field(GETXTZREWARDS200RESPONSEDATAINNER_ONE_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(GETXTZREWARDS200RESPONSEDATAINNER_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
     @validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
-        instance = cls()
+    def actual_instance_must_validate_anyof(cls, v):
         error_messages = []
-        match = 0
         # validate data type: XTZDailyReward
         if type(v) is not XTZDailyReward:
             error_messages.append(f"Error! Input type `{type(v)}` is not `XTZDailyReward`")
         else:
-            match += 1
+            return v
 
         # validate data type: XTZCycleReward
         if type(v) is not XTZCycleReward:
             error_messages.append(f"Error! Input type `{type(v)}` is not `XTZCycleReward`")
         else:
-            match += 1
+            return v
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into GetXtzRewards200ResponseDataInner with oneOf schemas: XTZCycleReward, XTZDailyReward. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into GetXtzRewards200ResponseDataInner with oneOf schemas: XTZCycleReward, XTZDailyReward. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into GetXtzRewards200ResponseDataInner with anyOf schemas: XTZCycleReward, XTZDailyReward. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetXtzRewards200ResponseDataInner:
-        return cls.from_json(json.dumps(obj))
-
-    @classmethod
     def from_json(cls, json_str: str) -> GetXtzRewards200ResponseDataInner:
         """Returns the object represented by the json string"""
         instance = cls()
         error_messages = []
-        match = 0
-
-        # deserialize data into XTZDailyReward
+        # anyof_schema_1_validator: Optional[XTZDailyReward] = None
         try:
             instance.actual_instance = XTZDailyReward.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into XTZCycleReward
+             error_messages.append(str(e))
+        # anyof_schema_2_validator: Optional[XTZCycleReward] = None
         try:
             instance.actual_instance = XTZCycleReward.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
+             error_messages.append(str(e))
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into GetXtzRewards200ResponseDataInner with oneOf schemas: XTZCycleReward, XTZDailyReward. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into GetXtzRewards200ResponseDataInner with oneOf schemas: XTZCycleReward, XTZDailyReward. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into GetXtzRewards200ResponseDataInner with anyOf schemas: XTZCycleReward, XTZDailyReward. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is not None:
             return self.actual_instance.to_json()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_stakes201_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, conlist
-from kiln_connect.openapi_client.models.xtz_stake import XTZStake
+from typing import Optional
+from pydantic import BaseModel
+from kiln_connect.openapi_client.models.core_stake import CoreStake
 
-class GetXtzStakes200Response(BaseModel):
+class PostEthStakes201Response(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    data: Optional[conlist(XTZStake)] = None
+    data: Optional[CoreStake] = None
     __properties = ["data"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,40 +40,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetXtzStakes200Response:
-        """Create an instance of GetXtzStakes200Response from a JSON string"""
+    def from_json(cls, json_str: str) -> PostEthStakes201Response:
+        """Create an instance of PostEthStakes201Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
+        # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetXtzStakes200Response:
-        """Create an instance of GetXtzStakes200Response from a dict"""
+    def from_dict(cls, obj: dict) -> PostEthStakes201Response:
+        """Create an instance of PostEthStakes201Response from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GetXtzStakes200Response.parse_obj(obj)
+            return PostEthStakes201Response.parse_obj(obj)
 
-        _obj = GetXtzStakes200Response.parse_obj({
-            "data": [XTZStake.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None
+        _obj = PostEthStakes201Response.parse_obj({
+            "data": CoreStake.from_dict(obj.get("data")) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_account201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_account201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_keys201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_keys201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,100 +9,84 @@
     Contact: contact@kiln.fi
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import annotations
 from inspect import getfullargspec
-import json
 import pprint
 import re  # noqa: F401
 
-from typing import Any, List, Optional
+from typing import List, Optional
 from pydantic import BaseModel, Field, StrictStr, ValidationError, conlist, validator
 from kiln_connect.openapi_client.models.eth_post_keys_batch_response import ETHPostKeysBatchResponse
 from kiln_connect.openapi_client.models.eth_post_keys_cli_response_inner import ETHPostKeysCliResponseInner
 from typing import Any, List
 from pydantic import StrictStr, Field
 
-POSTETHKEYS201RESPONSEDATA_ONE_OF_SCHEMAS = ["ETHPostKeysBatchResponse", "List[ETHPostKeysCliResponseInner]"]
+POSTETHKEYS201RESPONSEDATA_ANY_OF_SCHEMAS = ["ETHPostKeysBatchResponse", "List[ETHPostKeysCliResponseInner]"]
 
 class PostEthKeys201ResponseData(BaseModel):
-    """
-    PostEthKeys201ResponseData
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
     """
     # data type: List[ETHPostKeysCliResponseInner]
-    oneof_schema_1_validator: Optional[conlist(ETHPostKeysCliResponseInner)] = None
+    anyof_schema_1_validator: Optional[conlist(ETHPostKeysCliResponseInner)] = None
     # data type: ETHPostKeysBatchResponse
-    oneof_schema_2_validator: Optional[ETHPostKeysBatchResponse] = None
+    anyof_schema_2_validator: Optional[ETHPostKeysBatchResponse] = None
     actual_instance: Any
-    one_of_schemas: List[str] = Field(POSTETHKEYS201RESPONSEDATA_ONE_OF_SCHEMAS, const=True)
+    any_of_schemas: List[str] = Field(POSTETHKEYS201RESPONSEDATA_ANY_OF_SCHEMAS, const=True)
 
     class Config:
         validate_assignment = True
 
     @validator('actual_instance')
-    def actual_instance_must_validate_oneof(cls, v):
-        instance = cls()
+    def actual_instance_must_validate_anyof(cls, v):
         error_messages = []
-        match = 0
         # validate data type: List[ETHPostKeysCliResponseInner]
-        try:
-            instance.oneof_schema_1_validator = v
-            match += 1
-        except ValidationError as e:
-            error_messages.append(str(e))
+        if type(v) is not List[ETHPostKeysCliResponseInner]:
+            error_messages.append(f"Error! Input type `{type(v)}` is not `List[ETHPostKeysCliResponseInner]`")
+        else:
+            return v
+
         # validate data type: ETHPostKeysBatchResponse
         if type(v) is not ETHPostKeysBatchResponse:
             error_messages.append(f"Error! Input type `{type(v)}` is not `ETHPostKeysBatchResponse`")
         else:
-            match += 1
+            return v
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into PostEthKeys201ResponseData with oneOf schemas: ETHPostKeysBatchResponse, List[ETHPostKeysCliResponseInner]. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into PostEthKeys201ResponseData with oneOf schemas: ETHPostKeysBatchResponse, List[ETHPostKeysCliResponseInner]. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into PostEthKeys201ResponseData with anyOf schemas: ETHPostKeysBatchResponse, List[ETHPostKeysCliResponseInner]. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PostEthKeys201ResponseData:
-        return cls.from_json(json.dumps(obj))
-
-    @classmethod
     def from_json(cls, json_str: str) -> PostEthKeys201ResponseData:
         """Returns the object represented by the json string"""
         instance = cls()
         error_messages = []
-        match = 0
-
-        # deserialize data into List[ETHPostKeysCliResponseInner]
+        # anyof_schema_1_validator: Optional[conlist(ETHPostKeysCliResponseInner)] = None
         try:
-            # validation
-            instance.oneof_schema_1_validator = json.loads(json_str)
-            # assign value to actual_instance
-            instance.actual_instance = instance.oneof_schema_1_validator
-            match += 1
+            instance.actual_instance = List[ETHPostKeysCliResponseInner].from_json(json_str)
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
-        # deserialize data into ETHPostKeysBatchResponse
+             error_messages.append(str(e))
+        # anyof_schema_2_validator: Optional[ETHPostKeysBatchResponse] = None
         try:
             instance.actual_instance = ETHPostKeysBatchResponse.from_json(json_str)
-            match += 1
+            return instance
         except ValidationError as e:
-            error_messages.append(str(e))
+             error_messages.append(str(e))
 
-        if match > 1:
-            # more than 1 match
-            raise ValueError("Multiple matches found when deserializing the JSON string into PostEthKeys201ResponseData with oneOf schemas: ETHPostKeysBatchResponse, List[ETHPostKeysCliResponseInner]. Details: " + ", ".join(error_messages))
-        elif match == 0:
+        if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into PostEthKeys201ResponseData with oneOf schemas: ETHPostKeysBatchResponse, List[ETHPostKeysCliResponseInner]. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into PostEthKeys201ResponseData with anyOf schemas: ETHPostKeysBatchResponse, List[ETHPostKeysCliResponseInner]. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is not None:
             return self.actual_instance.to_json()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_stakes201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/get_account_portfolio200_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
-from kiln_connect.openapi_client.models.core_stake import CoreStake
+from kiln_connect.openapi_client.models.portfolio import Portfolio
 
-class PostSolStakes201Response(BaseModel):
+class GetAccountPortfolio200Response(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    data: Optional[CoreStake] = None
+    data: Optional[Portfolio] = None
     __properties = ["data"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,36 +40,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PostSolStakes201Response:
-        """Create an instance of PostSolStakes201Response from a JSON string"""
+    def from_json(cls, json_str: str) -> GetAccountPortfolio200Response:
+        """Create an instance of GetAccountPortfolio200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PostSolStakes201Response:
-        """Create an instance of PostSolStakes201Response from a dict"""
+    def from_dict(cls, obj: dict) -> GetAccountPortfolio200Response:
+        """Create an instance of GetAccountPortfolio200Response from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return PostSolStakes201Response.parse_obj(obj)
+            return GetAccountPortfolio200Response.parse_obj(obj)
 
-        _obj = PostSolStakes201Response.parse_obj({
-            "data": CoreStake.from_dict(obj.get("data")) if obj.get("data") is not None else None
+        _obj = GetAccountPortfolio200Response.parse_obj({
+            "data": Portfolio.from_dict(obj.get("data")) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_broadcast_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_broadcast_tx.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
 class SOLBroadcastTx(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    tx_hash: Optional[StrictStr] = None
+    tx_hash: Optional[StrictStr] = Field(None, description="Hash of the transaction")
     __properties = ["tx_hash"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_broadcast_tx_payload.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
-class SOLBroadcastTxPayload(BaseModel):
+class ATOMBroadcastTxPayload(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    tx_serialized: StrictStr = ...
+    tx_serialized: StrictStr = Field(..., description="Signed transaction serialized in hex")
     __properties = ["tx_serialized"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,33 +39,33 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SOLBroadcastTxPayload:
-        """Create an instance of SOLBroadcastTxPayload from a JSON string"""
+    def from_json(cls, json_str: str) -> ATOMBroadcastTxPayload:
+        """Create an instance of ATOMBroadcastTxPayload from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SOLBroadcastTxPayload:
-        """Create an instance of SOLBroadcastTxPayload from a dict"""
+    def from_dict(cls, obj: dict) -> ATOMBroadcastTxPayload:
+        """Create an instance of ATOMBroadcastTxPayload from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SOLBroadcastTxPayload.parse_obj(obj)
+            return ATOMBroadcastTxPayload.parse_obj(obj)
 
-        _obj = SOLBroadcastTxPayload.parse_obj({
+        _obj = ATOMBroadcastTxPayload.parse_obj({
             "tx_serialized": obj.get("tx_serialized")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_network_stats.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/atom_network_stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,63 +13,67 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field
 
-class SOLNetworkStats(BaseModel):
+class ATOMNetworkStats(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
+    nb_validators: Optional[float] = Field(None, description="Number of validators in the network")
     network_gross_apy: Optional[float] = Field(None, description="Gross annual percentage yield")
-    supply_staked_percent: Optional[float] = Field(None, description="Supply of Solana currently staked")
-    nb_validators: Optional[float] = Field(None, description="Number of active stakes")
-    __properties = ["network_gross_apy", "supply_staked_percent", "nb_validators"]
+    supply_staked_percent: Optional[float] = Field(None, description="Supply of ATOM currently staked")
+    atom_price_usd: Optional[float] = Field(None, description="Price of ATOM in USD")
+    updated_at: Optional[datetime] = Field(None, description="Last date this data was updated")
+    __properties = ["nb_validators", "network_gross_apy", "supply_staked_percent", "atom_price_usd", "updated_at"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SOLNetworkStats:
-        """Create an instance of SOLNetworkStats from a JSON string"""
+    def from_json(cls, json_str: str) -> ATOMNetworkStats:
+        """Create an instance of ATOMNetworkStats from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SOLNetworkStats:
-        """Create an instance of SOLNetworkStats from a dict"""
+    def from_dict(cls, obj: dict) -> ATOMNetworkStats:
+        """Create an instance of ATOMNetworkStats from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SOLNetworkStats.parse_obj(obj)
+            return ATOMNetworkStats.parse_obj(obj)
 
-        _obj = SOLNetworkStats.parse_obj({
+        _obj = ATOMNetworkStats.parse_obj({
+            "nb_validators": obj.get("nb_validators"),
             "network_gross_apy": obj.get("network_gross_apy"),
             "supply_staked_percent": obj.get("supply_staked_percent"),
-            "nb_validators": obj.get("nb_validators")
+            "atom_price_usd": obj.get("atom_price_usd"),
+            "updated_at": obj.get("updated_at")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_create_account.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_create_account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_create_account_with_seed.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_create_account_with_seed.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_deactivate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_deactivate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_delegate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_delegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_merge.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_merge.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_redelegate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_redelegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_split.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_split.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_withdraw.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_operation_withdraw.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_post_stakes_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_post_stakes_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_prepared_tx.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,60 +14,58 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List
-from pydantic import BaseModel, StrictStr, conlist
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr
 
-class SOLPrepareTxPayload(BaseModel):
+class SOLPreparedTx(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    unsigned_tx_serialized: StrictStr = ...
-    signatures: conlist(StrictStr) = ...
-    __properties = ["unsigned_tx_serialized", "signatures"]
+    signed_tx_serialized: Optional[StrictStr] = Field(None, description="Hex encoded signed transaction")
+    __properties = ["signed_tx_serialized"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SOLPrepareTxPayload:
-        """Create an instance of SOLPrepareTxPayload from a JSON string"""
+    def from_json(cls, json_str: str) -> SOLPreparedTx:
+        """Create an instance of SOLPreparedTx from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SOLPrepareTxPayload:
-        """Create an instance of SOLPrepareTxPayload from a dict"""
+    def from_dict(cls, obj: dict) -> SOLPreparedTx:
+        """Create an instance of SOLPreparedTx from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SOLPrepareTxPayload.parse_obj(obj)
+            return SOLPreparedTx.parse_obj(obj)
 
-        _obj = SOLPrepareTxPayload.parse_obj({
-            "unsigned_tx_serialized": obj.get("unsigned_tx_serialized"),
-            "signatures": obj.get("signatures")
+        _obj = SOLPreparedTx.parse_obj({
+            "signed_tx_serialized": obj.get("signed_tx_serialized")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_prepared_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_signed_tx.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictStr
 
-class SOLPreparedTx(BaseModel):
+class ADASignedTx(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    signed_tx_serialized: Optional[StrictStr] = None
+    signed_tx_serialized: Optional[StrictStr] = Field(None, description="Signed serialized transaction")
     __properties = ["signed_tx_serialized"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,33 +39,33 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SOLPreparedTx:
-        """Create an instance of SOLPreparedTx from a JSON string"""
+    def from_json(cls, json_str: str) -> ADASignedTx:
+        """Create an instance of ADASignedTx from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SOLPreparedTx:
-        """Create an instance of SOLPreparedTx from a dict"""
+    def from_dict(cls, obj: dict) -> ADASignedTx:
+        """Create an instance of ADASignedTx from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SOLPreparedTx.parse_obj(obj)
+            return ADASignedTx.parse_obj(obj)
 
-        _obj = SOLPreparedTx.parse_obj({
+        _obj = ADASignedTx.parse_obj({
             "signed_tx_serialized": obj.get("signed_tx_serialized")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_reward_by_day.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_reward_by_day.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_reward_by_epoch.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_reward_by_epoch.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_unsigned_tx.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,60 +14,62 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, StrictStr
+from typing import Any, Dict, List, Optional
+from pydantic import BaseModel, Field, StrictStr, conlist
 
-class SOLStakeTx(BaseModel):
+class ADAUnsignedTx(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    unsigned_tx_hash: Optional[StrictStr] = None
-    unsigned_tx_serialized: Optional[StrictStr] = None
-    __properties = ["unsigned_tx_hash", "unsigned_tx_serialized"]
+    unsigned_tx_hash: Optional[StrictStr] = Field(None, description="Hash of the unsigned transaction")
+    unsigned_tx_serialized: Optional[StrictStr] = Field(None, description="Unsigned serialized transaction")
+    inputs: Optional[conlist(Dict[str, Any])] = Field(None, description="List of inputs to spend")
+    __properties = ["unsigned_tx_hash", "unsigned_tx_serialized", "inputs"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SOLStakeTx:
-        """Create an instance of SOLStakeTx from a JSON string"""
+    def from_json(cls, json_str: str) -> ADAUnsignedTx:
+        """Create an instance of ADAUnsignedTx from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SOLStakeTx:
-        """Create an instance of SOLStakeTx from a dict"""
+    def from_dict(cls, obj: dict) -> ADAUnsignedTx:
+        """Create an instance of ADAUnsignedTx from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SOLStakeTx.parse_obj(obj)
+            return ADAUnsignedTx.parse_obj(obj)
 
-        _obj = SOLStakeTx.parse_obj({
+        _obj = ADAUnsignedTx.parse_obj({
             "unsigned_tx_hash": obj.get("unsigned_tx_hash"),
-            "unsigned_tx_serialized": obj.get("unsigned_tx_serialized")
+            "unsigned_tx_serialized": obj.get("unsigned_tx_serialized"),
+            "inputs": obj.get("inputs")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_stake_tx_payload.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
 class SOLStakeTxPayload(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     account_id: StrictStr = Field(..., description="Kiln Account ID")
     wallet: StrictStr = Field(..., description="Wallet address")
     amount_lamports: StrictStr = Field(..., description="Amount in lamports (minimum value must be 10000001)")
     vote_account_address: StrictStr = Field(..., description="Vote account address")
-    __properties = ["account_id", "wallet", "amount_lamports", "vote_account_address"]
+    memo: Optional[StrictStr] = Field(None, description="Custom message to send as a memo in the transaction")
+    __properties = ["account_id", "wallet", "amount_lamports", "vote_account_address", "memo"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -67,11 +68,12 @@
         if type(obj) is not dict:
             return SOLStakeTxPayload.parse_obj(obj)
 
         _obj = SOLStakeTxPayload.parse_obj({
             "account_id": obj.get("account_id"),
             "wallet": obj.get("wallet"),
             "amount_lamports": obj.get("amount_lamports"),
-            "vote_account_address": obj.get("vote_account_address")
+            "vote_account_address": obj.get("vote_account_address"),
+            "memo": obj.get("memo")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/soltx_status.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/adatx_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class SOLTxStatus(BaseModel):
+class ADATxStatus(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     status: Optional[StrictStr] = Field(None, description="Transaction status")
-    receipt: Optional[Dict[str, Any]] = None
+    receipt: Optional[Dict[str, Any]] = Field(None, description="Transaction receipt. Object shape can be found [here](https://github.com/blockfrost/openapi/blob/master/src/generated-types.ts#L4493)")
     __properties = ["status", "receipt"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,34 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SOLTxStatus:
-        """Create an instance of SOLTxStatus from a JSON string"""
+    def from_json(cls, json_str: str) -> ADATxStatus:
+        """Create an instance of ADATxStatus from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SOLTxStatus:
-        """Create an instance of SOLTxStatus from a dict"""
+    def from_dict(cls, obj: dict) -> ADATxStatus:
+        """Create an instance of ADATxStatus from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SOLTxStatus.parse_obj(obj)
+            return ADATxStatus.parse_obj(obj)
 
-        _obj = SOLTxStatus.parse_obj({
+        _obj = ADATxStatus.parse_obj({
             "status": obj.get("status"),
             "receipt": obj.get("receipt")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     account_id: StrictStr = Field(..., description="Kiln Account ID to stake into")
     wallet: StrictStr = Field(..., description="Wallet that you wish to delegate from")
-    baker_address: StrictStr = Field(..., description="Baker address to delegate to. Defaults to Kiln's baker")
+    baker_address: StrictStr = Field(..., description="Baker address to delegate to.")
     __properties = ["account_id", "wallet", "baker_address"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_cycle_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_cycle_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_daily_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_daily_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_network_stats.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_activation.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_matic_prepare_tx201_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,67 +13,63 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel
+from kiln_connect.openapi_client.models.matic_signed_tx import MATICSignedTx
 
-class XTZOperationActivation(BaseModel):
+class PostMaticPrepareTx201Response(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    type: Optional[StrictStr] = Field(None, description="Type of the operation")
-    var_date: Optional[datetime] = Field(None, alias="date", description="When did the operation occur in an RFC3339 format")
-    staker_address: Optional[StrictStr] = Field(None, description="The wallet address for the stake")
-    baker_address: Optional[StrictStr] = Field(None, description="The baker address to which the wallet is staked")
-    cycle: Optional[StrictInt] = Field(None, description="The cycle at which the stake was active and started earning")
-    __properties = ["type", "date", "staker_address", "baker_address", "cycle"]
+    data: Optional[MATICSignedTx] = None
+    __properties = ["data"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> XTZOperationActivation:
-        """Create an instance of XTZOperationActivation from a JSON string"""
+    def from_json(cls, json_str: str) -> PostMaticPrepareTx201Response:
+        """Create an instance of PostMaticPrepareTx201Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> XTZOperationActivation:
-        """Create an instance of XTZOperationActivation from a dict"""
+    def from_dict(cls, obj: dict) -> PostMaticPrepareTx201Response:
+        """Create an instance of PostMaticPrepareTx201Response from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return XTZOperationActivation.parse_obj(obj)
+            return PostMaticPrepareTx201Response.parse_obj(obj)
 
-        _obj = XTZOperationActivation.parse_obj({
-            "type": obj.get("type"),
-            "var_date": obj.get("date"),
-            "staker_address": obj.get("staker_address"),
-            "baker_address": obj.get("baker_address"),
-            "cycle": obj.get("cycle")
+        _obj = PostMaticPrepareTx201Response.parse_obj({
+            "data": MATICSignedTx.from_dict(obj.get("data")) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_delegate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_operation_delegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_payment.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_operation_undelegate.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,73 +17,69 @@
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class XTZOperationPayment(BaseModel):
+class XTZOperationUndelegate(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     type: Optional[StrictStr] = Field(None, description="Type of the operation")
     var_date: Optional[datetime] = Field(None, alias="date", description="When did the operation occur in an RFC3339 format")
     staker_address: Optional[StrictStr] = Field(None, description="The wallet address for the stake")
     baker_address: Optional[StrictStr] = Field(None, description="The baker address to which the wallet is staked")
-    sender_address: Optional[StrictStr] = Field(None, description="The address that executed the payment")
     operation: Optional[StrictStr] = Field(None, description="The operation hash")
     operation_gas_used: Optional[StrictStr] = Field(None, description="The operation gas used if any")
     baker_fee: Optional[StrictStr] = Field(None, description="The operation baker fee if applicable")
     block: Optional[StrictInt] = Field(None, description="The block number in which the operation was included")
-    amount: Optional[StrictStr] = Field(None, description="The reward amount that was paid out")
-    __properties = ["type", "date", "staker_address", "baker_address", "sender_address", "operation", "operation_gas_used", "baker_fee", "block", "amount"]
+    __properties = ["type", "date", "staker_address", "baker_address", "operation", "operation_gas_used", "baker_fee", "block"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> XTZOperationPayment:
-        """Create an instance of XTZOperationPayment from a JSON string"""
+    def from_json(cls, json_str: str) -> XTZOperationUndelegate:
+        """Create an instance of XTZOperationUndelegate from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> XTZOperationPayment:
-        """Create an instance of XTZOperationPayment from a dict"""
+    def from_dict(cls, obj: dict) -> XTZOperationUndelegate:
+        """Create an instance of XTZOperationUndelegate from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return XTZOperationPayment.parse_obj(obj)
+            return XTZOperationUndelegate.parse_obj(obj)
 
-        _obj = XTZOperationPayment.parse_obj({
+        _obj = XTZOperationUndelegate.parse_obj({
             "type": obj.get("type"),
             "var_date": obj.get("date"),
             "staker_address": obj.get("staker_address"),
             "baker_address": obj.get("baker_address"),
-            "sender_address": obj.get("sender_address"),
             "operation": obj.get("operation"),
             "operation_gas_used": obj.get("operation_gas_used"),
             "baker_fee": obj.get("baker_fee"),
-            "block": obj.get("block"),
-            "amount": obj.get("amount")
+            "block": obj.get("block")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_undelegate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/ada_prepare_tx_payload.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,73 +13,69 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class XTZOperationUndelegate(BaseModel):
+from typing import List
+from pydantic import BaseModel, Field, StrictStr, conlist
+from kiln_connect.openapi_client.models.ada_prepare_tx_payload_signed_messages_inner import ADAPrepareTxPayloadSignedMessagesInner
+
+class ADAPrepareTxPayload(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    type: Optional[StrictStr] = Field(None, description="Type of the operation")
-    var_date: Optional[datetime] = Field(None, alias="date", description="When did the operation occur in an RFC3339 format")
-    staker_address: Optional[StrictStr] = Field(None, description="The wallet address for the stake")
-    baker_address: Optional[StrictStr] = Field(None, description="The baker address to which the wallet is staked")
-    operation: Optional[StrictStr] = Field(None, description="The operation hash")
-    operation_gas_used: Optional[StrictStr] = Field(None, description="The operation gas used if any")
-    baker_fee: Optional[StrictStr] = Field(None, description="The operation baker fee if applicable")
-    block: Optional[StrictInt] = Field(None, description="The block number in which the operation was included")
-    __properties = ["type", "date", "staker_address", "baker_address", "operation", "operation_gas_used", "baker_fee", "block"]
+    unsigned_tx_serialized: StrictStr = Field(..., description="Unsigned serialized transaction")
+    signed_messages: conlist(ADAPrepareTxPayloadSignedMessagesInner) = Field(..., description="Signed messages")
+    __properties = ["unsigned_tx_serialized", "signed_messages"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> XTZOperationUndelegate:
-        """Create an instance of XTZOperationUndelegate from a JSON string"""
+    def from_json(cls, json_str: str) -> ADAPrepareTxPayload:
+        """Create an instance of ADAPrepareTxPayload from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in signed_messages (list)
+        _items = []
+        if self.signed_messages:
+            for _item in self.signed_messages:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['signed_messages'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> XTZOperationUndelegate:
-        """Create an instance of XTZOperationUndelegate from a dict"""
+    def from_dict(cls, obj: dict) -> ADAPrepareTxPayload:
+        """Create an instance of ADAPrepareTxPayload from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return XTZOperationUndelegate.parse_obj(obj)
+            return ADAPrepareTxPayload.parse_obj(obj)
 
-        _obj = XTZOperationUndelegate.parse_obj({
-            "type": obj.get("type"),
-            "var_date": obj.get("date"),
-            "staker_address": obj.get("staker_address"),
-            "baker_address": obj.get("baker_address"),
-            "operation": obj.get("operation"),
-            "operation_gas_used": obj.get("operation_gas_used"),
-            "baker_fee": obj.get("baker_fee"),
-            "block": obj.get("block")
+        _obj = ADAPrepareTxPayload.parse_obj({
+            "unsigned_tx_serialized": obj.get("unsigned_tx_serialized"),
+            "signed_messages": [ADAPrepareTxPayloadSignedMessagesInner.from_dict(_item) for _item in obj.get("signed_messages")] if obj.get("signed_messages") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_signed_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/xtz_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_unsigned_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/matic_unsigned_tx.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class XTZUnsignedTx(BaseModel):
+class MATICUnsignedTx(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     unsigned_tx_hash: Optional[StrictStr] = Field(None, description="Hash of the unsigned transaction")
     unsigned_tx_serialized: Optional[StrictStr] = Field(None, description="Unsigned serialized transaction")
@@ -40,34 +40,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> XTZUnsignedTx:
-        """Create an instance of XTZUnsignedTx from a JSON string"""
+    def from_json(cls, json_str: str) -> MATICUnsignedTx:
+        """Create an instance of MATICUnsignedTx from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> XTZUnsignedTx:
-        """Create an instance of XTZUnsignedTx from a dict"""
+    def from_dict(cls, obj: dict) -> MATICUnsignedTx:
+        """Create an instance of MATICUnsignedTx from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return XTZUnsignedTx.parse_obj(obj)
+            return MATICUnsignedTx.parse_obj(obj)
 
-        _obj = XTZUnsignedTx.parse_obj({
+        _obj = MATICUnsignedTx.parse_obj({
             "unsigned_tx_hash": obj.get("unsigned_tx_hash"),
             "unsigned_tx_serialized": obj.get("unsigned_tx_serialized")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtztx_status.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,64 +14,58 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+
 from pydantic import BaseModel, Field, StrictStr
-from kiln_connect.openapi_client.models.xtztx_status_receipt import XTZTxStatusReceipt
 
-class XTZTxStatus(BaseModel):
+class SOLBroadcastTxPayload(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    status: Optional[StrictStr] = Field(None, description="Transaction status")
-    receipt: Optional[XTZTxStatusReceipt] = None
-    __properties = ["status", "receipt"]
+    tx_serialized: StrictStr = Field(..., description="Hex encoded signed transaction")
+    __properties = ["tx_serialized"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> XTZTxStatus:
-        """Create an instance of XTZTxStatus from a JSON string"""
+    def from_json(cls, json_str: str) -> SOLBroadcastTxPayload:
+        """Create an instance of SOLBroadcastTxPayload from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of receipt
-        if self.receipt:
-            _dict['receipt'] = self.receipt.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> XTZTxStatus:
-        """Create an instance of XTZTxStatus from a dict"""
+    def from_dict(cls, obj: dict) -> SOLBroadcastTxPayload:
+        """Create an instance of SOLBroadcastTxPayload from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return XTZTxStatus.parse_obj(obj)
+            return SOLBroadcastTxPayload.parse_obj(obj)
 
-        _obj = XTZTxStatus.parse_obj({
-            "status": obj.get("status"),
-            "receipt": XTZTxStatusReceipt.from_dict(obj.get("receipt")) if obj.get("receipt") is not None else None
+        _obj = SOLBroadcastTxPayload.parse_obj({
+            "tx_serialized": obj.get("tx_serialized")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtztx_status_receipt.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/models/post_atom_broadcast_tx201_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,70 +14,62 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, Dict, Optional
-from pydantic import BaseModel, StrictStr
+from typing import Optional
+from pydantic import BaseModel
+from kiln_connect.openapi_client.models.atomtx_hash import ATOMTxHash
 
-class XTZTxStatusReceipt(BaseModel):
+class PostAtomBroadcastTx201Response(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    protocol: Optional[StrictStr] = None
-    chain_id: Optional[StrictStr] = None
-    hash: Optional[StrictStr] = None
-    branch: Optional[StrictStr] = None
-    contents: Optional[Dict[str, Any]] = None
-    signature: Optional[StrictStr] = None
-    metadata: Optional[Dict[str, Any]] = None
-    __properties = ["protocol", "chain_id", "hash", "branch", "contents", "signature", "metadata"]
+    data: Optional[ATOMTxHash] = None
+    __properties = ["data"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> XTZTxStatusReceipt:
-        """Create an instance of XTZTxStatusReceipt from a JSON string"""
+    def from_json(cls, json_str: str) -> PostAtomBroadcastTx201Response:
+        """Create an instance of PostAtomBroadcastTx201Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> XTZTxStatusReceipt:
-        """Create an instance of XTZTxStatusReceipt from a dict"""
+    def from_dict(cls, obj: dict) -> PostAtomBroadcastTx201Response:
+        """Create an instance of PostAtomBroadcastTx201Response from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return XTZTxStatusReceipt.parse_obj(obj)
+            return PostAtomBroadcastTx201Response.parse_obj(obj)
 
-        _obj = XTZTxStatusReceipt.parse_obj({
-            "protocol": obj.get("protocol"),
-            "chain_id": obj.get("chain_id"),
-            "hash": obj.get("hash"),
-            "branch": obj.get("branch"),
-            "contents": obj.get("contents"),
-            "signature": obj.get("signature"),
-            "metadata": obj.get("metadata")
+        _obj = PostAtomBroadcastTx201Response.parse_obj({
+            "data": ATOMTxHash.from_dict(obj.get("data")) if obj.get("data") is not None else None
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/rest.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_account_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,61 +13,47 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.account_portfolio import AccountPortfolio  # noqa: E501
+from kiln_connect.openapi_client.models.eth_post_keys_batch_response import ETHPostKeysBatchResponse  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestAccountPortfolio(unittest.TestCase):
-    """AccountPortfolio unit test stubs"""
+class TestETHPostKeysBatchResponse(unittest.TestCase):
+    """ETHPostKeysBatchResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test AccountPortfolio
+        """Test ETHPostKeysBatchResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AccountPortfolio`
+        # uncomment below to create an instance of `ETHPostKeysBatchResponse`
         """
-        model = kiln_connect.openapi_client.models.account_portfolio.AccountPortfolio()  # noqa: E501
+        model = kiln_connect.openapi_client.models.eth_post_keys_batch_response.ETHPostKeysBatchResponse()  # noqa: E501
         if include_optional :
-            return AccountPortfolio(
-                total_balance_usd = 182981229.16751668, 
-                total_rewards_usd = 4526.16751668, 
-                total_stakes = 56, 
-                total_active_stakes = 52, 
-                protocols = [
-                    kiln_connect.openapi_client.models.account_portfolio_protocols_inner.AccountPortfolio_protocols_inner(
-                        token = 'eth', 
-                        name = 'Ethereum', 
-                        total_stakes = 12, 
-                        total_active_stakes = 10, 
-                        total_balance = kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance.AccountPortfolio_protocols_inner_total_balance(
-                            amount_usd = 10896.4568, 
-                            amount = 1896.4563, ), 
-                        total_rewards = kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards.AccountPortfolio_protocols_inner_total_rewards(
-                            amount_usd = 10896.4568, 
-                            amount = 1896.4568, ), 
-                        balance_share_percent = 42.59, 
-                        rewards_share_percent = 42.59, )
-                    ]
+            return ETHPostKeysBatchResponse(
+                format = 'batch_deposit', 
+                pubkeys = ["8f36e2f4e921b1ed5ce9c94f21e1f26a748ac4e0c57f0d8973e7d576a2f8953b87dd86300de718238de23b1fecb19db5"], 
+                withdrawal_credentials = ["010000000000000000000000e1f4acc0affb36a805474e3b6ab786738c6900a2"], 
+                signatures = ["b7947eabf631d4772c4014a9fec2ecac2c15fc5175ad83023bbdfc9e6618cb8e78829231477c060bc9339482058ff195141f2aeb801c0329a1a4afebd7e76ce0ba1d9d88f8820d052836a79d59aea673db9eb5009db4a4f6e04fb7ffbdbdd604"], 
+                deposit_data_roots = ["37e329240dd23a4bcd86cd62b97fdf0873b565876f29678e1edbf5514fe344d6"]
             )
         else :
-            return AccountPortfolio(
+            return ETHPostKeysBatchResponse(
         )
         """
 
-    def testAccountPortfolio(self):
-        """Test AccountPortfolio"""
+    def testETHPostKeysBatchResponse(self):
+        """Test ETHPostKeysBatchResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_portfolio_protocols_inner_total_rewards.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,54 +13,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner import AccountPortfolioProtocolsInner  # noqa: E501
+from kiln_connect.openapi_client.models.portfolio_protocols_inner_total_rewards import PortfolioProtocolsInnerTotalRewards  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestAccountPortfolioProtocolsInner(unittest.TestCase):
-    """AccountPortfolioProtocolsInner unit test stubs"""
+class TestPortfolioProtocolsInnerTotalRewards(unittest.TestCase):
+    """PortfolioProtocolsInnerTotalRewards unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test AccountPortfolioProtocolsInner
+        """Test PortfolioProtocolsInnerTotalRewards
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AccountPortfolioProtocolsInner`
+        # uncomment below to create an instance of `PortfolioProtocolsInnerTotalRewards`
         """
-        model = kiln_connect.openapi_client.models.account_portfolio_protocols_inner.AccountPortfolioProtocolsInner()  # noqa: E501
+        model = kiln_connect.openapi_client.models.portfolio_protocols_inner_total_rewards.PortfolioProtocolsInnerTotalRewards()  # noqa: E501
         if include_optional :
-            return AccountPortfolioProtocolsInner(
-                token = 'eth', 
-                name = 'Ethereum', 
-                total_stakes = 12, 
-                total_active_stakes = 10, 
-                total_balance = kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance.AccountPortfolio_protocols_inner_total_balance(
-                    amount_usd = 10896.4568, 
-                    amount = 1896.4563, ), 
-                total_rewards = kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards.AccountPortfolio_protocols_inner_total_rewards(
-                    amount_usd = 10896.4568, 
-                    amount = 1896.4568, ), 
-                balance_share_percent = 42.59, 
-                rewards_share_percent = 42.59
+            return PortfolioProtocolsInnerTotalRewards(
+                amount_usd = 10896.4568, 
+                amount = 1896.4568
             )
         else :
-            return AccountPortfolioProtocolsInner(
+            return PortfolioProtocolsInnerTotalRewards(
         )
         """
 
-    def testAccountPortfolioProtocolsInner(self):
-        """Test AccountPortfolioProtocolsInner"""
+    def testPortfolioProtocolsInnerTotalRewards(self):
+        """Test PortfolioProtocolsInnerTotalRewards"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_portfolio_protocols_inner_total_balance.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,44 +13,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance import AccountPortfolioProtocolsInnerTotalBalance  # noqa: E501
+from kiln_connect.openapi_client.models.portfolio_protocols_inner_total_balance import PortfolioProtocolsInnerTotalBalance  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestAccountPortfolioProtocolsInnerTotalBalance(unittest.TestCase):
-    """AccountPortfolioProtocolsInnerTotalBalance unit test stubs"""
+class TestPortfolioProtocolsInnerTotalBalance(unittest.TestCase):
+    """PortfolioProtocolsInnerTotalBalance unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test AccountPortfolioProtocolsInnerTotalBalance
+        """Test PortfolioProtocolsInnerTotalBalance
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AccountPortfolioProtocolsInnerTotalBalance`
+        # uncomment below to create an instance of `PortfolioProtocolsInnerTotalBalance`
         """
-        model = kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance.AccountPortfolioProtocolsInnerTotalBalance()  # noqa: E501
+        model = kiln_connect.openapi_client.models.portfolio_protocols_inner_total_balance.PortfolioProtocolsInnerTotalBalance()  # noqa: E501
         if include_optional :
-            return AccountPortfolioProtocolsInnerTotalBalance(
+            return PortfolioProtocolsInnerTotalBalance(
                 amount_usd = 10896.4568, 
                 amount = 1896.4563
             )
         else :
-            return AccountPortfolioProtocolsInnerTotalBalance(
+            return PortfolioProtocolsInnerTotalBalance(
         )
         """
 
-    def testAccountPortfolioProtocolsInnerTotalBalance(self):
-        """Test AccountPortfolioProtocolsInnerTotalBalance"""
+    def testPortfolioProtocolsInnerTotalBalance(self):
+        """Test PortfolioProtocolsInnerTotalBalance"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,44 +13,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards import AccountPortfolioProtocolsInnerTotalRewards  # noqa: E501
+from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestAccountPortfolioProtocolsInnerTotalRewards(unittest.TestCase):
-    """AccountPortfolioProtocolsInnerTotalRewards unit test stubs"""
+class TestGetSolRewards200Response(unittest.TestCase):
+    """GetSolRewards200Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test AccountPortfolioProtocolsInnerTotalRewards
+        """Test GetSolRewards200Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AccountPortfolioProtocolsInnerTotalRewards`
+        # uncomment below to create an instance of `GetSolRewards200Response`
         """
-        model = kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards.AccountPortfolioProtocolsInnerTotalRewards()  # noqa: E501
+        model = kiln_connect.openapi_client.models.get_sol_rewards200_response.GetSolRewards200Response()  # noqa: E501
         if include_optional :
-            return AccountPortfolioProtocolsInnerTotalRewards(
-                amount_usd = 10896.4568, 
-                amount = 1896.4568
+            return GetSolRewards200Response(
+                data = [
+                    null
+                    ]
             )
         else :
-            return AccountPortfolioProtocolsInnerTotalRewards(
+            return GetSolRewards200Response(
         )
         """
 
-    def testAccountPortfolioProtocolsInnerTotalRewards(self):
-        """Test AccountPortfolioProtocolsInnerTotalRewards"""
+    def testGetSolRewards200Response(self):
+        """Test GetSolRewards200Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_accounts_api.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_accounts_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 
     def setUp(self):
         self.api = kiln_connect.openapi_client.api.accounts_api.AccountsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
+    def test_delete_account(self):
+        """Test case for delete_account
+
+        Account  # noqa: E501
+        """
+        pass
+
     def test_get_account(self):
         """Test case for get_account
 
         Account  # noqa: E501
         """
         pass
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_api.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_organizations_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,37 +12,30 @@
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.api.atom_api import AtomApi  # noqa: E501
+from kiln_connect.openapi_client.api.organizations_api import OrganizationsApi  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
 
-class TestAtomApi(unittest.TestCase):
-    """AtomApi unit test stubs"""
+class TestOrganizationsApi(unittest.TestCase):
+    """OrganizationsApi unit test stubs"""
 
     def setUp(self):
-        self.api = kiln_connect.openapi_client.api.atom_api.AtomApi()  # noqa: E501
+        self.api = kiln_connect.openapi_client.api.organizations_api.OrganizationsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_atom_rewards(self):
-        """Test case for get_atom_rewards
+    def test_get_organization_portfolio(self):
+        """Test case for get_organization_portfolio
 
-        Rewards  # noqa: E501
-        """
-        pass
-
-    def test_get_atom_stakes(self):
-        """Test case for get_atom_stakes
-
-        Stakes  # noqa: E501
+        Organization Portfolio  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_core_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_core_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_api.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,21 @@
     def test_get_eth_tx_status(self):
         """Test case for get_eth_tx_status
 
         Transaction Status  # noqa: E501
         """
         pass
 
+    def test_get_exit_message(self):
+        """Test case for get_exit_message
+
+        Exit Messages  # noqa: E501
+        """
+        pass
+
     def test_post_eth_broadcast_tx(self):
         """Test case for post_eth_broadcast_tx
 
         Broadcast Transaction  # noqa: E501
         """
         pass
 
@@ -102,10 +109,17 @@
     def test_post_eth_stake_tx(self):
         """Test case for post_eth_stake_tx
 
         Stake Transaction  # noqa: E501
         """
         pass
 
+    def test_post_eth_stakes(self):
+        """Test case for post_eth_stakes
+
+        Create stakes  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_kiln_stats.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_kiln_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_network_stats.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_network_stats.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,18 @@
         # uncomment below to create an instance of `ETHNetworkStats`
         """
         model = kiln_connect.openapi_client.models.eth_network_stats.ETHNetworkStats()  # noqa: E501
         if include_optional :
             return ETHNetworkStats(
                 network_gross_apy = 4.5, 
                 supply_staked_percent = 12.4, 
-                eth_price_usd = 2000.0
+                eth_price_usd = 2000.0, 
+                estimated_entry_time_seconds = 3600.0, 
+                estimated_exit_time_seconds = 3600.0, 
+                estimated_withdrawal_time_seconds = 3600.0
             )
         else :
             return ETHNetworkStats(
         )
         """
 
     def testETHNetworkStats(self):
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         """
         model = kiln_connect.openapi_client.models.eth_operation_consensus_withdrawal.ETHOperationConsensusWithdrawal()  # noqa: E501
         if include_optional :
             return ETHOperationConsensusWithdrawal(
                 type = 'consensus_withdrawal', 
                 time = '2023-01-14T01:13:59Z', 
                 validator_address = '0x95373bcf8e2c64e1c373a6e534c002f210adbcc84c5abda3b6306677e171430ae50781a51c9f579a47622e334dba2412', 
+                validator_index = 1, 
                 block = 15955054, 
                 fee_recipient = '0x1e68238cE926DEC62b3FBC99AB06eB1D85CE0270', 
                 amount = '3467036438000000000'
             )
         else :
             return ETHOperationConsensusWithdrawal(
         )
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_deposit.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_operation_deposit.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         """
         model = kiln_connect.openapi_client.models.eth_operation_deposit.ETHOperationDeposit()  # noqa: E501
         if include_optional :
             return ETHOperationDeposit(
                 type = 'deposit', 
                 time = '2023-01-14T01:13:59Z', 
                 validator_address = '0x95373bcf8e2c64e1c373a6e534c002f210adbcc84c5abda3b6306677e171430ae50781a51c9f579a47622e334dba2412', 
+                validator_index = 1, 
                 tx_hash = '0x43244f90814b31dec250de24df5bb023a338790c1d5a39244cf1064cf6d98c94', 
                 tx_sender = '0x41bf25fc8c52d292bd66d3bcecd8a919ecb9ef88', 
                 tx_gas_used = '2700999916653262', 
                 tx_effective_gas_price = '1499997889', 
                 proxies = ["0x1e68238cE926DEC62b3FBC99AB06eB1D85CE0270","0x43244f90814b31dec250de24df5bb023eB1D85CE"], 
                 block = 15955054, 
                 block_base_fee = '7',
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         """
         model = kiln_connect.openapi_client.models.eth_operation_execution_reward.ETHOperationExecutionReward()  # noqa: E501
         if include_optional :
             return ETHOperationExecutionReward(
                 type = 'execution_reward', 
                 time = '2023-01-14T01:13:59Z', 
                 validator_address = '0x95373bcf8e2c64e1c373a6e534c002f210adbcc84c5abda3b6306677e171430ae50781a51c9f579a47622e334dba2412', 
+                validator_index = 1, 
                 block = 15955054, 
                 fee_recipient = '0x1e68238cE926DEC62b3FBC99AB06eB1D85CE0270', 
                 mev_payout_tx_hash = '0x43244f90814b31dec250de24df5bb023a338790c1d5a39244cf1064cf6d98c94', 
                 amount = '3467036438000000000'
             )
         else :
             return ETHOperationExecutionReward(
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atomtx_hash.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,47 +13,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.eth_post_keys_batch_response import ETHPostKeysBatchResponse  # noqa: E501
+from kiln_connect.openapi_client.models.atomtx_hash import ATOMTxHash  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestETHPostKeysBatchResponse(unittest.TestCase):
-    """ETHPostKeysBatchResponse unit test stubs"""
+class TestATOMTxHash(unittest.TestCase):
+    """ATOMTxHash unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ETHPostKeysBatchResponse
+        """Test ATOMTxHash
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ETHPostKeysBatchResponse`
+        # uncomment below to create an instance of `ATOMTxHash`
         """
-        model = kiln_connect.openapi_client.models.eth_post_keys_batch_response.ETHPostKeysBatchResponse()  # noqa: E501
+        model = kiln_connect.openapi_client.models.atomtx_hash.ATOMTxHash()  # noqa: E501
         if include_optional :
-            return ETHPostKeysBatchResponse(
-                format = 'batch_deposit', 
-                pubkeys = ["8f36e2f4e921b1ed5ce9c94f21e1f26a748ac4e0c57f0d8973e7d576a2f8953b87dd86300de718238de23b1fecb19db5"], 
-                withdrawal_credentials = ["010000000000000000000000e1f4acc0affb36a805474e3b6ab786738c6900a2"], 
-                signatures = ["b7947eabf631d4772c4014a9fec2ecac2c15fc5175ad83023bbdfc9e6618cb8e78829231477c060bc9339482058ff195141f2aeb801c0329a1a4afebd7e76ce0ba1d9d88f8820d052836a79d59aea673db9eb5009db4a4f6e04fb7ffbdbdd604"], 
-                deposit_data_roots = ["37e329240dd23a4bcd86cd62b97fdf0873b565876f29678e1edbf5514fe344d6"]
+            return ATOMTxHash(
+                tx_hash = '2B4F732E12D5D5AF1F907AD03B199167A718EDC6201DE5713143AB80990420CB'
             )
         else :
-            return ETHPostKeysBatchResponse(
+            return ATOMTxHash(
         )
         """
 
-    def testETHPostKeysBatchResponse(self):
-        """Test ETHPostKeysBatchResponse"""
+    def testATOMTxHash(self):
+        """Test ATOMTxHash"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_signed_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_stake.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,27 +36,30 @@
             optional params are included """
         # uncomment below to create an instance of `ETHStake`
         """
         model = kiln_connect.openapi_client.models.eth_stake.ETHStake()  # noqa: E501
         if include_optional :
             return ETHStake(
                 validator_address = '0x95373bcf8e2c64e1c373a6e534c002f210adbcc84c5abda3b6306677e171430ae50781a51c9f579a47622e334dba2412', 
+                validator_index = 1, 
                 state = 'active_ongoing', 
                 activated_at = '2023-01-14T01:13:59Z', 
                 activated_epoch = 174049, 
+                delegated_at = '2023-01-14T01:13:59Z', 
                 delegated_block = 16397387, 
                 deposit_tx_sender = '0xe1f4acc0affB36a805474e3b6ab786738C6900A2', 
                 execution_fee_recipient = '0xe1f4acc0affB36a805474e3b6ab786738C6900A2', 
                 withdrawal_credentials = '010000000000000000000000e1f4acc0affb36a805474e3b6ab786738c6900a2', 
                 effective_balance = '32000000000000000000', 
                 balance = '32076187808000000000', 
                 consensus_rewards = '76187808000000000', 
                 execution_rewards = '0', 
                 rewards = '76187808000000000', 
                 gross_apy = 3.407, 
+                is_kiln = True, 
                 updated_at = '2023-01-14T01:13:59Z'
             )
         else :
             return ETHStake(
         )
         """
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_adatx_status.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,71 +13,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.ethtx_status import ETHTxStatus  # noqa: E501
+from kiln_connect.openapi_client.models.adatx_status import ADATxStatus  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestETHTxStatus(unittest.TestCase):
-    """ETHTxStatus unit test stubs"""
+class TestADATxStatus(unittest.TestCase):
+    """ADATxStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ETHTxStatus
+        """Test ADATxStatus
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ETHTxStatus`
+        # uncomment below to create an instance of `ADATxStatus`
         """
-        model = kiln_connect.openapi_client.models.ethtx_status.ETHTxStatus()  # noqa: E501
+        model = kiln_connect.openapi_client.models.adatx_status.ADATxStatus()  # noqa: E501
         if include_optional :
-            return ETHTxStatus(
+            return ADATxStatus(
                 status = 'success', 
-                receipt = kiln_connect.openapi_client.models.ethtx_status_receipt.ETHTxStatus_receipt(
-                    status = True, 
-                    transaction_hash = '0xff34f4ed4a4196e3f84a67d215c91f60cb2afc2241666406c4e23044a323314c', 
-                    transaction_index = 1, 
-                    block_hash = '0x47f276879340589c610334c0e7f9cc87cc559ae359a90e9fc609b3104fd6929b', 
-                    block_number = 8645017, 
-                    from = '0xa111B576408B1CcDacA3eF26f22f082C49bcaa55', 
-                    to = '0xa111B576408B1CcDacA3eF26f22f082C49bcaa55', 
-                    contract_address = '0xa111B576408B1CcDacA3eF26f22f082C49bcaa55', 
-                    cumulative_gas_used = 21000, 
-                    gas_used = 21000, 
-                    effective_gas_price = 0.22, 
-                    logs = [
-                        kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner.ETHTxStatus_receipt_logs_inner(
-                            address = '', 
-                            data = '', 
-                            topics = [
-                                ''
-                                ], 
-                            log_index = 1.337, 
-                            transaction_index = 1.337, 
-                            transaction_hash = '', 
-                            block_hash = '', 
-                            block_number = 1.337, 
-                            removed = True, )
-                        ], 
-                    logs_bloom = '', 
-                    events = kiln_connect.openapi_client.models.events.events(), )
+                receipt = {"hash":"20082206aadbbb2dfded4afc9346831c5bd3a6a3f8a75f59dbe6166c05e918f6","block":"2612449e345ec0f58aae05c693a09943f599592e28eedec70ee8c1a4f3d1e834","block_height":660450,"block_time":1677170968,"slot":21487768,"index":1,"output_amount":[{"unit":"lovelace","quantity":"10027100000"}],"fees":"300000","deposit":"2000000","size":429,"invalid_before":null,"invalid_hereafter":"21494910","utxo_count":2,"withdrawal_count":0,"mir_cert_count":0,"delegation_count":1,"stake_cert_count":1,"pool_update_count":0,"pool_retire_count":0,"asset_mint_or_burn_count":0,"redeemer_count":0,"valid_contract":true}
             )
         else :
-            return ETHTxStatus(
+            return ADATxStatus(
         )
         """
 
-    def testETHTxStatus(self):
-        """Test ETHTxStatus"""
+    def testADATxStatus(self):
+        """Test ADATxStatus"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_stake.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,69 +13,54 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.ethtx_status_receipt import ETHTxStatusReceipt  # noqa: E501
+from kiln_connect.openapi_client.models.sol_stake import SOLStake  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestETHTxStatusReceipt(unittest.TestCase):
-    """ETHTxStatusReceipt unit test stubs"""
+class TestSOLStake(unittest.TestCase):
+    """SOLStake unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ETHTxStatusReceipt
+        """Test SOLStake
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ETHTxStatusReceipt`
+        # uncomment below to create an instance of `SOLStake`
         """
-        model = kiln_connect.openapi_client.models.ethtx_status_receipt.ETHTxStatusReceipt()  # noqa: E501
+        model = kiln_connect.openapi_client.models.sol_stake.SOLStake()  # noqa: E501
         if include_optional :
-            return ETHTxStatusReceipt(
-                status = True, 
-                transaction_hash = '0xff34f4ed4a4196e3f84a67d215c91f60cb2afc2241666406c4e23044a323314c', 
-                transaction_index = 1, 
-                block_hash = '0x47f276879340589c610334c0e7f9cc87cc559ae359a90e9fc609b3104fd6929b', 
-                block_number = 8645017, 
-                var_from = '0xa111B576408B1CcDacA3eF26f22f082C49bcaa55', 
-                to = '0xa111B576408B1CcDacA3eF26f22f082C49bcaa55', 
-                contract_address = '0xa111B576408B1CcDacA3eF26f22f082C49bcaa55', 
-                cumulative_gas_used = 21000, 
-                gas_used = 21000, 
-                effective_gas_price = 0.22, 
-                logs = [
-                    kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner.ETHTxStatus_receipt_logs_inner(
-                        address = '', 
-                        data = '', 
-                        topics = [
-                            ''
-                            ], 
-                        log_index = 1.337, 
-                        transaction_index = 1.337, 
-                        transaction_hash = '', 
-                        block_hash = '', 
-                        block_number = 1.337, 
-                        removed = True, )
-                    ], 
-                logs_bloom = '', 
-                events = kiln_connect.openapi_client.models.events.events()
+            return SOLStake(
+                stake_account = '3sfokk2DFsd88ujd8sfa9slsdf99kjnFJksdf', 
+                vote_account = '6hNweZvzTudTuprZrAXb1A9grKvVG6xgjyvdJUqAMk78', 
+                withdraw_pubkey = '4wdr76KJTFgH68YtGddmnF45WdD8LMv9eLsdf', 
+                state = 'active', 
+                activated_at = '2023-01-14T01:13:59Z', 
+                activated_epoch = 150, 
+                deactivated_at = '2023-01-14T01:13:59Z', 
+                deactivated_epoch = 150, 
+                balance = '1000000000', 
+                rewards = '1000000000', 
+                net_apy = 3.407, 
+                updated_at = '2023-01-14T01:13:59Z'
             )
         else :
-            return ETHTxStatusReceipt(
+            return SOLStake(
         )
         """
 
-    def testETHTxStatusReceipt(self):
-        """Test ETHTxStatusReceipt"""
+    def testSOLStake(self):
+        """Test SOLStake"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_broadcasted_tx.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,53 +13,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner import ETHTxStatusReceiptLogsInner  # noqa: E501
+from kiln_connect.openapi_client.models.matic_broadcasted_tx import MATICBroadcastedTx  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestETHTxStatusReceiptLogsInner(unittest.TestCase):
-    """ETHTxStatusReceiptLogsInner unit test stubs"""
+class TestMATICBroadcastedTx(unittest.TestCase):
+    """MATICBroadcastedTx unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test ETHTxStatusReceiptLogsInner
+        """Test MATICBroadcastedTx
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ETHTxStatusReceiptLogsInner`
+        # uncomment below to create an instance of `MATICBroadcastedTx`
         """
-        model = kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner.ETHTxStatusReceiptLogsInner()  # noqa: E501
+        model = kiln_connect.openapi_client.models.matic_broadcasted_tx.MATICBroadcastedTx()  # noqa: E501
         if include_optional :
-            return ETHTxStatusReceiptLogsInner(
-                address = '', 
-                data = '', 
-                topics = [
-                    ''
-                    ], 
-                log_index = 1.337, 
-                transaction_index = 1.337, 
-                transaction_hash = '', 
-                block_hash = '', 
-                block_number = 1.337, 
-                removed = True
+            return MATICBroadcastedTx(
+                tx_hash = '0x43244f90814b31dec250de24df5bb023a338790c1d5a39244cf1064cf6d98c94'
             )
         else :
-            return ETHTxStatusReceiptLogsInner(
+            return MATICBroadcastedTx(
         )
         """
 
-    def testETHTxStatusReceiptLogsInner(self):
-        """Test ETHTxStatusReceiptLogsInner"""
+    def testMATICBroadcastedTx(self):
+        """Test MATICBroadcastedTx"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,29 +35,29 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `GetAccountPortfolio200Response`
         """
         model = kiln_connect.openapi_client.models.get_account_portfolio200_response.GetAccountPortfolio200Response()  # noqa: E501
         if include_optional :
             return GetAccountPortfolio200Response(
-                data = kiln_connect.openapi_client.models.account_portfolio.AccountPortfolio(
+                data = kiln_connect.openapi_client.models.portfolio.Portfolio(
                     total_balance_usd = 182981229.16751668, 
                     total_rewards_usd = 4526.16751668, 
                     total_stakes = 56, 
                     total_active_stakes = 52, 
                     protocols = [
-                        kiln_connect.openapi_client.models.account_portfolio_protocols_inner.AccountPortfolio_protocols_inner(
+                        kiln_connect.openapi_client.models.portfolio_protocols_inner.Portfolio_protocols_inner(
                             token = 'eth', 
                             name = 'Ethereum', 
                             total_stakes = 12, 
                             total_active_stakes = 10, 
-                            total_balance = kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_balance.AccountPortfolio_protocols_inner_total_balance(
+                            total_balance = kiln_connect.openapi_client.models.portfolio_protocols_inner_total_balance.Portfolio_protocols_inner_total_balance(
                                 amount_usd = 10896.4568, 
                                 amount = 1896.4563, ), 
-                            total_rewards = kiln_connect.openapi_client.models.account_portfolio_protocols_inner_total_rewards.AccountPortfolio_protocols_inner_total_rewards(
+                            total_rewards = kiln_connect.openapi_client.models.portfolio_protocols_inner_total_rewards.Portfolio_protocols_inner_total_rewards(
                                 amount_usd = 10896.4568, 
                                 amount = 1896.4568, ), 
                             balance_share_percent = 42.59, 
                             rewards_share_percent = 42.59, )
                         ], )
             )
         else :
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_accounts200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_accounts200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_atom_rewards200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_atom_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_atom_stakes200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_atom_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,18 @@
         """
         model = kiln_connect.openapi_client.models.get_eth_network_stats200_response.GetEthNetworkStats200Response()  # noqa: E501
         if include_optional :
             return GetEthNetworkStats200Response(
                 data = kiln_connect.openapi_client.models.eth_network_stats.ETHNetworkStats(
                     network_gross_apy = 4.5, 
                     supply_staked_percent = 12.4, 
-                    eth_price_usd = 2000.0, )
+                    eth_price_usd = 2000.0, 
+                    estimated_entry_time_seconds = 3600.0, 
+                    estimated_exit_time_seconds = 3600.0, 
+                    estimated_withdrawal_time_seconds = 3600.0, )
             )
         else :
             return GetEthNetworkStats200Response(
         )
         """
 
     def testGetEthNetworkStats200Response(self):
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         """
         model = kiln_connect.openapi_client.models.get_eth_operations200_response_data_inner.GetEthOperations200ResponseDataInner()  # noqa: E501
         if include_optional :
             return GetEthOperations200ResponseDataInner(
                 type = 'execution_reward', 
                 time = '2023-01-14T01:13:59Z', 
                 validator_address = '0x95373bcf8e2c64e1c373a6e534c002f210adbcc84c5abda3b6306677e171430ae50781a51c9f579a47622e334dba2412', 
+                validator_index = 1, 
                 tx_hash = '0x43244f90814b31dec250de24df5bb023a338790c1d5a39244cf1064cf6d98c94', 
                 tx_sender = '0x41bf25fc8c52d292bd66d3bcecd8a919ecb9ef88', 
                 tx_gas_used = '2700999916653262', 
                 tx_effective_gas_price = '1499997889', 
                 proxies = ["0x1e68238cE926DEC62b3FBC99AB06eB1D85CE0270","0x43244f90814b31dec250de24df5bb023eB1D85CE"], 
                 block = 15955054, 
                 block_base_fee = '7',
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,27 +38,30 @@
         """
         model = kiln_connect.openapi_client.models.get_eth_stakes200_response.GetEthStakes200Response()  # noqa: E501
         if include_optional :
             return GetEthStakes200Response(
                 data = [
                     kiln_connect.openapi_client.models.eth_stake.ETHStake(
                         validator_address = '0x95373bcf8e2c64e1c373a6e534c002f210adbcc84c5abda3b6306677e171430ae50781a51c9f579a47622e334dba2412', 
+                        validator_index = 1, 
                         state = 'active_ongoing', 
                         activated_at = '2023-01-14T01:13:59Z', 
                         activated_epoch = 174049, 
+                        delegated_at = '2023-01-14T01:13:59Z', 
                         delegated_block = 16397387, 
                         deposit_tx_sender = '0xe1f4acc0affB36a805474e3b6ab786738C6900A2', 
                         execution_fee_recipient = '0xe1f4acc0affB36a805474e3b6ab786738C6900A2', 
                         withdrawal_credentials = '010000000000000000000000e1f4acc0affb36a805474e3b6ab786738c6900a2', 
                         effective_balance = '32000000000000000000', 
                         balance = '32076187808000000000', 
                         consensus_rewards = '76187808000000000', 
                         execution_rewards = '0', 
                         rewards = '76187808000000000', 
                         gross_apy = 3.407, 
+                        is_kiln = True, 
                         updated_at = '2023-01-14T01:13:59Z', )
                     ]
             )
         else :
             return GetEthStakes200Response(
         )
         """
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_ada_tx_status200_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,72 +13,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.get_eth_tx_status200_response import GetEthTxStatus200Response  # noqa: E501
+from kiln_connect.openapi_client.models.get_ada_tx_status200_response import GetAdaTxStatus200Response  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestGetEthTxStatus200Response(unittest.TestCase):
-    """GetEthTxStatus200Response unit test stubs"""
+class TestGetAdaTxStatus200Response(unittest.TestCase):
+    """GetAdaTxStatus200Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetEthTxStatus200Response
+        """Test GetAdaTxStatus200Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `GetEthTxStatus200Response`
+        # uncomment below to create an instance of `GetAdaTxStatus200Response`
         """
-        model = kiln_connect.openapi_client.models.get_eth_tx_status200_response.GetEthTxStatus200Response()  # noqa: E501
+        model = kiln_connect.openapi_client.models.get_ada_tx_status200_response.GetAdaTxStatus200Response()  # noqa: E501
         if include_optional :
-            return GetEthTxStatus200Response(
-                data = kiln_connect.openapi_client.models.ethtx_status.ETHTxStatus(
+            return GetAdaTxStatus200Response(
+                data = kiln_connect.openapi_client.models.adatx_status.ADATxStatus(
                     status = 'success', 
-                    receipt = kiln_connect.openapi_client.models.ethtx_status_receipt.ETHTxStatus_receipt(
-                        status = True, 
-                        transaction_hash = '0xff34f4ed4a4196e3f84a67d215c91f60cb2afc2241666406c4e23044a323314c', 
-                        transaction_index = 1, 
-                        block_hash = '0x47f276879340589c610334c0e7f9cc87cc559ae359a90e9fc609b3104fd6929b', 
-                        block_number = 8645017, 
-                        from = '0xa111B576408B1CcDacA3eF26f22f082C49bcaa55', 
-                        to = '0xa111B576408B1CcDacA3eF26f22f082C49bcaa55', 
-                        contract_address = '0xa111B576408B1CcDacA3eF26f22f082C49bcaa55', 
-                        cumulative_gas_used = 21000, 
-                        gas_used = 21000, 
-                        effective_gas_price = 0.22, 
-                        logs = [
-                            kiln_connect.openapi_client.models.ethtx_status_receipt_logs_inner.ETHTxStatus_receipt_logs_inner(
-                                address = '', 
-                                data = '', 
-                                topics = [
-                                    ''
-                                    ], 
-                                log_index = 1.337, 
-                                transaction_index = 1.337, 
-                                transaction_hash = '', 
-                                block_hash = '', 
-                                block_number = 1.337, 
-                                removed = True, )
-                            ], 
-                        logs_bloom = '', 
-                        events = kiln_connect.openapi_client.models.events.events(), ), )
+                    receipt = {"hash":"20082206aadbbb2dfded4afc9346831c5bd3a6a3f8a75f59dbe6166c05e918f6","block":"2612449e345ec0f58aae05c693a09943f599592e28eedec70ee8c1a4f3d1e834","block_height":660450,"block_time":1677170968,"slot":21487768,"index":1,"output_amount":[{"unit":"lovelace","quantity":"10027100000"}],"fees":"300000","deposit":"2000000","size":429,"invalid_before":null,"invalid_hereafter":"21494910","utxo_count":2,"withdrawal_count":0,"mir_cert_count":0,"delegation_count":1,"stake_cert_count":1,"pool_update_count":0,"pool_retire_count":0,"asset_mint_or_burn_count":0,"redeemer_count":0,"valid_contract":true}, )
             )
         else :
-            return GetEthTxStatus200Response(
+            return GetAdaTxStatus200Response(
         )
         """
 
-    def testGetEthTxStatus200Response(self):
-        """Test GetEthTxStatus200Response"""
+    def testGetAdaTxStatus200Response(self):
+        """Test GetAdaTxStatus200Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_operations200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_operations200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response  # noqa: E501
+from kiln_connect.openapi_client.models.get_xtz_rewards200_response import GetXtzRewards200Response  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestGetSolRewards200Response(unittest.TestCase):
-    """GetSolRewards200Response unit test stubs"""
+class TestGetXtzRewards200Response(unittest.TestCase):
+    """GetXtzRewards200Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetSolRewards200Response
+        """Test GetXtzRewards200Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `GetSolRewards200Response`
+        # uncomment below to create an instance of `GetXtzRewards200Response`
         """
-        model = kiln_connect.openapi_client.models.get_sol_rewards200_response.GetSolRewards200Response()  # noqa: E501
+        model = kiln_connect.openapi_client.models.get_xtz_rewards200_response.GetXtzRewards200Response()  # noqa: E501
         if include_optional :
-            return GetSolRewards200Response(
+            return GetXtzRewards200Response(
                 data = [
                     null
                     ]
             )
         else :
-            return GetSolRewards200Response(
+            return GetXtzRewards200Response(
         )
         """
 
-    def testGetSolRewards200Response(self):
-        """Test GetSolRewards200Response"""
+    def testGetXtzRewards200Response(self):
+        """Test GetXtzRewards200Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_matic_prepare_tx201_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,45 +13,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.get_sol_tx_status200_response import GetSolTxStatus200Response  # noqa: E501
+from kiln_connect.openapi_client.models.post_matic_prepare_tx201_response import PostMaticPrepareTx201Response  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestGetSolTxStatus200Response(unittest.TestCase):
-    """GetSolTxStatus200Response unit test stubs"""
+class TestPostMaticPrepareTx201Response(unittest.TestCase):
+    """PostMaticPrepareTx201Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetSolTxStatus200Response
+        """Test PostMaticPrepareTx201Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `GetSolTxStatus200Response`
+        # uncomment below to create an instance of `PostMaticPrepareTx201Response`
         """
-        model = kiln_connect.openapi_client.models.get_sol_tx_status200_response.GetSolTxStatus200Response()  # noqa: E501
+        model = kiln_connect.openapi_client.models.post_matic_prepare_tx201_response.PostMaticPrepareTx201Response()  # noqa: E501
         if include_optional :
-            return GetSolTxStatus200Response(
-                data = kiln_connect.openapi_client.models.soltx_status.SOLTxStatus(
-                    status = 'success', 
-                    receipt = kiln_connect.openapi_client.models.receipt.receipt(), )
+            return PostMaticPrepareTx201Response(
+                data = kiln_connect.openapi_client.models.matic_signed_tx.MATICSignedTx(
+                    signed_tx_serialized = '0x20a40259b763d549dfa1c082776a036dd8dabbe8b5e32ee721be017512dc', )
             )
         else :
-            return GetSolTxStatus200Response(
+            return PostMaticPrepareTx201Response(
         )
         """
 
-    def testGetSolTxStatus200Response(self):
-        """Test GetSolTxStatus200Response"""
+    def testPostMaticPrepareTx201Response(self):
+        """Test PostMaticPrepareTx201Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_operations200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_operations200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,45 +13,51 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.get_xtz_rewards200_response import GetXtzRewards200Response  # noqa: E501
+from kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner import GetXtzRewards200ResponseDataInner  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestGetXtzRewards200Response(unittest.TestCase):
-    """GetXtzRewards200Response unit test stubs"""
+class TestGetXtzRewards200ResponseDataInner(unittest.TestCase):
+    """GetXtzRewards200ResponseDataInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetXtzRewards200Response
+        """Test GetXtzRewards200ResponseDataInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `GetXtzRewards200Response`
+        # uncomment below to create an instance of `GetXtzRewards200ResponseDataInner`
         """
-        model = kiln_connect.openapi_client.models.get_xtz_rewards200_response.GetXtzRewards200Response()  # noqa: E501
+        model = kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner.GetXtzRewards200ResponseDataInner()  # noqa: E501
         if include_optional :
-            return GetXtzRewards200Response(
-                data = [
-                    null
-                    ]
+            return GetXtzRewards200ResponseDataInner(
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023', 
+                rewards = '27098488', 
+                active_balance = '34329999165', 
+                gross_apy = 36.053, 
+                cycle = 271, 
+                cycle_begins_at = '2022-09-01T08:44Z'
             )
         else :
-            return GetXtzRewards200Response(
+            return GetXtzRewards200ResponseDataInner(
+                var_date = 'Sun Jan 15 00:00:00 UTC 2023',
+                cycle = 271,
+                cycle_begins_at = '2022-09-01T08:44Z',
         )
         """
 
-    def testGetXtzRewards200Response(self):
-        """Test GetXtzRewards200Response"""
+    def testGetXtzRewards200ResponseDataInner(self):
+        """Test GetXtzRewards200ResponseDataInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_operation_delegate.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,51 +13,51 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner import GetXtzRewards200ResponseDataInner  # noqa: E501
+from kiln_connect.openapi_client.models.xtz_operation_delegate import XTZOperationDelegate  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestGetXtzRewards200ResponseDataInner(unittest.TestCase):
-    """GetXtzRewards200ResponseDataInner unit test stubs"""
+class TestXTZOperationDelegate(unittest.TestCase):
+    """XTZOperationDelegate unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test GetXtzRewards200ResponseDataInner
+        """Test XTZOperationDelegate
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `GetXtzRewards200ResponseDataInner`
+        # uncomment below to create an instance of `XTZOperationDelegate`
         """
-        model = kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner.GetXtzRewards200ResponseDataInner()  # noqa: E501
+        model = kiln_connect.openapi_client.models.xtz_operation_delegate.XTZOperationDelegate()  # noqa: E501
         if include_optional :
-            return GetXtzRewards200ResponseDataInner(
-                var_date = 'Sun Jan 15 00:00:00 UTC 2023', 
-                rewards = '27098488', 
-                active_balance = '34329999165', 
-                gross_apy = 36.053, 
-                cycle = 271, 
-                cycle_begins_at = '2022-09-01T08:44Z'
+            return XTZOperationDelegate(
+                type = 'delegate', 
+                var_date = '2023-01-14T01:13:59Z', 
+                staker_address = 'tz1QQZKGt3ouyd7x8JUDwcvRyxzsmD7CFbMd', 
+                baker_address = 'tz3btDQsDkqq2G7eBdrrLqetaAfLVw6BnPez', 
+                operation = 'opLq44uJLP7f3V3zCVDCDgXayV3CQLGqihdoAYtMnXLW4f1q2fb', 
+                operation_gas_used = '10', 
+                baker_fee = '42', 
+                block = 1342, 
+                amount = '420000'
             )
         else :
-            return GetXtzRewards200ResponseDataInner(
-                var_date = 'Sun Jan 15 00:00:00 UTC 2023',
-                cycle = 271,
-                cycle_begins_at = '2022-09-01T08:44Z',
+            return XTZOperationDelegate(
         )
         """
 
-    def testGetXtzRewards200ResponseDataInner(self):
-        """Test GetXtzRewards200ResponseDataInner"""
+    def testXTZOperationDelegate(self):
+        """Test XTZOperationDelegate"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,55 +10,95 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
-import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.get_xtz_tx_status200_response import GetXtzTxStatus200Response  # noqa: E501
+from kiln_connect.openapi_client.api.xtz_api import XtzApi  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestGetXtzTxStatus200Response(unittest.TestCase):
-    """GetXtzTxStatus200Response unit test stubs"""
+
+class TestXtzApi(unittest.TestCase):
+    """XtzApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = kiln_connect.openapi_client.api.xtz_api.XtzApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional):
-        """Test GetXtzTxStatus200Response
-            include_option is a boolean, when False only required
-            params are included, when True both required and
-            optional params are included """
-        # uncomment below to create an instance of `GetXtzTxStatus200Response`
-        """
-        model = kiln_connect.openapi_client.models.get_xtz_tx_status200_response.GetXtzTxStatus200Response()  # noqa: E501
-        if include_optional :
-            return GetXtzTxStatus200Response(
-                data = kiln_connect.openapi_client.models.xtztx_status.XTZTxStatus(
-                    status = '', 
-                    receipt = kiln_connect.openapi_client.models.xtztx_status_receipt.XTZTxStatus_receipt(
-                        protocol = '', 
-                        chain_id = '', 
-                        hash = '', 
-                        branch = '', 
-                        contents = kiln_connect.openapi_client.models.contents.contents(), 
-                        signature = '', 
-                        metadata = kiln_connect.openapi_client.models.metadata.metadata(), ), )
-            )
-        else :
-            return GetXtzTxStatus200Response(
-        )
-        """
-
-    def testGetXtzTxStatus200Response(self):
-        """Test GetXtzTxStatus200Response"""
-        # inst_req_only = self.make_instance(include_optional=False)
-        # inst_req_and_optional = self.make_instance(include_optional=True)
+    def test_get_xtz_network_stats(self):
+        """Test case for get_xtz_network_stats
+
+        Network Stats  # noqa: E501
+        """
+        pass
+
+    def test_get_xtz_operations(self):
+        """Test case for get_xtz_operations
+
+        Operations  # noqa: E501
+        """
+        pass
+
+    def test_get_xtz_reports(self):
+        """Test case for get_xtz_reports
+
+        Excel Reports  # noqa: E501
+        """
+        pass
+
+    def test_get_xtz_rewards(self):
+        """Test case for get_xtz_rewards
+
+        Rewards  # noqa: E501
+        """
+        pass
+
+    def test_get_xtz_stakes(self):
+        """Test case for get_xtz_stakes
+
+        Stakes  # noqa: E501
+        """
+        pass
+
+    def test_get_xtz_tx_status(self):
+        """Test case for get_xtz_tx_status
+
+        Transaction Status  # noqa: E501
+        """
+        pass
+
+    def test_post_xtz_broadcast_tx(self):
+        """Test case for post_xtz_broadcast_tx
+
+        Broadcast Transaction  # noqa: E501
+        """
+        pass
+
+    def test_post_xtz_prepare_tx(self):
+        """Test case for post_xtz_prepare_tx
+
+        Prepare Transaction  # noqa: E501
+        """
+        pass
+
+    def test_post_xtz_stake_tx(self):
+        """Test case for post_xtz_stake_tx
+
+        Stake Transaction  # noqa: E501
+        """
+        pass
+
+    def test_post_xtz_un_stake_tx(self):
+        """Test case for post_xtz_un_stake_tx
+
+        Unstake Transaction  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_account201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_account201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             optional params are included """
         # uncomment below to create an instance of `PostSolBroadcastTx201Response`
         """
         model = kiln_connect.openapi_client.models.post_sol_broadcast_tx201_response.PostSolBroadcastTx201Response()  # noqa: E501
         if include_optional :
             return PostSolBroadcastTx201Response(
                 data = kiln_connect.openapi_client.models.sol_broadcast_tx.SOLBroadcastTx(
-                    tx_hash = '', )
+                    tx_hash = 'sV6dgQyxByL66t9uTPmffitncWNmnkR8oEC1gQ29jPrKFHm9TkMGvS3TgcQeNz9pSN7913aPXe6MMHFS4xqTafL', )
             )
         else :
             return PostSolBroadcastTx201Response(
         )
         """
 
     def testPostSolBroadcastTx201Response(self):
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,44 +13,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.post_sol_prepare_tx201_response import PostSolPrepareTx201Response  # noqa: E501
+from kiln_connect.openapi_client.models.post_xtz_prepare_tx201_response import PostXtzPrepareTx201Response  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestPostSolPrepareTx201Response(unittest.TestCase):
-    """PostSolPrepareTx201Response unit test stubs"""
+class TestPostXtzPrepareTx201Response(unittest.TestCase):
+    """PostXtzPrepareTx201Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PostSolPrepareTx201Response
+        """Test PostXtzPrepareTx201Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PostSolPrepareTx201Response`
+        # uncomment below to create an instance of `PostXtzPrepareTx201Response`
         """
-        model = kiln_connect.openapi_client.models.post_sol_prepare_tx201_response.PostSolPrepareTx201Response()  # noqa: E501
+        model = kiln_connect.openapi_client.models.post_xtz_prepare_tx201_response.PostXtzPrepareTx201Response()  # noqa: E501
         if include_optional :
-            return PostSolPrepareTx201Response(
-                data = kiln_connect.openapi_client.models.sol_prepared_tx.SOLPreparedTx(
-                    signed_tx_serialized = '', )
+            return PostXtzPrepareTx201Response(
+                data = kiln_connect.openapi_client.models.xtz_signed_tx.XTZSignedTx(
+                    signed_tx_serialized = '0x20a40259b763d549dfa1c082776a036dd8dabbe8b5e32ee721be017512dc', )
             )
         else :
-            return PostSolPrepareTx201Response(
+            return PostXtzPrepareTx201Response(
         )
         """
 
-    def testPostSolPrepareTx201Response(self):
-        """Test PostSolPrepareTx201Response"""
+    def testPostXtzPrepareTx201Response(self):
+        """Test PostXtzPrepareTx201Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_stakes201_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,45 +13,51 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.post_sol_stake_tx201_response import PostSolStakeTx201Response  # noqa: E501
+from kiln_connect.openapi_client.models.post_eth_stakes201_response import PostEthStakes201Response  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestPostSolStakeTx201Response(unittest.TestCase):
-    """PostSolStakeTx201Response unit test stubs"""
+class TestPostEthStakes201Response(unittest.TestCase):
+    """PostEthStakes201Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PostSolStakeTx201Response
+        """Test PostEthStakes201Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PostSolStakeTx201Response`
+        # uncomment below to create an instance of `PostEthStakes201Response`
         """
-        model = kiln_connect.openapi_client.models.post_sol_stake_tx201_response.PostSolStakeTx201Response()  # noqa: E501
+        model = kiln_connect.openapi_client.models.post_eth_stakes201_response.PostEthStakes201Response()  # noqa: E501
         if include_optional :
-            return PostSolStakeTx201Response(
-                data = kiln_connect.openapi_client.models.sol_stake_tx.SOLStakeTx(
-                    unsigned_tx_hash = '', 
-                    unsigned_tx_serialized = '', )
+            return PostEthStakes201Response(
+                data = kiln_connect.openapi_client.models.core_stake.CoreStake(
+                    id = '92f5bfd4-ea38-4824-84f7-686eddff5539', 
+                    tags = [
+                        'tag1'
+                        ], 
+                    metadata = kiln_connect.openapi_client.models.metadata.metadata(), 
+                    protocol = 'ethereum', 
+                    created_at = '2023-02-06T21:48:11.038Z', 
+                    updated_at = '2023-02-06T21:48:11.038Z', )
             )
         else :
-            return PostSolStakeTx201Response(
+            return PostEthStakes201Response(
         )
         """
 
-    def testPostSolStakeTx201Response(self):
-        """Test PostSolStakeTx201Response"""
+    def testPostEthStakes201Response(self):
+        """Test PostEthStakes201Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_stakes_payload.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,51 +13,52 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.post_sol_stakes201_response import PostSolStakes201Response  # noqa: E501
+from kiln_connect.openapi_client.models.post_eth_stakes_payload import PostETHStakesPayload  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestPostSolStakes201Response(unittest.TestCase):
-    """PostSolStakes201Response unit test stubs"""
+class TestPostETHStakesPayload(unittest.TestCase):
+    """PostETHStakesPayload unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PostSolStakes201Response
+        """Test PostETHStakesPayload
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PostSolStakes201Response`
+        # uncomment below to create an instance of `PostETHStakesPayload`
         """
-        model = kiln_connect.openapi_client.models.post_sol_stakes201_response.PostSolStakes201Response()  # noqa: E501
+        model = kiln_connect.openapi_client.models.post_eth_stakes_payload.PostETHStakesPayload()  # noqa: E501
         if include_optional :
-            return PostSolStakes201Response(
-                data = kiln_connect.openapi_client.models.core_stake.CoreStake(
-                    id = '92f5bfd4-ea38-4824-84f7-686eddff5539', 
-                    tags = [
-                        'tag1'
-                        ], 
-                    metadata = kiln_connect.openapi_client.models.metadata.metadata(), 
-                    protocol = 'ethereum', 
-                    created_at = '2023-02-06T21:48:11.038Z', 
-                    updated_at = '2023-02-06T21:48:11.038Z', )
+            return PostETHStakesPayload(
+                stakes = [
+                    kiln_connect.openapi_client.models.post_eth_stakes_payload_stakes_inner.PostETHStakesPayload_stakes_inner(
+                        validator = '0x95373bcf8e2c64e1c373a6e534c002f210adbcc84c5abda3b6306677e171430ae50781a51c9f579a47622e334dba2412', )
+                    ], 
+                account_id = '92f5bfd4-ea38-4824-84f7-686eddff5539'
             )
         else :
-            return PostSolStakes201Response(
+            return PostETHStakesPayload(
+                stakes = [
+                    kiln_connect.openapi_client.models.post_eth_stakes_payload_stakes_inner.PostETHStakesPayload_stakes_inner(
+                        validator = '0x95373bcf8e2c64e1c373a6e534c002f210adbcc84c5abda3b6306677e171430ae50781a51c9f579a47622e334dba2412', )
+                    ],
+                account_id = '92f5bfd4-ea38-4824-84f7-686eddff5539',
         )
         """
 
-    def testPostSolStakes201Response(self):
-        """Test PostSolStakes201Response"""
+    def testPostETHStakesPayload(self):
+        """Test PostETHStakesPayload"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_ada_prepare_tx201_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,44 +13,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.post_xtz_prepare_tx201_response import PostXtzPrepareTx201Response  # noqa: E501
+from kiln_connect.openapi_client.models.post_ada_prepare_tx201_response import PostAdaPrepareTx201Response  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestPostXtzPrepareTx201Response(unittest.TestCase):
-    """PostXtzPrepareTx201Response unit test stubs"""
+class TestPostAdaPrepareTx201Response(unittest.TestCase):
+    """PostAdaPrepareTx201Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PostXtzPrepareTx201Response
+        """Test PostAdaPrepareTx201Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PostXtzPrepareTx201Response`
+        # uncomment below to create an instance of `PostAdaPrepareTx201Response`
         """
-        model = kiln_connect.openapi_client.models.post_xtz_prepare_tx201_response.PostXtzPrepareTx201Response()  # noqa: E501
+        model = kiln_connect.openapi_client.models.post_ada_prepare_tx201_response.PostAdaPrepareTx201Response()  # noqa: E501
         if include_optional :
-            return PostXtzPrepareTx201Response(
-                data = kiln_connect.openapi_client.models.xtz_signed_tx.XTZSignedTx(
-                    signed_tx_serialized = '0x20a40259b763d549dfa1c082776a036dd8dabbe8b5e32ee721be017512dc', )
+            return PostAdaPrepareTx201Response(
+                data = kiln_connect.openapi_client.models.ada_signed_tx.ADASignedTx(
+                    signed_tx_serialized = '84a500818258203d244a2821a0cb32df614cf4380e6c6e0114bc7c734cfa2a3940498ad86865e100018182583900491a1d0747fa91f319625e39076232ad4cc274e3257f345ced82dbb2a8565045c49103b521a3827ff64b98889350a22fa9a0b5ccf72b279b1b0000000255928400021a000493e0031a01ad4330048282008200581ca8565045c49103b521a3827ff64b98889350a22fa9a0b5ccf72b279b83028200581ca8565045c49103b521a3827ff64b98889350a22fa9a0b5ccf72b279b581ce54d5f9340218a9816cafafc92dc3d5212b6d149ce75e9637cbcd7e0a0f5f6', )
             )
         else :
-            return PostXtzPrepareTx201Response(
+            return PostAdaPrepareTx201Response(
         )
         """
 
-    def testPostXtzPrepareTx201Response(self):
-        """Test PostXtzPrepareTx201Response"""
+    def testPostAdaPrepareTx201Response(self):
+        """Test PostAdaPrepareTx201Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_matic_approve_tx201_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.post_xtz_stake_tx201_response import PostXtzStakeTx201Response  # noqa: E501
+from kiln_connect.openapi_client.models.post_matic_approve_tx201_response import PostMaticApproveTx201Response  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestPostXtzStakeTx201Response(unittest.TestCase):
-    """PostXtzStakeTx201Response unit test stubs"""
+class TestPostMaticApproveTx201Response(unittest.TestCase):
+    """PostMaticApproveTx201Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test PostXtzStakeTx201Response
+        """Test PostMaticApproveTx201Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PostXtzStakeTx201Response`
+        # uncomment below to create an instance of `PostMaticApproveTx201Response`
         """
-        model = kiln_connect.openapi_client.models.post_xtz_stake_tx201_response.PostXtzStakeTx201Response()  # noqa: E501
+        model = kiln_connect.openapi_client.models.post_matic_approve_tx201_response.PostMaticApproveTx201Response()  # noqa: E501
         if include_optional :
-            return PostXtzStakeTx201Response(
-                data = kiln_connect.openapi_client.models.xtz_unsigned_tx.XTZUnsignedTx(
+            return PostMaticApproveTx201Response(
+                data = kiln_connect.openapi_client.models.matic_unsigned_tx.MATICUnsignedTx(
                     unsigned_tx_hash = '0x43244f90814b31dec250de24df5bb023a338790c1d5a39244cf1064cf6d98c94', 
                     unsigned_tx_serialized = '0x20a40259b763d549dfa1c082776a036dd8dabbe8b5e32ee721be017512dc', )
             )
         else :
-            return PostXtzStakeTx201Response(
+            return PostMaticApproveTx201Response(
         )
         """
 
-    def testPostXtzStakeTx201Response(self):
-        """Test PostXtzStakeTx201Response"""
+    def testPostMaticApproveTx201Response(self):
+        """Test PostMaticApproveTx201Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_api.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `SOLBroadcastTx`
         """
         model = kiln_connect.openapi_client.models.sol_broadcast_tx.SOLBroadcastTx()  # noqa: E501
         if include_optional :
             return SOLBroadcastTx(
-                tx_hash = ''
+                tx_hash = 'sV6dgQyxByL66t9uTPmffitncWNmnkR8oEC1gQ29jPrKFHm9TkMGvS3TgcQeNz9pSN7913aPXe6MMHFS4xqTafL'
             )
         else :
             return SOLBroadcastTx(
         )
         """
 
     def testSOLBroadcastTx(self):
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,44 +13,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.sol_broadcast_tx_payload import SOLBroadcastTxPayload  # noqa: E501
+from kiln_connect.openapi_client.models.xtz_broadcasted_tx import XTZBroadcastedTx  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestSOLBroadcastTxPayload(unittest.TestCase):
-    """SOLBroadcastTxPayload unit test stubs"""
+class TestXTZBroadcastedTx(unittest.TestCase):
+    """XTZBroadcastedTx unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SOLBroadcastTxPayload
+        """Test XTZBroadcastedTx
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SOLBroadcastTxPayload`
+        # uncomment below to create an instance of `XTZBroadcastedTx`
         """
-        model = kiln_connect.openapi_client.models.sol_broadcast_tx_payload.SOLBroadcastTxPayload()  # noqa: E501
+        model = kiln_connect.openapi_client.models.xtz_broadcasted_tx.XTZBroadcastedTx()  # noqa: E501
         if include_optional :
-            return SOLBroadcastTxPayload(
-                tx_serialized = ''
+            return XTZBroadcastedTx(
+                tx_hash = 'oo3UAUpr685s3F7Fmc2ry8KHo4vdWGKo7LeimesAg56NBd6sDjs'
             )
         else :
-            return SOLBroadcastTxPayload(
-                tx_serialized = '',
+            return XTZBroadcastedTx(
         )
         """
 
-    def testSOLBroadcastTxPayload(self):
-        """Test SOLBroadcastTxPayload"""
+    def testXTZBroadcastedTx(self):
+        """Test XTZBroadcastedTx"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_network_stats.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_create_account.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_create_account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_create_account_with_seed.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_create_account_with_seed.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_deactivate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_deactivate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_delegate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_delegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_merge.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_merge.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_redelegate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_redelegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_split.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_split.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_withdraw.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_operation_withdraw.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_atom_stakes_payload_stakes_inner.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,50 +13,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.sol_prepare_tx_payload import SOLPrepareTxPayload  # noqa: E501
+from kiln_connect.openapi_client.models.post_atom_stakes_payload_stakes_inner import PostATOMStakesPayloadStakesInner  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestSOLPrepareTxPayload(unittest.TestCase):
-    """SOLPrepareTxPayload unit test stubs"""
+class TestPostATOMStakesPayloadStakesInner(unittest.TestCase):
+    """PostATOMStakesPayloadStakesInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SOLPrepareTxPayload
+        """Test PostATOMStakesPayloadStakesInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SOLPrepareTxPayload`
+        # uncomment below to create an instance of `PostATOMStakesPayloadStakesInner`
         """
-        model = kiln_connect.openapi_client.models.sol_prepare_tx_payload.SOLPrepareTxPayload()  # noqa: E501
+        model = kiln_connect.openapi_client.models.post_atom_stakes_payload_stakes_inner.PostATOMStakesPayloadStakesInner()  # noqa: E501
         if include_optional :
-            return SOLPrepareTxPayload(
-                unsigned_tx_serialized = '', 
-                signatures = [
-                    ''
-                    ]
+            return PostATOMStakesPayloadStakesInner(
+                stake_id = 'cosmosvaloper1y0us8xvsvfvqkk9c6nt5cfyu5au5tww2ztve7q_cosmos1005jmz7uk4pwwc0mefqxmw03ut0elruv0e9wv3', 
+                balance = 1000000
             )
         else :
-            return SOLPrepareTxPayload(
-                unsigned_tx_serialized = '',
-                signatures = [
-                    ''
-                    ],
+            return PostATOMStakesPayloadStakesInner(
         )
         """
 
-    def testSOLPrepareTxPayload(self):
-        """Test SOLPrepareTxPayload"""
+    def testPostATOMStakesPayloadStakesInner(self):
+        """Test PostATOMStakesPayloadStakesInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_prepared_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_signed_tx.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,43 +13,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.sol_prepared_tx import SOLPreparedTx  # noqa: E501
+from kiln_connect.openapi_client.models.matic_signed_tx import MATICSignedTx  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestSOLPreparedTx(unittest.TestCase):
-    """SOLPreparedTx unit test stubs"""
+class TestMATICSignedTx(unittest.TestCase):
+    """MATICSignedTx unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SOLPreparedTx
+        """Test MATICSignedTx
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SOLPreparedTx`
+        # uncomment below to create an instance of `MATICSignedTx`
         """
-        model = kiln_connect.openapi_client.models.sol_prepared_tx.SOLPreparedTx()  # noqa: E501
+        model = kiln_connect.openapi_client.models.matic_signed_tx.MATICSignedTx()  # noqa: E501
         if include_optional :
-            return SOLPreparedTx(
-                signed_tx_serialized = ''
+            return MATICSignedTx(
+                signed_tx_serialized = '0x20a40259b763d549dfa1c082776a036dd8dabbe8b5e32ee721be017512dc'
             )
         else :
-            return SOLPreparedTx(
+            return MATICSignedTx(
         )
         """
 
-    def testSOLPreparedTx(self):
-        """Test SOLPreparedTx"""
+    def testMATICSignedTx(self):
+        """Test MATICSignedTx"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_reward_by_day.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_reward_by_day.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_stake.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,54 +13,54 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.sol_stake import SOLStake  # noqa: E501
+from kiln_connect.openapi_client.models.xtz_stake import XTZStake  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestSOLStake(unittest.TestCase):
-    """SOLStake unit test stubs"""
+class TestXTZStake(unittest.TestCase):
+    """XTZStake unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SOLStake
+        """Test XTZStake
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SOLStake`
+        # uncomment below to create an instance of `XTZStake`
         """
-        model = kiln_connect.openapi_client.models.sol_stake.SOLStake()  # noqa: E501
+        model = kiln_connect.openapi_client.models.xtz_stake.XTZStake()  # noqa: E501
         if include_optional :
-            return SOLStake(
-                stake_account = '3sfokk2DFsd88ujd8sfa9slsdf99kjnFJksdf', 
-                vote_account = '6hNweZvzTudTuprZrAXb1A9grKvVG6xgjyvdJUqAMk78', 
-                withdraw_pubkey = '4wdr76KJTFgH68YtGddmnF45WdD8LMv9eLsdf', 
+            return XTZStake(
+                stake_address = 'tz1VZ4iC4wzTR7iK2Q7PoQGVDAojuY42fDxD', 
+                baker_address = 'tz2FCNBrERXtaTtNX6iimR1UJ5JSDxvdHM93', 
                 state = 'active', 
                 activated_at = '2023-01-14T01:13:59Z', 
-                activated_epoch = 150, 
-                deactivated_at = '2023-01-14T01:13:59Z', 
-                deactivated_epoch = 150, 
-                balance = '1000000000', 
-                rewards = '1000000000', 
-                net_apy = 3.407, 
+                activated_cycle = 542, 
+                delegated_at = '2023-01-14T01:13:59Z', 
+                delegated_cycle = 542, 
+                delegated_block = '16397387', 
+                balance = '32076187808000000000', 
+                rewards = '76187808000000000', 
+                gross_apy = 3.407, 
                 updated_at = '2023-01-14T01:13:59Z'
             )
         else :
-            return SOLStake(
+            return XTZStake(
         )
         """
 
-    def testSOLStake(self):
-        """Test SOLStake"""
+    def testXTZStake(self):
+        """Test XTZStake"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,44 +13,51 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.sol_stake_tx import SOLStakeTx  # noqa: E501
+from kiln_connect.openapi_client.models.sol_stake_tx_payload import SOLStakeTxPayload  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestSOLStakeTx(unittest.TestCase):
-    """SOLStakeTx unit test stubs"""
+class TestSOLStakeTxPayload(unittest.TestCase):
+    """SOLStakeTxPayload unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SOLStakeTx
+        """Test SOLStakeTxPayload
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SOLStakeTx`
+        # uncomment below to create an instance of `SOLStakeTxPayload`
         """
-        model = kiln_connect.openapi_client.models.sol_stake_tx.SOLStakeTx()  # noqa: E501
+        model = kiln_connect.openapi_client.models.sol_stake_tx_payload.SOLStakeTxPayload()  # noqa: E501
         if include_optional :
-            return SOLStakeTx(
-                unsigned_tx_hash = '', 
-                unsigned_tx_serialized = ''
+            return SOLStakeTxPayload(
+                account_id = 'd3f1b917-72b1-4982-a4dd-93fce579a708', 
+                wallet = '4icse2mPXNgyxxn11tVM7sTnSqDqwJSEzdnaCQnRzvA9', 
+                amount_lamports = '1000000000000000', 
+                vote_account_address = '5pPRHniefFjkiaArbGX3Y8NUysJmQ9tMZg3FrFGwHzSm', 
+                memo = 'custom message'
             )
         else :
-            return SOLStakeTx(
+            return SOLStakeTxPayload(
+                account_id = 'd3f1b917-72b1-4982-a4dd-93fce579a708',
+                wallet = '4icse2mPXNgyxxn11tVM7sTnSqDqwJSEzdnaCQnRzvA9',
+                amount_lamports = '1000000000000000',
+                vote_account_address = '5pPRHniefFjkiaArbGX3Y8NUysJmQ9tMZg3FrFGwHzSm',
         )
         """
 
-    def testSOLStakeTx(self):
-        """Test SOLStakeTx"""
+    def testSOLStakeTxPayload(self):
+        """Test SOLStakeTxPayload"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,50 +13,47 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.sol_stake_tx_payload import SOLStakeTxPayload  # noqa: E501
+from kiln_connect.openapi_client.models.sol_withdraw_stake_tx_payload import SOLWithdrawStakeTxPayload  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestSOLStakeTxPayload(unittest.TestCase):
-    """SOLStakeTxPayload unit test stubs"""
+class TestSOLWithdrawStakeTxPayload(unittest.TestCase):
+    """SOLWithdrawStakeTxPayload unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SOLStakeTxPayload
+        """Test SOLWithdrawStakeTxPayload
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SOLStakeTxPayload`
+        # uncomment below to create an instance of `SOLWithdrawStakeTxPayload`
         """
-        model = kiln_connect.openapi_client.models.sol_stake_tx_payload.SOLStakeTxPayload()  # noqa: E501
+        model = kiln_connect.openapi_client.models.sol_withdraw_stake_tx_payload.SOLWithdrawStakeTxPayload()  # noqa: E501
         if include_optional :
-            return SOLStakeTxPayload(
-                account_id = 'd3f1b917-72b1-4982-a4dd-93fce579a708', 
+            return SOLWithdrawStakeTxPayload(
+                stake_account = '3M7sFDMdUxfNNSmKk2ZmDKgKJFzuLvxpuXKDTLRGXpcK', 
                 wallet = '4icse2mPXNgyxxn11tVM7sTnSqDqwJSEzdnaCQnRzvA9', 
-                amount_lamports = '1000000000000000', 
-                vote_account_address = '5pPRHniefFjkiaArbGX3Y8NUysJmQ9tMZg3FrFGwHzSm'
+                amount_lamports = '1000000000000000'
             )
         else :
-            return SOLStakeTxPayload(
-                account_id = 'd3f1b917-72b1-4982-a4dd-93fce579a708',
+            return SOLWithdrawStakeTxPayload(
+                stake_account = '3M7sFDMdUxfNNSmKk2ZmDKgKJFzuLvxpuXKDTLRGXpcK',
                 wallet = '4icse2mPXNgyxxn11tVM7sTnSqDqwJSEzdnaCQnRzvA9',
-                amount_lamports = '1000000000000000',
-                vote_account_address = '5pPRHniefFjkiaArbGX3Y8NUysJmQ9tMZg3FrFGwHzSm',
         )
         """
 
-    def testSOLStakeTxPayload(self):
-        """Test SOLStakeTxPayload"""
+    def testSOLWithdrawStakeTxPayload(self):
+        """Test SOLWithdrawStakeTxPayload"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,47 +13,48 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.sol_withdraw_stake_tx_payload import SOLWithdrawStakeTxPayload  # noqa: E501
+from kiln_connect.openapi_client.models.xtz_craft_stake_tx_payload import XTZCraftStakeTxPayload  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestSOLWithdrawStakeTxPayload(unittest.TestCase):
-    """SOLWithdrawStakeTxPayload unit test stubs"""
+class TestXTZCraftStakeTxPayload(unittest.TestCase):
+    """XTZCraftStakeTxPayload unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SOLWithdrawStakeTxPayload
+        """Test XTZCraftStakeTxPayload
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SOLWithdrawStakeTxPayload`
+        # uncomment below to create an instance of `XTZCraftStakeTxPayload`
         """
-        model = kiln_connect.openapi_client.models.sol_withdraw_stake_tx_payload.SOLWithdrawStakeTxPayload()  # noqa: E501
+        model = kiln_connect.openapi_client.models.xtz_craft_stake_tx_payload.XTZCraftStakeTxPayload()  # noqa: E501
         if include_optional :
-            return SOLWithdrawStakeTxPayload(
-                stake_account = '3M7sFDMdUxfNNSmKk2ZmDKgKJFzuLvxpuXKDTLRGXpcK', 
-                wallet = '4icse2mPXNgyxxn11tVM7sTnSqDqwJSEzdnaCQnRzvA9', 
-                amount_lamports = '1000000000000000'
+            return XTZCraftStakeTxPayload(
+                account_id = 'b7177fd2-fbb3-479f-aa92-db9fb16e229f', 
+                wallet = 'tz1QQZKGt3ouyd7x8JUDwcvRyxzsmD7CFbMd', 
+                baker_address = 'tz3btDQsDkqq2G7eBdrrLqetaAfLVw6BnPez'
             )
         else :
-            return SOLWithdrawStakeTxPayload(
-                stake_account = '3M7sFDMdUxfNNSmKk2ZmDKgKJFzuLvxpuXKDTLRGXpcK',
-                wallet = '4icse2mPXNgyxxn11tVM7sTnSqDqwJSEzdnaCQnRzvA9',
+            return XTZCraftStakeTxPayload(
+                account_id = 'b7177fd2-fbb3-479f-aa92-db9fb16e229f',
+                wallet = 'tz1QQZKGt3ouyd7x8JUDwcvRyxzsmD7CFbMd',
+                baker_address = 'tz3btDQsDkqq2G7eBdrrLqetaAfLVw6BnPez',
         )
         """
 
-    def testSOLWithdrawStakeTxPayload(self):
-        """Test SOLWithdrawStakeTxPayload"""
+    def testXTZCraftStakeTxPayload(self):
+        """Test XTZCraftStakeTxPayload"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_soltx_status.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_portfolio_protocols_inner.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,44 +13,54 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.soltx_status import SOLTxStatus  # noqa: E501
+from kiln_connect.openapi_client.models.portfolio_protocols_inner import PortfolioProtocolsInner  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestSOLTxStatus(unittest.TestCase):
-    """SOLTxStatus unit test stubs"""
+class TestPortfolioProtocolsInner(unittest.TestCase):
+    """PortfolioProtocolsInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SOLTxStatus
+        """Test PortfolioProtocolsInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SOLTxStatus`
+        # uncomment below to create an instance of `PortfolioProtocolsInner`
         """
-        model = kiln_connect.openapi_client.models.soltx_status.SOLTxStatus()  # noqa: E501
+        model = kiln_connect.openapi_client.models.portfolio_protocols_inner.PortfolioProtocolsInner()  # noqa: E501
         if include_optional :
-            return SOLTxStatus(
-                status = 'success', 
-                receipt = None
+            return PortfolioProtocolsInner(
+                token = 'eth', 
+                name = 'Ethereum', 
+                total_stakes = 12, 
+                total_active_stakes = 10, 
+                total_balance = kiln_connect.openapi_client.models.portfolio_protocols_inner_total_balance.Portfolio_protocols_inner_total_balance(
+                    amount_usd = 10896.4568, 
+                    amount = 1896.4563, ), 
+                total_rewards = kiln_connect.openapi_client.models.portfolio_protocols_inner_total_rewards.Portfolio_protocols_inner_total_rewards(
+                    amount_usd = 10896.4568, 
+                    amount = 1896.4568, ), 
+                balance_share_percent = 42.59, 
+                rewards_share_percent = 42.59
             )
         else :
-            return SOLTxStatus(
+            return PortfolioProtocolsInner(
         )
         """
 
-    def testSOLTxStatus(self):
-        """Test SOLTxStatus"""
+    def testPortfolioProtocolsInner(self):
+        """Test PortfolioProtocolsInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_api.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,86 +12,86 @@
 
 
 from __future__ import absolute_import
 
 import unittest
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.api.xtz_api import XtzApi  # noqa: E501
+from kiln_connect.openapi_client.api.matic_api import MaticApi  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
 
-class TestXtzApi(unittest.TestCase):
-    """XtzApi unit test stubs"""
+class TestMaticApi(unittest.TestCase):
+    """MaticApi unit test stubs"""
 
     def setUp(self):
-        self.api = kiln_connect.openapi_client.api.xtz_api.XtzApi()  # noqa: E501
+        self.api = kiln_connect.openapi_client.api.matic_api.MaticApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_get_xtz_network_stats(self):
-        """Test case for get_xtz_network_stats
+    def test_get_matic_tx_status(self):
+        """Test case for get_matic_tx_status
 
-        Network Stats  # noqa: E501
+        Transaction Status  # noqa: E501
         """
         pass
 
-    def test_get_xtz_operations(self):
-        """Test case for get_xtz_operations
+    def test_post_matic_approve_tx(self):
+        """Test case for post_matic_approve_tx
 
-        Operations  # noqa: E501
+        Approve Transaction  # noqa: E501
         """
         pass
 
-    def test_get_xtz_rewards(self):
-        """Test case for get_xtz_rewards
+    def test_post_matic_broadcast_tx(self):
+        """Test case for post_matic_broadcast_tx
 
-        Rewards  # noqa: E501
+        Broadcast Transaction  # noqa: E501
         """
         pass
 
-    def test_get_xtz_stakes(self):
-        """Test case for get_xtz_stakes
+    def test_post_matic_buy_voucher_tx(self):
+        """Test case for post_matic_buy_voucher_tx
 
-        Stakes  # noqa: E501
+        Buy Voucher Transaction  # noqa: E501
         """
         pass
 
-    def test_get_xtz_tx_status(self):
-        """Test case for get_xtz_tx_status
+    def test_post_matic_prepare_tx(self):
+        """Test case for post_matic_prepare_tx
 
-        Transaction Status  # noqa: E501
+        Prepare Transaction  # noqa: E501
         """
         pass
 
-    def test_post_xtz_broadcast_tx(self):
-        """Test case for post_xtz_broadcast_tx
+    def test_post_matic_restake_rewards_tx(self):
+        """Test case for post_matic_restake_rewards_tx
 
-        Broadcast Transaction  # noqa: E501
+        Restake Rewards Transaction  # noqa: E501
         """
         pass
 
-    def test_post_xtz_prepare_tx(self):
-        """Test case for post_xtz_prepare_tx
+    def test_post_matic_sell_voucher_tx(self):
+        """Test case for post_matic_sell_voucher_tx
 
-        Prepare Transaction  # noqa: E501
+        Sell Voucher Transaction  # noqa: E501
         """
         pass
 
-    def test_post_xtz_stake_tx(self):
-        """Test case for post_xtz_stake_tx
+    def test_post_matic_unstake_claim_tokens_tx(self):
+        """Test case for post_matic_unstake_claim_tokens_tx
 
-        Stake Transaction  # noqa: E501
+        Unstake Claim Tokens Transaction  # noqa: E501
         """
         pass
 
-    def test_post_xtz_un_stake_tx(self):
-        """Test case for post_xtz_un_stake_tx
+    def test_post_matic_withdraw_rewards_tx(self):
+        """Test case for post_matic_withdraw_rewards_tx
 
-        Unstake Transaction  # noqa: E501
+        Withdraw Rewards Transaction  # noqa: E501
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_ada_broadcast_tx201_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,43 +13,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.xtz_broadcasted_tx import XTZBroadcastedTx  # noqa: E501
+from kiln_connect.openapi_client.models.post_ada_broadcast_tx201_response import PostAdaBroadcastTx201Response  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestXTZBroadcastedTx(unittest.TestCase):
-    """XTZBroadcastedTx unit test stubs"""
+class TestPostAdaBroadcastTx201Response(unittest.TestCase):
+    """PostAdaBroadcastTx201Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XTZBroadcastedTx
+        """Test PostAdaBroadcastTx201Response
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `XTZBroadcastedTx`
+        # uncomment below to create an instance of `PostAdaBroadcastTx201Response`
         """
-        model = kiln_connect.openapi_client.models.xtz_broadcasted_tx.XTZBroadcastedTx()  # noqa: E501
+        model = kiln_connect.openapi_client.models.post_ada_broadcast_tx201_response.PostAdaBroadcastTx201Response()  # noqa: E501
         if include_optional :
-            return XTZBroadcastedTx(
-                tx_hash = 'oo3UAUpr685s3F7Fmc2ry8KHo4vdWGKo7LeimesAg56NBd6sDjs'
+            return PostAdaBroadcastTx201Response(
+                data = kiln_connect.openapi_client.models.adatx_hash.ADATxHash(
+                    tx_hash = '7f12d9eacd762d130838289397480e495db0fd268bd3be4fd55c74a74fd8372d', )
             )
         else :
-            return XTZBroadcastedTx(
+            return PostAdaBroadcastTx201Response(
         )
         """
 
-    def testXTZBroadcastedTx(self):
-        """Test XTZBroadcastedTx"""
+    def testPostAdaBroadcastTx201Response(self):
+        """Test PostAdaBroadcastTx201Response"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_craft_stake_tx_payload.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,48 +13,50 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.xtz_craft_stake_tx_payload import XTZCraftStakeTxPayload  # noqa: E501
+from kiln_connect.openapi_client.models.atom_craft_stake_tx_payload import ATOMCraftStakeTxPayload  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestXTZCraftStakeTxPayload(unittest.TestCase):
-    """XTZCraftStakeTxPayload unit test stubs"""
+class TestATOMCraftStakeTxPayload(unittest.TestCase):
+    """ATOMCraftStakeTxPayload unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XTZCraftStakeTxPayload
+        """Test ATOMCraftStakeTxPayload
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `XTZCraftStakeTxPayload`
+        # uncomment below to create an instance of `ATOMCraftStakeTxPayload`
         """
-        model = kiln_connect.openapi_client.models.xtz_craft_stake_tx_payload.XTZCraftStakeTxPayload()  # noqa: E501
+        model = kiln_connect.openapi_client.models.atom_craft_stake_tx_payload.ATOMCraftStakeTxPayload()  # noqa: E501
         if include_optional :
-            return XTZCraftStakeTxPayload(
+            return ATOMCraftStakeTxPayload(
                 account_id = 'b7177fd2-fbb3-479f-aa92-db9fb16e229f', 
-                wallet = 'tz1QQZKGt3ouyd7x8JUDwcvRyxzsmD7CFbMd', 
-                baker_address = 'tz3btDQsDkqq2G7eBdrrLqetaAfLVw6BnPez'
+                pubkey = '039ce47b2a813d13876131a9c3be77e8c4afa49e948744abbee11f939e2a420f46', 
+                validator = 'cosmosvaloper16ys0eg935mkqpkydkgfcj9age2au8l96naere9', 
+                amount_uatom = '1000000000000000000000000'
             )
         else :
-            return XTZCraftStakeTxPayload(
+            return ATOMCraftStakeTxPayload(
                 account_id = 'b7177fd2-fbb3-479f-aa92-db9fb16e229f',
-                wallet = 'tz1QQZKGt3ouyd7x8JUDwcvRyxzsmD7CFbMd',
-                baker_address = 'tz3btDQsDkqq2G7eBdrrLqetaAfLVw6BnPez',
+                pubkey = '039ce47b2a813d13876131a9c3be77e8c4afa49e948744abbee11f939e2a420f46',
+                validator = 'cosmosvaloper16ys0eg935mkqpkydkgfcj9age2au8l96naere9',
+                amount_uatom = '1000000000000000000000000',
         )
         """
 
-    def testXTZCraftStakeTxPayload(self):
-        """Test XTZCraftStakeTxPayload"""
+    def testATOMCraftStakeTxPayload(self):
+        """Test ATOMCraftStakeTxPayload"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_daily_reward.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_daily_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_network_stats.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_activation.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_operation_activation.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_delegate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_adatx_hash.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,51 +13,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.xtz_operation_delegate import XTZOperationDelegate  # noqa: E501
+from kiln_connect.openapi_client.models.adatx_hash import ADATxHash  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestXTZOperationDelegate(unittest.TestCase):
-    """XTZOperationDelegate unit test stubs"""
+class TestADATxHash(unittest.TestCase):
+    """ADATxHash unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XTZOperationDelegate
+        """Test ADATxHash
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `XTZOperationDelegate`
+        # uncomment below to create an instance of `ADATxHash`
         """
-        model = kiln_connect.openapi_client.models.xtz_operation_delegate.XTZOperationDelegate()  # noqa: E501
+        model = kiln_connect.openapi_client.models.adatx_hash.ADATxHash()  # noqa: E501
         if include_optional :
-            return XTZOperationDelegate(
-                type = 'delegate', 
-                var_date = '2023-01-14T01:13:59Z', 
-                staker_address = 'tz1QQZKGt3ouyd7x8JUDwcvRyxzsmD7CFbMd', 
-                baker_address = 'tz3btDQsDkqq2G7eBdrrLqetaAfLVw6BnPez', 
-                operation = 'opLq44uJLP7f3V3zCVDCDgXayV3CQLGqihdoAYtMnXLW4f1q2fb', 
-                operation_gas_used = '10', 
-                baker_fee = '42', 
-                block = 1342, 
-                amount = '420000'
+            return ADATxHash(
+                tx_hash = '7f12d9eacd762d130838289397480e495db0fd268bd3be4fd55c74a74fd8372d'
             )
         else :
-            return XTZOperationDelegate(
+            return ADATxHash(
         )
         """
 
-    def testXTZOperationDelegate(self):
-        """Test XTZOperationDelegate"""
+    def testADATxHash(self):
+        """Test ADATxHash"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_payment.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_operation_payment.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_undelegate.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_operation_undelegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_signed_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_xtz_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_stake.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_ada_unsigned_tx.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,54 +13,45 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.xtz_stake import XTZStake  # noqa: E501
+from kiln_connect.openapi_client.models.ada_unsigned_tx import ADAUnsignedTx  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestXTZStake(unittest.TestCase):
-    """XTZStake unit test stubs"""
+class TestADAUnsignedTx(unittest.TestCase):
+    """ADAUnsignedTx unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XTZStake
+        """Test ADAUnsignedTx
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `XTZStake`
+        # uncomment below to create an instance of `ADAUnsignedTx`
         """
-        model = kiln_connect.openapi_client.models.xtz_stake.XTZStake()  # noqa: E501
+        model = kiln_connect.openapi_client.models.ada_unsigned_tx.ADAUnsignedTx()  # noqa: E501
         if include_optional :
-            return XTZStake(
-                stake_address = 'tz1VZ4iC4wzTR7iK2Q7PoQGVDAojuY42fDxD', 
-                baker_address = 'tz2FCNBrERXtaTtNX6iimR1UJ5JSDxvdHM93', 
-                state = 'active', 
-                activated_at = '2023-01-14T01:13:59Z', 
-                activated_cycle = 542, 
-                delegated_at = '2023-01-14T01:13:59Z', 
-                delegated_cycle = 542, 
-                delegated_block = '16397387', 
-                balance = '32076187808000000000', 
-                rewards = '76187808000000000', 
-                gross_apy = 3.407, 
-                updated_at = '2023-01-14T01:13:59Z'
+            return ADAUnsignedTx(
+                unsigned_tx_hash = 'ea62bc381a2d8fc338f24634674a168fdc8f1a09b978f24f026041f4e00c876f', 
+                unsigned_tx_serialized = '84a500818258203d244a2821a0cb32df614cf4380e6c6e0114bc7c734cfa2a3940498ad86865e100018182583900491a1d0747fa91f319625e39076232ad4cc274e3257f345ced82dbb2a8565045c49103b521a3827ff64b98889350a22fa9a0b5ccf72b279b1b0000000255928400021a000493e0031a01ad4330048282008200581ca8565045c49103b521a3827ff64b98889350a22fa9a0b5ccf72b279b83028200581ca8565045c49103b521a3827ff64b98889350a22fa9a0b5ccf72b279b581ce54d5f9340218a9816cafafc92dc3d5212b6d149ce75e9637cbcd7e0a0f5f6', 
+                inputs = [{"transaction_id":"3d244a2821a0cb32df614cf4380e6c6e0114bc7c734cfa2a3940498ad86865e1","index":0}]
             )
         else :
-            return XTZStake(
+            return ADAUnsignedTx(
         )
         """
 
-    def testXTZStake(self):
-        """Test XTZStake"""
+    def testADAUnsignedTx(self):
+        """Test ADAUnsignedTx"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_matic_unsigned_tx.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,44 +13,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.xtz_unsigned_tx import XTZUnsignedTx  # noqa: E501
+from kiln_connect.openapi_client.models.matic_unsigned_tx import MATICUnsignedTx  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestXTZUnsignedTx(unittest.TestCase):
-    """XTZUnsignedTx unit test stubs"""
+class TestMATICUnsignedTx(unittest.TestCase):
+    """MATICUnsignedTx unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XTZUnsignedTx
+        """Test MATICUnsignedTx
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `XTZUnsignedTx`
+        # uncomment below to create an instance of `MATICUnsignedTx`
         """
-        model = kiln_connect.openapi_client.models.xtz_unsigned_tx.XTZUnsignedTx()  # noqa: E501
+        model = kiln_connect.openapi_client.models.matic_unsigned_tx.MATICUnsignedTx()  # noqa: E501
         if include_optional :
-            return XTZUnsignedTx(
+            return MATICUnsignedTx(
                 unsigned_tx_hash = '0x43244f90814b31dec250de24df5bb023a338790c1d5a39244cf1064cf6d98c94', 
                 unsigned_tx_serialized = '0x20a40259b763d549dfa1c082776a036dd8dabbe8b5e32ee721be017512dc'
             )
         else :
-            return XTZUnsignedTx(
+            return MATICUnsignedTx(
         )
         """
 
-    def testXTZUnsignedTx(self):
-        """Test XTZUnsignedTx"""
+    def testMATICUnsignedTx(self):
+        """Test MATICUnsignedTx"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtztx_status.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_atom_network_stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,51 +13,47 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.xtztx_status import XTZTxStatus  # noqa: E501
+from kiln_connect.openapi_client.models.atom_network_stats import ATOMNetworkStats  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestXTZTxStatus(unittest.TestCase):
-    """XTZTxStatus unit test stubs"""
+class TestATOMNetworkStats(unittest.TestCase):
+    """ATOMNetworkStats unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XTZTxStatus
+        """Test ATOMNetworkStats
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `XTZTxStatus`
+        # uncomment below to create an instance of `ATOMNetworkStats`
         """
-        model = kiln_connect.openapi_client.models.xtztx_status.XTZTxStatus()  # noqa: E501
+        model = kiln_connect.openapi_client.models.atom_network_stats.ATOMNetworkStats()  # noqa: E501
         if include_optional :
-            return XTZTxStatus(
-                status = '', 
-                receipt = kiln_connect.openapi_client.models.xtztx_status_receipt.XTZTxStatus_receipt(
-                    protocol = '', 
-                    chain_id = '', 
-                    hash = '', 
-                    branch = '', 
-                    contents = kiln_connect.openapi_client.models.contents.contents(), 
-                    signature = '', 
-                    metadata = kiln_connect.openapi_client.models.metadata.metadata(), )
+            return ATOMNetworkStats(
+                nb_validators = 100, 
+                network_gross_apy = 4.5, 
+                supply_staked_percent = 12.4, 
+                atom_price_usd = 10.53, 
+                updated_at = '2023-01-14T01:13:59Z'
             )
         else :
-            return XTZTxStatus(
+            return ATOMNetworkStats(
         )
         """
 
-    def testXTZTxStatus(self):
-        """Test XTZTxStatus"""
+    def testATOMNetworkStats(self):
+        """Test ATOMNetworkStats"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py` & `kiln_connect-1.0.0.dev7/kiln_connect/openapi_client/test/test_post_eth_stakes_payload_stakes_inner.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,49 +13,43 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import kiln_connect.openapi_client
-from kiln_connect.openapi_client.models.xtztx_status_receipt import XTZTxStatusReceipt  # noqa: E501
+from kiln_connect.openapi_client.models.post_eth_stakes_payload_stakes_inner import PostETHStakesPayloadStakesInner  # noqa: E501
 from kiln_connect.openapi_client.rest import ApiException
 
-class TestXTZTxStatusReceipt(unittest.TestCase):
-    """XTZTxStatusReceipt unit test stubs"""
+class TestPostETHStakesPayloadStakesInner(unittest.TestCase):
+    """PostETHStakesPayloadStakesInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XTZTxStatusReceipt
+        """Test PostETHStakesPayloadStakesInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `XTZTxStatusReceipt`
+        # uncomment below to create an instance of `PostETHStakesPayloadStakesInner`
         """
-        model = kiln_connect.openapi_client.models.xtztx_status_receipt.XTZTxStatusReceipt()  # noqa: E501
+        model = kiln_connect.openapi_client.models.post_eth_stakes_payload_stakes_inner.PostETHStakesPayloadStakesInner()  # noqa: E501
         if include_optional :
-            return XTZTxStatusReceipt(
-                protocol = '', 
-                chain_id = '', 
-                hash = '', 
-                branch = '', 
-                contents = kiln_connect.openapi_client.models.contents.contents(), 
-                signature = '', 
-                metadata = kiln_connect.openapi_client.models.metadata.metadata()
+            return PostETHStakesPayloadStakesInner(
+                validator = '0x95373bcf8e2c64e1c373a6e534c002f210adbcc84c5abda3b6306677e171430ae50781a51c9f579a47622e334dba2412'
             )
         else :
-            return XTZTxStatusReceipt(
+            return PostETHStakesPayloadStakesInner(
         )
         """
 
-    def testXTZTxStatusReceipt(self):
-        """Test XTZTxStatusReceipt"""
+    def testPostETHStakesPayloadStakesInner(self):
+        """Test PostETHStakesPayloadStakesInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/sol.py` & `kiln_connect-1.0.0.dev7/kiln_connect/sol.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/kiln_connect/xtz.py` & `kiln_connect-1.0.0.dev7/kiln_connect/xtz.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev6/pyproject.toml` & `kiln_connect-1.0.0.dev7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kiln-connect"
-version = "1.0.0-dev6"
+version = "1.0.0-dev7"
 description = ""
 authors = ["s. rannou <mxs@sbrk.org>"]
 maintainers = ["s. rannou <mxs@sbrk.org>"]
 readme = "docs/README.md"
 homepage = "https://kiln.fi/"
 repository = "https://github.com/kilnfi/sdk-py"
 keywords = ["staking", "blockchain"]
```

### Comparing `kiln_connect-1.0.0.dev6/PKG-INFO` & `kiln_connect-1.0.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiln-connect
-Version: 1.0.0.dev6
+Version: 1.0.0.dev7
 Summary: 
 Home-page: https://kiln.fi/
 Keywords: staking,blockchain
 Author: s. rannou
 Author-email: mxs@sbrk.org
 Maintainer: s. rannou
 Maintainer-email: mxs@sbrk.org
```

