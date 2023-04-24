# Comparing `tmp/kiln_connect-1.0.0.dev5.tar.gz` & `tmp/kiln_connect-1.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiln_connect-1.0.0.dev5.tar", max compression
+gzip compressed data, was "kiln_connect-1.0.0.dev6.tar", max compression
```

## Comparing `kiln_connect-1.0.0.dev5.tar` & `kiln_connect-1.0.0.dev6.tar`

### file list

```diff
@@ -1,244 +1,256 @@
--rw-r--r--   0        0        0     5728 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev5/docs/README.md
--rw-r--r--   0        0        0        0 2023-02-14 16:33:38.709950 kiln_connect-1.0.0.dev5/kiln_cli/__init__.py
--rw-r--r--   0        0        0     4536 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev5/kiln_cli/accounts.py
--rw-r--r--   0        0        0     2520 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_cli/atom.py
--rw-r--r--   0        0        0     6670 2023-04-06 15:53:36.351598 kiln_connect-1.0.0.dev5/kiln_cli/eth.py
--rw-r--r--   0        0        0      410 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_cli/main.py
--rwxr-xr-x   0        0        0    10741 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_cli/sol.py
--rw-r--r--   0        0        0     6844 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev5/kiln_cli/xtz.py
--rw-r--r--   0        0        0      155 2023-03-03 17:16:30.658551 kiln_connect-1.0.0.dev5/kiln_connect/__init__.py
--rw-r--r--   0        0        0      535 2023-03-08 16:23:14.337182 kiln_connect-1.0.0.dev5/kiln_connect/accounts.py
--rw-r--r--   0        0        0      656 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/atom.py
--rw-r--r--   0        0        0      942 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev5/kiln_connect/errors.py
--rw-r--r--   0        0        0     4144 2023-04-14 03:37:21.881892 kiln_connect-1.0.0.dev5/kiln_connect/eth.py
--rw-r--r--   0        0        0     5301 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/integrations.py
--rw-r--r--   0        0        0     3649 2023-04-17 13:51:44.551380 kiln_connect-1.0.0.dev5/kiln_connect/kiln_connect.py
--rw-r--r--   0        0        0    11600 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/__init__.py
--rw-r--r--   0        0        0      394 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/__init__.py
--rw-r--r--   0        0        0    32819 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/accounts_api.py
--rw-r--r--   0        0        0    21212 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/atom_api.py
--rw-r--r--   0        0        0    79556 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/eth_api.py
--rw-r--r--   0        0        0   104060 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/sol_api.py
--rw-r--r--   0        0        0    59673 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/xtz_api.py
--rw-r--r--   0        0        0    30218 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api_client.py
--rw-r--r--   0        0        0    17494 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/configuration.py
--rw-r--r--   0        0        0     5713 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/exceptions.py
--rw-r--r--   0        0        0    10698 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/__init__.py
--rw-r--r--   0        0        0     3006 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account.py
--rw-r--r--   0        0        0     2782 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_payload.py
--rw-r--r--   0        0        0     4028 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_portfolio.py
--rw-r--r--   0        0        0     4878 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py
--rw-r--r--   0        0        0     3019 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py
--rw-r--r--   0        0        0     3016 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py
--rw-r--r--   0        0        0     3478 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/atom_reward.py
--rw-r--r--   0        0        0     4849 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/atom_stake.py
--rw-r--r--   0        0        0     3245 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/core_stake.py
--rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2639 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_broadcasted_tx.py
--rw-r--r--   0        0        0     3090 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2910 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_kiln_stats.py
--rw-r--r--   0        0        0     2971 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py
--rw-r--r--   0        0        0     3028 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_network_stats.py
--rw-r--r--   0        0        0     3485 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py
--rw-r--r--   0        0        0     4582 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_operation_deposit.py
--rw-r--r--   0        0        0     3820 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_operation_execution_reward.py
--rw-r--r--   0        0        0     3522 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py
--rw-r--r--   0        0        0     4456 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py
--rw-r--r--   0        0        0     3376 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_post_keys_payload.py
--rw-r--r--   0        0        0     3042 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py
--rw-r--r--   0        0        0     3846 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_reward.py
--rw-r--r--   0        0        0     2662 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_signed_tx.py
--rw-r--r--   0        0        0     7278 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_stake.py
--rw-r--r--   0        0        0     4514 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_unsigned_tx.py
--rw-r--r--   0        0        0     3024 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/ethtx_status.py
--rw-r--r--   0        0        0     5288 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/ethtx_status_receipt.py
--rw-r--r--   0        0        0     3681 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py
--rw-r--r--   0        0        0     2972 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_account_portfolio200_response.py
--rw-r--r--   0        0        0     3064 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_accounts200_response.py
--rw-r--r--   0        0        0     3098 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_atom_rewards200_response.py
--rw-r--r--   0        0        0     3087 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_atom_stakes200_response.py
--rw-r--r--   0        0        0     2929 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py
--rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py
--rw-r--r--   0        0        0     3220 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_operations200_response.py
--rw-r--r--   0        0        0     7941 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py
--rw-r--r--   0        0        0     3087 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_rewards200_response.py
--rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_stakes200_response.py
--rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py
--rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py
--rw-r--r--   0        0        0     3220 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_operations200_response.py
--rw-r--r--   0        0        0    13955 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_operations200_response_data_inner.py
--rw-r--r--   0        0        0     3187 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_rewards200_response.py
--rw-r--r--   0        0        0     5115 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_stakes200_response.py
--rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py
--rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py
--rw-r--r--   0        0        0     3187 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py
--rw-r--r--   0        0        0     5085 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py
--rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py
--rw-r--r--   0        0        0     2879 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_account201_response.py
--rw-r--r--   0        0        0     2966 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2959 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_keys201_response.py
--rw-r--r--   0        0        0     5501 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py
--rw-r--r--   0        0        0     2932 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py
--rw-r--r--   0        0        0     2926 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py
--rw-r--r--   0        0        0     2958 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2940 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py
--rw-r--r--   0        0        0     2914 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py
--rw-r--r--   0        0        0     2902 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_sol_stakes201_response.py
--rw-r--r--   0        0        0     2966 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2932 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py
--rw-r--r--   0        0        0     2926 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py
--rw-r--r--   0        0        0     2572 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_broadcast_tx.py
--rw-r--r--   0        0        0     2607 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2816 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py
--rw-r--r--   0        0        0     3015 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py
--rw-r--r--   0        0        0     3025 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_network_stats.py
--rw-r--r--   0        0        0     4048 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_create_account.py
--rw-r--r--   0        0        0     4104 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_create_account_with_seed.py
--rw-r--r--   0        0        0     3866 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_deactivate.py
--rw-r--r--   0        0        0     4037 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_delegate.py
--rw-r--r--   0        0        0     4064 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_merge.py
--rw-r--r--   0        0        0     4244 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_redelegate.py
--rw-r--r--   0        0        0     4313 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_split.py
--rw-r--r--   0        0        0     4218 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_withdraw.py
--rw-r--r--   0        0        0     3299 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_post_stakes_payload.py
--rw-r--r--   0        0        0     3072 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py
--rw-r--r--   0        0        0     2765 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py
--rw-r--r--   0        0        0     2617 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_prepared_tx.py
--rw-r--r--   0        0        0     3142 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_reward_by_day.py
--rw-r--r--   0        0        0     3317 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_reward_by_epoch.py
--rw-r--r--   0        0        0     3070 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py
--rw-r--r--   0        0        0     5250 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_stake.py
--rw-r--r--   0        0        0     2734 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_stake_tx.py
--rw-r--r--   0        0        0     3095 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_stake_tx_payload.py
--rw-r--r--   0        0        0     2996 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py
--rw-r--r--   0        0        0     2705 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/soltx_status.py
--rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2639 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py
--rw-r--r--   0        0        0     2984 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2664 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py
--rw-r--r--   0        0        0     3294 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_cycle_reward.py
--rw-r--r--   0        0        0     3130 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_daily_reward.py
--rw-r--r--   0        0        0     3522 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_network_stats.py
--rw-r--r--   0        0        0     2832 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py
--rw-r--r--   0        0        0     2662 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_signed_tx.py
--rw-r--r--   0        0        0     5809 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_stake.py
--rw-r--r--   0        0        0     2871 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_unsigned_tx.py
--rw-r--r--   0        0        0     3024 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtztx_status.py
--rw-r--r--   0        0        0     3193 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtztx_status_receipt.py
--rw-r--r--   0        0        0    13289 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/rest.py
--rw-r--r--   0        0        0        0 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/__init__.py
--rw-r--r--   0        0        0     2257 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account.py
--rw-r--r--   0        0        0     2283 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_payload.py
--rw-r--r--   0        0        0     3364 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_portfolio.py
--rw-r--r--   0        0        0     3074 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py
--rw-r--r--   0        0        0     2552 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py
--rw-r--r--   0        0        0     2552 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py
--rw-r--r--   0        0        0     2053 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_accounts_api.py
--rw-r--r--   0        0        0     1632 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_atom_api.py
--rw-r--r--   0        0        0     2284 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_atom_reward.py
--rw-r--r--   0        0        0     2624 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_atom_stake.py
--rw-r--r--   0        0        0     2719 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_core_stake.py
--rw-r--r--   0        0        0     2949 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_api.py
--rw-r--r--   0        0        0     2414 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2252 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py
--rw-r--r--   0        0        0     2620 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2337 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_kiln_stats.py
--rw-r--r--   0        0        0     2310 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py
--rw-r--r--   0        0        0     2273 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_network_stats.py
--rw-r--r--   0        0        0     2735 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py
--rw-r--r--   0        0        0     3049 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_operation_deposit.py
--rw-r--r--   0        0        0     2791 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py
--rw-r--r--   0        0        0     2875 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py
--rw-r--r--   0        0        0     3182 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py
--rw-r--r--   0        0        0     2587 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py
--rw-r--r--   0        0        0     2809 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py
--rw-r--r--   0        0        0     2432 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_reward.py
--rw-r--r--   0        0        0     2201 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_signed_tx.py
--rw-r--r--   0        0        0     3015 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_stake.py
--rw-r--r--   0        0        0     4064 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py
--rw-r--r--   0        0        0     3737 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_ethtx_status.py
--rw-r--r--   0        0        0     3576 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py
--rw-r--r--   0        0        0     2650 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py
--rw-r--r--   0        0        0     3709 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py
--rw-r--r--   0        0        0     2595 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_accounts200_response.py
--rw-r--r--   0        0        0     2625 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_atom_rewards200_response.py
--rw-r--r--   0        0        0     3007 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_atom_stakes200_response.py
--rw-r--r--   0        0        0     2615 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py
--rw-r--r--   0        0        0     2553 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py
--rw-r--r--   0        0        0     2363 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py
--rw-r--r--   0        0        0     3451 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py
--rw-r--r--   0        0        0     2803 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py
--rw-r--r--   0        0        0     3444 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py
--rw-r--r--   0        0        0     4114 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py
--rw-r--r--   0        0        0     2550 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py
--rw-r--r--   0        0        0     2363 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_operations200_response.py
--rw-r--r--   0        0        0     3163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_operations200_response_data_inner.py
--rw-r--r--   0        0        0     2327 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py
--rw-r--r--   0        0        0     2706 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3141 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py
--rw-r--r--   0        0        0     2480 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py
--rw-r--r--   0        0        0     2650 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py
--rw-r--r--   0        0        0     2327 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py
--rw-r--r--   0        0        0     2779 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py
--rw-r--r--   0        0        0     3071 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py
--rw-r--r--   0        0        0     2877 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py
--rw-r--r--   0        0        0     2535 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_account201_response.py
--rw-r--r--   0        0        0     2514 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2259 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py
--rw-r--r--   0        0        0     2899 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py
--rw-r--r--   0        0        0     2489 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py
--rw-r--r--   0        0        0     4344 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py
--rw-r--r--   0        0        0     2444 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2431 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py
--rw-r--r--   0        0        0     2447 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py
--rw-r--r--   0        0        0     2746 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py
--rw-r--r--   0        0        0     2499 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py
--rw-r--r--   0        0        0     2489 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py
--rw-r--r--   0        0        0     2581 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py
--rw-r--r--   0        0        0     3493 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_api.py
--rw-r--r--   0        0        0     2162 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py
--rw-r--r--   0        0        0     2290 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2599 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py
--rw-r--r--   0        0        0     2750 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py
--rw-r--r--   0        0        0     2270 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_network_stats.py
--rw-r--r--   0        0        0     2792 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_create_account.py
--rw-r--r--   0        0        0     2873 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_create_account_with_seed.py
--rw-r--r--   0        0        0     2687 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_deactivate.py
--rw-r--r--   0        0        0     2741 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_delegate.py
--rw-r--r--   0        0        0     2644 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_merge.py
--rw-r--r--   0        0        0     2786 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_redelegate.py
--rw-r--r--   0        0        0     2740 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_split.py
--rw-r--r--   0        0        0     2788 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_withdraw.py
--rw-r--r--   0        0        0     2953 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py
--rw-r--r--   0        0        0     2451 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py
--rw-r--r--   0        0        0     2439 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py
--rw-r--r--   0        0        0     2163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_prepared_tx.py
--rw-r--r--   0        0        0     2363 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_reward_by_day.py
--rw-r--r--   0        0        0     2379 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py
--rw-r--r--   0        0        0     2773 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py
--rw-r--r--   0        0        0     2728 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_stake.py
--rw-r--r--   0        0        0     2169 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_stake_tx.py
--rw-r--r--   0        0        0     2739 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py
--rw-r--r--   0        0        0     2630 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py
--rw-r--r--   0        0        0     2163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_soltx_status.py
--rw-r--r--   0        0        0     2541 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_api.py
--rw-r--r--   0        0        0     2414 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py
--rw-r--r--   0        0        0     2237 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py
--rw-r--r--   0        0        0     2646 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py
--rw-r--r--   0        0        0     2388 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py
--rw-r--r--   0        0        0     2426 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py
--rw-r--r--   0        0        0     2374 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_daily_reward.py
--rw-r--r--   0        0        0     2362 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_network_stats.py
--rw-r--r--   0        0        0     2601 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py
--rw-r--r--   0        0        0     2201 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_signed_tx.py
--rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_stake.py
--rw-r--r--   0        0        0     2333 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py
--rw-r--r--   0        0        0     2580 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtztx_status.py
--rw-r--r--   0        0        0     2502 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py
--rw-r--r--   0        0        0     6471 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/sol.py
--rw-r--r--   0        0        0      451 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev5/kiln_connect/utils.py
--rw-r--r--   0        0        0     4442 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev5/kiln_connect/xtz.py
--rw-r--r--   0        0        0     1011 2023-04-17 13:51:55.438598 kiln_connect-1.0.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     6658 1970-01-01 00:00:00.000000 kiln_connect-1.0.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0     5728 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev6/docs/README.md
+-rw-r--r--   0        0        0        0 2023-02-14 16:33:38.709950 kiln_connect-1.0.0.dev6/kiln_cli/__init__.py
+-rw-r--r--   0        0        0     4536 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev6/kiln_cli/accounts.py
+-rw-r--r--   0        0        0     2472 2023-04-24 06:41:57.416792 kiln_connect-1.0.0.dev6/kiln_cli/atom.py
+-rw-r--r--   0        0        0     6670 2023-04-06 15:53:36.351598 kiln_connect-1.0.0.dev6/kiln_cli/eth.py
+-rw-r--r--   0        0        0      410 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_cli/main.py
+-rwxr-xr-x   0        0        0    10741 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_cli/sol.py
+-rw-r--r--   0        0        0    10177 2023-04-24 06:41:57.416792 kiln_connect-1.0.0.dev6/kiln_cli/xtz.py
+-rw-r--r--   0        0        0      155 2023-03-03 17:16:30.658551 kiln_connect-1.0.0.dev6/kiln_connect/__init__.py
+-rw-r--r--   0        0        0      535 2023-03-08 16:23:14.337182 kiln_connect-1.0.0.dev6/kiln_connect/accounts.py
+-rw-r--r--   0        0        0      641 2023-04-24 06:41:57.416792 kiln_connect-1.0.0.dev6/kiln_connect/atom.py
+-rw-r--r--   0        0        0      942 2023-04-04 13:04:32.720789 kiln_connect-1.0.0.dev6/kiln_connect/errors.py
+-rw-r--r--   0        0        0     4144 2023-04-14 03:37:21.881892 kiln_connect-1.0.0.dev6/kiln_connect/eth.py
+-rw-r--r--   0        0        0     5301 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/integrations.py
+-rw-r--r--   0        0        0     3649 2023-04-17 13:51:44.551380 kiln_connect-1.0.0.dev6/kiln_connect/kiln_connect.py
+-rw-r--r--   0        0        0    12202 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/__init__.py
+-rw-r--r--   0        0        0      394 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    32819 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/accounts_api.py
+-rw-r--r--   0        0        0    21212 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/atom_api.py
+-rw-r--r--   0        0        0    84284 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/eth_api.py
+-rw-r--r--   0        0        0   104060 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/sol_api.py
+-rw-r--r--   0        0        0    66804 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/xtz_api.py
+-rw-r--r--   0        0        0    30218 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api_client.py
+-rw-r--r--   0        0        0    17494 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/configuration.py
+-rw-r--r--   0        0        0     5713 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/exceptions.py
+-rw-r--r--   0        0        0    11300 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0     3006 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account.py
+-rw-r--r--   0        0        0     2782 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_payload.py
+-rw-r--r--   0        0        0     4028 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio.py
+-rw-r--r--   0        0        0     4878 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py
+-rw-r--r--   0        0        0     3019 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py
+-rw-r--r--   0        0        0     3016 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py
+-rw-r--r--   0        0        0     3478 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/atom_reward.py
+-rw-r--r--   0        0        0     4849 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/atom_stake.py
+-rw-r--r--   0        0        0     3245 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/core_stake.py
+-rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2639 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_broadcasted_tx.py
+-rw-r--r--   0        0        0     3090 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2910 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_kiln_stats.py
+-rw-r--r--   0        0        0     2971 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py
+-rw-r--r--   0        0        0     3028 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_network_stats.py
+-rw-r--r--   0        0        0     3485 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py
+-rw-r--r--   0        0        0     4582 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_deposit.py
+-rw-r--r--   0        0        0     3820 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_execution_reward.py
+-rw-r--r--   0        0        0     3522 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py
+-rw-r--r--   0        0        0     4456 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py
+-rw-r--r--   0        0        0     3376 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_payload.py
+-rw-r--r--   0        0        0     3042 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py
+-rw-r--r--   0        0        0     3846 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_reward.py
+-rw-r--r--   0        0        0     2662 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_signed_tx.py
+-rw-r--r--   0        0        0     7278 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_stake.py
+-rw-r--r--   0        0        0     4514 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_unsigned_tx.py
+-rw-r--r--   0        0        0     3024 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status.py
+-rw-r--r--   0        0        0     5288 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status_receipt.py
+-rw-r--r--   0        0        0     3681 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py
+-rw-r--r--   0        0        0     2972 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_account_portfolio200_response.py
+-rw-r--r--   0        0        0     3064 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_accounts200_response.py
+-rw-r--r--   0        0        0     3098 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_atom_rewards200_response.py
+-rw-r--r--   0        0        0     3087 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_atom_stakes200_response.py
+-rw-r--r--   0        0        0     2929 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py
+-rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py
+-rw-r--r--   0        0        0     3220 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_operations200_response.py
+-rw-r--r--   0        0        0     7941 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     3087 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_rewards200_response.py
+-rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_stakes200_response.py
+-rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py
+-rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py
+-rw-r--r--   0        0        0     3220 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_operations200_response.py
+-rw-r--r--   0        0        0    13955 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     3187 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_rewards200_response.py
+-rw-r--r--   0        0        0     5115 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_stakes200_response.py
+-rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py
+-rw-r--r--   0        0        0     2962 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py
+-rw-r--r--   0        0        0     3220 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_operations200_response.py
+-rw-r--r--   0        0        0     8863 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     3187 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py
+-rw-r--r--   0        0        0     5085 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3076 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py
+-rw-r--r--   0        0        0     2917 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py
+-rw-r--r--   0        0        0     2879 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_account201_response.py
+-rw-r--r--   0        0        0     2966 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2959 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_keys201_response.py
+-rw-r--r--   0        0        0     5501 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py
+-rw-r--r--   0        0        0     2932 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2926 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py
+-rw-r--r--   0        0        0     2958 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2940 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2914 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py
+-rw-r--r--   0        0        0     2902 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_stakes201_response.py
+-rw-r--r--   0        0        0     2966 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2932 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2926 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py
+-rw-r--r--   0        0        0     2572 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_broadcast_tx.py
+-rw-r--r--   0        0        0     2607 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2816 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py
+-rw-r--r--   0        0        0     3015 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py
+-rw-r--r--   0        0        0     3025 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_network_stats.py
+-rw-r--r--   0        0        0     4048 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_create_account.py
+-rw-r--r--   0        0        0     4104 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_create_account_with_seed.py
+-rw-r--r--   0        0        0     3866 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_deactivate.py
+-rw-r--r--   0        0        0     4037 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_delegate.py
+-rw-r--r--   0        0        0     4064 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_merge.py
+-rw-r--r--   0        0        0     4244 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_redelegate.py
+-rw-r--r--   0        0        0     4313 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_split.py
+-rw-r--r--   0        0        0     4218 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_withdraw.py
+-rw-r--r--   0        0        0     3299 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_post_stakes_payload.py
+-rw-r--r--   0        0        0     3072 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     2765 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2617 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_prepared_tx.py
+-rw-r--r--   0        0        0     3142 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_reward_by_day.py
+-rw-r--r--   0        0        0     3317 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_reward_by_epoch.py
+-rw-r--r--   0        0        0     3070 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py
+-rw-r--r--   0        0        0     4916 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake.py
+-rw-r--r--   0        0        0     2734 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake_tx.py
+-rw-r--r--   0        0        0     3095 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake_tx_payload.py
+-rw-r--r--   0        0        0     2996 2023-04-13 07:25:59.404645 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py
+-rw-r--r--   0        0        0     2705 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/soltx_status.py
+-rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2639 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py
+-rw-r--r--   0        0        0     2984 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2664 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py
+-rw-r--r--   0        0        0     3294 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_cycle_reward.py
+-rw-r--r--   0        0        0     3130 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_daily_reward.py
+-rw-r--r--   0        0        0     3522 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_network_stats.py
+-rw-r--r--   0        0        0     3415 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_activation.py
+-rw-r--r--   0        0        0     4022 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_delegate.py
+-rw-r--r--   0        0        0     4212 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_payment.py
+-rw-r--r--   0        0        0     3903 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_operation_undelegate.py
+-rw-r--r--   0        0        0     2832 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2662 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_signed_tx.py
+-rw-r--r--   0        0        0     5809 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_stake.py
+-rw-r--r--   0        0        0     2871 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_unsigned_tx.py
+-rw-r--r--   0        0        0     3024 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtztx_status.py
+-rw-r--r--   0        0        0     3193 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtztx_status_receipt.py
+-rw-r--r--   0        0        0    13289 2023-04-13 07:25:59.411312 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/rest.py
+-rw-r--r--   0        0        0        0 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/__init__.py
+-rw-r--r--   0        0        0     2257 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account.py
+-rw-r--r--   0        0        0     2283 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_payload.py
+-rw-r--r--   0        0        0     3364 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio.py
+-rw-r--r--   0        0        0     3074 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py
+-rw-r--r--   0        0        0     2552 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py
+-rw-r--r--   0        0        0     2552 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py
+-rw-r--r--   0        0        0     2053 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_accounts_api.py
+-rw-r--r--   0        0        0     1632 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_api.py
+-rw-r--r--   0        0        0     2284 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_reward.py
+-rw-r--r--   0        0        0     2624 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_stake.py
+-rw-r--r--   0        0        0     2719 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_core_stake.py
+-rw-r--r--   0        0        0     2949 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_api.py
+-rw-r--r--   0        0        0     2414 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2252 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py
+-rw-r--r--   0        0        0     2620 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2337 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_kiln_stats.py
+-rw-r--r--   0        0        0     2310 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py
+-rw-r--r--   0        0        0     2273 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_network_stats.py
+-rw-r--r--   0        0        0     2735 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py
+-rw-r--r--   0        0        0     3049 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_deposit.py
+-rw-r--r--   0        0        0     2791 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py
+-rw-r--r--   0        0        0     2875 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py
+-rw-r--r--   0        0        0     3182 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py
+-rw-r--r--   0        0        0     2587 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py
+-rw-r--r--   0        0        0     2809 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2432 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_reward.py
+-rw-r--r--   0        0        0     2201 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_signed_tx.py
+-rw-r--r--   0        0        0     3015 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_stake.py
+-rw-r--r--   0        0        0     4064 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py
+-rw-r--r--   0        0        0     3737 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status.py
+-rw-r--r--   0        0        0     3576 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py
+-rw-r--r--   0        0        0     2650 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py
+-rw-r--r--   0        0        0     3709 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py
+-rw-r--r--   0        0        0     2595 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_accounts200_response.py
+-rw-r--r--   0        0        0     2625 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_atom_rewards200_response.py
+-rw-r--r--   0        0        0     3007 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_atom_stakes200_response.py
+-rw-r--r--   0        0        0     2615 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py
+-rw-r--r--   0        0        0     2553 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py
+-rw-r--r--   0        0        0     2363 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py
+-rw-r--r--   0        0        0     3451 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     2803 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py
+-rw-r--r--   0        0        0     3444 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py
+-rw-r--r--   0        0        0     4114 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py
+-rw-r--r--   0        0        0     2550 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py
+-rw-r--r--   0        0        0     2363 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_operations200_response.py
+-rw-r--r--   0        0        0     3163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     2327 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py
+-rw-r--r--   0        0        0     2706 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3093 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py
+-rw-r--r--   0        0        0     2480 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py
+-rw-r--r--   0        0        0     2650 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py
+-rw-r--r--   0        0        0     2363 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_operations200_response.py
+-rw-r--r--   0        0        0     2967 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_operations200_response_data_inner.py
+-rw-r--r--   0        0        0     2327 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py
+-rw-r--r--   0        0        0     2779 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py
+-rw-r--r--   0        0        0     3071 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py
+-rw-r--r--   0        0        0     2877 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py
+-rw-r--r--   0        0        0     2535 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_account201_response.py
+-rw-r--r--   0        0        0     2514 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2259 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py
+-rw-r--r--   0        0        0     2899 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py
+-rw-r--r--   0        0        0     2489 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py
+-rw-r--r--   0        0        0     4344 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py
+-rw-r--r--   0        0        0     2444 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2431 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2447 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py
+-rw-r--r--   0        0        0     2746 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py
+-rw-r--r--   0        0        0     2499 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py
+-rw-r--r--   0        0        0     2489 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py
+-rw-r--r--   0        0        0     2581 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py
+-rw-r--r--   0        0        0     3493 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_api.py
+-rw-r--r--   0        0        0     2162 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py
+-rw-r--r--   0        0        0     2290 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2599 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py
+-rw-r--r--   0        0        0     2750 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py
+-rw-r--r--   0        0        0     2270 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_network_stats.py
+-rw-r--r--   0        0        0     2792 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_create_account.py
+-rw-r--r--   0        0        0     2873 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_create_account_with_seed.py
+-rw-r--r--   0        0        0     2687 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_deactivate.py
+-rw-r--r--   0        0        0     2741 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_delegate.py
+-rw-r--r--   0        0        0     2644 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_merge.py
+-rw-r--r--   0        0        0     2786 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_redelegate.py
+-rw-r--r--   0        0        0     2740 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_split.py
+-rw-r--r--   0        0        0     2788 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_withdraw.py
+-rw-r--r--   0        0        0     2953 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py
+-rw-r--r--   0        0        0     2451 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py
+-rw-r--r--   0        0        0     2439 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_prepared_tx.py
+-rw-r--r--   0        0        0     2363 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_reward_by_day.py
+-rw-r--r--   0        0        0     2379 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py
+-rw-r--r--   0        0        0     2773 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py
+-rw-r--r--   0        0        0     2688 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake.py
+-rw-r--r--   0        0        0     2169 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake_tx.py
+-rw-r--r--   0        0        0     2739 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py
+-rw-r--r--   0        0        0     2630 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py
+-rw-r--r--   0        0        0     2163 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_soltx_status.py
+-rw-r--r--   0        0        0     2684 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_api.py
+-rw-r--r--   0        0        0     2414 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py
+-rw-r--r--   0        0        0     2237 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py
+-rw-r--r--   0        0        0     2646 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py
+-rw-r--r--   0        0        0     2388 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py
+-rw-r--r--   0        0        0     2426 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py
+-rw-r--r--   0        0        0     2374 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_daily_reward.py
+-rw-r--r--   0        0        0     2362 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_network_stats.py
+-rw-r--r--   0        0        0     2494 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_activation.py
+-rw-r--r--   0        0        0     2668 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_delegate.py
+-rw-r--r--   0        0        0     2727 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_payment.py
+-rw-r--r--   0        0        0     2658 2023-04-24 06:41:57.420125 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_operation_undelegate.py
+-rw-r--r--   0        0        0     2601 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py
+-rw-r--r--   0        0        0     2201 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_signed_tx.py
+-rw-r--r--   0        0        0     2666 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_stake.py
+-rw-r--r--   0        0        0     2333 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py
+-rw-r--r--   0        0        0     2580 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtztx_status.py
+-rw-r--r--   0        0        0     2502 2023-04-13 07:25:59.407978 kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py
+-rw-r--r--   0        0        0     6471 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/sol.py
+-rw-r--r--   0        0        0      451 2023-04-17 03:17:38.302253 kiln_connect-1.0.0.dev6/kiln_connect/utils.py
+-rw-r--r--   0        0        0     4442 2023-04-04 13:04:32.727455 kiln_connect-1.0.0.dev6/kiln_connect/xtz.py
+-rw-r--r--   0        0        0     1011 2023-04-24 06:43:22.622507 kiln_connect-1.0.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     6658 1970-01-01 00:00:00.000000 kiln_connect-1.0.0.dev6/PKG-INFO
```

### Comparing `kiln_connect-1.0.0.dev5/docs/README.md` & `kiln_connect-1.0.0.dev6/docs/README.md`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_cli/accounts.py` & `kiln_connect-1.0.0.dev6/kiln_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_cli/atom.py` & `kiln_connect-1.0.0.dev6/kiln_cli/atom.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,21 +6,18 @@
 Code here is voluntarily kept simple: it could be refactored with some
 levels of abstraction to avoid repetitions, but would imply readers to
 understand things unrelated to what their primary goal is: use the
 SDK. So let's keep it stupid simple so the integration work is
 simpler.
 """
 
-import click
-import re
 import typer
 
 from rich.console import Console
 from rich.table import Table
-from typing import Tuple
 
 import kiln_connect
 
 atom_cli = typer.Typer(
     name='atom', help='Staking utilities for ATOM', no_args_is_help=True)
```

### Comparing `kiln_connect-1.0.0.dev5/kiln_cli/eth.py` & `kiln_connect-1.0.0.dev6/kiln_cli/eth.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_cli/sol.py` & `kiln_connect-1.0.0.dev6/kiln_cli/sol.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/accounts.py` & `kiln_connect-1.0.0.dev6/kiln_connect/accounts.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/atom.py` & `kiln_connect-1.0.0.dev6/kiln_connect/atom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Atom wrapper class.
 
 This ATOM class is meant to be accessed via KilnConnect.ATOM, it is
 publicly exported in the SDK. This file contains helpers to
 integration our Atom API with integrations such as Fireblocks. It
 provides convenient shortcuts to use our SDK.
 """
-import logging
 
 from kiln_connect.integrations import Integrations
 
 from kiln_connect.openapi_client import (
     ApiClient,
 )
 from kiln_connect.openapi_client import (
```

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/errors.py` & `kiln_connect-1.0.0.dev6/kiln_connect/errors.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/eth.py` & `kiln_connect-1.0.0.dev6/kiln_connect/eth.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/integrations.py` & `kiln_connect-1.0.0.dev6/kiln_connect/integrations.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/kiln_connect.py` & `kiln_connect-1.0.0.dev6/kiln_connect/kiln_connect.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/__init__.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 from kiln_connect.openapi_client.models.get_sol_operations200_response import GetSolOperations200Response
 from kiln_connect.openapi_client.models.get_sol_operations200_response_data_inner import GetSolOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response
 from kiln_connect.openapi_client.models.get_sol_rewards200_response_data_inner import GetSolRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_stakes200_response import GetSolStakes200Response
 from kiln_connect.openapi_client.models.get_sol_tx_status200_response import GetSolTxStatus200Response
 from kiln_connect.openapi_client.models.get_xtz_network_stats200_response import GetXtzNetworkStats200Response
+from kiln_connect.openapi_client.models.get_xtz_operations200_response import GetXtzOperations200Response
+from kiln_connect.openapi_client.models.get_xtz_operations200_response_data_inner import GetXtzOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response import GetXtzRewards200Response
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner import GetXtzRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_xtz_stakes200_response import GetXtzStakes200Response
 from kiln_connect.openapi_client.models.get_xtz_tx_status200_response import GetXtzTxStatus200Response
 from kiln_connect.openapi_client.models.post_account201_response import PostAccount201Response
 from kiln_connect.openapi_client.models.post_eth_broadcast_tx201_response import PostEthBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_eth_keys201_response import PostEthKeys201Response
@@ -127,13 +129,17 @@
 from kiln_connect.openapi_client.models.xtz_broadcast_tx_payload import XTZBroadcastTxPayload
 from kiln_connect.openapi_client.models.xtz_broadcasted_tx import XTZBroadcastedTx
 from kiln_connect.openapi_client.models.xtz_craft_stake_tx_payload import XTZCraftStakeTxPayload
 from kiln_connect.openapi_client.models.xtz_craft_un_stake_tx_payload import XTZCraftUnStakeTxPayload
 from kiln_connect.openapi_client.models.xtz_cycle_reward import XTZCycleReward
 from kiln_connect.openapi_client.models.xtz_daily_reward import XTZDailyReward
 from kiln_connect.openapi_client.models.xtz_network_stats import XTZNetworkStats
+from kiln_connect.openapi_client.models.xtz_operation_activation import XTZOperationActivation
+from kiln_connect.openapi_client.models.xtz_operation_delegate import XTZOperationDelegate
+from kiln_connect.openapi_client.models.xtz_operation_payment import XTZOperationPayment
+from kiln_connect.openapi_client.models.xtz_operation_undelegate import XTZOperationUndelegate
 from kiln_connect.openapi_client.models.xtz_prepare_tx_payload import XTZPrepareTxPayload
 from kiln_connect.openapi_client.models.xtz_signed_tx import XTZSignedTx
 from kiln_connect.openapi_client.models.xtz_stake import XTZStake
 from kiln_connect.openapi_client.models.xtztx_status import XTZTxStatus
 from kiln_connect.openapi_client.models.xtztx_status_receipt import XTZTxStatusReceipt
 from kiln_connect.openapi_client.models.xtz_unsigned_tx import XTZUnsignedTx
```

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/accounts_api.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/atom_api.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/atom_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/eth_api.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/xtz_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,195 +20,55 @@
 
 from datetime import date
 
 from pydantic import Field, StrictStr, conlist
 
 from typing import Optional
 
-from kiln_connect.openapi_client.models.eth_broadcast_tx_payload import ETHBroadcastTxPayload
-from kiln_connect.openapi_client.models.eth_craft_stake_tx_payload import ETHCraftStakeTxPayload
-from kiln_connect.openapi_client.models.eth_post_keys_payload import ETHPostKeysPayload
-from kiln_connect.openapi_client.models.eth_prepare_tx_payload import ETHPrepareTxPayload
-from kiln_connect.openapi_client.models.get_eth_kiln_stats200_response import GetEthKilnStats200Response
-from kiln_connect.openapi_client.models.get_eth_network_stats200_response import GetEthNetworkStats200Response
-from kiln_connect.openapi_client.models.get_eth_operations200_response import GetEthOperations200Response
-from kiln_connect.openapi_client.models.get_eth_rewards200_response import GetEthRewards200Response
-from kiln_connect.openapi_client.models.get_eth_stakes200_response import GetEthStakes200Response
-from kiln_connect.openapi_client.models.get_eth_tx_status200_response import GetEthTxStatus200Response
-from kiln_connect.openapi_client.models.post_eth_broadcast_tx201_response import PostEthBroadcastTx201Response
-from kiln_connect.openapi_client.models.post_eth_keys201_response import PostEthKeys201Response
-from kiln_connect.openapi_client.models.post_eth_prepare_tx201_response import PostEthPrepareTx201Response
-from kiln_connect.openapi_client.models.post_eth_stake_tx201_response import PostEthStakeTx201Response
+from kiln_connect.openapi_client.models.get_xtz_network_stats200_response import GetXtzNetworkStats200Response
+from kiln_connect.openapi_client.models.get_xtz_operations200_response import GetXtzOperations200Response
+from kiln_connect.openapi_client.models.get_xtz_rewards200_response import GetXtzRewards200Response
+from kiln_connect.openapi_client.models.get_xtz_stakes200_response import GetXtzStakes200Response
+from kiln_connect.openapi_client.models.get_xtz_tx_status200_response import GetXtzTxStatus200Response
+from kiln_connect.openapi_client.models.post_xtz_broadcast_tx201_response import PostXtzBroadcastTx201Response
+from kiln_connect.openapi_client.models.post_xtz_prepare_tx201_response import PostXtzPrepareTx201Response
+from kiln_connect.openapi_client.models.post_xtz_stake_tx201_response import PostXtzStakeTx201Response
+from kiln_connect.openapi_client.models.xtz_broadcast_tx_payload import XTZBroadcastTxPayload
+from kiln_connect.openapi_client.models.xtz_craft_stake_tx_payload import XTZCraftStakeTxPayload
+from kiln_connect.openapi_client.models.xtz_craft_un_stake_tx_payload import XTZCraftUnStakeTxPayload
+from kiln_connect.openapi_client.models.xtz_prepare_tx_payload import XTZPrepareTxPayload
 
 from kiln_connect.openapi_client.api_client import ApiClient
 from kiln_connect.openapi_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class EthApi(object):
+class XtzApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_eth_kiln_stats(self, **kwargs) -> GetEthKilnStats200Response:  # noqa: E501
-        """Kiln Stats  # noqa: E501
-
-        Get some Kiln statistics on Ethereum staking  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_eth_kiln_stats(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: GetEthKilnStats200Response
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_eth_kiln_stats_with_http_info(**kwargs)  # noqa: E501
-
-    @validate_arguments
-    def get_eth_kiln_stats_with_http_info(self, **kwargs):  # noqa: E501
-        """Kiln Stats  # noqa: E501
-
-        Get some Kiln statistics on Ethereum staking  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_eth_kiln_stats_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(GetEthKilnStats200Response, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = [
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_eth_kiln_stats" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-
-        # process the query parameters
-        _query_params = []
-
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-
-        # process the body parameter
-        _body_params = None
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json; charset=utf-8'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['bearerAuth']  # noqa: E501
-
-        _response_types_map = {
-            '200': "GetEthKilnStats200Response",
-            '401': None,
-            '500': None,
-        }
-
-        return self.api_client.call_api(
-            '/v1/eth/kiln-stats', 'GET',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def get_eth_network_stats(self, **kwargs) -> GetEthNetworkStats200Response:  # noqa: E501
+    def get_xtz_network_stats(self, **kwargs) -> GetXtzNetworkStats200Response:  # noqa: E501
         """Network Stats  # noqa: E501
 
-        Get some network statistics on Ethereum staking  # noqa: E501
+        Get some network statistics on Tezos staking  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_network_stats(async_req=True)
+        >>> thread = api.get_xtz_network_stats(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -216,28 +76,28 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GetEthNetworkStats200Response
+        :rtype: GetXtzNetworkStats200Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_eth_network_stats_with_http_info(**kwargs)  # noqa: E501
+        return self.get_xtz_network_stats_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_eth_network_stats_with_http_info(self, **kwargs):  # noqa: E501
+    def get_xtz_network_stats_with_http_info(self, **kwargs):  # noqa: E501
         """Network Stats  # noqa: E501
 
-        Get some network statistics on Ethereum staking  # noqa: E501
+        Get some network statistics on Tezos staking  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_network_stats_with_http_info(async_req=True)
+        >>> thread = api.get_xtz_network_stats_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -253,15 +113,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GetEthNetworkStats200Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetXtzNetworkStats200Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -277,15 +137,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_eth_network_stats" % _key
+                    " to method get_xtz_network_stats" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -308,21 +168,21 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json; charset=utf-8'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "GetEthNetworkStats200Response",
+            '200': "GetXtzNetworkStats200Response",
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
-            '/v1/eth/network-stats', 'GET',
+            '/v1/xtz/network-stats', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -331,26 +191,24 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_eth_operations(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> GetEthOperations200Response:  # noqa: E501
+    def get_xtz_operations(self, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> GetXtzOperations200Response:  # noqa: E501
         """Operations  # noqa: E501
 
-        Get the operations of Ethereum stakes  # noqa: E501
+        Get historical operations of Tezos stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_operations(validators, wallets, accounts, async_req=True)
+        >>> thread = api.get_xtz_operations(wallets, accounts, async_req=True)
         >>> result = thread.get()
 
-        :param validators: Comma-separated list of validators addresses
-        :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -360,32 +218,30 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GetEthOperations200Response
+        :rtype: GetXtzOperations200Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_eth_operations_with_http_info(validators, wallets, accounts, **kwargs)  # noqa: E501
+        return self.get_xtz_operations_with_http_info(wallets, accounts, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_eth_operations_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
+    def get_xtz_operations_with_http_info(self, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
         """Operations  # noqa: E501
 
-        Get the operations of Ethereum stakes  # noqa: E501
+        Get historical operations of Tezos stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_operations_with_http_info(validators, wallets, accounts, async_req=True)
+        >>> thread = api.get_xtz_operations_with_http_info(wallets, accounts, async_req=True)
         >>> result = thread.get()
 
-        :param validators: Comma-separated list of validators addresses
-        :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -403,21 +259,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GetEthOperations200Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetXtzOperations200Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'validators',
             'wallets',
             'accounts'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -430,29 +285,26 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_eth_operations" % _key
+                    " to method get_xtz_operations" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('validators') is not None:  # noqa: E501
-            _query_params.append(('validators', _params['validators']))
-            _collection_formats['validators'] = 'csv'
         if _params.get('wallets') is not None:  # noqa: E501
             _query_params.append(('wallets', _params['wallets']))
             _collection_formats['wallets'] = 'csv'
         if _params.get('accounts') is not None:  # noqa: E501
             _query_params.append(('accounts', _params['accounts']))
             _collection_formats['accounts'] = 'csv'
 
@@ -470,185 +322,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json; charset=utf-8'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "GetEthOperations200Response",
-            '400': None,
-            '401': None,
-            '500': None,
-        }
-
-        return self.api_client.call_api(
-            '/v1/eth/operations', 'GET',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def get_eth_reports(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> bytearray:  # noqa: E501
-        """Excel Reports  # noqa: E501
-
-        Generates an Excel report sheet for your stakes and rewards  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_eth_reports(validators, wallets, accounts, async_req=True)
-        >>> result = thread.get()
-
-        :param validators: Comma-separated list of validators addresses
-        :type validators: List[str]
-        :param wallets: Comma-separated list of wallets addresses
-        :type wallets: List[str]
-        :param accounts: Comma-separated list of Kiln accounts identifiers
-        :type accounts: List[str]
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: bytearray
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_eth_reports_with_http_info(validators, wallets, accounts, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def get_eth_reports_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
-        """Excel Reports  # noqa: E501
-
-        Generates an Excel report sheet for your stakes and rewards  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_eth_reports_with_http_info(validators, wallets, accounts, async_req=True)
-        >>> result = thread.get()
-
-        :param validators: Comma-separated list of validators addresses
-        :type validators: List[str]
-        :param wallets: Comma-separated list of wallets addresses
-        :type wallets: List[str]
-        :param accounts: Comma-separated list of Kiln accounts identifiers
-        :type accounts: List[str]
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(bytearray, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'validators',
-            'wallets',
-            'accounts'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_eth_reports" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-
-        # process the query parameters
-        _query_params = []
-        if _params.get('validators') is not None:  # noqa: E501
-            _query_params.append(('validators', _params['validators']))
-            _collection_formats['validators'] = 'csv'
-        if _params.get('wallets') is not None:  # noqa: E501
-            _query_params.append(('wallets', _params['wallets']))
-            _collection_formats['wallets'] = 'csv'
-        if _params.get('accounts') is not None:  # noqa: E501
-            _query_params.append(('accounts', _params['accounts']))
-            _collection_formats['accounts'] = 'csv'
-
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-
-        # process the body parameter
-        _body_params = None
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/octet-stream'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['bearerAuth']  # noqa: E501
-
-        _response_types_map = {
-            '200': "bytearray",
+            '200': "GetXtzOperations200Response",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
-            '/v1/eth/reports', 'GET',
+            '/v1/xtz/operations', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -657,73 +346,81 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_eth_rewards(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, start_date : Annotated[Optional[date], Field(description="Get rewards from this date (YYYY-MM-DD)")] = None, end_date : Annotated[Optional[date], Field(description="Get rewards to this date (YYYY-MM-DD)")] = None, **kwargs) -> GetEthRewards200Response:  # noqa: E501
+    def get_xtz_rewards(self, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, format : Annotated[Optional[StrictStr], Field(description="The format of the response. Defaults to daily")] = None, start_date : Annotated[Optional[date], Field(description="Get rewards from this date (YYYY-MM-DD)")] = None, end_date : Annotated[Optional[date], Field(description="Get rewards to this date (YYYY-MM-DD)")] = None, start_cycle : Annotated[Optional[float], Field(description="The cycle from which we want to fetch rewards. Must be used with format=cycle")] = None, end_cycle : Annotated[Optional[float], Field(description="The cycle until which we want to fetch rewards. Must be used with format=cycle")] = None, **kwargs) -> GetXtzRewards200Response:  # noqa: E501
         """Rewards  # noqa: E501
 
-        Get historical rewards by day of Ethereum stakes  # noqa: E501
+        Get historical rewards of Tezos stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_rewards(validators, wallets, accounts, start_date, end_date, async_req=True)
+        >>> thread = api.get_xtz_rewards(wallets, accounts, format, start_date, end_date, start_cycle, end_cycle, async_req=True)
         >>> result = thread.get()
 
-        :param validators: Comma-separated list of validators addresses
-        :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
+        :param format: The format of the response. Defaults to daily
+        :type format: str
         :param start_date: Get rewards from this date (YYYY-MM-DD)
         :type start_date: date
         :param end_date: Get rewards to this date (YYYY-MM-DD)
         :type end_date: date
+        :param start_cycle: The cycle from which we want to fetch rewards. Must be used with format=cycle
+        :type start_cycle: float
+        :param end_cycle: The cycle until which we want to fetch rewards. Must be used with format=cycle
+        :type end_cycle: float
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GetEthRewards200Response
+        :rtype: GetXtzRewards200Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_eth_rewards_with_http_info(validators, wallets, accounts, start_date, end_date, **kwargs)  # noqa: E501
+        return self.get_xtz_rewards_with_http_info(wallets, accounts, format, start_date, end_date, start_cycle, end_cycle, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_eth_rewards_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, start_date : Annotated[Optional[date], Field(description="Get rewards from this date (YYYY-MM-DD)")] = None, end_date : Annotated[Optional[date], Field(description="Get rewards to this date (YYYY-MM-DD)")] = None, **kwargs):  # noqa: E501
+    def get_xtz_rewards_with_http_info(self, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, format : Annotated[Optional[StrictStr], Field(description="The format of the response. Defaults to daily")] = None, start_date : Annotated[Optional[date], Field(description="Get rewards from this date (YYYY-MM-DD)")] = None, end_date : Annotated[Optional[date], Field(description="Get rewards to this date (YYYY-MM-DD)")] = None, start_cycle : Annotated[Optional[float], Field(description="The cycle from which we want to fetch rewards. Must be used with format=cycle")] = None, end_cycle : Annotated[Optional[float], Field(description="The cycle until which we want to fetch rewards. Must be used with format=cycle")] = None, **kwargs):  # noqa: E501
         """Rewards  # noqa: E501
 
-        Get historical rewards by day of Ethereum stakes  # noqa: E501
+        Get historical rewards of Tezos stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_rewards_with_http_info(validators, wallets, accounts, start_date, end_date, async_req=True)
+        >>> thread = api.get_xtz_rewards_with_http_info(wallets, accounts, format, start_date, end_date, start_cycle, end_cycle, async_req=True)
         >>> result = thread.get()
 
-        :param validators: Comma-separated list of validators addresses
-        :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
+        :param format: The format of the response. Defaults to daily
+        :type format: str
         :param start_date: Get rewards from this date (YYYY-MM-DD)
         :type start_date: date
         :param end_date: Get rewards to this date (YYYY-MM-DD)
         :type end_date: date
+        :param start_cycle: The cycle from which we want to fetch rewards. Must be used with format=cycle
+        :type start_cycle: float
+        :param end_cycle: The cycle until which we want to fetch rewards. Must be used with format=cycle
+        :type end_cycle: float
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -737,25 +434,27 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GetEthRewards200Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetXtzRewards200Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'validators',
             'wallets',
             'accounts',
+            'format',
             'start_date',
-            'end_date'
+            'end_date',
+            'start_cycle',
+            'end_cycle'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -766,39 +465,42 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_eth_rewards" % _key
+                    " to method get_xtz_rewards" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('validators') is not None:  # noqa: E501
-            _query_params.append(('validators', _params['validators']))
-            _collection_formats['validators'] = 'csv'
         if _params.get('wallets') is not None:  # noqa: E501
             _query_params.append(('wallets', _params['wallets']))
             _collection_formats['wallets'] = 'csv'
         if _params.get('accounts') is not None:  # noqa: E501
             _query_params.append(('accounts', _params['accounts']))
             _collection_formats['accounts'] = 'csv'
+        if _params.get('format') is not None:  # noqa: E501
+            _query_params.append(('format', _params['format']))
         if _params.get('start_date') is not None:  # noqa: E501
             _query_params.append(('start_date', _params['start_date']))
         if _params.get('end_date') is not None:  # noqa: E501
             _query_params.append(('end_date', _params['end_date']))
+        if _params.get('start_cycle') is not None:  # noqa: E501
+            _query_params.append(('start_cycle', _params['start_cycle']))
+        if _params.get('end_cycle') is not None:  # noqa: E501
+            _query_params.append(('end_cycle', _params['end_cycle']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -810,22 +512,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json; charset=utf-8'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "GetEthRewards200Response",
+            '200': "GetXtzRewards200Response",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
-            '/v1/eth/rewards', 'GET',
+            '/v1/xtz/rewards', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -834,26 +536,24 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_eth_stakes(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> GetEthStakes200Response:  # noqa: E501
+    def get_xtz_stakes(self, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs) -> GetXtzStakes200Response:  # noqa: E501
         """Stakes  # noqa: E501
 
-        Get the status of Ethereum stakes  # noqa: E501
+        Get the status of Tezos stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_stakes(validators, wallets, accounts, async_req=True)
+        >>> thread = api.get_xtz_stakes(wallets, accounts, async_req=True)
         >>> result = thread.get()
 
-        :param validators: Comma-separated list of validators addresses
-        :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -863,32 +563,30 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GetEthStakes200Response
+        :rtype: GetXtzStakes200Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_eth_stakes_with_http_info(validators, wallets, accounts, **kwargs)  # noqa: E501
+        return self.get_xtz_stakes_with_http_info(wallets, accounts, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_eth_stakes_with_http_info(self, validators : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of validators addresses")] = None, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
+    def get_xtz_stakes_with_http_info(self, wallets : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of wallets addresses")] = None, accounts : Annotated[Optional[conlist(StrictStr)], Field(description="Comma-separated list of Kiln accounts identifiers")] = None, **kwargs):  # noqa: E501
         """Stakes  # noqa: E501
 
-        Get the status of Ethereum stakes  # noqa: E501
+        Get the status of Tezos stakes  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_stakes_with_http_info(validators, wallets, accounts, async_req=True)
+        >>> thread = api.get_xtz_stakes_with_http_info(wallets, accounts, async_req=True)
         >>> result = thread.get()
 
-        :param validators: Comma-separated list of validators addresses
-        :type validators: List[str]
         :param wallets: Comma-separated list of wallets addresses
         :type wallets: List[str]
         :param accounts: Comma-separated list of Kiln accounts identifiers
         :type accounts: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -906,21 +604,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GetEthStakes200Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetXtzStakes200Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'validators',
             'wallets',
             'accounts'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -933,29 +630,26 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_eth_stakes" % _key
+                    " to method get_xtz_stakes" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('validators') is not None:  # noqa: E501
-            _query_params.append(('validators', _params['validators']))
-            _collection_formats['validators'] = 'csv'
         if _params.get('wallets') is not None:  # noqa: E501
             _query_params.append(('wallets', _params['wallets']))
             _collection_formats['wallets'] = 'csv'
         if _params.get('accounts') is not None:  # noqa: E501
             _query_params.append(('accounts', _params['accounts']))
             _collection_formats['accounts'] = 'csv'
 
@@ -973,22 +667,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json; charset=utf-8'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "GetEthStakes200Response",
+            '200': "GetXtzStakes200Response",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
-            '/v1/eth/stakes', 'GET',
+            '/v1/xtz/stakes', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -997,57 +691,61 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_eth_tx_status(self, tx_hash : Annotated[StrictStr, Field(..., description="Hash of the transaction")], **kwargs) -> GetEthTxStatus200Response:  # noqa: E501
+    def get_xtz_tx_status(self, tx_hash : Annotated[StrictStr, Field(..., description="Hash of the transaction")], block_number : Annotated[StrictStr, Field(..., description="Block number in which the transaction was included")], **kwargs) -> GetXtzTxStatus200Response:  # noqa: E501
         """Transaction Status  # noqa: E501
 
-        Get the status of an Ethereum transaction  # noqa: E501
+        Get the status of a Tezos transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_tx_status(tx_hash, async_req=True)
+        >>> thread = api.get_xtz_tx_status(tx_hash, block_number, async_req=True)
         >>> result = thread.get()
 
         :param tx_hash: Hash of the transaction (required)
         :type tx_hash: str
+        :param block_number: Block number in which the transaction was included (required)
+        :type block_number: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GetEthTxStatus200Response
+        :rtype: GetXtzTxStatus200Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_eth_tx_status_with_http_info(tx_hash, **kwargs)  # noqa: E501
+        return self.get_xtz_tx_status_with_http_info(tx_hash, block_number, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_eth_tx_status_with_http_info(self, tx_hash : Annotated[StrictStr, Field(..., description="Hash of the transaction")], **kwargs):  # noqa: E501
+    def get_xtz_tx_status_with_http_info(self, tx_hash : Annotated[StrictStr, Field(..., description="Hash of the transaction")], block_number : Annotated[StrictStr, Field(..., description="Block number in which the transaction was included")], **kwargs):  # noqa: E501
         """Transaction Status  # noqa: E501
 
-        Get the status of an Ethereum transaction  # noqa: E501
+        Get the status of a Tezos transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_eth_tx_status_with_http_info(tx_hash, async_req=True)
+        >>> thread = api.get_xtz_tx_status_with_http_info(tx_hash, block_number, async_req=True)
         >>> result = thread.get()
 
         :param tx_hash: Hash of the transaction (required)
         :type tx_hash: str
+        :param block_number: Block number in which the transaction was included (required)
+        :type block_number: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1061,21 +759,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GetEthTxStatus200Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetXtzTxStatus200Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'tx_hash'
+            'tx_hash',
+            'block_number'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1086,28 +785,30 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_eth_tx_status" % _key
+                    " to method get_xtz_tx_status" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
         if _params.get('tx_hash') is not None:  # noqa: E501
             _query_params.append(('tx_hash', _params['tx_hash']))
+        if _params.get('block_number') is not None:  # noqa: E501
+            _query_params.append(('block_number', _params['block_number']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -1119,22 +820,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json; charset=utf-8'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '200': "GetEthTxStatus200Response",
+            '200': "GetXtzTxStatus200Response",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
-            '/v1/eth/transaction/status', 'GET',
+            '/v1/xtz/transaction/status', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1143,57 +844,57 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def post_eth_broadcast_tx(self, eth_broadcast_tx_payload : Annotated[ETHBroadcastTxPayload, Field(..., description="Transaction to broadcast")], **kwargs) -> PostEthBroadcastTx201Response:  # noqa: E501
+    def post_xtz_broadcast_tx(self, xtz_broadcast_tx_payload : Annotated[XTZBroadcastTxPayload, Field(..., description="Transaction to broadcast")], **kwargs) -> PostXtzBroadcastTx201Response:  # noqa: E501
         """Broadcast Transaction  # noqa: E501
 
-        Broadcasts a signed Ethereum transaction  # noqa: E501
+        Broadcasts a signed Tezos transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.post_eth_broadcast_tx(eth_broadcast_tx_payload, async_req=True)
+        >>> thread = api.post_xtz_broadcast_tx(xtz_broadcast_tx_payload, async_req=True)
         >>> result = thread.get()
 
-        :param eth_broadcast_tx_payload: Transaction to broadcast (required)
-        :type eth_broadcast_tx_payload: ETHBroadcastTxPayload
+        :param xtz_broadcast_tx_payload: Transaction to broadcast (required)
+        :type xtz_broadcast_tx_payload: XTZBroadcastTxPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PostEthBroadcastTx201Response
+        :rtype: PostXtzBroadcastTx201Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.post_eth_broadcast_tx_with_http_info(eth_broadcast_tx_payload, **kwargs)  # noqa: E501
+        return self.post_xtz_broadcast_tx_with_http_info(xtz_broadcast_tx_payload, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def post_eth_broadcast_tx_with_http_info(self, eth_broadcast_tx_payload : Annotated[ETHBroadcastTxPayload, Field(..., description="Transaction to broadcast")], **kwargs):  # noqa: E501
+    def post_xtz_broadcast_tx_with_http_info(self, xtz_broadcast_tx_payload : Annotated[XTZBroadcastTxPayload, Field(..., description="Transaction to broadcast")], **kwargs):  # noqa: E501
         """Broadcast Transaction  # noqa: E501
 
-        Broadcasts a signed Ethereum transaction  # noqa: E501
+        Broadcasts a signed Tezos transaction  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.post_eth_broadcast_tx_with_http_info(eth_broadcast_tx_payload, async_req=True)
+        >>> thread = api.post_xtz_broadcast_tx_with_http_info(xtz_broadcast_tx_payload, async_req=True)
         >>> result = thread.get()
 
-        :param eth_broadcast_tx_payload: Transaction to broadcast (required)
-        :type eth_broadcast_tx_payload: ETHBroadcastTxPayload
+        :param xtz_broadcast_tx_payload: Transaction to broadcast (required)
+        :type xtz_broadcast_tx_payload: XTZBroadcastTxPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1207,21 +908,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PostEthBroadcastTx201Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PostXtzBroadcastTx201Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'eth_broadcast_tx_payload'
+            'xtz_broadcast_tx_payload'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1232,15 +933,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method post_eth_broadcast_tx" % _key
+                    " to method post_xtz_broadcast_tx" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -1254,16 +955,16 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['eth_broadcast_tx_payload']:
-            _body_params = _params['eth_broadcast_tx_payload']
+        if _params['xtz_broadcast_tx_payload']:
+            _body_params = _params['xtz_broadcast_tx_payload']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json; charset=utf-8'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -1272,22 +973,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '201': "PostEthBroadcastTx201Response",
+            '201': "PostXtzBroadcastTx201Response",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
-            '/v1/eth/transaction/broadcast', 'POST',
+            '/v1/xtz/transaction/broadcast', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1296,57 +997,57 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def post_eth_keys(self, eth_post_keys_payload : Annotated[ETHPostKeysPayload, Field(..., description="Ethereum keys to generate")], **kwargs) -> PostEthKeys201Response:  # noqa: E501
-        """Validation Keys  # noqa: E501
+    def post_xtz_prepare_tx(self, xtz_prepare_tx_payload : Annotated[XTZPrepareTxPayload, Field(..., description="Transaction to prepare")], **kwargs) -> PostXtzPrepareTx201Response:  # noqa: E501
+        """Prepare Transaction  # noqa: E501
 
-        Create Ethereum validation keys on Kiln's infrastructure.  # noqa: E501
+        Prepare a Tezos transaction for broadcasting. It takes a serialized transaction and its signatures and returns a serialized signed transaction that can be broadcasted.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.post_eth_keys(eth_post_keys_payload, async_req=True)
+        >>> thread = api.post_xtz_prepare_tx(xtz_prepare_tx_payload, async_req=True)
         >>> result = thread.get()
 
-        :param eth_post_keys_payload: Ethereum keys to generate (required)
-        :type eth_post_keys_payload: ETHPostKeysPayload
+        :param xtz_prepare_tx_payload: Transaction to prepare (required)
+        :type xtz_prepare_tx_payload: XTZPrepareTxPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PostEthKeys201Response
+        :rtype: PostXtzPrepareTx201Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.post_eth_keys_with_http_info(eth_post_keys_payload, **kwargs)  # noqa: E501
+        return self.post_xtz_prepare_tx_with_http_info(xtz_prepare_tx_payload, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def post_eth_keys_with_http_info(self, eth_post_keys_payload : Annotated[ETHPostKeysPayload, Field(..., description="Ethereum keys to generate")], **kwargs):  # noqa: E501
-        """Validation Keys  # noqa: E501
+    def post_xtz_prepare_tx_with_http_info(self, xtz_prepare_tx_payload : Annotated[XTZPrepareTxPayload, Field(..., description="Transaction to prepare")], **kwargs):  # noqa: E501
+        """Prepare Transaction  # noqa: E501
 
-        Create Ethereum validation keys on Kiln's infrastructure.  # noqa: E501
+        Prepare a Tezos transaction for broadcasting. It takes a serialized transaction and its signatures and returns a serialized signed transaction that can be broadcasted.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.post_eth_keys_with_http_info(eth_post_keys_payload, async_req=True)
+        >>> thread = api.post_xtz_prepare_tx_with_http_info(xtz_prepare_tx_payload, async_req=True)
         >>> result = thread.get()
 
-        :param eth_post_keys_payload: Ethereum keys to generate (required)
-        :type eth_post_keys_payload: ETHPostKeysPayload
+        :param xtz_prepare_tx_payload: Transaction to prepare (required)
+        :type xtz_prepare_tx_payload: XTZPrepareTxPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1360,21 +1061,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PostEthKeys201Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PostXtzPrepareTx201Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'eth_post_keys_payload'
+            'xtz_prepare_tx_payload'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1385,15 +1086,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method post_eth_keys" % _key
+                    " to method post_xtz_prepare_tx" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -1407,16 +1108,16 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['eth_post_keys_payload']:
-            _body_params = _params['eth_post_keys_payload']
+        if _params['xtz_prepare_tx_payload']:
+            _body_params = _params['xtz_prepare_tx_payload']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json; charset=utf-8'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -1425,22 +1126,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '201': "PostEthKeys201Response",
+            '201': "PostXtzPrepareTx201Response",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
-            '/v1/eth/keys', 'POST',
+            '/v1/xtz/transaction/prepare', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1449,57 +1150,57 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def post_eth_prepare_tx(self, eth_prepare_tx_payload : Annotated[ETHPrepareTxPayload, Field(..., description="Transaction to prepare")], **kwargs) -> PostEthPrepareTx201Response:  # noqa: E501
-        """Prepare Transaction  # noqa: E501
+    def post_xtz_stake_tx(self, xtz_craft_stake_tx_payload : Annotated[XTZCraftStakeTxPayload, Field(..., description="Transaction to craft")], **kwargs) -> PostXtzStakeTx201Response:  # noqa: E501
+        """Stake Transaction  # noqa: E501
 
-        Prepare an Ethereum transaction for broadcasting. It takes a serialized transaction and its signatures and returns a serialized signed transaction that can be broadcasted.  # noqa: E501
+        Generates a delegation transaction on Tezos  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.post_eth_prepare_tx(eth_prepare_tx_payload, async_req=True)
+        >>> thread = api.post_xtz_stake_tx(xtz_craft_stake_tx_payload, async_req=True)
         >>> result = thread.get()
 
-        :param eth_prepare_tx_payload: Transaction to prepare (required)
-        :type eth_prepare_tx_payload: ETHPrepareTxPayload
+        :param xtz_craft_stake_tx_payload: Transaction to craft (required)
+        :type xtz_craft_stake_tx_payload: XTZCraftStakeTxPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PostEthPrepareTx201Response
+        :rtype: PostXtzStakeTx201Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.post_eth_prepare_tx_with_http_info(eth_prepare_tx_payload, **kwargs)  # noqa: E501
+        return self.post_xtz_stake_tx_with_http_info(xtz_craft_stake_tx_payload, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def post_eth_prepare_tx_with_http_info(self, eth_prepare_tx_payload : Annotated[ETHPrepareTxPayload, Field(..., description="Transaction to prepare")], **kwargs):  # noqa: E501
-        """Prepare Transaction  # noqa: E501
+    def post_xtz_stake_tx_with_http_info(self, xtz_craft_stake_tx_payload : Annotated[XTZCraftStakeTxPayload, Field(..., description="Transaction to craft")], **kwargs):  # noqa: E501
+        """Stake Transaction  # noqa: E501
 
-        Prepare an Ethereum transaction for broadcasting. It takes a serialized transaction and its signatures and returns a serialized signed transaction that can be broadcasted.  # noqa: E501
+        Generates a delegation transaction on Tezos  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.post_eth_prepare_tx_with_http_info(eth_prepare_tx_payload, async_req=True)
+        >>> thread = api.post_xtz_stake_tx_with_http_info(xtz_craft_stake_tx_payload, async_req=True)
         >>> result = thread.get()
 
-        :param eth_prepare_tx_payload: Transaction to prepare (required)
-        :type eth_prepare_tx_payload: ETHPrepareTxPayload
+        :param xtz_craft_stake_tx_payload: Transaction to craft (required)
+        :type xtz_craft_stake_tx_payload: XTZCraftStakeTxPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1513,21 +1214,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PostEthPrepareTx201Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PostXtzStakeTx201Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'eth_prepare_tx_payload'
+            'xtz_craft_stake_tx_payload'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1538,15 +1239,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method post_eth_prepare_tx" % _key
+                    " to method post_xtz_stake_tx" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -1560,16 +1261,16 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['eth_prepare_tx_payload']:
-            _body_params = _params['eth_prepare_tx_payload']
+        if _params['xtz_craft_stake_tx_payload']:
+            _body_params = _params['xtz_craft_stake_tx_payload']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json; charset=utf-8'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -1578,22 +1279,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '201': "PostEthPrepareTx201Response",
+            '201': "PostXtzStakeTx201Response",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
-            '/v1/eth/transaction/prepare', 'POST',
+            '/v1/xtz/transaction/stake', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1602,57 +1303,57 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def post_eth_stake_tx(self, eth_craft_stake_tx_payload : Annotated[ETHCraftStakeTxPayload, Field(..., description="Transaction to craft")], **kwargs) -> PostEthStakeTx201Response:  # noqa: E501
-        """Stake Transaction  # noqa: E501
+    def post_xtz_un_stake_tx(self, xtz_craft_un_stake_tx_payload : Annotated[XTZCraftUnStakeTxPayload, Field(..., description="Transaction to craft")], **kwargs) -> PostXtzStakeTx201Response:  # noqa: E501
+        """Unstake Transaction  # noqa: E501
 
-        Generates an Ethereum EIP 1559 stake transaction  # noqa: E501
+        Generates an undelegate transaction on Tezos  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.post_eth_stake_tx(eth_craft_stake_tx_payload, async_req=True)
+        >>> thread = api.post_xtz_un_stake_tx(xtz_craft_un_stake_tx_payload, async_req=True)
         >>> result = thread.get()
 
-        :param eth_craft_stake_tx_payload: Transaction to craft (required)
-        :type eth_craft_stake_tx_payload: ETHCraftStakeTxPayload
+        :param xtz_craft_un_stake_tx_payload: Transaction to craft (required)
+        :type xtz_craft_un_stake_tx_payload: XTZCraftUnStakeTxPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PostEthStakeTx201Response
+        :rtype: PostXtzStakeTx201Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.post_eth_stake_tx_with_http_info(eth_craft_stake_tx_payload, **kwargs)  # noqa: E501
+        return self.post_xtz_un_stake_tx_with_http_info(xtz_craft_un_stake_tx_payload, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def post_eth_stake_tx_with_http_info(self, eth_craft_stake_tx_payload : Annotated[ETHCraftStakeTxPayload, Field(..., description="Transaction to craft")], **kwargs):  # noqa: E501
-        """Stake Transaction  # noqa: E501
+    def post_xtz_un_stake_tx_with_http_info(self, xtz_craft_un_stake_tx_payload : Annotated[XTZCraftUnStakeTxPayload, Field(..., description="Transaction to craft")], **kwargs):  # noqa: E501
+        """Unstake Transaction  # noqa: E501
 
-        Generates an Ethereum EIP 1559 stake transaction  # noqa: E501
+        Generates an undelegate transaction on Tezos  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.post_eth_stake_tx_with_http_info(eth_craft_stake_tx_payload, async_req=True)
+        >>> thread = api.post_xtz_un_stake_tx_with_http_info(xtz_craft_un_stake_tx_payload, async_req=True)
         >>> result = thread.get()
 
-        :param eth_craft_stake_tx_payload: Transaction to craft (required)
-        :type eth_craft_stake_tx_payload: ETHCraftStakeTxPayload
+        :param xtz_craft_un_stake_tx_payload: Transaction to craft (required)
+        :type xtz_craft_un_stake_tx_payload: XTZCraftUnStakeTxPayload
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1666,21 +1367,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PostEthStakeTx201Response, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PostXtzStakeTx201Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'eth_craft_stake_tx_payload'
+            'xtz_craft_un_stake_tx_payload'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1691,15 +1392,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method post_eth_stake_tx" % _key
+                    " to method post_xtz_un_stake_tx" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -1713,16 +1414,16 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['eth_craft_stake_tx_payload']:
-            _body_params = _params['eth_craft_stake_tx_payload']
+        if _params['xtz_craft_un_stake_tx_payload']:
+            _body_params = _params['xtz_craft_un_stake_tx_payload']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json; charset=utf-8'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -1731,22 +1432,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearerAuth']  # noqa: E501
 
         _response_types_map = {
-            '201': "PostEthStakeTx201Response",
+            '201': "PostXtzStakeTx201Response",
             '400': None,
             '401': None,
             '500': None,
         }
 
         return self.api_client.call_api(
-            '/v1/eth/transaction/stake', 'POST',
+            '/v1/xtz/transaction/unstake', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api/sol_api.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api/sol_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/api_client.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/configuration.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/exceptions.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/__init__.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 from kiln_connect.openapi_client.models.get_sol_operations200_response import GetSolOperations200Response
 from kiln_connect.openapi_client.models.get_sol_operations200_response_data_inner import GetSolOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_rewards200_response import GetSolRewards200Response
 from kiln_connect.openapi_client.models.get_sol_rewards200_response_data_inner import GetSolRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_sol_stakes200_response import GetSolStakes200Response
 from kiln_connect.openapi_client.models.get_sol_tx_status200_response import GetSolTxStatus200Response
 from kiln_connect.openapi_client.models.get_xtz_network_stats200_response import GetXtzNetworkStats200Response
+from kiln_connect.openapi_client.models.get_xtz_operations200_response import GetXtzOperations200Response
+from kiln_connect.openapi_client.models.get_xtz_operations200_response_data_inner import GetXtzOperations200ResponseDataInner
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response import GetXtzRewards200Response
 from kiln_connect.openapi_client.models.get_xtz_rewards200_response_data_inner import GetXtzRewards200ResponseDataInner
 from kiln_connect.openapi_client.models.get_xtz_stakes200_response import GetXtzStakes200Response
 from kiln_connect.openapi_client.models.get_xtz_tx_status200_response import GetXtzTxStatus200Response
 from kiln_connect.openapi_client.models.post_account201_response import PostAccount201Response
 from kiln_connect.openapi_client.models.post_eth_broadcast_tx201_response import PostEthBroadcastTx201Response
 from kiln_connect.openapi_client.models.post_eth_keys201_response import PostEthKeys201Response
@@ -108,13 +110,17 @@
 from kiln_connect.openapi_client.models.xtz_broadcast_tx_payload import XTZBroadcastTxPayload
 from kiln_connect.openapi_client.models.xtz_broadcasted_tx import XTZBroadcastedTx
 from kiln_connect.openapi_client.models.xtz_craft_stake_tx_payload import XTZCraftStakeTxPayload
 from kiln_connect.openapi_client.models.xtz_craft_un_stake_tx_payload import XTZCraftUnStakeTxPayload
 from kiln_connect.openapi_client.models.xtz_cycle_reward import XTZCycleReward
 from kiln_connect.openapi_client.models.xtz_daily_reward import XTZDailyReward
 from kiln_connect.openapi_client.models.xtz_network_stats import XTZNetworkStats
+from kiln_connect.openapi_client.models.xtz_operation_activation import XTZOperationActivation
+from kiln_connect.openapi_client.models.xtz_operation_delegate import XTZOperationDelegate
+from kiln_connect.openapi_client.models.xtz_operation_payment import XTZOperationPayment
+from kiln_connect.openapi_client.models.xtz_operation_undelegate import XTZOperationUndelegate
 from kiln_connect.openapi_client.models.xtz_prepare_tx_payload import XTZPrepareTxPayload
 from kiln_connect.openapi_client.models.xtz_signed_tx import XTZSignedTx
 from kiln_connect.openapi_client.models.xtz_stake import XTZStake
 from kiln_connect.openapi_client.models.xtztx_status import XTZTxStatus
 from kiln_connect.openapi_client.models.xtztx_status_receipt import XTZTxStatusReceipt
 from kiln_connect.openapi_client.models.xtz_unsigned_tx import XTZUnsignedTx
```

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_portfolio.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_balance.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/account_portfolio_protocols_inner_total_rewards.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/atom_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/atom_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/atom_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/atom_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/core_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/core_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_broadcasted_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_kiln_stats.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_kiln_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_kiln_stats_gross_apy.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_network_stats.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_consensus_withdrawal.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_operation_deposit.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_deposit.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_operation_execution_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_operation_execution_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_batch_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_cli_response_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_post_keys_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_post_keys_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_signed_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/eth_unsigned_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/eth_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/ethtx_status.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/ethtx_status_receipt.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status_receipt.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/ethtx_status_receipt_logs_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_account_portfolio200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_account_portfolio200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_accounts200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_accounts200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_atom_rewards200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_atom_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_atom_stakes200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_atom_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_kiln_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_operations200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_operations200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_rewards200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_stakes200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_eth_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_operations200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_operations200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_rewards200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_rewards200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_stakes200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_sol_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_rewards200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/get_xtz_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_account201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_account201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_keys201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_keys201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_keys201_response_data.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_eth_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_sol_stakes201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_sol_stakes201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/post_xtz_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_broadcast_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_broadcast_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_deactivate_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_merge_stakes_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_network_stats.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_create_account.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_create_account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_create_account_with_seed.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_create_account_with_seed.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_deactivate.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_deactivate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_delegate.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_delegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_merge.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_merge.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_redelegate.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_redelegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_split.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_split.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_operation_withdraw.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_operation_withdraw.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_post_stakes_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_post_stakes_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_post_stakes_payload_stakes_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_prepared_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_prepared_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_reward_by_day.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_reward_by_day.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_reward_by_epoch.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_reward_by_epoch.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_split_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,20 +31,19 @@
     vote_account: Optional[StrictStr] = Field(None, description="Vote account to which this stake was re-delegated.")
     withdraw_pubkey: Optional[StrictStr] = Field(None, description="Withdraw pubkey")
     state: Optional[StrictStr] = Field(None, description="Stake state")
     activated_at: Optional[datetime] = Field(None, description="Date at which this stake was activated")
     activated_epoch: Optional[StrictInt] = Field(None, description="Epoch at which this stake was activated")
     deactivated_at: Optional[datetime] = Field(None, description="Date at which this stake was deactivated")
     deactivated_epoch: Optional[StrictInt] = Field(None, description="Epoch at which this stake was deactivated")
-    delegated_epoch: Optional[StrictInt] = Field(None, description="Epoch at which this stake was delegated")
     balance: Optional[StrictStr] = Field(None, description="Current balance in Lamport")
     rewards: Optional[StrictStr] = Field(None, description="Sum of rewards rewards in Lamport earned by this stake")
     net_apy: Optional[float] = Field(None, description="Net annual percentage yield")
     updated_at: Optional[datetime] = Field(None, description="Last date this data was updated")
-    __properties = ["stake_account", "vote_account", "withdraw_pubkey", "state", "activated_at", "activated_epoch", "deactivated_at", "deactivated_epoch", "delegated_epoch", "balance", "rewards", "net_apy", "updated_at"]
+    __properties = ["stake_account", "vote_account", "withdraw_pubkey", "state", "activated_at", "activated_epoch", "deactivated_at", "deactivated_epoch", "balance", "rewards", "net_apy", "updated_at"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -73,18 +72,14 @@
         if self.deactivated_at is None:
             _dict['deactivated_at'] = None
 
         # set to None if deactivated_epoch (nullable) is None
         if self.deactivated_epoch is None:
             _dict['deactivated_epoch'] = None
 
-        # set to None if delegated_epoch (nullable) is None
-        if self.delegated_epoch is None:
-            _dict['delegated_epoch'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> SOLStake:
         """Create an instance of SOLStake from a dict"""
         if obj is None:
             return None
@@ -97,15 +92,14 @@
             "vote_account": obj.get("vote_account"),
             "withdraw_pubkey": obj.get("withdraw_pubkey"),
             "state": obj.get("state"),
             "activated_at": obj.get("activated_at"),
             "activated_epoch": obj.get("activated_epoch"),
             "deactivated_at": obj.get("deactivated_at"),
             "deactivated_epoch": obj.get("deactivated_epoch"),
-            "delegated_epoch": obj.get("delegated_epoch"),
             "balance": obj.get("balance"),
             "rewards": obj.get("rewards"),
             "net_apy": obj.get("net_apy"),
             "updated_at": obj.get("updated_at")
         })
         return _obj
```

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_stake_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/sol_withdraw_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/soltx_status.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/soltx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_craft_un_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_cycle_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_cycle_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_daily_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_daily_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_network_stats.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_signed_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtz_unsigned_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtz_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtztx_status.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtztx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/models/xtztx_status_receipt.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/models/xtztx_status_receipt.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/rest.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_portfolio.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_balance.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_account_portfolio_protocols_inner_total_rewards.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_accounts_api.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_accounts_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_atom_api.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_atom_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_atom_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_atom_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_core_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_core_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_api.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_kiln_stats.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_kiln_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_kiln_stats_gross_apy.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_network_stats.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_consensus_withdrawal.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_operation_deposit.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_deposit.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_operation_execution_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_batch_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_cli_response_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_post_keys_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_signed_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_eth_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_ethtx_status.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status_receipt.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_ethtx_status_receipt_logs_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_account_portfolio200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_accounts200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_accounts200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_atom_rewards200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_atom_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_atom_stakes200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_atom_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_kiln_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_operations200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_eth_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_operations200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_operations200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_operations200_response_data_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_operations200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_rewards200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_stakes200_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,14 @@
                         vote_account = '6hNweZvzTudTuprZrAXb1A9grKvVG6xgjyvdJUqAMk78', 
                         withdraw_pubkey = '4wdr76KJTFgH68YtGddmnF45WdD8LMv9eLsdf', 
                         state = 'active', 
                         activated_at = '2023-01-14T01:13:59Z', 
                         activated_epoch = 150, 
                         deactivated_at = '2023-01-14T01:13:59Z', 
                         deactivated_epoch = 150, 
-                        delegated_epoch = 150, 
                         balance = '1000000000', 
                         rewards = '1000000000', 
                         net_apy = 3.407, 
                         updated_at = '2023-01-14T01:13:59Z', )
                     ]
             )
         else :
```

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_sol_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_network_stats200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_rewards200_response_data_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_stakes200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_get_xtz_tx_status200_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_account201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_account201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_keys201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_keys201_response_data.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_eth_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_sol_stakes201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_broadcast_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_prepare_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_post_xtz_stake_tx201_response.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_api.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_api.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_broadcast_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_deactivate_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_merge_stakes_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_network_stats.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_create_account.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_create_account.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_create_account_with_seed.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_create_account_with_seed.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_deactivate.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_deactivate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_delegate.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_delegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_merge.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_merge.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_redelegate.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_redelegate.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_split.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_split.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_operation_withdraw.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_operation_withdraw.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_post_stakes_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_post_stakes_payload_stakes_inner.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_prepared_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_prepared_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_reward_by_day.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_reward_by_day.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_reward_by_epoch.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_split_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
                 vote_account = '6hNweZvzTudTuprZrAXb1A9grKvVG6xgjyvdJUqAMk78', 
                 withdraw_pubkey = '4wdr76KJTFgH68YtGddmnF45WdD8LMv9eLsdf', 
                 state = 'active', 
                 activated_at = '2023-01-14T01:13:59Z', 
                 activated_epoch = 150, 
                 deactivated_at = '2023-01-14T01:13:59Z', 
                 deactivated_epoch = 150, 
-                delegated_epoch = 150, 
                 balance = '1000000000', 
                 rewards = '1000000000', 
                 net_apy = 3.407, 
                 updated_at = '2023-01-14T01:13:59Z'
             )
         else :
             return SOLStake(
```

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_stake_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_sol_withdraw_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_soltx_status.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_soltx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_api.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,21 @@
     def test_get_xtz_network_stats(self):
         """Test case for get_xtz_network_stats
 
         Network Stats  # noqa: E501
         """
         pass
 
+    def test_get_xtz_operations(self):
+        """Test case for get_xtz_operations
+
+        Operations  # noqa: E501
+        """
+        pass
+
     def test_get_xtz_rewards(self):
         """Test case for get_xtz_rewards
 
         Rewards  # noqa: E501
         """
         pass
```

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_broadcast_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_broadcasted_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_craft_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_craft_un_stake_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_cycle_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_daily_reward.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_daily_reward.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_network_stats.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_network_stats.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_prepare_tx_payload.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_signed_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_signed_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_stake.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_stake.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtz_unsigned_tx.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtztx_status.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtztx_status.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py` & `kiln_connect-1.0.0.dev6/kiln_connect/openapi_client/test/test_xtztx_status_receipt.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/sol.py` & `kiln_connect-1.0.0.dev6/kiln_connect/sol.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/kiln_connect/xtz.py` & `kiln_connect-1.0.0.dev6/kiln_connect/xtz.py`

 * *Files identical despite different names*

### Comparing `kiln_connect-1.0.0.dev5/pyproject.toml` & `kiln_connect-1.0.0.dev6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kiln-connect"
-version = "1.0.0-dev5"
+version = "1.0.0-dev6"
 description = ""
 authors = ["s. rannou <mxs@sbrk.org>"]
 maintainers = ["s. rannou <mxs@sbrk.org>"]
 readme = "docs/README.md"
 homepage = "https://kiln.fi/"
 repository = "https://github.com/kilnfi/sdk-py"
 keywords = ["staking", "blockchain"]
```

### Comparing `kiln_connect-1.0.0.dev5/PKG-INFO` & `kiln_connect-1.0.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiln-connect
-Version: 1.0.0.dev5
+Version: 1.0.0.dev6
 Summary: 
 Home-page: https://kiln.fi/
 Keywords: staking,blockchain
 Author: s. rannou
 Author-email: mxs@sbrk.org
 Maintainer: s. rannou
 Maintainer-email: mxs@sbrk.org
```

