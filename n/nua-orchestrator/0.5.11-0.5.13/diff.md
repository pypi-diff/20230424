# Comparing `tmp/nua_orchestrator-0.5.11.tar.gz` & `tmp/nua_orchestrator-0.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_orchestrator-0.5.11.tar", max compression
+gzip compressed data, was "nua_orchestrator-0.5.13.tar", max compression
```

## Comparing `nua_orchestrator-0.5.11.tar` & `nua_orchestrator-0.5.13.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     3468 2023-04-05 18:09:40.677146 nua_orchestrator-0.5.11/README.md
--rw-r--r--   0        0        0     2721 2023-04-18 16:55:14.980703 nua_orchestrator-0.5.11/pyproject.toml
--rw-r--r--   0        0        0      135 2023-02-01 13:54:28.100764 nua_orchestrator-0.5.11/src/nua/orchestrator/__init__.py
--rw-r--r--   0        0        0      118 2023-04-06 11:36:39.585136 nua_orchestrator-0.5.11/src/nua/orchestrator/__main__.py
--rw-r--r--   0        0        0     2132 2023-04-08 16:30:35.041481 nua_orchestrator-0.5.11/src/nua/orchestrator/admin_local.py
--rw-r--r--   0        0        0    42925 2023-04-17 13:48:52.412413 nua_orchestrator-0.5.11/src/nua/orchestrator/app_deployment.py
--rw-r--r--   0        0        0    12313 2023-04-11 14:23:48.025954 nua_orchestrator-0.5.11/src/nua/orchestrator/app_instance.py
--rw-r--r--   0        0        0     1639 2023-02-06 17:21:30.501023 nua_orchestrator-0.5.11/src/nua/orchestrator/app_management.py
--rw-r--r--   0        0        0        0 2023-01-25 13:12:45.648052 nua_orchestrator-0.5.11/src/nua/orchestrator/assign/__init__.py
--rw-r--r--   0        0        0      313 2023-04-16 08:40:02.375778 nua_orchestrator-0.5.11/src/nua/orchestrator/assign/db_utils.py
--rw-r--r--   0        0        0     3205 2023-04-04 11:21:10.875934 nua_orchestrator-0.5.11/src/nua/orchestrator/assign/engine.py
--rw-r--r--   0        0        0     6378 2023-04-16 15:02:45.960265 nua_orchestrator-0.5.11/src/nua/orchestrator/assign/evaluators.py
--rw-r--r--   0        0        0        0 2023-01-07 10:14:00.389172 nua_orchestrator-0.5.11/src/nua/orchestrator/backup/__init__.py
--rw-r--r--   0        0        0     1618 2023-01-25 16:15:09.490835 nua_orchestrator-0.5.11/src/nua/orchestrator/backup/backup_engine.py
--rw-r--r--   0        0        0      719 2023-04-08 16:18:44.073578 nua_orchestrator-0.5.11/src/nua/orchestrator/backup/backup_functions.py
--rw-r--r--   0        0        0      973 2023-04-08 16:18:44.073632 nua_orchestrator-0.5.11/src/nua/orchestrator/backup/backup_report.py
--rw-r--r--   0        0        0        0 2023-01-16 08:42:52.912983 nua_orchestrator-0.5.11/src/nua/orchestrator/bootstrap/__init__.py
--rw-r--r--   0        0        0     7146 2023-04-18 16:54:53.265819 nua_orchestrator-0.5.11/src/nua/orchestrator/bootstrap/bootstrap.py
--rw-r--r--   0        0        0      118 2023-01-08 08:57:33.879748 nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/__init__.py
--rw-r--r--   0        0        0     2546 2023-04-14 13:33:56.045209 nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/certbot.py
--rw-r--r--   0        0        0     4681 2023-04-17 17:50:04.647730 nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/commands.py
--rw-r--r--   0        0        0        0 2023-03-11 08:22:42.855026 nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/config/__init__.py
--rw-r--r--   0        0        0      403 2023-03-15 21:17:19.131952 nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/config/cli.ini
--rw-r--r--   0        0        0      774 2023-03-15 21:17:19.132102 nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf
--rw-r--r--   0        0        0     2533 2023-03-29 10:44:10.215539 nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/installer.py
--rw-r--r--   0        0        0        0 2023-01-08 21:09:12.167216 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0        0 2022-12-03 19:23:00.344340 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-10 14:02:02.204067 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/api.py
--rw-r--r--   0        0        0      286 2023-02-16 11:05:25.839048 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/backup.py
--rw-r--r--   0        0        0     1887 2023-04-14 13:33:56.045871 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/deploy_remove.py
--rw-r--r--   0        0        0     1387 2023-04-04 11:21:10.877158 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/restore.py
--rw-r--r--   0        0        0     1442 2023-04-11 14:23:48.026102 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/start_stop.py
--rw-r--r--   0        0        0     1416 2023-04-16 08:46:30.714375 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/status.py
--rw-r--r--   0        0        0     1404 2023-04-16 08:40:22.069040 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/configuration.py
--rw-r--r--   0        0        0     1308 2023-04-06 11:36:39.585561 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/debug.py
--rw-r--r--   0        0        0      798 2023-04-08 16:18:44.073946 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/init.py
--rw-r--r--   0        0        0     6483 2023-04-16 08:46:30.714460 nua_orchestrator-0.5.11/src/nua/orchestrator/cli/main.py
--rw-r--r--   0        0        0      267 2022-11-17 17:42:00.921923 nua_orchestrator-0.5.11/src/nua/orchestrator/config.py
--rw-r--r--   0        0        0      248 2022-11-17 17:42:00.922443 nua_orchestrator-0.5.11/src/nua/orchestrator/constants.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922490 nua_orchestrator-0.5.11/src/nua/orchestrator/db/__init__.py
--rw-r--r--   0        0        0      301 2023-01-06 12:47:38.582693 nua_orchestrator-0.5.11/src/nua/orchestrator/db/create.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922589 nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/__init__.py
--rw-r--r--   0        0        0     1707 2022-11-17 17:42:00.922655 nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/auth.py
--rw-r--r--   0        0        0       96 2022-11-17 17:42:00.922706 nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/base.py
--rw-r--r--   0        0        0     2073 2023-04-18 09:50:17.612727 nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/deployconfig.py
--rw-r--r--   0        0        0      856 2023-04-18 09:50:17.612881 nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/host.py
--rw-r--r--   0        0        0     1033 2023-04-18 09:50:17.613199 nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/image.py
--rw-r--r--   0        0        0     4153 2023-04-18 09:50:17.613726 nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/instance.py
--rw-r--r--   0        0        0     1602 2023-04-18 09:50:17.613874 nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/setting.py
--rw-r--r--   0        0        0      392 2023-01-25 13:12:45.649061 nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/user_count.py
--rw-r--r--   0        0        0      504 2023-01-06 12:47:38.583466 nua_orchestrator-0.5.11/src/nua/orchestrator/db/session.py
--rw-r--r--   0        0        0    16381 2023-04-12 10:07:58.740008 nua_orchestrator-0.5.11/src/nua/orchestrator/db/store.py
--rw-r--r--   0        0        0        0 2023-04-06 15:46:47.654975 nua_orchestrator-0.5.11/src/nua/orchestrator/db_migration/__init__.py
--rw-r--r--   0        0        0      211 2023-04-08 16:30:07.204201 nua_orchestrator-0.5.11/src/nua/orchestrator/db_migration/migrations.py
--rw-r--r--   0        0        0      724 2023-04-06 15:46:47.655336 nua_orchestrator-0.5.11/src/nua/orchestrator/db_migration/tools.py
--rw-r--r--   0        0        0        0 2023-01-31 10:30:37.322898 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/__init__.py
--rw-r--r--   0        0        0     1044 2023-02-02 12:51:27.404427 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/mariadb.json
--rw-r--r--   0        0        0     2250 2023-04-17 07:02:55.385046 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/mariadb.py
--rw-r--r--   0        0        0      160 2023-02-28 08:14:12.801866 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/mongo.json
--rw-r--r--   0        0        0     1438 2023-04-17 07:02:55.385309 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/mongo.py
--rw-r--r--   0        0        0      674 2023-02-02 12:51:27.404513 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/postgres.json
--rw-r--r--   0        0        0     1734 2023-04-17 07:02:55.385618 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/postgres.py
--rw-r--r--   0        0        0      414 2023-02-03 15:39:09.009427 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/redis-cache.json
--rw-r--r--   0        0        0     1146 2023-04-17 07:02:55.385868 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/redis-cache.py
--rw-r--r--   0        0        0     1399 2023-04-17 07:02:55.386092 nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-16 20:24:06.976924 nua_orchestrator-0.5.11/src/nua/orchestrator/db_utils/__init__.py
--rw-r--r--   0        0        0     7096 2023-04-16 20:26:03.674866 nua_orchestrator-0.5.11/src/nua/orchestrator/db_utils/mariadb_utils.py
--rw-r--r--   0        0        0     8152 2023-04-17 08:30:47.030493 nua_orchestrator-0.5.11/src/nua/orchestrator/db_utils/postgres_utils.py
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.403836 nua_orchestrator-0.5.11/src/nua/orchestrator/default_conf/__init__.py
--rw-r--r--   0        0        0     1689 2023-01-25 16:15:09.491276 nua_orchestrator-0.5.11/src/nua/orchestrator/default_conf/nua_defaults_settings.toml
--rw-r--r--   0        0        0    12028 2023-04-12 15:00:23.382828 nua_orchestrator-0.5.11/src/nua/orchestrator/deploy_utils.py
--rw-r--r--   0        0        0    18053 2023-04-14 13:29:17.687942 nua_orchestrator-0.5.11/src/nua/orchestrator/docker_utils.py
--rw-r--r--   0        0        0     1111 2023-04-08 16:18:44.074215 nua_orchestrator-0.5.11/src/nua/orchestrator/domain_split.py
--rw-r--r--   0        0        0     2596 2023-01-07 09:59:37.811449 nua_orchestrator-0.5.11/src/nua/orchestrator/healthcheck.py
--rw-r--r--   0        0        0     1444 2023-04-08 16:30:35.180413 nua_orchestrator-0.5.11/src/nua/orchestrator/higher_package.py
--rw-r--r--   0        0        0     1417 2023-04-08 16:30:35.183610 nua_orchestrator-0.5.11/src/nua/orchestrator/internal_secrets.py
--rw-r--r--   0        0        0        0 2023-01-11 17:21:08.504814 nua_orchestrator-0.5.11/src/nua/orchestrator/net_utils/__init__.py
--rw-r--r--   0        0        0      367 2023-04-08 16:30:07.252175 nua_orchestrator-0.5.11/src/nua/orchestrator/net_utils/external_ip.py
--rw-r--r--   0        0        0      407 2023-01-11 17:21:08.504884 nua_orchestrator-0.5.11/src/nua/orchestrator/net_utils/ports.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132385 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/__init__.py
--rw-r--r--   0        0        0     1633 2023-04-15 14:11:09.450734 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/cmd.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132886 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/html/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133023 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/html/css/__init__.py
--rw-r--r--   0        0        0     1410 2023-03-15 21:17:19.133148 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/html/css/style.css
--rw-r--r--   0        0        0      528 2023-03-15 21:17:19.133492 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/html/index.html
--rw-r--r--   0        0        0     2248 2023-04-15 14:11:09.451331 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/installer.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133754 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/__init__.py
--rw-r--r--   0        0        0      585 2023-03-15 21:17:19.134024 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/default_site
--rw-r--r--   0        0        0     1790 2023-03-15 21:17:19.134140 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/http_located.j2
--rw-r--r--   0        0        0     1427 2023-04-04 11:21:10.877419 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/http_not_located.j2
--rw-r--r--   0        0        0     2332 2023-03-15 21:17:19.134351 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/https_located.j2
--rw-r--r--   0        0        0     3553 2023-04-04 11:21:10.878037 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/https_not_located.j2
--rw-r--r--   0        0        0     2201 2023-04-04 11:21:10.878343 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2
--rw-r--r--   0        0        0     1115 2023-03-15 21:17:19.134715 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/nginx.conf
--rw-r--r--   0        0        0     4896 2023-04-15 14:11:09.452020 nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/utils.py
--rw-r--r--   0        0        0     4620 2023-04-05 05:50:21.473543 nua_orchestrator-0.5.11/src/nua/orchestrator/nua_db_setup.py
--rw-r--r--   0        0        0     1430 2023-04-08 16:30:35.213876 nua_orchestrator-0.5.11/src/nua/orchestrator/nua_env.py
--rw-r--r--   0        0        0     1078 2023-04-05 05:50:21.473685 nua_orchestrator-0.5.11/src/nua/orchestrator/persistent.py
--rw-r--r--   0        0        0     3860 2023-04-04 11:21:10.878990 nua_orchestrator-0.5.11/src/nua/orchestrator/port_normalization.py
--rw-r--r--   0        0        0     3367 2023-04-17 07:02:55.386411 nua_orchestrator-0.5.11/src/nua/orchestrator/register_plugins.py
--rw-r--r--   0        0        0     2848 2023-01-08 20:45:01.446656 nua_orchestrator-0.5.11/src/nua/orchestrator/registry.py
--rw-r--r--   0        0        0    15845 2023-04-08 16:30:35.246133 nua_orchestrator-0.5.11/src/nua/orchestrator/resource.py
--rw-r--r--   0        0        0     1737 2023-04-08 16:18:44.074313 nua_orchestrator-0.5.11/src/nua/orchestrator/resource_deps.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.924261 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/__init__.py
--rw-r--r--   0        0        0      307 2023-02-06 17:21:30.505291 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/deactivate_all_instances.py
--rw-r--r--   0        0        0      263 2023-01-19 17:57:22.674122 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/docker_list_all.py
--rw-r--r--   0        0        0     1211 2023-04-17 20:53:06.739901 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/docker_remove_all.py
--rw-r--r--   0        0        0      337 2023-04-06 15:46:47.655692 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/list_instances.py
--rw-r--r--   0        0        0      735 2023-04-17 08:29:13.917800 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/mariadb_restore.py
--rw-r--r--   0        0        0      614 2023-04-06 15:46:47.655840 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/print_instances.py
--rw-r--r--   0        0        0      319 2023-01-25 13:12:45.650893 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/print_mounted_volumes.py
--rw-r--r--   0        0        0      307 2023-01-25 13:12:45.650983 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/print_used_ports.py
--rw-r--r--   0        0        0      782 2023-04-17 08:29:27.370236 nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/set_pg_pwd.py
--rw-r--r--   0        0        0     3738 2023-02-08 17:48:17.607646 nua_orchestrator-0.5.11/src/nua/orchestrator/search_cmd.py
--rw-r--r--   0        0        0       59 2023-01-08 11:06:40.699794 nua_orchestrator-0.5.11/src/nua/orchestrator/services/__init__.py
--rw-r--r--   0        0        0      451 2023-04-16 21:08:39.554885 nua_orchestrator-0.5.11/src/nua/orchestrator/services/mariadb.py
--rw-r--r--   0        0        0      658 2023-04-16 21:08:39.554936 nua_orchestrator-0.5.11/src/nua/orchestrator/services/postgres.py
--rw-r--r--   0        0        0     1127 2023-01-30 14:35:45.686645 nua_orchestrator-0.5.11/src/nua/orchestrator/services/service_base.py
--rw-r--r--   0        0        0     1911 2023-02-08 11:40:48.305440 nua_orchestrator-0.5.11/src/nua/orchestrator/services/service_loader.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.925777 nua_orchestrator-0.5.11/src/nua/orchestrator/util/__init__.py
--rw-r--r--   0        0        0     1521 2023-04-08 16:18:44.074369 nua_orchestrator-0.5.11/src/nua/orchestrator/util/deep_access_dict.py
--rw-r--r--   0        0        0      397 2023-04-17 08:27:43.783766 nua_orchestrator-0.5.11/src/nua/orchestrator/util/deep_update.py
--rw-r--r--   0        0        0     3782 2023-04-08 16:30:35.277111 nua_orchestrator-0.5.11/src/nua/orchestrator/utils.py
--rw-r--r--   0        0        0       88 2022-11-17 17:42:00.925948 nua_orchestrator-0.5.11/src/nua/orchestrator/version.py
--rw-r--r--   0        0        0     6470 2023-04-08 16:18:44.074470 nua_orchestrator-0.5.11/src/nua/orchestrator/volume.py
--rw-r--r--   0        0        0     4477 1970-01-01 00:00:00.000000 nua_orchestrator-0.5.11/PKG-INFO
+-rw-r--r--   0        0        0     3789 2023-04-24 21:25:56.870296 nua_orchestrator-0.5.13/README.md
+-rw-r--r--   0        0        0     2721 2023-04-24 21:28:00.790633 nua_orchestrator-0.5.13/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-02-01 13:54:28.100764 nua_orchestrator-0.5.13/src/nua/orchestrator/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-06 11:36:39.585136 nua_orchestrator-0.5.13/src/nua/orchestrator/__main__.py
+-rw-r--r--   0        0        0     2132 2023-04-08 16:30:35.041481 nua_orchestrator-0.5.13/src/nua/orchestrator/admin_local.py
+-rw-r--r--   0        0        0    42885 2023-04-24 21:25:56.872804 nua_orchestrator-0.5.13/src/nua/orchestrator/app_deployment.py
+-rw-r--r--   0        0        0    12313 2023-04-11 14:23:48.025954 nua_orchestrator-0.5.13/src/nua/orchestrator/app_instance.py
+-rw-r--r--   0        0        0     1639 2023-02-06 17:21:30.501023 nua_orchestrator-0.5.13/src/nua/orchestrator/app_management.py
+-rw-r--r--   0        0        0        0 2023-01-25 13:12:45.648052 nua_orchestrator-0.5.13/src/nua/orchestrator/assign/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-16 08:40:02.375778 nua_orchestrator-0.5.13/src/nua/orchestrator/assign/db_utils.py
+-rw-r--r--   0        0        0     3205 2023-04-04 11:21:10.875934 nua_orchestrator-0.5.13/src/nua/orchestrator/assign/engine.py
+-rw-r--r--   0        0        0     6378 2023-04-16 15:02:45.960265 nua_orchestrator-0.5.13/src/nua/orchestrator/assign/evaluators.py
+-rw-r--r--   0        0        0        0 2023-01-07 10:14:00.389172 nua_orchestrator-0.5.13/src/nua/orchestrator/backup/__init__.py
+-rw-r--r--   0        0        0     1618 2023-01-25 16:15:09.490835 nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_engine.py
+-rw-r--r--   0        0        0      719 2023-04-08 16:18:44.073578 nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_functions.py
+-rw-r--r--   0        0        0      973 2023-04-08 16:18:44.073632 nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_report.py
+-rw-r--r--   0        0        0        0 2023-01-16 08:42:52.912983 nua_orchestrator-0.5.13/src/nua/orchestrator/bootstrap/__init__.py
+-rw-r--r--   0        0        0     7132 2023-04-24 21:25:56.873313 nua_orchestrator-0.5.13/src/nua/orchestrator/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0      118 2023-01-08 08:57:33.879748 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/__init__.py
+-rw-r--r--   0        0        0     2546 2023-04-21 16:49:16.834079 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/certbot.py
+-rw-r--r--   0        0        0     4666 2023-04-24 21:25:56.873579 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/commands.py
+-rw-r--r--   0        0        0        0 2023-03-11 08:22:42.855026 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/config/__init__.py
+-rw-r--r--   0        0        0      403 2023-03-15 21:17:19.131952 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/config/cli.ini
+-rw-r--r--   0        0        0      774 2023-03-15 21:17:19.132102 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf
+-rw-r--r--   0        0        0     2507 2023-04-24 21:25:56.873772 nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/installer.py
+-rw-r--r--   0        0        0        0 2023-01-08 21:09:12.167216 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-03 19:23:00.344340 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-10 14:02:02.204067 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/api.py
+-rw-r--r--   0        0        0      286 2023-02-16 11:05:25.839048 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/backup.py
+-rw-r--r--   0        0        0     1887 2023-04-14 13:33:56.045871 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/deploy_remove.py
+-rw-r--r--   0        0        0     1387 2023-04-04 11:21:10.877158 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/restore.py
+-rw-r--r--   0        0        0     1442 2023-04-11 14:23:48.026102 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/start_stop.py
+-rw-r--r--   0        0        0     1416 2023-04-16 08:46:30.714375 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/status.py
+-rw-r--r--   0        0        0     1404 2023-04-16 08:40:22.069040 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/configuration.py
+-rw-r--r--   0        0        0     1308 2023-04-06 11:36:39.585561 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/debug.py
+-rw-r--r--   0        0        0      798 2023-04-08 16:18:44.073946 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/init.py
+-rw-r--r--   0        0        0     6483 2023-04-16 08:46:30.714460 nua_orchestrator-0.5.13/src/nua/orchestrator/cli/main.py
+-rw-r--r--   0        0        0      267 2022-11-17 17:42:00.921923 nua_orchestrator-0.5.13/src/nua/orchestrator/config.py
+-rw-r--r--   0        0        0      248 2022-11-17 17:42:00.922443 nua_orchestrator-0.5.13/src/nua/orchestrator/constants.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922490 nua_orchestrator-0.5.13/src/nua/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0      301 2023-01-06 12:47:38.582693 nua_orchestrator-0.5.13/src/nua/orchestrator/db/create.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922589 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/__init__.py
+-rw-r--r--   0        0        0     1707 2022-11-17 17:42:00.922655 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/auth.py
+-rw-r--r--   0        0        0       96 2022-11-17 17:42:00.922706 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/base.py
+-rw-r--r--   0        0        0     2073 2023-04-18 09:50:17.612727 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/deployconfig.py
+-rw-r--r--   0        0        0      856 2023-04-18 09:50:17.612881 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/host.py
+-rw-r--r--   0        0        0     1033 2023-04-18 09:50:17.613199 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/image.py
+-rw-r--r--   0        0        0     4153 2023-04-18 09:50:17.613726 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/instance.py
+-rw-r--r--   0        0        0     1602 2023-04-18 09:50:17.613874 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/setting.py
+-rw-r--r--   0        0        0      392 2023-01-25 13:12:45.649061 nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/user_count.py
+-rw-r--r--   0        0        0      504 2023-01-06 12:47:38.583466 nua_orchestrator-0.5.13/src/nua/orchestrator/db/session.py
+-rw-r--r--   0        0        0    16381 2023-04-12 10:07:58.740008 nua_orchestrator-0.5.13/src/nua/orchestrator/db/store.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:46:47.654975 nua_orchestrator-0.5.13/src/nua/orchestrator/db_migration/__init__.py
+-rw-r--r--   0        0        0      211 2023-04-08 16:30:07.204201 nua_orchestrator-0.5.13/src/nua/orchestrator/db_migration/migrations.py
+-rw-r--r--   0        0        0      724 2023-04-06 15:46:47.655336 nua_orchestrator-0.5.13/src/nua/orchestrator/db_migration/tools.py
+-rw-r--r--   0        0        0        0 2023-01-31 10:30:37.322898 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/__init__.py
+-rw-r--r--   0        0        0     1044 2023-02-02 12:51:27.404427 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mariadb.json
+-rw-r--r--   0        0        0     2250 2023-04-17 07:02:55.385046 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mariadb.py
+-rw-r--r--   0        0        0      160 2023-02-28 08:14:12.801866 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mongo.json
+-rw-r--r--   0        0        0     1438 2023-04-17 07:02:55.385309 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mongo.py
+-rw-r--r--   0        0        0      674 2023-02-02 12:51:27.404513 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/postgres.json
+-rw-r--r--   0        0        0     1734 2023-04-17 07:02:55.385618 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/postgres.py
+-rw-r--r--   0        0        0      414 2023-02-03 15:39:09.009427 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/redis-cache.json
+-rw-r--r--   0        0        0     1146 2023-04-17 07:02:55.385868 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/redis-cache.py
+-rw-r--r--   0        0        0     1399 2023-04-17 07:02:55.386092 nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-16 20:24:06.976924 nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/__init__.py
+-rw-r--r--   0        0        0     7074 2023-04-24 21:25:56.874060 nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/mariadb_utils.py
+-rw-r--r--   0        0        0     8130 2023-04-24 21:25:56.874228 nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/postgres_utils.py
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.403836 nua_orchestrator-0.5.13/src/nua/orchestrator/default_conf/__init__.py
+-rw-r--r--   0        0        0     1689 2023-01-25 16:15:09.491276 nua_orchestrator-0.5.13/src/nua/orchestrator/default_conf/nua_defaults_settings.toml
+-rw-r--r--   0        0        0    12007 2023-04-24 21:25:56.874494 nua_orchestrator-0.5.13/src/nua/orchestrator/deploy_utils.py
+-rw-r--r--   0        0        0    18027 2023-04-24 21:25:56.874767 nua_orchestrator-0.5.13/src/nua/orchestrator/docker_utils.py
+-rw-r--r--   0        0        0     1111 2023-04-08 16:18:44.074215 nua_orchestrator-0.5.13/src/nua/orchestrator/domain_split.py
+-rw-r--r--   0        0        0     2596 2023-01-07 09:59:37.811449 nua_orchestrator-0.5.13/src/nua/orchestrator/healthcheck.py
+-rw-r--r--   0        0        0     1444 2023-04-08 16:30:35.180413 nua_orchestrator-0.5.13/src/nua/orchestrator/higher_package.py
+-rw-r--r--   0        0        0     1417 2023-04-08 16:30:35.183610 nua_orchestrator-0.5.13/src/nua/orchestrator/internal_secrets.py
+-rw-r--r--   0        0        0        0 2023-01-11 17:21:08.504814 nua_orchestrator-0.5.13/src/nua/orchestrator/net_utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-08 16:30:07.252175 nua_orchestrator-0.5.13/src/nua/orchestrator/net_utils/external_ip.py
+-rw-r--r--   0        0        0      407 2023-01-11 17:21:08.504884 nua_orchestrator-0.5.13/src/nua/orchestrator/net_utils/ports.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132385 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/__init__.py
+-rw-r--r--   0        0        0     1622 2023-04-24 21:25:56.874974 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/cmd.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132886 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133023 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/css/__init__.py
+-rw-r--r--   0        0        0     1410 2023-03-15 21:17:19.133148 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/css/style.css
+-rw-r--r--   0        0        0      528 2023-03-15 21:17:19.133492 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/index.html
+-rw-r--r--   0        0        0     2248 2023-04-15 14:11:09.451331 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/installer.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133754 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/__init__.py
+-rw-r--r--   0        0        0      585 2023-03-15 21:17:19.134024 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/default_site
+-rw-r--r--   0        0        0     1790 2023-03-15 21:17:19.134140 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/http_located.j2
+-rw-r--r--   0        0        0     1427 2023-04-04 11:21:10.877419 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/http_not_located.j2
+-rw-r--r--   0        0        0     2332 2023-03-15 21:17:19.134351 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_located.j2
+-rw-r--r--   0        0        0     3553 2023-04-04 11:21:10.878037 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_not_located.j2
+-rw-r--r--   0        0        0     2201 2023-04-04 11:21:10.878343 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2
+-rw-r--r--   0        0        0     1115 2023-03-15 21:17:19.134715 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/nginx.conf
+-rw-r--r--   0        0        0     4895 2023-04-24 21:25:56.875166 nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/utils.py
+-rw-r--r--   0        0        0     4620 2023-04-24 21:08:40.326542 nua_orchestrator-0.5.13/src/nua/orchestrator/nua_db_setup.py
+-rw-r--r--   0        0        0     1430 2023-04-08 16:30:35.213876 nua_orchestrator-0.5.13/src/nua/orchestrator/nua_env.py
+-rw-r--r--   0        0        0     1078 2023-04-05 05:50:21.473685 nua_orchestrator-0.5.13/src/nua/orchestrator/persistent.py
+-rw-r--r--   0        0        0     3860 2023-04-04 11:21:10.878990 nua_orchestrator-0.5.13/src/nua/orchestrator/port_normalization.py
+-rw-r--r--   0        0        0     3351 2023-04-24 21:25:56.875342 nua_orchestrator-0.5.13/src/nua/orchestrator/register_plugins.py
+-rw-r--r--   0        0        0     2848 2023-01-08 20:45:01.446656 nua_orchestrator-0.5.13/src/nua/orchestrator/registry.py
+-rw-r--r--   0        0        0    15807 2023-04-24 21:25:56.875604 nua_orchestrator-0.5.13/src/nua/orchestrator/resource.py
+-rw-r--r--   0        0        0     1737 2023-04-08 16:18:44.074313 nua_orchestrator-0.5.13/src/nua/orchestrator/resource_deps.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.924261 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/__init__.py
+-rw-r--r--   0        0        0      307 2023-02-06 17:21:30.505291 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/deactivate_all_instances.py
+-rw-r--r--   0        0        0      263 2023-01-19 17:57:22.674122 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/docker_list_all.py
+-rw-r--r--   0        0        0     1211 2023-04-17 20:53:06.739901 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/docker_remove_all.py
+-rw-r--r--   0        0        0      337 2023-04-06 15:46:47.655692 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/list_instances.py
+-rw-r--r--   0        0        0      735 2023-04-17 08:29:13.917800 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/mariadb_restore.py
+-rw-r--r--   0        0        0      614 2023-04-06 15:46:47.655840 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/print_instances.py
+-rw-r--r--   0        0        0      319 2023-01-25 13:12:45.650893 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/print_mounted_volumes.py
+-rw-r--r--   0        0        0      307 2023-01-25 13:12:45.650983 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/print_used_ports.py
+-rw-r--r--   0        0        0      782 2023-04-17 08:29:27.370236 nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/set_pg_pwd.py
+-rw-r--r--   0        0        0     3738 2023-02-08 17:48:17.607646 nua_orchestrator-0.5.13/src/nua/orchestrator/search_cmd.py
+-rw-r--r--   0        0        0       59 2023-01-08 11:06:40.699794 nua_orchestrator-0.5.13/src/nua/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0      451 2023-04-16 21:08:39.554885 nua_orchestrator-0.5.13/src/nua/orchestrator/services/mariadb.py
+-rw-r--r--   0        0        0      658 2023-04-16 21:08:39.554936 nua_orchestrator-0.5.13/src/nua/orchestrator/services/postgres.py
+-rw-r--r--   0        0        0     1127 2023-01-30 14:35:45.686645 nua_orchestrator-0.5.13/src/nua/orchestrator/services/service_base.py
+-rw-r--r--   0        0        0     1911 2023-02-08 11:40:48.305440 nua_orchestrator-0.5.13/src/nua/orchestrator/services/service_loader.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.925777 nua_orchestrator-0.5.13/src/nua/orchestrator/util/__init__.py
+-rw-r--r--   0        0        0     1521 2023-04-08 16:18:44.074369 nua_orchestrator-0.5.13/src/nua/orchestrator/util/deep_access_dict.py
+-rw-r--r--   0        0        0      397 2023-04-17 08:27:43.783766 nua_orchestrator-0.5.13/src/nua/orchestrator/util/deep_update.py
+-rw-r--r--   0        0        0     3782 2023-04-08 16:30:35.277111 nua_orchestrator-0.5.13/src/nua/orchestrator/utils.py
+-rw-r--r--   0        0        0       88 2022-11-17 17:42:00.925948 nua_orchestrator-0.5.13/src/nua/orchestrator/version.py
+-rw-r--r--   0        0        0     6470 2023-04-08 16:18:44.074470 nua_orchestrator-0.5.13/src/nua/orchestrator/volume.py
+-rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 nua_orchestrator-0.5.13/PKG-INFO
```

### Comparing `nua_orchestrator-0.5.11/README.md` & `nua_orchestrator-0.5.13/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Nua orchestrator
 
+[Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
+
+This packaged is deployed on the Nua server.
+
+For end-users, the main entry point is the `nua` command line tool (see: [Nua on PyPI](https://pypi.org/project/nua/) or [nua-cli on GitHub](https://github.com/abilian/nua/tree/main/nua-cli)).
+
+
 ## Role of the orchestrator
 
 The orchestrator is in charge of configuring application and resources and deploying them on the host.
 
 ## Requirements
 
 The host must be a linux server installed with the distribution:
@@ -23,57 +30,65 @@
 
 The following Python packages (provided by Ubuntu) are required:
 
 - `python3.10`
 - `python3.10-venv`
 - `python3.10-dev`
 - `python3-pip`
+- `pipx`
 
-i.e. you should run `apt-get install python3.10 python3.10-venv python3.10-dev python3-pip` before installing Nua.
+i.e. you should run `apt-get install python3.10 python3.10-venv python3.10-dev python3-pip pipx` before installing Nua.
 
 Note: this is temporary, the installation script will take care of this kind of details later.
 
 
 ## Installation
 
-### The bootstrap command
+### All-in-one command
+
+Simply run:
+
+```console
+curl -L https://nua.rocks/install.py | sudo python3
+```
+
+### Using the `nua-bootstrap` command
 
-To install, you will need to use the bootstrapping script: `nua-bootstrap`.
+The `nua-orchestrator` package provides a `nua-bootstrap` command which will install Nua on the host.
+
+#### Installation procedure (from released version)
+
+From the root account:
+
+```console
+pipx install nua-orchestrator
+nua-bootstrap
+```
+
+#### Installation procedure (from git)
 
 At the moment, this implies a first temporary installation of Nua (which can be done in a temporary directory), from a sudo-able account:
 
 ```console
-git clone https://github.com/abilian/nua
-cd nua/nua-orchestrator
+git clone https://github.com/abilian/nua src
+cd src/nua-orchestrator
 ./install.py
 sudo ./env/bin/nua-bootstrap
 ```
 
 That command will do many things:
 
 - create the `nua` account
 - install the required packages (Docker, postgres, Nginx, ...)
 - apply default configuration to the host
 - ...
 
 ### Remarks
 
 - `nua-bootstrap` can be safely launched on an existing configuration,
-- `nua-bootstrap` must be launched as root, if not, a warning is displayed:
-
-```console
-$ nua-bootstrap
-Installing Nua bootstrap on local host.
-Warning: Nua was already installed.
-Nua bootstrap script requires root privileges.
-Please try again, this time using 'sudo'.
-- When sudo, use absolute script path.
-- Possible command:
-    sudo /home/nua/env/bin/nua-bootstrap
-```
 
 ### Installation phases
 
 Installation can take several minutes, here an excerpt of main messages displayed during installation:
 
 ```console
 sudo /home/nua/env/bin/nua-bootstrap
```

### Comparing `nua_orchestrator-0.5.11/pyproject.toml` & `nua_orchestrator-0.5.13/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-orchestrator"
-version = "0.5.11"
+version = "0.5.13"
 description = "Nua orchestrator - local implementation"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -28,18 +28,18 @@
 nua-deactivate-all = "nua.orchestrator.scripts.deactivate_all_instances:main"
 nua-docker-list-all = "nua.orchestrator.scripts.docker_list_all:main"
 nua-docker-rm-all = "nua.orchestrator.scripts.docker_remove_all:main"
 nua_test_services = "nua.orchestrator.service:test"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nua-lib = "=0.5.11"
-nua-agent = "=0.5.11"
-nua-build = "=0.5.11"
-nua-autobuild = "=0.5.11"
+nua-lib = "=0.5.13"
+nua-agent = "=0.5.13"
+nua-build = "=0.5.13"
+nua-autobuild = "=0.5.13"
 SQLAlchemy-serializer = "^1.4.1"
 SQLAlchemy = "^1.4.36"
 psycopg2-binary = "^2.9.3"
 setuptools = "*"
 wheel = "*"
 tomli = "^2"
 paramiko = "^2.11.0"
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/admin_local.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/admin_local.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/app_deployment.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/app_deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 from pathlib import Path
 from pprint import pformat
 from typing import Any
 
 from nua.lib.console import print_green, print_red
 from nua.lib.panic import (
     Abort,
+    bold_debug,
+    debug,
+    important,
     info,
     show,
     vprint,
-    vprint_green,
-    vprint_magenta,
     warning,
 )
 from nua.lib.tool.state import verbosity
 
 from . import config
 from .app_instance import AppInstance
 from .assign.engine import instance_key_evaluator
@@ -166,15 +167,15 @@
         # See later
         return
         # assuming nua_db_setup was run at initialization of the command
         services = Services()
         services.load()
         self.available_services = services.loaded
         with verbosity(2):
-            vprint_magenta(
+            bold_debug(
                 f"Available local services: {pformat(list(services.loaded.keys()))}"
             )
 
     def load_deploy_config(self, deploy_config: str):
         config_path = Path(deploy_config).expanduser().resolve()
         with verbosity(1):
             info(f"Deploy apps from: {config_path}")
@@ -319,16 +320,16 @@
         """Apply configuration to Nginx, especially configurations that can not be
         deployed before all previous apps are stopped."""
         self.configure_nginx()
         # registering https apps with certbot requires that the base nginx config is
         # deployed.
         register_certbot_domains(self.apps)
         with verbosity(3):
-            vprint_green("AppDeployment .apps:")
-            vprint_magenta(pformat(self.apps))
+            bold_debug("AppDeployment .apps:")
+            debug(pformat(self.apps))
 
     def merge_nginx_configuration(self):
         """Apply configuration to Nginx, when apps are already deployed."""
         if not self.already_deployed_domains:
             # easy, either first deployment or all apps removed, start from zero:
             return self.apply_nginx_configuration()
         for host in self.apps_per_domain:
@@ -343,16 +344,16 @@
             with verbosity(1):
                 info(f"Configure Nginx for domain '{hostname}'")
             configure_nginx_hostname(host)
         # registering https apps with certbot requires that the base nginx config is
         # deployed.
         register_certbot_domains(self.apps)
         with verbosity(3):
-            vprint_green("AppDeployment .apps:")
-            vprint_magenta(self.apps)
+            bold_debug("AppDeployment .apps:")
+            debug(self.apps)
 
     def remove_nginx_configuration(self, stop_domain: str):
         """Remove apps from the nginx configuration.
 
         To stop nginx redirection before actually stopping the apps.
         """
         with verbosity(1):
@@ -900,15 +901,15 @@
         # volumes need to be mounted before beeing passed as arguments to
         # docker.run()
         mounted_volumes = mount_resource_volumes(site)
         start_one_container(site, mounted_volumes)
 
     def store_container_instance(self, site: AppInstance):
         with verbosity(3):
-            vprint_green("Saving AppInstance configuration in Nua DB")
+            bold_debug("Saving AppInstance configuration in Nua DB")
         store.store_instance(
             app_id=site.app_id,
             nua_tag=site.nua_tag,
             domain=site.domain,
             container=site.container_name,
             image=site.image,
             state=site.running_status,
@@ -1022,25 +1023,25 @@
             self.display_persistent_data(site)
         print()
 
     def display_persistent_data(self, site: AppInstance):
         with verbosity(3):
             content = site.persistent_full_dict()
             if content:
-                vprint_green("Persistent generated variables:")
-                vprint(pformat(content))
+                bold_debug("Persistent generated variables:")
+                debug(pformat(content))
 
     def display_used_volumes(self):
         with verbosity(1):
             current_mounted = store.list_instances_container_active_volumes()
             if not current_mounted:
                 return
-            vprint_green("Volumes used by current Nua configuration:")
+            important("Volumes used by current Nua configuration:")
             for volume in current_mounted:
-                vprint_magenta(Volume.string(volume))
+                show(Volume.string(volume))
 
     def display_unused_volumes(self):
         with verbosity(1):
             unused = unused_volumes(self.orig_mounted_volumes)
             if not unused:
                 return
             print_green(
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/app_instance.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/app_instance.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/app_management.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/app_management.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/assign/engine.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/assign/engine.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/assign/evaluators.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/assign/evaluators.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/backup/backup_engine.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_engine.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/backup/backup_functions.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_functions.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/backup/backup_report.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/backup/backup_report.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/bootstrap/bootstrap.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/bootstrap/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 def bootstrap_install_mariadb_or_fail():
     if not bootstrap_install_mariadb() or not set_random_mariadb_pwd():
         raise Abort("Can't initialize Mariadb.")
 
 
 def install_packages():
     print_blue("Installing base packages...")
-    install_package_list(HOST_PACKAGES, update=False, clean=False, keep_lists=True)
+    install_package_list(HOST_PACKAGES, clean=False, keep_lists=True)
 
 
 def create_nua_user():
     if not user_exists(NUA):
         print_blue("Creating user 'nua'...")
         cmd = "useradd --inactive -1 -G docker -m -s /bin/bash -U nua"
         # cmd = "useradd --inactive -1 -G sudo,docker -m -s /bin/bash -U nua"
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/certbot.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/certbot.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/commands.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     - NUA_CERTBOT_VERBOSE: show certbot log
     - NUA_CERTBOT_TEST: use certbot test environment (only for tests)
 """
 
 import os
 from pathlib import Path
 
-from nua.lib.panic import show, vprint, vprint_magenta
+from nua.lib.panic import important, show, vprint
 from nua.lib.shell import sh
 from nua.lib.tool.state import verbosity
 
 from nua.orchestrator import config
 
 from ..nginx.cmd import nginx_is_active, nginx_restart, nginx_stop
 from ..nua_env import certbot_exe, nua_home_path
@@ -62,15 +62,15 @@
     run_args.append(email)
     run_args.append(f"-d {domain}")
     return " ".join(run_args)
 
 
 def apply_none_strategy(_top_domain: str, domains: list[str]):
     with verbosity(1):
-        vprint_magenta(f"Use HTTP protocol for: {' '.join(domains)}")
+        important(f"Use HTTP protocol for: {' '.join(domains)}")
     return
 
 
 def cert_exists(domain: str) -> bool:
     path = letsencrypt_path() / "live" / domain
     if os.getuid():  # aka not root
         cmd = f"sudo test -d {path} && echo ok || echo ko"
@@ -132,15 +132,15 @@
     - implementation mode "auto":
         - let certbot rewrite redirections,
         - let certbot manage cron,
         - apply "auto" rules and parameters.
     """
     sorted_domains = sorted(domains)
     with verbosity(1):
-        vprint_magenta(f"Use HTTPS protocol (Certbot) for: {' '.join(sorted_domains)}")
+        important(f"Use HTTPS protocol (Certbot) for: {' '.join(sorted_domains)}")
     # cmd = certbot_run(top_domain, domains)
     # cmd = certbot_certonly(top_domain, domains)
     #
     # If all domain are already known from letsencrypt, we may try a direct
     # reload using nginx (so without killing nginx websites)
     # Else, we need to stop nginx and use the standalone procedure.
     if nginx_is_active() and all(cert_exists(domain) for domain in sorted_domains):
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf` & `nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/certbot/installer.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/certbot/installer.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 def _generate_dhparam() -> None:
     pem_file = nua_home_path() / "letsencrypt" / "ssl-dhparams.pem"
     if pem_file.is_file() and pem_file.stat().st_size > 0:
         print_magenta(
             "Existing file 'ssl-dhparams.pem' will be used, no dhparam generation."
         )
         return
-    print_magenta("Generating Certbot dhparam (duration: more than 10 minutes...)")
-    cmd = f"openssl dhparam -out {pem_file} 4096"
+    print_magenta("Generating Certbot dhparam")
+    cmd = f"openssl dhparam -dsaparam -out {pem_file} 4096"
     if os.getuid():  # aka not root
         cmd = f"sudo {cmd}"
     output = sh(cmd, timeout=3600, show_cmd=True, capture_output=True)
     print(output)
 
 
 def _set_cron() -> None:
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/api.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/api.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/deploy_remove.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/deploy_remove.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/restore.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/restore.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/start_stop.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/start_stop.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/cli/commands/status.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/cli/configuration.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/cli/debug.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/debug.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/cli/init.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/init.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/cli/main.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/auth.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/auth.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/deployconfig.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/deployconfig.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/host.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/host.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/image.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/image.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/instance.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/instance.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db/model/setting.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db/model/setting.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db/store.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db/store.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_migration/tools.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_migration/tools.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/mariadb.json` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mariadb.json`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/mariadb.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mariadb.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/mongo.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/mongo.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/postgres.json` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/postgres.json`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/postgres.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/postgres.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/redis-cache.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/redis-cache.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_plugins/sqlite.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_plugins/sqlite.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_utils/mariadb_utils.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/mariadb_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,14 @@
     install_package_list(
         [
             f"mariadb-server-{MARIADB_VERSION}",
             "libmariadb3",
             "libmariadb-dev",
             # "mariadb-client",
         ],
-        update=False,
         clean=False,
         keep_lists=True,
     )
     allow_docker_connection()
     return mariadb_check_installed()
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/db_utils/postgres_utils.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/db_utils/postgres_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
     """
     print_magenta(f"Installation of postgres version {PG_VERSION}")
     # detect prior installation of other versions:
     if not _pg_verify_no_prior_installation():
         return False
     install_package_list(
         [f"postgresql-{PG_VERSION}", "libpq-dev"],
-        update=False,
         clean=False,
         keep_lists=True,
     )
     allow_docker_connection()
     return pg_check_installed()
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/default_conf/nua_defaults_settings.toml` & `nua_orchestrator-0.5.13/src/nua/orchestrator/default_conf/nua_defaults_settings.toml`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/deploy_utils.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/deploy_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from pprint import pformat
 
 import docker
 import docker.types
 from nua.autobuild.docker_build_utils import display_one_docker_img, docker_require
 from nua.build.archive_search import ArchiveSearch
-from nua.lib.panic import Abort, info, vprint, vprint_blue, vprint_green, warning
+from nua.lib.panic import Abort, important, info, vprint, warning
 from nua.lib.tool.state import verbosity
 
 from .app_instance import AppInstance
 from .db import store
 from .docker_utils import (  # docker_volume_prune,
     docker_host_gateway_ip,
     docker_network_create_bridge,
@@ -54,27 +54,27 @@
         raise Abort(
             f"image non compatible Nua: {path}.", explanation="No Nua config found"
         )
 
     metadata = image_nua_config["metadata"]
     msg = "Installing App: {id} {version}, {title}".format(**metadata)
     if verbosity(0):
-        vprint_blue(msg)
+        important(msg)
 
     client = docker.from_env()
     # images_before = {img.id for img in client.images.list()}
     with open(path, "rb") as input:  # noqa: S108
         loaded = client.images.load(input)
     if not loaded or len(loaded) > 1:
         warning("loaded image result is strange:", f"{loaded=}")
     loaded_img = loaded[0]
     # images_after = {img.id for img in client.images.list()}
     # new = images_after - images_before
     with verbosity(1):
-        vprint_green("Installing image:")
+        important("Installing image:")
         display_one_docker_img(loaded_img)
     return loaded_img.id, image_nua_config
 
 
 def port_allocator(start_ports: int, end_ports: int, allocated_ports: set) -> Callable:
     def allocator() -> int:
         # O(n2), but very few ports to configure
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/docker_utils.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/docker_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from docker import DockerClient
 from docker.errors import APIError, NotFound
 from docker.models.containers import Container
 from docker.models.images import Image
 from nua.autobuild.docker_build_utils import docker_require
 from nua.lib.console import print_red
-from nua.lib.panic import Abort, info, vprint, vprint_green, vprint_magenta, warning
+from nua.lib.panic import Abort, important, info, show, vprint, warning
 from nua.lib.shell import chmod_r, mkdir_p
 from nua.lib.tool.state import verbosity
 
 from . import config
 from .db import store
 from .resource import Resource
 from .volume import Volume
@@ -298,16 +298,16 @@
     """
     params = docker_run_params(rsite)
     with verbosity(1):
         # info(f"Docker run image: {rsite.image_id}")
         info(f"Docker run image: {rsite.image}")
         info(f"        image id: {rsite.image_id_short}")
         with verbosity(2):
-            vprint_green("Docker run parameters:")
-            vprint_magenta(pformat(params))
+            important("Docker run parameters:")
+            show(pformat(params))
 
     docker_remove_prior_container_live(rsite)
     with verbosity(2):
         if "network" in params:
             info("Network:", params["network"])
 
     container = _docker_run(rsite, secrets, params)
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/domain_split.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/domain_split.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/healthcheck.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/healthcheck.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/higher_package.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/higher_package.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/internal_secrets.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/internal_secrets.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/cmd.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/cmd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Nginx utils to install nginx config and adapt with app using nginx."""
 import os
 from time import sleep
 
-from nua.lib.panic import show, vprint, vprint_green
+from nua.lib.panic import debug, important, show
 from nua.lib.shell import sh
 from nua.lib.tool.state import verbosity
 
 from .. import config
 
 
 def nginx_is_active() -> bool:
@@ -25,37 +25,37 @@
         cmd = stop_cmd
     else:
         cmd = f"sudo {stop_cmd}"
     with verbosity(2):
         show(cmd)
     output = sh(cmd, show_cmd=False, capture_output=True)
     with verbosity(3):
-        vprint(output)
+        debug(output)
     sleep(1)
 
 
 def nginx_restart():
     # assuming some recent ubuntu distribution:
     delay = config.read("host", "nginx_wait_after_restart") or 1
     with verbosity(2):
-        vprint_green("Restart Nginx")
+        important("Restart Nginx")
     cmd = "systemctl restart nginx"
     if os.geteuid() == 0:
         sh(cmd, show_cmd=False)
     else:
         sh(f"sudo {cmd}", show_cmd=False)
     sleep(delay)
 
 
 def nginx_reload():
     # assuming some recent ubuntu distribution:
     if not nginx_is_active():
         return nginx_restart()
     delay = config.read("host", "nginx_wait_after_restart") or 1
     with verbosity(2):
-        vprint_green("Reload Nginx")
+        important("Reload Nginx")
     cmd = "systemctl reload nginx"
     if os.geteuid() == 0:
         sh(cmd, show_cmd=False)
     else:
         sh(f"sudo {cmd}", show_cmd=False)
     sleep(delay)
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/html/css/style.css` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/css/style.css`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/html/index.html` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/html/index.html`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/installer.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/installer.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/default_site` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/default_site`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/http_located.j2` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/http_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/http_not_located.j2` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/http_not_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/https_located.j2` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/https_not_located.j2` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_not_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/templates/nginx.conf` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nginx/utils.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nginx/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Nginx utils to install nginx config and adapt with app using nginx."""
 import os
 from importlib import resources as rso
 from pathlib import Path
 from pprint import pformat
 
 from nua.lib.actions import jinja2_render_from_str_template
-from nua.lib.panic import info, vprint, vprint_magenta, warning
+from nua.lib.panic import bold_debug, debug, info, warning
 from nua.lib.shell import chown_r, mkdir_p, rm_fr
 from nua.lib.tool.state import verbosity
 
 from .. import nua_env
 from ..certbot.certbot import use_https
 
 CONF_TEMPLATE = "nua.orchestrator.nginx.templates"
@@ -100,16 +100,16 @@
                                   'protocol': 'tcp',
                                   'proxy': 'auto',
                                   'ssl': True}],
 
                    ...
     """
     with verbosity(4):
-        vprint("configure_nginx_hostname: host")
-        vprint(pformat(host))
+        bold_debug("configure_nginx_hostname: host")
+        debug(pformat(host))
     _set_instances_proxy_auto_port(host)
     _set_located_port_list(host)
     nua_nginx_path = nua_env.nginx_path()
     template = read_nginx_template(host)
     dest_path = nua_nginx_path / "sites" / host["hostname"]
     if "host_use" in host["apps"][0]:
         _actual_configure_nginx_hostname(template, dest_path, host)
@@ -120,37 +120,37 @@
 
 def remove_nginx_configuration_hostname(stop_domain: str):
     """Remove configuration for dommain.
 
     warning: only for user 'nua' or 'root'
     """
     with verbosity(4):
-        vprint("remove_nginx_configuration_hostname:")
-        vprint(stop_domain)
+        bold_debug("remove_nginx_configuration_hostname:")
+        debug(stop_domain)
     nua_nginx_path = nua_env.nginx_path()
     dest_path = nua_nginx_path / "sites" / stop_domain
     dest_path.unlink(missing_ok=True)
 
 
 def _actual_configure_nginx_hostname(
     template: str,
     dest_path: str | Path,
     host: dict,
 ):
     with verbosity(4):
-        vprint_magenta(f"{host['hostname']} template:")
-        vprint(template)
+        bold_debug(f"{host['hostname']} template:")
+        debug(template)
     with verbosity(2):
         info("Nginx configuration:", dest_path)
     jinja2_render_from_str_template(template, dest_path, host)
     if dest_path.exists():
         with verbosity(3):
-            vprint("Nginx configuration content:")
+            bold_debug("Nginx configuration content:")
             with open(dest_path, encoding="utf8") as rfile:
-                vprint(rfile.read())
+                debug(rfile.read())
     else:
         warning(f"host '{host['hostname']}', Nginx configuration not created")
     os.chmod(dest_path, 0o644)
 
 
 def chown_r_nua_nginx():
     if not os.getuid():
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nua_db_setup.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nua_db_setup.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/nua_env.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/nua_env.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/persistent.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/persistent.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/port_normalization.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/port_normalization.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/register_plugins.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/register_plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import importlib.util
 from collections.abc import Callable
 from importlib import resources as rso
 from pathlib import Path
 from pprint import pformat
 
 from nua.agent.nua_config import hyphen_get
-from nua.lib.panic import vprint, vprint_magenta
+from nua.lib.panic import bold_debug, debug
 from nua.lib.tool.state import verbosity
 
 from .utils import dehyphen, hyphen
 
 LOADED_MODULES = {}
 MODULES_PROPERTIES = {}
 DOCKER_MODULES = set()
@@ -34,22 +34,22 @@
                 continue
             load_module(path.stem, dir)
     with verbosity(3):
         _show_plugin_info()
 
 
 def _show_plugin_info():
-    vprint_magenta("plugins registered:")
-    vprint("PLUGIN_DIRS:", pformat(PLUGIN_DIRS))
-    vprint("LOADED_MODULES:", pformat(LOADED_MODULES))
-    vprint("DOCKER_MODULES:", pformat(DOCKER_MODULES))
-    vprint("ASSIGN_MODULES:", pformat(ASSIGN_MODULES))
-    vprint("NETWORK_MODULES:", pformat(NETWORK_MODULES))
-    vprint("FAMILIES:", pformat(FAMILIES))
-    vprint("FAMILY_SET:", pformat(FAMILY_SET))
+    bold_debug("plugins registered:")
+    debug("PLUGIN_DIRS:", pformat(PLUGIN_DIRS))
+    debug("LOADED_MODULES:", pformat(LOADED_MODULES))
+    debug("DOCKER_MODULES:", pformat(DOCKER_MODULES))
+    debug("ASSIGN_MODULES:", pformat(ASSIGN_MODULES))
+    debug("NETWORK_MODULES:", pformat(NETWORK_MODULES))
+    debug("FAMILIES:", pformat(FAMILIES))
+    debug("FAMILY_SET:", pformat(FAMILY_SET))
 
 
 def load_module(name: str, plugin_dir: str):
     spec = importlib.util.find_spec(f".{name}", plugin_dir)
     if not spec:
         return
     module = spec.loader.load_module()
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/registry.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/registry.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/resource.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections.abc import Callable
 from copy import deepcopy
 from pprint import pformat
 from typing import Any
 
 from nua.agent.nua_config import nomalize_env_values
-from nua.lib.panic import Abort, vprint, vprint_green, warning
+from nua.lib.panic import Abort, debug, important, vprint, warning
 from nua.lib.tool.state import verbosity
 
 from .backup.backup_engine import backup_resource, backup_volume
 from .backup.backup_report import global_backup_report
 from .healthcheck import HealthCheck
 from .port_normalization import (
     normalize_ports_list,
@@ -481,19 +481,17 @@
                 vprint(f"not a DB: {self.type}")
             return
         if configure_fct := load_plugin_function(self.type, "configure_db"):
             with verbosity(4):
                 vprint(f"configure_fct: {configure_fct}")
             configure_fct(self)
             with verbosity(2):
-                vprint_green(
-                    f"Configure resource DB '{self.resource_name}': {self.type}"
-                )
+                important(f"Configure resource DB '{self.resource_name}': {self.type}")
             with verbosity(3):
-                vprint(pformat(self))
+                debug(pformat(self))
 
     def load_meta_packages_requirements(self):
         """Some plugin may require some meta-packages requirements for main
         app.
 
         For example : postgres DB-> postgres-client -> psycopg2
         (for future use)
```

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/resource_deps.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/resource_deps.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/docker_remove_all.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/docker_remove_all.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/mariadb_restore.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/mariadb_restore.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/print_instances.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/print_instances.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/scripts/set_pg_pwd.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/scripts/set_pg_pwd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/search_cmd.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/search_cmd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/services/postgres.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/services/postgres.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/services/service_base.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/services/service_base.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/services/service_loader.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/services/service_loader.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/util/deep_access_dict.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/util/deep_access_dict.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/utils.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/src/nua/orchestrator/volume.py` & `nua_orchestrator-0.5.13/src/nua/orchestrator/volume.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.11/PKG-INFO` & `nua_orchestrator-0.5.13/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 Metadata-Version: 2.1
 Name: nua-orchestrator
-Version: 0.5.11
+Version: 0.5.13
 Summary: Nua orchestrator - local implementation
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=1.4.36,<2.0.0)
 Requires-Dist: SQLAlchemy-serializer (>=1.4.1,<2.0.0)
 Requires-Dist: docker (>=6,<7)
-Requires-Dist: nua-agent (==0.5.11)
-Requires-Dist: nua-autobuild (==0.5.11)
-Requires-Dist: nua-build (==0.5.11)
-Requires-Dist: nua-lib (==0.5.11)
+Requires-Dist: nua-agent (==0.5.13)
+Requires-Dist: nua-autobuild (==0.5.13)
+Requires-Dist: nua-build (==0.5.13)
+Requires-Dist: nua-lib (==0.5.13)
 Requires-Dist: paramiko (>=2.11.0,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21,<0.22)
 Requires-Dist: pyyaml (>=6,<7)
 Requires-Dist: setuptools
 Requires-Dist: tomli (>=2,<3)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: wheel
 Description-Content-Type: text/markdown
 
 # Nua orchestrator
 
+[Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
+
+This packaged is deployed on the Nua server.
+
+For end-users, the main entry point is the `nua` command line tool (see: [Nua on PyPI](https://pypi.org/project/nua/) or [nua-cli on GitHub](https://github.com/abilian/nua/tree/main/nua-cli)).
+
+
 ## Role of the orchestrator
 
 The orchestrator is in charge of configuring application and resources and deploying them on the host.
 
 ## Requirements
 
 The host must be a linux server installed with the distribution:
@@ -52,57 +59,65 @@
 
 The following Python packages (provided by Ubuntu) are required:
 
 - `python3.10`
 - `python3.10-venv`
 - `python3.10-dev`
 - `python3-pip`
+- `pipx`
 
-i.e. you should run `apt-get install python3.10 python3.10-venv python3.10-dev python3-pip` before installing Nua.
+i.e. you should run `apt-get install python3.10 python3.10-venv python3.10-dev python3-pip pipx` before installing Nua.
 
 Note: this is temporary, the installation script will take care of this kind of details later.
 
 
 ## Installation
 
-### The bootstrap command
+### All-in-one command
+
+Simply run:
+
+```console
+curl -L https://nua.rocks/install.py | sudo python3
+```
+
+### Using the `nua-bootstrap` command
 
-To install, you will need to use the bootstrapping script: `nua-bootstrap`.
+The `nua-orchestrator` package provides a `nua-bootstrap` command which will install Nua on the host.
+
+#### Installation procedure (from released version)
+
+From the root account:
+
+```console
+pipx install nua-orchestrator
+nua-bootstrap
+```
+
+#### Installation procedure (from git)
 
 At the moment, this implies a first temporary installation of Nua (which can be done in a temporary directory), from a sudo-able account:
 
 ```console
-git clone https://github.com/abilian/nua
-cd nua/nua-orchestrator
+git clone https://github.com/abilian/nua src
+cd src/nua-orchestrator
 ./install.py
 sudo ./env/bin/nua-bootstrap
 ```
 
 That command will do many things:
 
 - create the `nua` account
 - install the required packages (Docker, postgres, Nginx, ...)
 - apply default configuration to the host
 - ...
 
 ### Remarks
 
 - `nua-bootstrap` can be safely launched on an existing configuration,
-- `nua-bootstrap` must be launched as root, if not, a warning is displayed:
-
-```console
-$ nua-bootstrap
-Installing Nua bootstrap on local host.
-Warning: Nua was already installed.
-Nua bootstrap script requires root privileges.
-Please try again, this time using 'sudo'.
-- When sudo, use absolute script path.
-- Possible command:
-    sudo /home/nua/env/bin/nua-bootstrap
-```
 
 ### Installation phases
 
 Installation can take several minutes, here an excerpt of main messages displayed during installation:
 
 ```console
 sudo /home/nua/env/bin/nua-bootstrap
```

