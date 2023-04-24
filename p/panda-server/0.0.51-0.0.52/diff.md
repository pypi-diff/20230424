# Comparing `tmp/panda-server-0.0.51.tar.gz` & `tmp/panda-server-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda-server-0.0.51.tar", last modified: Wed Apr 19 15:31:41 2023, max compression
+gzip compressed data, was "panda-server-0.0.52.tar", last modified: Mon Apr 24 06:51:18 2023, max compression
```

## Comparing `panda-server-0.0.51.tar` & `panda-server-0.0.52.tar`

### file list

```diff
@@ -1,237 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.009645 panda-server-0.0.51/
--rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-04-19 15:31:28.000000 panda-server-0.0.51/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-19 15:31:28.000000 panda-server-0.0.51/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 15:31:28.000000 panda-server-0.0.51/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-19 15:31:41.009645 panda-server-0.0.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 15:31:28.000000 panda-server-0.0.51/PandaPkgInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 15:31:28.000000 panda-server-0.0.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.977645 panda-server-0.0.51/panda_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 15:31:40.000000 panda-server-0.0.51/panda_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:28.000000 panda-server-0.0.51/pandaserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/brokerage/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/brokerage/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/config/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/config/daemon_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/config/panda_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/configurator/Carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/configurator/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/configurator/aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.981645 panda-server-0.0.51/pandaserver/daemons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/master.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.985645 panda-server-0.0.51/pandaserver/daemons/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0 runner    (1001) docker     (123)    37494 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25064 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/daemons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/dataservice/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Activator.py
--rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    39385 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/AdderSimplePlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Closer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/CloserAtlasPlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DDMHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DataService.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DataServiceUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/DynDataDistributer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/EventPicker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Finisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16870 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/Setupper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113610 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/SetupperAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/SetupperDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/SetupperPluginBase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/eventLookupClientEI.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/dataservice/forkSetupper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/jobdispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58936 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16316 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/jobdispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/proxycache/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/proxycache/DBMSql.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/proxycache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/proxycache/panda_activeusers_query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/proxycache/panda_proxy_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/server/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/server/.gacl
--rwxr-xr-x   0 runner    (1001) docker     (123)    22396 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/server/panda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.989645 panda-server-0.0.51/pandaserver/srvcore/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/srvcore/srv_msg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:40.997645 panda-server-0.0.51/pandaserver/taskbuffer/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/EiDBProxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)  1232383 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   137660 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19062 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/taskbuffer/workflow_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/SchemaChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/test/alice/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/banUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/boostPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/boostUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/callbackDDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/finishJob.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/finishTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/frontier_retagging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/getJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/killUser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/test/lsst/
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reassignJobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reassignSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reassignTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reassignWaiting.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/reloadInputDS.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/setPriority.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testEvgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testG4sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testG4sim17.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testReco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testSiteMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/test/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/userinterface/
--rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/userinterface/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)    89144 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/userinterface/UserIF.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/userinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.001645 panda-server-0.0.51/pandaserver/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/psnakemake_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.005645 panda-server-0.0.51/pandaserver/workflow/snakeparser/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-04-19 15:31:29.000000 panda-server-0.0.51/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-19 15:31:41.009645 panda-server-0.0.51/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    13632 2023-04-19 15:31:29.000000 panda-server-0.0.51/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.005645 panda-server-0.0.51/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/conda_meta.yaml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.009645 panda-server-0.0.51/templates/init.d/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/init.d/panda_server.exe.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.009645 panda-server-0.0.51/templates/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/logrotate.d/panda_server.logrotate.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-add_main.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-add_sub.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-backupJobArch.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-boostUser.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-callback.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-configurator.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-copyArchive.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-datasetManager.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-esPreemption.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-evpPD2P.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-frontier_retagging.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-httpd.conf.rpmnew.template
--rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-network_configurator.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-pilot_streaming.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-priority.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-proxyCache.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-schedconfig_json.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-sw_tags.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-tmpwatch.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server-vomsrenew.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/panda_server.cfg.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/pandasrv.cron.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:31:41.009645 panda-server-0.0.51/templates/sysconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-19 15:31:29.000000 panda-server-0.0.51/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/
+-rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-04-24 06:51:06.000000 panda-server-0.0.52/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 06:51:06.000000 panda-server-0.0.52/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 06:51:06.000000 panda-server-0.0.52/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 06:51:18.824622 panda-server-0.0.52/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 06:51:06.000000 panda-server-0.0.52/PandaPkgInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 06:51:06.000000 panda-server-0.0.52/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.792619 panda-server-0.0.52/panda_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 06:51:18.000000 panda-server-0.0.52/panda_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.792619 panda-server-0.0.52/pandaserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.792619 panda-server-0.0.52/pandaserver/brokerage/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/brokerage/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.796620 panda-server-0.0.52/pandaserver/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/config/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7052 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/config/panda_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.796620 panda-server-0.0.52/pandaserver/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/configurator/Carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/configurator/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/configurator/aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.796620 panda-server-0.0.52/pandaserver/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/master.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.800620 panda-server-0.0.52/pandaserver/daemons/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37494 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25064 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/daemons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.800620 panda-server-0.0.52/pandaserver/dataservice/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Activator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39385 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/AdderSimplePlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Closer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/CloserAtlasPlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DDMHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DataService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DataServiceUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/DynDataDistributer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/EventPicker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Finisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16870 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/Setupper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113610 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/SetupperAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/SetupperDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/SetupperPluginBase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/eventLookupClientEI.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/dataservice/forkSetupper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.804620 panda-server-0.0.52/pandaserver/jobdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58936 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16316 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/jobdispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.804620 panda-server-0.0.52/pandaserver/proxycache/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/proxycache/DBMSql.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/proxycache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/proxycache/panda_activeusers_query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/proxycache/panda_proxy_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.804620 panda-server-0.0.52/pandaserver/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/server/.gacl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22396 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/server/panda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.804620 panda-server-0.0.52/pandaserver/srvcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/srvcore/srv_msg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.812621 panda-server-0.0.52/pandaserver/taskbuffer/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/EiDBProxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1229216 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   137660 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19209 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/taskbuffer/workflow_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/test/alice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/banUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/boostUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/callbackDDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/finishJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/finishTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/frontier_retagging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/getJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/killUser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/test/lsst/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reassignJobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reassignSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/setPriority.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testG4sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testG4sim17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testReco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testSiteMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/test/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/userinterface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/userinterface/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89144 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/userinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/psnakemake_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.820622 panda-server-0.0.52/pandaserver/workflow/snakeparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-04-24 06:51:06.000000 panda-server-0.0.52/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 06:51:18.824622 panda-server-0.0.52/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13632 2023-04-24 06:51:06.000000 panda-server-0.0.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/conda_meta.yaml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/templates/init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/init.d/panda_server.exe.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/templates/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/logrotate.d/panda_server.logrotate.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-add_main.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-add_sub.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-backupJobArch.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-boostUser.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-callback.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-configurator.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      167 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-copyArchive.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-datasetManager.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-esPreemption.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-evpPD2P.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-frontier_retagging.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-httpd.conf.rpmnew.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-network_configurator.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-pilot_streaming.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-priority.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-proxyCache.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-schedconfig_json.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-sw_tags.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-tmpwatch.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server-vomsrenew.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/panda_server.cfg.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/pandasrv.cron.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:51:18.824622 panda-server-0.0.52/templates/sysconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-24 06:51:06.000000 panda-server-0.0.52/templates/sysconfig/panda_server.sysconfig.rpmnew.template
```

### Comparing `panda-server-0.0.51/ChangeLog.txt` & `panda-server-0.0.52/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/LICENSE.txt` & `panda-server-0.0.52/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/panda_server.egg-info/SOURCES.txt` & `panda-server-0.0.52/panda_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/brokerage/SiteMapper.py` & `panda-server-0.0.52/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/brokerage/broker.py` & `panda-server-0.0.52/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/config/daemon_config.py` & `panda-server-0.0.52/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/config/panda_config.py` & `panda-server-0.0.52/pandaserver/config/panda_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 if 'pserverporthttp' not in tmpSelf.__dict__:
     tmpSelf.__dict__['pserverporthttp'] = 25080
 
 # set host for http
 if 'pserverhosthttp' not in tmpSelf.__dict__:
     tmpSelf.__dict__['pserverhosthttp'] = tmpSelf.__dict__['pserverhost']
 
+# disable http
+if 'disableHTTP' not in tmpSelf.__dict__:
+    tmpSelf.__dict__['disableHTTP'] = False
+
 # change the number of database connections for FastCGI/WSGI
 if tmpSelf.__dict__['useFastCGI'] or tmpSelf.__dict__['useWSGI']:
     tmpSelf.__dict__['nDBConnection'] = tmpSelf.__dict__['nDBConForFastCGIWSGI']
 
 # DB backend
 if 'backend' not in tmpSelf.__dict__:
     tmpSelf.__dict__['backend'] = 'oracle'
```

### Comparing `panda-server-0.0.51/pandaserver/configurator/Carbon.py` & `panda-server-0.0.52/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/configurator/Configurator.py` & `panda-server-0.0.52/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/configurator/aux.py` & `panda-server-0.0.52/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/master.py` & `panda-server-0.0.52/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/add_main.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/add_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     except Exception:
         gracePeriod = 1
 
     # lock interval in minutes
     lock_interval = 10
 
     # retry interval in minutes
-    retry_interval = 3
+    retry_interval = 1
 
     # instantiate TB
     if tbuf is None:
         from pandaserver.taskbuffer.TaskBuffer import taskBuffer
         taskBuffer.init(panda_config.dbhost,panda_config.dbpasswd,nDBConnection=1, useTimeout=True)
     else:
         taskBuffer = tbuf
```

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/add_sub.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/carbon.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/configurator.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/copyArchive.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/datasetManager.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/datasetManager.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/dummy_test.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/dummy_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/evpPD2P.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/metric_collector.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/pilotStreaming.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/task_evaluator.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/tmpwatch.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/scripts/worker_synchronization.py` & `panda-server-0.0.52/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/daemons/utils.py` & `panda-server-0.0.52/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/Activator.py` & `panda-server-0.0.52/pandaserver/dataservice/Activator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda-server-0.0.52/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/AdderGen.py` & `panda-server-0.0.52/pandaserver/dataservice/AdderGen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/AdderResult.py` & `panda-server-0.0.52/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/AdderSimplePlugin.py` & `panda-server-0.0.52/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/Closer.py` & `panda-server-0.0.52/pandaserver/dataservice/Closer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/CloserAtlasPlugin.py` & `panda-server-0.0.52/pandaserver/dataservice/CloserAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/DDM.py` & `panda-server-0.0.52/pandaserver/dataservice/DDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/DDMHandler.py` & `panda-server-0.0.52/pandaserver/dataservice/DDMHandler.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/DataService.py` & `panda-server-0.0.52/pandaserver/dataservice/DataService.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/DataServiceUtils.py` & `panda-server-0.0.52/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/DynDataDistributer.py` & `panda-server-0.0.52/pandaserver/dataservice/DynDataDistributer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/EventPicker.py` & `panda-server-0.0.52/pandaserver/dataservice/EventPicker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/Finisher.py` & `panda-server-0.0.52/pandaserver/dataservice/Finisher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/Notifier.py` & `panda-server-0.0.52/pandaserver/dataservice/Notifier.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/ProcessLimiter.py` & `panda-server-0.0.52/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda-server-0.0.52/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/Setupper.py` & `panda-server-0.0.52/pandaserver/dataservice/Setupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/SetupperAtlasPlugin.py` & `panda-server-0.0.52/pandaserver/dataservice/SetupperAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/SetupperDummyPlugin.py` & `panda-server-0.0.52/pandaserver/dataservice/SetupperDummyPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/SetupperPluginBase.py` & `panda-server-0.0.52/pandaserver/dataservice/SetupperPluginBase.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/eventLookupClientEI.py` & `panda-server-0.0.52/pandaserver/dataservice/eventLookupClientEI.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/dataservice/forkSetupper.py` & `panda-server-0.0.52/pandaserver/dataservice/forkSetupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda-server-0.0.52/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/jobdispatcher/JobDispatcher.py` & `panda-server-0.0.52/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/jobdispatcher/Protocol.py` & `panda-server-0.0.52/pandaserver/jobdispatcher/Protocol.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/jobdispatcher/Watcher.py` & `panda-server-0.0.52/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/proxycache/DBMSql.py` & `panda-server-0.0.52/pandaserver/proxycache/DBMSql.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/proxycache/panda_activeusers_query.py` & `panda-server-0.0.52/pandaserver/proxycache/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/proxycache/panda_proxy_cache.py` & `panda-server-0.0.52/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/server/panda.py` & `panda-server-0.0.52/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/srvcore/CoreUtils.py` & `panda-server-0.0.52/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/srvcore/MailUtils.py` & `panda-server-0.0.52/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/srvcore/oidc_utils.py` & `panda-server-0.0.52/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/srvcore/srv_msg_utils.py` & `panda-server-0.0.52/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/CloudSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/ConBridge.py` & `panda-server-0.0.52/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/DBProxyPool.py` & `panda-server-0.0.52/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/DatasetSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/DdmSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/EiDBProxy.py` & `panda-server-0.0.52/pandaserver/taskbuffer/EiDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/ErrorCode.py` & `panda-server-0.0.52/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/EventServiceUtils.py` & `panda-server-0.0.52/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/FileSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/GlobalShares.py` & `panda-server-0.0.52/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/Initializer.py` & `panda-server-0.0.52/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/JobSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/JobSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/JobUtils.py` & `panda-server-0.0.52/pandaserver/taskbuffer/JobUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/NucleusSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/OraDBProxy.py` & `panda-server-0.0.52/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1433,15 +1433,19 @@
                 type, value, traceBack = sys.exc_info()
                 _logger.error("keepJob : %s %s" % (type,value))
                 return False
 
     # archive job to jobArchived and remove the job from jobsActive or jobsDefined
     def archiveJob(self,job,fromJobsDefined,useCommit=True,extraInfo=None,fromJobsWaiting=False):
         comment = ' /* DBProxy.archiveJob */'
-        _logger.debug("archiveJob : %s %s" % (job.PandaID, job.jobStatus))
+        methodName = comment.split(' ')[-2].split('.')[-1]
+        methodName = methodName + " < PandaID={} jediTaskID={} >".format(job.PandaID, job.jediTaskID)
+        tmpLog = LogWrapper(_logger, methodName)
+        tmpLog.debug("start for jobStatus=%s" % job.jobStatus)
+        start_time = datetime.datetime.utcnow()
         if fromJobsDefined:
             sql0 = "SELECT jobStatus FROM ATLAS_PANDA.jobsDefined4 WHERE PandaID=:PandaID "
             sql1 = "DELETE FROM ATLAS_PANDA.jobsDefined4 WHERE PandaID=:PandaID AND (jobStatus=:oldJobStatus1 OR jobStatus=:oldJobStatus2)"
         elif fromJobsWaiting:
             sql0 = "SELECT jobStatus FROM ATLAS_PANDA.jobsWaiting4 WHERE PandaID=:PandaID "
             sql1 = "DELETE FROM ATLAS_PANDA.jobsWaiting4 WHERE PandaID=:PandaID"
         else:
@@ -1489,15 +1493,15 @@
                     sqlPMod = "UPDATE ATLAS_PANDA.jobParamsTable SET modificationTime=:modificationTime WHERE PandaID=:PandaID"
                     sqlGetSub = "SELECT DISTINCT destinationDBlock FROM ATLAS_PANDA.filesTable4 WHERE type=:type AND PandaID=:PandaID"
                     sqlCloseSub  = 'UPDATE /*+ INDEX_RS_ASC(TAB("DATASETS"."NAME")) */ ATLAS_PANDA.Datasets tab '
                     sqlCloseSub += 'SET status=:status,modificationDate=CURRENT_DATE WHERE name=:name'
                     sqlDFile = "SELECT %s FROM ATLAS_PANDA.filesTable4 " % FileSpec.columnNames()
                     sqlDFile+= "WHERE PandaID=:PandaID"
                     for upFile in upOutputs:
-                        _logger.debug("look for downstream jobs for %s" % upFile)
+                        tmpLog.debug("look for downstream jobs for %s" % upFile)
                         if useCommit:
                             self.conn.begin()
                         # select PandaID
                         varMap = {}
                         varMap[':lfn']  = upFile
                         varMap[':type'] = 'input'
                         self.cur.arraysize = 100000
@@ -1506,22 +1510,22 @@
                         if useCommit:
                             if not self._commit():
                                 raise RuntimeError('Commit error')
                         iDownJobs = 0
                         nDownJobs = len(res)
                         nDownChunk = 20
                         inTransaction = False
-                        _logger.debug("archiveJob : {0} found {1} downstream jobs for {2}".format(job.PandaID,nDownJobs,upFile))
+                        tmpLog.debug("found {} downstream jobs for {}".format(nDownJobs, upFile))
                         # loop over all downstream IDs
                         for downID, in res:
                             if useCommit:
                                 if not inTransaction:
                                     self.conn.begin()
                                     inTransaction = True
-                            _logger.debug("archiveJob : {0} delete : {1} ({2}/{3})".format(job.PandaID,downID,iDownJobs,nDownJobs))
+                            tmpLog.debug("delete : {} ({}/{})".format(downID, iDownJobs, nDownJobs))
                             iDownJobs += 1
                             # select jobs
                             varMap = {}
                             varMap[':PandaID'] = downID
                             self.cur.arraysize = 10
                             self.cur.execute(sqlDJS+comment, varMap)
                             resJob = self.cur.fetchall()
@@ -1606,30 +1610,30 @@
                                         continue
                                     if tmpDestinationDBlock not in toBeClosedSubList[dJob.jobDefinitionID]:
                                         # set tobeclosed
                                         varMap = {}
                                         varMap[':status'] = 'tobeclosed'
                                         varMap[':name'] = tmpDestinationDBlock
                                         self.cur.execute(sqlCloseSub+comment, varMap)
-                                        _logger.debug("set tobeclosed for %s" % tmpDestinationDBlock)
+                                        tmpLog.debug("set tobeclosed for %s" % tmpDestinationDBlock)
                                         # append
                                         toBeClosedSubList[dJob.jobDefinitionID].append(tmpDestinationDBlock)
                                         # close top-level user dataset
                                         topUserDsName = re.sub('_sub\d+$','',tmpDestinationDBlock)
                                         if not useJEDI and topUserDsName != tmpDestinationDBlock and topUserDsName not in topUserDsList:
                                             # set tobeclosed
                                             varMap = {}
                                             if dJob.processingType.startswith('gangarobot') or \
                                                    dJob.processingType.startswith('hammercloud'):
                                                 varMap[':status'] = 'completed'
                                             else:
                                                 varMap[':status'] = 'tobeclosed'
                                             varMap[':name'] = topUserDsName
                                             self.cur.execute(sqlCloseSub+comment, varMap)
-                                            _logger.debug("set %s for %s" % (varMap[':status'],topUserDsName))
+                                            tmpLog.debug("set %s for %s" % (varMap[':status'],topUserDsName))
                                             # append
                                             topUserDsList.append(topUserDsName)
                             if useCommit and (iDownJobs % nDownChunk) == 0:
                                 if not self._commit():
                                     raise RuntimeError('Commit error')
                                 inTransaction = False
                         if useCommit and inTransaction:
@@ -1650,15 +1654,15 @@
                             for item in callbackUrl.split():
                                 if item.startswith('vuid='):
                                     vuid = item.split('=')[-1]
                                     break
                         except Exception:
                             pass
                         if vuid == '':
-                            _logger.error("cannot extract vuid from %s" % job.jobParameters)
+                            tmpLog.error("cannot extract vuid from %s" % job.jobParameters)
                         else:
                             # get name
                             varMap = {}
                             varMap[':vuid'] = vuid
                             varMap[':type'] = 'dispatch'
                             self.cur.arraysize = 10
                             self.cur.execute("SELECT name FROM ATLAS_PANDA.Datasets WHERE vuid=:vuid AND type=:type "+comment, varMap)
@@ -1679,15 +1683,15 @@
                                 sqlDJI = "INSERT INTO ATLAS_PANDA.jobsArchived4 (%s) " % JobSpec.columnNames()
                                 sqlDJI+= JobSpec.bindValuesExpression()
                                 sqlFMod = "UPDATE ATLAS_PANDA.filesTable4 SET modificationTime=:modificationTime WHERE PandaID=:PandaID"
                                 sqlMMod = "UPDATE ATLAS_PANDA.metaTable SET modificationTime=:modificationTime WHERE PandaID=:PandaID"
                                 sqlPMod = "UPDATE ATLAS_PANDA.jobParamsTable SET modificationTime=:modificationTime WHERE PandaID=:PandaID"
                                 lostJobIDs = []
                                 for tmpID, in resLost:
-                                    _logger.debug("fail due to lost files : %s" % tmpID)
+                                    tmpLog.debug("fail due to lost files : %s" % tmpID)
                                     varMap = {}
                                     varMap[':PandaID'] = tmpID
                                     self.cur.arraysize = 10
                                     self.cur.execute(sqlDJS+comment, varMap)
                                     resJob = self.cur.fetchall()
                                     if len(resJob) == 0:
                                         continue
@@ -1729,15 +1733,15 @@
                                                  varMap)
                                 resDDM = self.cur.fetchall()
                                 for tmpID, in resDDM:
                                     if tmpID not in lostJobIDs:
                                         ddmIDs.append(tmpID)
                                 # get offset
                                 ddmAttempt = job.attemptNr
-                                _logger.debug("get PandaID for reassign : %s ddmAttempt=%s" % (str(ddmIDs),ddmAttempt))
+                                tmpLog.debug("get PandaID for reassign : %s ddmAttempt=%s" % (str(ddmIDs),ddmAttempt))
                     if useCommit:
                         if not self._commit():
                             raise RuntimeError('Commit error')
                 elif job.prodSourceLabel == 'ddm' and job.jobStatus == 'failed' and job.transferType=='ddm' and job.attemptNr<2 \
                          and job.commandToPilot != 'tobekilled':
                     # instantiate new mover to retry subscription
                     newJob = JobSpec()
@@ -1785,74 +1789,72 @@
                     varMap = {}
                     varMap[':PandaID'] = job.PandaID
                     self.cur.execute(sql0+comment, varMap)
                     res0 = self.cur.fetchone()
                 # check input status for ES merge
                 if useJEDI and EventServiceUtils.isEventServiceMerge(job) and job.jobStatus == 'finished':
                     retInputStat = self.checkInputFileStatusInJEDI(job, useCommit=False, withLock=True)
-                    _logger.debug("archiveJob : {0} checkInput for ES merge -> {1}".format(job.PandaID, retInputStat))
+                    tmpLog.debug("checkInput for ES merge -> {}".format(retInputStat))
                     if retInputStat is None:
                         raise RuntimeError("archiveJob : {0} failed to check input".format(job.PandaID))
                     if retInputStat is False:
-                        _logger.debug("archiveJob : {0} set jobStatus=failed due to inconsisten input".format(job.PandaID))
+                        tmpLog.debug("set jobStatus=failed due to inconsisten input")
                         job.jobStatus = 'failed'
                         job.taskBufferErrorCode = ErrorCode.EC_EventServiceInconsistentIn
                         job.taskBufferErrorDiag = "inconsistent file status between Panda and JEDI"
                         for fileSpec in job.Files:
                             if fileSpec.type in ['output','log']:
                                 fileSpec.status = 'failed'
                 # actions for jobs without tasks
                 if not useJEDI:
                     # update HS06sec for non-JEDI jobs (e.g. HC)
                     hs06sec = self.setHS06sec(job.PandaID, inActive=True)
-                    _logger.debug("archiveJob : calculated hs06sec {0} for pandaID {1}".format(hs06sec, job.PandaID))
+                    tmpLog.debug("calculated hs06sec {0}".format(hs06sec))
                     if hs06sec is not None:
                         job.hs06sec = hs06sec
 
                     # update the g of CO2 emitted by the job
                     try:
                         gco2_regional, gco2_global = self.set_co2_emissions(job.PandaID, in_active=True)
-                        _logger.debug("archiveJob : calculated gCO2 regional {0} and global {1} for pandaID {2}".format(gco2_regional, gco2_global, job.PandaID))
+                        tmpLog.debug("calculated gCO2 regional {0} and global {1}".format(gco2_regional, gco2_global))
                         if gco2_regional is not None:
                             job.gco2_regional = gco2_regional
                         if gco2_global is not None:
                             job.gco2_global = gco2_global
                     except Exception:
-                        _logger.error(
-                            "archiveJob : failed calculating gCO2 for pandaID {0} with {1}".format(job.PandaID,
-                                                                                                   traceback.format_exc()))
+                        tmpLog.error(
+                            "failed calculating gCO2 with {}".format(traceback.format_exc()))
 
                 # actions for successful normal ES jobs
                 if useJEDI and EventServiceUtils.isEventServiceJob(job) \
                         and not EventServiceUtils.isJobCloningJob(job):
 
                     # update some job attributes
                     hs06sec = self.setHS06sec(job.PandaID, inActive=True)
                     if hs06sec is not None:
                         job.hs06sec = hs06sec
 
                     # update the g of CO2 emitted by the job
                     try:
                         gco2_regional, gco2_global = self.set_co2_emissions(job.PandaID, in_active=True)
-                        _logger.debug("archiveJob : calculated gCO2 regional {0} and global {1} for pandaID {1}".format(gco2_regional, gco2_global, job.PandaID))
+                        tmpLog.debug("calculated gCO2 regional {} and global {}".format(gco2_regional, gco2_global))
                         if gco2_regional is not None:
                              job.gco2_regional = gco2_regional
                         if gco2_global is not None:
                              job.gco2_global = gco2_global
                     except Exception:
-                        _logger.error(
-                            "archiveJob : failed calculating gCO2 for pandaID {0} with {1}".format(job.PandaID,
-                                                                                                   traceback.format_exc()))
+                        tmpLog.error(
+                            "failed calculating gCO2 with {}".format(traceback.format_exc()))
 
                     # post processing
                     oldJobSubStatus = job.jobSubStatus
                     if oldJobSubStatus == 'NULL':
                         oldJobSubStatus = None
                     retEvS,retNewPandaID = self.ppEventServiceJob(job,currentJobStatus,False)
-                    _logger.debug("archiveJob : {0} ppE -> {1}".format(job.PandaID, retEvS))
+                    tmpLog.debug("ppE -> {}".format(retEvS))
                     # DB error
                     if retEvS is None:
                         raise RuntimeError('Faied to retry for Event Service')
                     elif retEvS == 0:
                         # retry event ranges
                         job.jobStatus = 'merging'
                         job.jobSubStatus = 'es_retry'
@@ -1910,55 +1912,40 @@
                         job.jobStatus = 'closed'
                         job.jobSubStatus = 'es_badstatus'
                         job.taskBufferErrorCode = ErrorCode.EC_EventServiceBadStatus
                         job.taskBufferErrorDiag = "cloded in bad jobStatus like defined and pending"
                     # additional actions when retry
                     codeListWithRetry = [0, 4, 5, 8, 9]
                     if retEvS in codeListWithRetry and job.computingSite != EventServiceUtils.siteIdForWaitingCoJumboJobs:
-                        # resurrect consumers at other sites
-                        """
-                        if retEvS != 4 and EventServiceUtils.isResurrectConsumers(job.specialHandling):
-                            archivedConsumers = self.getOriginalConsumers(job.jediTaskID, job.jobsetID, job.PandaID)
-                            for archivedConsumer in archivedConsumers:
-                                archivedConsumer.attemptNr = job.attemptNr
-                                archivedConsumer.maxAttempt = job.maxAttempt
-                                tmpS,tmpID = self.ppEventServiceJob(archivedConsumer,None,False)
-                                _logger.debug('archiveJob : {0} tried to resurrect old consumer {1} ret={2} new={3}'.format(job.PandaID,
-                                                                                                                            archivedConsumer.PandaID,
-                                                                                                                            tmpS,tmpID))
-                                if tmpID is not None:
-                                    retNewPandaID = tmpID
-                        """
                         # check jumbo flag
                         sqlJumbo = "SELECT useJumbo FROM {0}.JEDI_Tasks ".format(panda_config.schemaJEDI)
                         sqlJumbo += "WHERE jediTaskID=:jediTaskID "
                         varMap = {}
                         varMap[':jediTaskID'] = job.jediTaskID
                         self.cur.execute(sqlJumbo+comment, varMap)
                         resJumbo = self.cur.fetchone()
                         if resJumbo is not None:
                             useJumbo, = resJumbo
                         else:
                             useJumbo = None
-                        _logger.debug("archiveJob : {0} useJumbo={1}".format(job.PandaID, useJumbo))
+                        tmpLog.debug("useJumbo={}".format(useJumbo))
                         # no new jobs
                         if retNewPandaID is None and (retEvS != 4 or EventServiceUtils.isCoJumboJob(job) or useJumbo is not None):
                             nActiveConsumers = self.getActiveConsumers(job.jediTaskID, job.jobsetID, job.PandaID)
                             # create a fake cojumbo
                             if nActiveConsumers == 0 and retEvS in [4, 5] and (EventServiceUtils.isCoJumboJob(job) or useJumbo is not None) \
                                     and job.computingSite != EventServiceUtils.siteIdForWaitingCoJumboJobs:
                                 nActiveConsumers = self.makeFakeCoJumbo(job)
                             # no ES queues for retry
                             if nActiveConsumers == 0:
                                 job.jobStatus = 'failed'
                                 job.taskBufferErrorCode = ErrorCode.EC_EventServiceNoEsQueues
                                 job.taskBufferErrorDiag = "no ES queues available for new consumers"
-                                _logger.debug('archiveJob : {0} set {1} since {2}'.format(job.PandaID,
-                                                                                          job.jobStatus,
-                                                                                          job.taskBufferErrorDiag))
+                                tmpLog.debug('set {} since {}'.format(job.jobStatus,
+                                                                      job.taskBufferErrorDiag))
                     # kill unused event ranges
                     if job.jobStatus == 'failed':
                         if not job.notDiscardEvents():
                             self.killUnusedEventRanges(job.jediTaskID,job.jobsetID)
                         self.updateRelatedEventServiceJobs(job,True)
                 elif useJEDI and EventServiceUtils.isEventServiceJob(job) \
                         and EventServiceUtils.isJobCloningJob(job):
@@ -2016,15 +2003,15 @@
                     self.cur.execute(sql2+comment, job.valuesMap())
                     # update files
                     for file in job.Files:
                         sqlF = ("UPDATE ATLAS_PANDA.filesTable4 SET %s" % file.bindUpdateChangesExpression()) + "WHERE row_ID=:row_ID"
                         varMap = file.valuesMap(onlyChanged=True)
                         if varMap != {}:
                             varMap[':row_ID'] = file.row_ID
-                            _logger.debug(sqlF+comment+str(varMap))
+                            tmpLog.debug(sqlF+comment+str(varMap))
                             self.cur.execute(sqlF+comment, varMap)
                     # update metadata and parameters
                     sqlFMod = "UPDATE ATLAS_PANDA.filesTable4 SET modificationTime=:modificationTime WHERE PandaID=:PandaID"
                     sqlMMod = "UPDATE ATLAS_PANDA.metaTable SET modificationTime=:modificationTime WHERE PandaID=:PandaID"
                     sqlPMod = "UPDATE ATLAS_PANDA.jobParamsTable SET modificationTime=:modificationTime WHERE PandaID=:PandaID"
                     varMap = {}
                     varMap[':PandaID'] = job.PandaID
@@ -2045,21 +2032,21 @@
                                 sqlGetCurFiles += """INDEX_RS_ASC(@"SEL$1" "TAB"@"SEL$1" ("DATASETS"."NAME")) """
                                 sqlGetCurFiles += """OUTLINE_LEAF(@"SEL$1") ALL_ROWS """
                                 sqlGetCurFiles += """IGNORE_OPTIM_EMBEDDED_HINTS """
                                 sqlGetCurFiles += """END_OUTLINE_DATA */ """
                                 sqlGetCurFiles += "currentfiles,vuid FROM ATLAS_PANDA.Datasets tab WHERE name=:name"
                                 self.cur.execute(sqlGetCurFiles+comment,varMap)
                                 resCurFiles = self.cur.fetchone()
-                                _logger.debug("archiveJob : %s %s" % (job.PandaID,str(resCurFiles)))
+                                tmpLog.debug("%s" % str(resCurFiles))
                                 if resCurFiles is not None:
                                     # increment currentfiles only for the first failed job since that is enough
                                     tmpCurrentFiles,tmpVUID = resCurFiles
-                                    _logger.debug("archiveJob : %s %s currentfiles=%s" % (job.PandaID,tmpFile.dispatchDBlock,tmpCurrentFiles))
+                                    tmpLog.debug("%s currentfiles=%s" % (tmpFile.dispatchDBlock, tmpCurrentFiles))
                                     if tmpCurrentFiles == 0:
-                                        _logger.debug("archiveJob : %s %s update currentfiles" % (job.PandaID,tmpFile.dispatchDBlock))
+                                        tmpLog.debug("%s update currentfiles" % tmpFile.dispatchDBlock)
                                         varMap = {}
                                         varMap[':vuid'] = tmpVUID
                                         sqlFailedInDis  = 'UPDATE ATLAS_PANDA.Datasets '
                                         sqlFailedInDis += 'SET currentfiles=currentfiles+1 WHERE vuid=:vuid'
                                         self.cur.execute(sqlFailedInDis+comment,varMap)
                                 myDisList.append(tmpFile.dispatchDBlock)
                     # collect to record state change
@@ -2116,51 +2103,51 @@
                         varMap[':jobStatus'] = 'merging'
                         if oldJobSubStatus in ['es_toolong']:
                             varMap[':jobSubStatus'] = oldJobSubStatus
                         else:
                             varMap[':jobSubStatus'] = 'es_wait'
                         self.cur.execute(sqlOJS+comment,varMap)
                         tmpJobStatus = varMap[':jobStatus']
-                        _logger.debug("archiveJob : %s change failed to merging" % job.PandaID)
+                        tmpLog.debug("change failed to merging")
                     elif job.jobStatus in ['failed'] and \
                             job.taskBufferErrorCode in [ErrorCode.EC_EventServiceLastUnprocessed, ErrorCode.EC_EventServiceUnprocessed] and \
                             (oldJobSubStatus in ['pilot_noevents'] or \
                                  (job.pilotErrorCode == 0 and job.ddmErrorCode == 0 and job.supErrorCode == 0 and job.jobDispatcherErrorCode == 0)):
                         varMap = {}
                         varMap[':PandaID'] = job.PandaID
                         varMap[':jobStatus'] = 'closed'
                         varMap[':jobSubStatus'] = oldJobSubStatus
                         self.cur.execute(sqlOJS+comment,varMap)
                         tmpJobStatus = varMap[':jobStatus']
-                        _logger.debug("archiveJob : {0} change failed to closed for {1}".format(job.PandaID, oldJobSubStatus))
+                        tmpLog.debug("change failed to closed for {}".format(oldJobSubStatus))
                 # commit
                 if useCommit:
                     if not self._commit():
                         raise RuntimeError('Commit error')
                 # record status change
                 try:
                     for tmpJob in updatedJobList:
                         self.recordStatusChange(tmpJob.PandaID,tmpJobStatus,jobInfo=tmpJob,useCommit=useCommit)
                         self.push_job_status_message(tmpJob, tmpJob.PandaID, tmpJobStatus)
                 except Exception:
-                    _logger.error('recordStatusChange in archiveJob')
-                _logger.debug("archiveJob : %s done" % job.PandaID)
-                return True,ddmIDs,ddmAttempt,newJob
+                    tmpLog.error('recordStatusChange in archiveJob')
+                exec_time = datetime.datetime.utcnow() - start_time
+                tmpLog.debug("done OK. took %s.%03d sec" % (exec_time.seconds, exec_time.microseconds/1000))
+                return True, ddmIDs, ddmAttempt, newJob
             except Exception:
                 # roll back
                 if useCommit:
                     self._rollback(True)
-                errtype,errvalue = sys.exc_info()[:2]
-                errStr = "archiveJob %s : %s %s" % (job.PandaID,errtype,errvalue)
-                errStr.strip()
-                errStr += traceback.format_exc()
-                _logger.error(errStr)
+                # error
+                self.dumpErrorMessage(_logger, methodName)
+                exec_time = datetime.datetime.utcnow() - start_time
+                tmpLog.debug("done NG. took %s.%03d sec" % (exec_time.seconds, exec_time.microseconds/1000))
                 if not useCommit:
                     raise RuntimeError('archiveJob failed')
-                return False,[],0,None
+                return False, [], 0, None
 
 
     # finalize pending jobs
     def finalizePendingJobs(self,prodUserName,jobDefinitionID,waitLock=False):
         comment = ' /* DBProxy.finalizePendingJobs */'
         methodName = comment.split(' ')[-2].split('.')[-1]
         tmpLog = LogWrapper(_logger, methodName + " < user={} jobdefID={} >".format(prodUserName, jobDefinitionID))
@@ -12469,15 +12456,15 @@
                 _logger.error("push_job_status_message %s %s: %s %s" % (panda_id, status, errType, errValue))
 
 
     # propagate result to JEDI
     def propagateResultToJEDI(self, jobSpec, cur, oldJobStatus=None, extraInfo=None, finishPending=False, waitLock=False):
         comment = ' /* DBProxy.propagateResultToJEDI */'
         methodName = comment.split(' ')[-2].split('.')[-1]
-        methodName += " <PandaID={0}>".format(jobSpec.PandaID)
+        methodName += " < PandaID={} jediTaskID={} >".format(jobSpec.PandaID, jobSpec.jediTaskID)
         tmpLog = LogWrapper(_logger,methodName)
         datasetContentsStat = {}
         # loop over all files
         finishUnmerge = set()
         hasInput = False
         tmpLog.debug('waitLock={0}'.format(waitLock))
         # make pseudo files for dynamic number of events
@@ -12824,14 +12811,15 @@
                             datasetContentsStat[datasetID]['nFilesUsed'] += 1
         # update JEDI_Datasets table
         nOutEvents = 0
         if datasetContentsStat != {}:
             tmpDatasetIDs = list(datasetContentsStat)
             tmpDatasetIDs.sort()
             for tmpDatasetID in tmpDatasetIDs:
+                tmpLog.debug('trying to lock datasetID={}'.format(tmpDatasetID))
                 tmpContentsStat = datasetContentsStat[tmpDatasetID]
                 sqlJediDL = "SELECT nFilesUsed,nFilesFailed,nFilesTobeUsed,nFilesFinished,nFilesOnHold,type,masterID FROM ATLAS_PANDA.JEDI_Datasets "
                 sqlJediDL += "WHERE jediTaskID=:jediTaskID AND datasetID=:datasetID FOR UPDATE "
                 if not waitLock:
                     sqlJediDL += "NOWAIT "
                 varMap = {}
                 varMap[':jediTaskID'] = jobSpec.jediTaskID
@@ -12965,20 +12953,18 @@
             self.updateUnmergedJobs(jobSpec, finishUnmerge)
         # update some job attributes
         self.setHS06sec(jobSpec.PandaID)
 
         # update the g of CO2 emitted by the job
         try:
             gco2_regional, gco2_global = self.set_co2_emissions(jobSpec.PandaID)
-            _logger.debug("archiveJob : calculated gCO2 regional {0} and global {1} for pandaID {2}".format(gco2_regional,
-                                                                                                            gco2_global,
-                                                                                                            jobSpec.PandaID))
+            tmpLog.debug("calculated gCO2 regional {0} and global {1}".format(gco2_regional,
+                                                                              gco2_global))
         except Exception:
-            _logger.error("archiveJob : failed calculating gCO2 for pandaID {0} with {1}".format(jobSpec.PandaID,
-                                                                                                 traceback.format_exc()))
+            tmpLog.error("failed calculating gCO2 with {}".format(traceback.format_exc()))
 
         # return
         return True
 
 
 
     # check if task is active
@@ -24916,40 +24902,22 @@
         tmp_log = LogWrapper(_logger, method_name)
         tmp_log.debug('start')
 
         try:
             # begin transaction
             self.conn.begin()
 
-            # get existing panda ddm relations
-            tmp_log.debug("getting existing panda ddm relations")
-            sql_get = "SELECT panda_site_name, ddm_endpoint_name, scope FROM ATLAS_PANDA.panda_ddm_relation"
-            self.cur.execute(sql_get + comment)
-            relation_tuple_list = self.cur.fetchall()
-            tmp_log.debug("finished getting existing panda ddm relations")
+            # Reset the relations. Important to do this inside the transaction
+            tmp_log.debug("Deleting existing panda ddm relations")
+            sql_delete = "DELETE FROM ATLAS_PANDA.panda_ddm_relation"
+            self.cur.execute(sql_delete + comment)
 
-            # see which sites need an update and which need to be inserted new
             var_map_insert = []
-            var_map_update = []
             for relation in relation_list:
-                panda_site_name_tmp = relation['panda_site_name']
-                ddm_endpoint_name_tmp = relation['ddm_endpoint_name']
-                scope_tmp = relation['scope']
-                if (panda_site_name_tmp, ddm_endpoint_name_tmp, scope_tmp) in relation_tuple_list:
-                    var_map_update.append(convert_dict_to_bind_vars(relation))
-                else:
-                    var_map_insert.append(convert_dict_to_bind_vars(relation))
-
-            tmp_log.debug("Updating panda ddm relations")
-            sql_update = "UPDATE ATLAS_PANDA.panda_ddm_relation set "\
-                         "roles=:roles, is_local=:is_local, order_read=:order_read, order_write=:order_write, "\
-                         "default_read=:default_read, default_write=:default_write "\
-                         "WHERE panda_site_name=:panda_site_name AND ddm_endpoint_name=:ddm_endpoint_name AND scope=:scope"
-            for shard in create_shards(var_map_update, 100):
-                self.cur.executemany(sql_update + comment, shard)
+                var_map_insert.append(convert_dict_to_bind_vars(relation))
 
             tmp_log.debug("Inserting panda ddm relations")
             sql_insert = "INSERT INTO ATLAS_PANDA.panda_ddm_relation (panda_site_name, ddm_endpoint_name, roles, "\
                          "is_local, order_read, order_write, default_read, default_write, scope) "\
                          "VALUES(:panda_site_name, :ddm_endpoint_name, :roles, "\
                          ":is_local, :order_read, :order_write, :default_read, :default_write, :scope)"
             for shard in create_shards(var_map_insert, 100):
```

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/PrioUtil.py` & `panda-server-0.0.52/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/ProcessGroups.py` & `panda-server-0.0.52/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/ResourceSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/SQLDumper.py` & `panda-server-0.0.52/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/SiteSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/TaskBuffer.py` & `panda-server-0.0.52/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda-server-0.0.52/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/Utils.py` & `panda-server-0.0.52/pandaserver/taskbuffer/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,15 +429,18 @@
             os.remove(fileFullPath)
         # write
         fo = open(fileFullPath,'wb')
         fileContent = file.file.read()
         fo.write(fileContent)
         fo.close()
         tmpLog.debug("written to {0}".format(fileFullPath))
-        retStr = 'http://{0}/cache{1}/{2}'.format(getServerHTTP(None),jediLogDir,fileBaseName)
+        if panda_config.disableHTTP:
+            retStr = 'https://{}/cache{}/{}'.format(getServer(None), jediLogDir, fileBaseName)
+        else:
+            retStr = 'http://{}/cache{}/{}'.format(getServerHTTP(None),jediLogDir,fileBaseName)
     except Exception:
         errtype,errvalue = sys.exc_info()[:2]
         errStr = "failed to write log with {0}:{1}".format(errtype.__name__,errvalue)
         tmpLog.error(errStr)
         tmpLog.debug("end")
         return errStr
     tmpLog.debug("end")
```

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/WorkerSpec.py` & `panda-server-0.0.52/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/WrappedCursor.py` & `panda-server-0.0.52/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/WrappedPickle.py` & `panda-server-0.0.52/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/retryModule.py` & `panda-server-0.0.52/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/taskbuffer/workflow_processor.py` & `panda-server-0.0.52/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/SchemaChecker.py` & `panda-server-0.0.52/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda-server-0.0.52/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda-server-0.0.52/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/banUser.py` & `panda-server-0.0.52/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/boostPrio.py` & `panda-server-0.0.52/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/boostUser.py` & `panda-server-0.0.52/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/callbackDDM.py` & `panda-server-0.0.52/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/finishJob.py` & `panda-server-0.0.52/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/frontier_retagging.py` & `panda-server-0.0.52/pandaserver/test/frontier_retagging.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/getJobs.py` & `panda-server-0.0.52/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/killJob.py` & `panda-server-0.0.52/pandaserver/test/killJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/killJobLowPrio.py` & `panda-server-0.0.52/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/killJobsInTask.py` & `panda-server-0.0.52/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/killProdJobs.py` & `panda-server-0.0.52/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/killTask.py` & `panda-server-0.0.52/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/killUser.py` & `panda-server-0.0.52/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/lsst/lsstSubmit.py` & `panda-server-0.0.52/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda-server-0.0.52/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda-server-0.0.52/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/reassignSite.py` & `panda-server-0.0.52/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/reassignTask.py` & `panda-server-0.0.52/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/reassignWaiting.py` & `panda-server-0.0.52/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/reloadInputDS.py` & `panda-server-0.0.52/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/sendCommandToJob.py` & `panda-server-0.0.52/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/setDebugMode.py` & `panda-server-0.0.52/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/setPriority.py` & `panda-server-0.0.52/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testEvgen.py` & `panda-server-0.0.52/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testEvgen17.py` & `panda-server-0.0.52/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testG4sim.py` & `panda-server-0.0.52/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testG4sim17.py` & `panda-server-0.0.52/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda-server-0.0.52/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testGlobalShares.py` & `panda-server-0.0.52/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testJobFlowATLAS.py` & `panda-server-0.0.52/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testReco.py` & `panda-server-0.0.52/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testSimulReco14.py` & `panda-server-0.0.52/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testSiteMap.py` & `panda-server-0.0.52/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/test/testutils.py` & `panda-server-0.0.52/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/userinterface/Client.py` & `panda-server-0.0.52/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/userinterface/UserIF.py` & `panda-server-0.0.52/pandaserver/userinterface/UserIF.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/workflow/pcwl_test.py` & `panda-server-0.0.52/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/workflow/pcwl_utils.py` & `panda-server-0.0.52/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/workflow/psnakemake_test.py` & `panda-server-0.0.52/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/workflow/snakeparser/extensions.py` & `panda-server-0.0.52/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/workflow/snakeparser/log.py` & `panda-server-0.0.52/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/workflow/snakeparser/parser.py` & `panda-server-0.0.52/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/workflow/snakeparser/utils.py` & `panda-server-0.0.52/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/pandaserver/workflow/workflow_utils.py` & `panda-server-0.0.52/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/setup.py` & `panda-server-0.0.52/setup.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/conda_meta.yaml.template` & `panda-server-0.0.52/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/init.d/panda_daemon.exe.template` & `panda-server-0.0.52/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/init.d/panda_httpd.exe.template` & `panda-server-0.0.52/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/init.d/panda_server.exe.template` & `panda-server-0.0.52/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/logrotate.d/panda_server.logrotate.template` & `panda-server-0.0.52/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda-server-0.0.52/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/panda_server-httpd.conf.rpmnew.template` & `panda-server-0.0.52/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/panda_server-makeSlsXml.exe.template` & `panda-server-0.0.52/templates/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/panda_server-vomsrenew.exe.template` & `panda-server-0.0.52/templates/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/panda_server.cfg.rpmnew.template` & `panda-server-0.0.52/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/pandasrv.cron.template` & `panda-server-0.0.52/templates/pandasrv.cron.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.51/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda-server-0.0.52/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files identical despite different names*

