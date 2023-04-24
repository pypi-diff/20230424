# Comparing `tmp/ipfabric-6.2.0b4.tar.gz` & `tmp/ipfabric-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.2.0b4.tar", max compression
+gzip compressed data, was "ipfabric-6.2.1.tar", max compression
```

## Comparing `ipfabric-6.2.0b4.tar` & `ipfabric-6.2.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1790 2023-03-16 16:58:08.617128 ipfabric-6.2.0b4/ipfabric/__init__.py
--rw-r--r--   0        0        0    17132 2023-04-05 16:49:28.923924 ipfabric-6.2.0b4/ipfabric/api.py
--rw-r--r--   0        0        0     9218 2023-04-04 13:54:22.367500 ipfabric-6.2.0b4/ipfabric/client.py
--rw-r--r--   0        0        0      322 2023-02-08 21:33:38.498830 ipfabric-6.2.0b4/ipfabric/models/__init__.py
--rw-r--r--   0        0        0     6054 2023-03-14 15:20:54.722357 ipfabric-6.2.0b4/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2786 2023-03-14 15:45:17.816340 ipfabric-6.2.0b4/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0     2110 2023-02-09 13:14:16.640525 ipfabric-6.2.0b4/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     5669 2023-02-09 13:14:16.640525 ipfabric-6.2.0b4/ipfabric/models/jobs.py
--rw-r--r--   0        0        0    12119 2023-04-05 17:31:47.761633 ipfabric-6.2.0b4/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0    12162 2023-03-14 14:52:33.106216 ipfabric-6.2.0b4/ipfabric/models/table.py
--rw-r--r--   0        0        0     2830 2023-02-09 13:14:16.655535 ipfabric-6.2.0b4/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1156 2023-02-25 14:47:47.471307 ipfabric-6.2.0b4/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      488 2023-02-08 13:05:11.993384 ipfabric-6.2.0b4/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2173 2023-02-08 13:05:11.998383 ipfabric-6.2.0b4/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1002 2023-02-08 13:05:12.003471 ipfabric-6.2.0b4/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     7018 2023-02-25 14:47:47.471307 ipfabric-6.2.0b4/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      324 2023-02-08 13:05:12.011503 ipfabric-6.2.0b4/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0      843 2023-02-08 13:05:12.016497 ipfabric-6.2.0b4/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      470 2023-02-08 13:05:12.021499 ipfabric-6.2.0b4/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     5644 2023-02-08 13:05:12.027499 ipfabric-6.2.0b4/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2045 2023-02-25 14:47:47.482435 ipfabric-6.2.0b4/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     2783 2023-02-25 14:47:47.482435 ipfabric-6.2.0b4/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0      759 2023-02-08 13:05:12.031562 ipfabric-6.2.0b4/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      633 2023-02-08 13:05:12.031562 ipfabric-6.2.0b4/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     3529 2023-02-25 14:51:16.763228 ipfabric-6.2.0b4/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1231 2023-02-08 13:05:12.050282 ipfabric-6.2.0b4/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1078 2023-02-08 13:05:12.065065 ipfabric-6.2.0b4/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     4773 2023-02-25 14:51:16.794519 ipfabric-6.2.0b4/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2159 2023-02-08 13:05:12.078066 ipfabric-6.2.0b4/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      431 2023-02-08 13:05:12.083210 ipfabric-6.2.0b4/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2062 2023-02-08 13:05:12.088455 ipfabric-6.2.0b4/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2228 2023-02-08 13:05:12.092469 ipfabric-6.2.0b4/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0      856 2023-02-08 13:05:12.097528 ipfabric-6.2.0b4/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0      867 2023-02-08 13:05:12.097528 ipfabric-6.2.0b4/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.2.0b4/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3602 2023-02-09 20:02:01.172909 ipfabric-6.2.0b4/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     6187 2023-02-08 13:05:11.963806 ipfabric-6.2.0b4/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.2.0b4/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.2.0b4/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.2.0b4/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     1413 2023-01-31 20:32:11.592169 ipfabric-6.2.0b4/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     5247 2023-04-05 17:31:47.706534 ipfabric-6.2.0b4/ipfabric/settings/user_mgmt.py
--rw-r--r--   0        0        0     1875 2023-02-08 14:40:46.626939 ipfabric-6.2.0b4/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     6439 2023-02-09 20:02:01.204437 ipfabric-6.2.0b4/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.2.0b4/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     7876 2023-03-30 17:03:49.576728 ipfabric-6.2.0b4/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.2.0b4/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/__init__.py
--rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/dashboard.json
--rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/groups.json
--rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/__init__.py
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/__init__.py
--rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/dashboard.json
--rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/groups.json
--rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/intents.json
--rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-03 16:42:03.278481 ipfabric-6.2.0b4/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     5784 2023-01-31 20:32:11.624088 ipfabric-6.2.0b4/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0     2519 2023-02-09 19:07:57.301096 ipfabric-6.2.0b4/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2396 2023-02-09 18:58:27.499064 ipfabric-6.2.0b4/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2573 2023-03-24 18:58:14.154592 ipfabric-6.2.0b4/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.2.0b4/LICENSE
--rw-r--r--   0        0        0     2016 2023-04-05 18:08:11.041198 ipfabric-6.2.0b4/pyproject.toml
--rw-r--r--   0        0        0     3705 2023-04-04 13:32:24.957368 ipfabric-6.2.0b4/README.md
--rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 ipfabric-6.2.0b4/setup.py
--rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 ipfabric-6.2.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1790 2023-03-16 16:58:08.617128 ipfabric-6.2.1/ipfabric/__init__.py
+-rw-r--r--   0        0        0    17096 2023-04-10 11:49:56.699072 ipfabric-6.2.1/ipfabric/api.py
+-rw-r--r--   0        0        0     9229 2023-04-10 11:49:19.028096 ipfabric-6.2.1/ipfabric/client.py
+-rw-r--r--   0        0        0      322 2023-02-08 21:33:38.498830 ipfabric-6.2.1/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0     6054 2023-03-14 15:20:54.722357 ipfabric-6.2.1/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2786 2023-03-14 15:45:17.816340 ipfabric-6.2.1/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0     2110 2023-02-09 13:14:16.640525 ipfabric-6.2.1/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     5669 2023-02-09 13:14:16.640525 ipfabric-6.2.1/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0    12119 2023-04-05 17:31:47.761633 ipfabric-6.2.1/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0    15036 2023-04-24 13:56:20.167261 ipfabric-6.2.1/ipfabric/models/table.py
+-rw-r--r--   0        0        0     2830 2023-02-09 13:14:16.655535 ipfabric-6.2.1/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1156 2023-02-25 14:47:47.471307 ipfabric-6.2.1/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      488 2023-02-08 13:05:11.993384 ipfabric-6.2.1/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2173 2023-02-08 13:05:11.998383 ipfabric-6.2.1/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1002 2023-02-08 13:05:12.003471 ipfabric-6.2.1/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     7018 2023-02-25 14:47:47.471307 ipfabric-6.2.1/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      324 2023-02-08 13:05:12.011503 ipfabric-6.2.1/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0      843 2023-02-08 13:05:12.016497 ipfabric-6.2.1/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      470 2023-02-08 13:05:12.021499 ipfabric-6.2.1/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     5644 2023-02-08 13:05:12.027499 ipfabric-6.2.1/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2045 2023-02-25 14:47:47.482435 ipfabric-6.2.1/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     2783 2023-02-25 14:47:47.482435 ipfabric-6.2.1/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0      759 2023-02-08 13:05:12.031562 ipfabric-6.2.1/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      633 2023-02-08 13:05:12.031562 ipfabric-6.2.1/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     3529 2023-02-25 14:51:16.763228 ipfabric-6.2.1/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1231 2023-02-08 13:05:12.050282 ipfabric-6.2.1/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1078 2023-02-08 13:05:12.065065 ipfabric-6.2.1/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     4773 2023-02-25 14:51:16.794519 ipfabric-6.2.1/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2159 2023-02-08 13:05:12.078066 ipfabric-6.2.1/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      431 2023-02-08 13:05:12.083210 ipfabric-6.2.1/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2062 2023-02-08 13:05:12.088455 ipfabric-6.2.1/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2228 2023-02-08 13:05:12.092469 ipfabric-6.2.1/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0      856 2023-02-08 13:05:12.097528 ipfabric-6.2.1/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0      867 2023-02-08 13:05:12.097528 ipfabric-6.2.1/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0      805 2023-02-09 20:01:36.099334 ipfabric-6.2.1/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3602 2023-02-09 20:02:01.172909 ipfabric-6.2.1/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     6187 2023-02-08 13:05:11.963806 ipfabric-6.2.1/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     8719 2022-12-14 14:57:33.723874 ipfabric-6.2.1/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1027 2022-12-14 14:57:33.723874 ipfabric-6.2.1/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     2096 2023-02-09 20:15:13.578462 ipfabric-6.2.1/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     1413 2023-01-31 20:32:11.592169 ipfabric-6.2.1/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     5247 2023-04-05 17:31:47.706534 ipfabric-6.2.1/ipfabric/settings/user_mgmt.py
+-rw-r--r--   0        0        0     1875 2023-02-08 14:40:46.626939 ipfabric-6.2.1/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     6439 2023-02-09 20:02:01.204437 ipfabric-6.2.1/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      430 2022-12-12 21:56:50.511542 ipfabric-6.2.1/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     7876 2023-03-30 17:03:49.576728 ipfabric-6.2.1/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5606 2023-01-03 15:30:13.772885 ipfabric-6.2.1/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.1/ipfabric/tools/factory_defaults/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-18 15:07:02.564189 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/__init__.py
+-rw-r--r--   0        0        0     3152 2022-08-18 15:07:02.565190 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/dashboard.json
+-rw-r--r--   0        0        0     5814 2022-08-18 15:07:02.566156 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/groups.json
+-rw-r--r--   0        0        0   121431 2022-08-18 15:07:02.568156 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/__init__.py
+-rw-r--r--   0        0        0     3152 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/dashboard.json
+-rw-r--r--   0        0        0     5822 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/groups.json
+-rw-r--r--   0        0        0   120081 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/intents.json
+-rw-r--r--   0        0        0        0 2022-09-28 15:44:51.125559 ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/__init__.py
+-rw-r--r--   0        0        0     4511 2023-04-03 16:42:03.278481 ipfabric-6.2.1/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     5784 2023-01-31 20:32:11.624088 ipfabric-6.2.1/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0     2519 2023-02-09 19:07:57.301096 ipfabric-6.2.1/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2396 2023-02-09 18:58:27.499064 ipfabric-6.2.1/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2573 2023-03-24 18:58:14.154592 ipfabric-6.2.1/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.2.1/LICENSE
+-rw-r--r--   0        0        0     2014 2023-04-24 14:07:27.097697 ipfabric-6.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3705 2023-04-04 13:32:24.957368 ipfabric-6.2.1/README.md
+-rw-r--r--   0        0        0     5234 1970-01-01 00:00:00.000000 ipfabric-6.2.1/setup.py
+-rw-r--r--   0        0        0     5132 1970-01-01 00:00:00.000000 ipfabric-6.2.1/PKG-INFO
```

### Comparing `ipfabric-6.2.0b4/ipfabric/__init__.py` & `ipfabric-6.2.1/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/api.py` & `ipfabric-6.2.1/ipfabric/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,14 @@
 
     def check_version(self, api_version: str = None, base_url: Union[URL, str] = None) -> tuple:
         """Checks API Version and returns the version to use in the URL and the OS Version
 
         Args:
             api_version: User defined API Version or None
             base_url: URL of IP Fabric
-            dev: Internal Use Only
 
         Returns:
             api_version, os_version
         """
         api_version = (
             api_version.lstrip("v").split(".")
             if api_version
```

### Comparing `ipfabric-6.2.0b4/ipfabric/client.py` & `ipfabric-6.2.1/ipfabric/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from urllib.parse import urlparse
 
 from ipfabric.api import IPFabricAPI
 from ipfabric.models import Technology, Inventory, Jobs, Intent
 
 logger = logging.getLogger("ipfabric")
 
-RE_PATH = re.compile(r"^\/?(api/)?v\d(\.\d)?/")
+RE_PATH = re.compile(r"^/?(api/)?v\d(\.\d)?/")
 RE_TABLE = re.compile(r"^tables/")
 
 
 def check_format(func):
     """
     Checks to make sure api/v1/ is not in the URL and converts filters from json str to dict
     """
 
     def wrapper(self, url, *args, **kwargs):
         if "filters" in kwargs and isinstance(kwargs["filters"], str):
             kwargs["filters"] = loads(kwargs["filters"])
         path = urlparse(url or kwargs["url"]).path
         r = RE_PATH.search(path)
-        url = path[r.end() :] if r else path
+        url = path[r.end():] if r else path  # fmt: skip
         url = url[1:] if url[0] == "/" else url
         return func(self, url, *args, **kwargs)
 
     return wrapper
 
 
 class IPFClient(IPFabricAPI):
```

### Comparing `ipfabric-6.2.0b4/ipfabric/models/intent.py` & `ipfabric-6.2.1/ipfabric/models/intent.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/intent_check.py` & `ipfabric-6.2.1/ipfabric/models/intent_check.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/inventory.py` & `ipfabric-6.2.1/ipfabric/models/inventory.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/jobs.py` & `ipfabric-6.2.1/ipfabric/models/jobs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/snapshot.py` & `ipfabric-6.2.1/ipfabric/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/table.py` & `ipfabric-6.2.1/ipfabric/models/table.py`

 * *Files 20% similar despite different names*

```diff
@@ -196,70 +196,117 @@
         for col in columns:
             if col in columns_ignore and col != "id":
                 logger.debug(f"Column {col} in columns_ignore, ignoring")
                 continue
             cols_for_return.add(col)
         return cols_for_return
 
-    def _compare_determine_columns(self, columns: set, columns_ignore: set, unique_keys: set):
+    def _compare_determine_columns(self, columns: set, columns_ignore: set, unique_keys: set, nested_keys: set):
         """
-        Determines which columns to use in the query.
+        Determines which columns to use in the query, and which columns to use
+        Only supports a single nested column
         Args:
             columns: set : Set of columns to use
             columns_ignore: set : Set of columns to ignore
             unique_keys: set : Set of columns for unique keys
+            nested_keys: set: Set of nested columns that belongs to a column in columns, columns_ignore, or unique_keys
 
         Returns:
-            list[str]: List of columns to use
+            tuple[list, list]: List of columns to use in query, List of columns to use when sorting data
         """
         # get all columns for the table
         table_columns = set(self.client.get_columns(self.endpoint))
 
+        # get any nested columns
+        nested_cols_for_return = None
+        # get a row of data
+        one_row_of_data = self.fetch(limit=1)
+        # loop over each column in the table columns
+        for col in table_columns:
+            # check if the data returned has nested columns
+            if isinstance(one_row_of_data[0][col], list):
+                # get all the nested column names
+                nested_cols = set(one_row_of_data[0][col][0].keys())
+                # create a set of nested column names requested by the user
+                nested_cols_for_return = {col for col in nested_cols if col in nested_keys}
+
         # Must always ignore some columns
         columns_ignore.update(IGNORE_COLUMNS)
 
         cols_for_return = set()
         # user passes unique_keys
         if unique_keys:
             if not table_columns.issuperset(unique_keys):
                 raise ValueError(f"Unique Key(s) {unique_keys - table_columns} not in table {self.name}")
-            [cols_for_return.add(u) for u in unique_keys]
+            for u in unique_keys:
+                cols_for_return.add(u)
+            return list(cols_for_return), nested_cols_for_return
         # user passes columns
         if columns:
             if not table_columns.issuperset(columns):
                 raise ValueError(f"Column(s) {columns - table_columns} not in table {self.name}")
             cols_for_return.update(self._ignore_columns(columns, columns_ignore))
+            return list(cols_for_return), nested_cols_for_return
         # user does not pass columns
+        # or only passed columns_ignore
         else:
             cols_for_return.update(self._ignore_columns(table_columns, columns_ignore))
-        return list(cols_for_return)
+            return list(cols_for_return), nested_cols_for_return
 
     @staticmethod
-    def _hash_data(json_data, unique_keys=None):
+    def _remove_keys_from_dict(dict_object, keys_to_remove):
+        if not keys_to_remove:
+            return dict_object
+
+        for v in dict_object.values():
+            if not isinstance(v, list):
+                continue
+
+            for item in v:
+                for key in keys_to_remove:
+                    if key in item:
+                        item.pop(key)
+
+        return dict_object
+
+    def _hash_data(self, json_data, unique_keys=None, nested_columns_ignore=None):
         """
         Hashes data. Turns any data into a string and hashes it, then returns the hash as a key for the data
         Args:
             json_data: list[dict] : List of dictionaries to hash
             unique_keys: list[str] : List of keys to use for hashing
+            nested_columns_ignore: list[str]: List of nested column keys to filter data
 
         Returns:
             dict[str]: dictionary with hash as key and values as the original data
         """
         # loop over each obj, turn the obj into a string, and hash it
         return_json = dict()
+        # user passes unique_keys
         if unique_keys:
+            # loop over each response
             for dict_obj in json_data:
-                hash_key = {key: dict_obj[key] for key in unique_keys}
+                dict_for_hash = self._remove_keys_from_dict(dict_object=dict_obj, keys_to_remove=nested_columns_ignore)
+                # create a dictionary, of only the keys/columns requested
+                hash_key = {key: dict_for_hash[key] for key in unique_keys}
+                # hash the data
                 unique_hash = deepdiff.DeepHash(hash_key)[hash_key]
+                # check if the data has already been processed.
                 if unique_hash in return_json:
+                    # raise error if data has already been processed
                     raise KeyError(f"Unique Key(s) {unique_keys} are not unique, please adjust unique_keys input.")
-                return_json[unique_hash] = dict_obj
+                # store the data, using the hash as a key
+                return_json[unique_hash] = dict_for_hash
+        # user passes columns and/or column ignore
         else:
+            # loop over each response
             for dict_obj in json_data:
-                return_json[deepdiff.DeepHash(dict_obj)[dict_obj]] = dict_obj
+                dict_for_hash = self._remove_keys_from_dict(dict_object=dict_obj, keys_to_remove=nested_columns_ignore)
+                # hash each object, and store it in a dictionary, with the hash as the key
+                return_json[deepdiff.DeepHash(dict_for_hash)[dict_for_hash]] = dict_for_hash
         return return_json
 
     @staticmethod
     def _make_set(data: Union[list, set, str] = None):
         if isinstance(data, str):
             return {data}
         elif data is None:
@@ -269,54 +316,58 @@
 
     def compare(
         self,
         snapshot_id: str = None,
         columns: Union[list, set] = None,
         columns_ignore: Union[list, set, str] = None,
         unique_keys: Union[list, set, str] = None,
+        nested_columns_ignore: Union[list, set, str] = None,
         **kwargs,
     ):
         """
         Compares a table from the current snapshot to the snapshot_id passed.
         Args:
             snapshot_id: str : The snapshot_id to compare to.
             columns: list : List of columns to compare. If None, will compare all columns.
             columns_ignore: list : List of columns to ignore. If None, will always ignore 'id' column.
             unique_keys: list : List of columns to use as unique keys. If None, will use all columns as primary key.
+            nested_columns_ignore: List of columns that belong to a nested columns
             **kwargs: dict : Optional Table.all() arguments to apply to the table before comparing.
 
         Returns:
             dict : dictionary containing the differences between the two snapshots.
                    Possible keys are 'added', 'removed' and 'changed'.
         """
         return_dict = dict()
 
         # determine which columns to use in query
         columns = self._make_set(columns)
         columns_ignore = self._make_set(columns_ignore)
         unique_keys = self._make_set(unique_keys)
-        cols_for_query = self._compare_determine_columns(columns, columns_ignore, unique_keys)
-
+        nested_columns_ignore = self._make_set(nested_columns_ignore)
+        cols_for_query, nested_cols = self._compare_determine_columns(
+            columns, columns_ignore, unique_keys, nested_columns_ignore
+        )
         data = self.all(columns=cols_for_query, **kwargs)
         data_compare = self.all(snapshot_id=snapshot_id, columns=cols_for_query, **kwargs)
 
         # since we turned the values into a hash, we can just compare the keys
         if unique_keys:
-            hashed_data_unique = self._hash_data(data, unique_keys)
-            hashed_data_compare_unique = self._hash_data(data_compare, unique_keys)
+            hashed_data_unique = self._hash_data(data, unique_keys, nested_cols)
+            hashed_data_compare_unique = self._hash_data(data_compare, unique_keys, nested_cols)
             changed = [
                 hashed_data_unique[hashed_str]
                 for hashed_str in hashed_data_unique.keys()
                 if hashed_str not in hashed_data_compare_unique.keys()
             ]
             return_dict["changed"] = changed
             return return_dict
         # compare both ways
-        hashed_data = self._hash_data(data)
-        hashed_data_compare = self._hash_data(data_compare)
+        hashed_data = self._hash_data(data, nested_columns_ignore=nested_cols)
+        hashed_data_compare = self._hash_data(data_compare, nested_columns_ignore=nested_cols)
         added = [
             hashed_data[hashed_str] for hashed_str in hashed_data.keys() if hashed_str not in hashed_data_compare.keys()
         ]
         removed = [
             hashed_data_compare[hashed_str]
             for hashed_str in hashed_data_compare.keys()
             if hashed_str not in hashed_data.keys()
```

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/__init__.py` & `ipfabric-6.2.1/ipfabric/models/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/addressing.py` & `ipfabric-6.2.1/ipfabric/models/technology/addressing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/dhcp.py` & `ipfabric-6.2.1/ipfabric/models/technology/dhcp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/fhrp.py` & `ipfabric-6.2.1/ipfabric/models/technology/fhrp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/interfaces.py` & `ipfabric-6.2.1/ipfabric/models/technology/interfaces.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.2.1/ipfabric/models/technology/load_balancing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/management.py` & `ipfabric-6.2.1/ipfabric/models/technology/management.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/mpls.py` & `ipfabric-6.2.1/ipfabric/models/technology/mpls.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/multicast.py` & `ipfabric-6.2.1/ipfabric/models/technology/multicast.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/neighbors.py` & `ipfabric-6.2.1/ipfabric/models/technology/neighbors.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/oam.py` & `ipfabric-6.2.1/ipfabric/models/technology/oam.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/platforms.py` & `ipfabric-6.2.1/ipfabric/models/technology/platforms.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/port_channels.py` & `ipfabric-6.2.1/ipfabric/models/technology/port_channels.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/qos.py` & `ipfabric-6.2.1/ipfabric/models/technology/qos.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/routing.py` & `ipfabric-6.2.1/ipfabric/models/technology/routing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/sdn.py` & `ipfabric-6.2.1/ipfabric/models/technology/sdn.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/security.py` & `ipfabric-6.2.1/ipfabric/models/technology/security.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/stp.py` & `ipfabric-6.2.1/ipfabric/models/technology/stp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/vlans.py` & `ipfabric-6.2.1/ipfabric/models/technology/vlans.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/models/technology/wireless.py` & `ipfabric-6.2.1/ipfabric/models/technology/wireless.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/__init__.py` & `ipfabric-6.2.1/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/api_tokens.py` & `ipfabric-6.2.1/ipfabric/settings/api_tokens.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/attributes.py` & `ipfabric-6.2.1/ipfabric/settings/attributes.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/authentication.py` & `ipfabric-6.2.1/ipfabric/settings/authentication.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/discovery.py` & `ipfabric-6.2.1/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/seeds.py` & `ipfabric-6.2.1/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/site_separation.py` & `ipfabric-6.2.1/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/user_mgmt.py` & `ipfabric-6.2.1/ipfabric/settings/user_mgmt.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/vendor_api.py` & `ipfabric-6.2.1/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.2.1/ipfabric/settings/vendor_api_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/configuration.py` & `ipfabric-6.2.1/ipfabric/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/discovery_history.py` & `ipfabric-6.2.1/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/dashboard.json` & `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/groups.json` & `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v4/4/intents.json` & `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v4/4/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/dashboard.json` & `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/groups.json` & `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v5/0/intents.json` & `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v5/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/dashboard.json` & `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/dashboard.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/groups.json` & `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/groups.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/factory_defaults/v6/0/intents.json` & `ipfabric-6.2.1/ipfabric/tools/factory_defaults/v6/0/intents.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/nist.py` & `ipfabric-6.2.1/ipfabric/tools/nist.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/restore_intents.py` & `ipfabric-6.2.1/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/shared.py` & `ipfabric-6.2.1/ipfabric/tools/shared.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.2.1/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.2.1/ipfabric/tools/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/LICENSE` & `ipfabric-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/pyproject.toml` & `ipfabric-6.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.2.0b4"
+version = "v6.2.1"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
```

### Comparing `ipfabric-6.2.0b4/README.md` & `ipfabric-6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.2.0b4/setup.py` & `ipfabric-6.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
               'openpyxl>=3.0.9,<4.0.0',
               'tabulate>=0.8.9,<0.10.0',
               'python-json-logger>=2.0.4,<3.0.0',
               'pyyaml>=6.0,<7.0']}
 
 setup_kwargs = {
     'name': 'ipfabric',
-    'version': '6.2.0b4',
+    'version': '6.2.1',
     'description': 'Python package for interacting with IP Fabric',
     'long_description': '# IP Fabric \n\nIPFabric is a Python module for connecting to and communicating against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation. \n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- Python 3.7 support will be removed.\n- The use of `token=\'<TOKEN>\'` or `username=\'<USER>\', password=\'<PASS>\'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth=\'TOKEN\')`\n  - User/Pass: `IPFClient(auth=(\'USER\', \'PASS\'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API\'s are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK\'s match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric\n```\n\n## Introduction\n\nPlease take a look at [API Programmability - Part 1: The Basics](https://ipfabric.io/blog/api-programmability-part-1/)\nfor instructions on creating an API token.\n\nMost of the methods and features can be located in [Examples](examples) to show how to use this package. \nAnother great introduction to this package can be found at [API Programmability - Part 2: Python](https://ipfabric.io/blog/api-programmability-python/)\n\n## Diagrams\n\nDiagramming in IP Fabric version v4.3 and above has been moved to it\'s own package.\n\nDiagramming will move back to this project in v7.0\n\n```\npip install ipfabric-diagrams\n```\n\n## Authentication\n### Username/Password\nSupply in client:\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=(\'user\', \'pass\'))\n```\n\n### Token\n```python\nfrom ipfabric import IPFClient\nipf = IPFClient(\'https://demo3.ipfabric.io/\', auth=\'token\')\n```\n\n### Environment \nThe easiest way to use this package is with a `.env` file.  You can copy the sample and edit it with your environment variables. \n\n```commandline\ncp sample.env .env\n```\n\nThis contains the following variables which can also be set as environment variables instead of a .env file.\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_TOKEN=TOKEN\nIPF_VERIFY=true\n```\n\nOr if using Username/Password:\n```\nIPF_URL="https://demo3.ipfabric.io"\nIPF_USERNAME=USER\nIPF_PASSWORD=PASS\n```\n\n## Development\n\n### Poetry Installation\n\nIPFabric uses [Poetry](https://pypi.org/project/poetry/) to make setting up a virtual environment with all dependencies\ninstalled quick and easy.\n\nInstall poetry globally:\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo run examples, install extras:\n```\npoetry install ipfabric -E examples\n```\n\n### Test and Build\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric\npoetry update\n```\n',
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric',
```

### Comparing `ipfabric-6.2.0b4/PKG-INFO` & `ipfabric-6.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.2.0b4
+Version: 6.2.1
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.7.1,<4.0.0
```

