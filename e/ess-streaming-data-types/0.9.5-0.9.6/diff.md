# Comparing `tmp/ess_streaming_data_types-0.9.5.tar.gz` & `tmp/ess_streaming_data_types-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ess_streaming_data_types-0.9.5.tar", last modified: Fri Oct 30 10:03:17 2020, max compression
+gzip compressed data, was "dist/ess_streaming_data_types-0.9.6.tar", last modified: Wed Dec  2 11:46:59 2020, max compression
```

## Comparing `ess_streaming_data_types-0.9.5.tar` & `ess_streaming_data_types-0.9.6.tar`

### file list

```diff
@@ -1,130 +1,119 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1374 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/LICENSE
--rw-rw-r--   0 matt      (1000) matt      (1000)       75 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/MANIFEST.in
--rw-rw-r--   0 matt      (1000) matt      (1000)       66 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/Makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)     2697 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     1838 2020-10-28 07:32:11.000000 ess_streaming_data_types-0.9.5/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.972326 ess_streaming_data_types-0.9.5/ess_streaming_data_types.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)     2697 2020-10-30 10:03:17.000000 ess_streaming_data_types-0.9.5/ess_streaming_data_types.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)     5434 2020-10-30 10:03:17.000000 ess_streaming_data_types-0.9.5/ess_streaming_data_types.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2020-10-30 10:03:17.000000 ess_streaming_data_types-0.9.5/ess_streaming_data_types.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       60 2020-10-30 10:03:17.000000 ess_streaming_data_types-0.9.5/ess_streaming_data_types.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       21 2020-10-30 10:03:17.000000 ess_streaming_data_types-0.9.5/ess_streaming_data_types.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       67 2020-06-22 09:43:25.000000 ess_streaming_data_types-0.9.5/requirements-dev.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       24 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/requirements.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)      995 2020-10-30 10:01:45.000000 ess_streaming_data_types-0.9.5/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.972326 ess_streaming_data_types-0.9.5/streaming_data_types/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1915 2020-10-28 07:32:11.000000 ess_streaming_data_types-0.9.5/streaming_data_types/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2688 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/action_response_answ.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2202 2020-10-28 07:32:11.000000 ess_streaming_data_types-0.9.5/streaming_data_types/area_detector_NDAr.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1944 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/epics_connection_info_ep00.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3669 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/eventdata_ev42.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.972326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.976326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/NDAr_NDArray_schema/
--rw-rw-r--   0 matt      (1000) matt      (1000)      280 2020-10-28 07:32:11.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/NDAr_NDArray_schema/DType.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4929 2020-10-28 07:32:11.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/NDAr_NDArray_schema/NDArray.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3037 2020-10-28 07:32:11.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/NDAr_NDArray_schema/NDAttribute.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-10-28 07:32:11.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/NDAr_NDArray_schema/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      793 2020-10-28 07:32:11.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/NDAr_NDArray_schema/epicsTimeStamp.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.976326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/action_response_answ/
--rw-rw-r--   0 matt      (1000) matt      (1000)      146 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/action_response_answ/ActionOutcome.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3892 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/action_response_answ/ActionResponse.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      148 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/action_response_answ/ActionType.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/action_response_answ/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.976326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/epics_connection_info_ep00/
--rw-rw-r--   0 matt      (1000) matt      (1000)     2228 2020-07-02 06:08:15.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/epics_connection_info_ep00/EpicsConnectionInfo.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      207 2020-07-02 06:08:15.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/epics_connection_info_ep00/EventType.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-07-02 06:08:15.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/epics_connection_info_ep00/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.976326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/eventdata_ev42/
--rw-rw-r--   0 matt      (1000) matt      (1000)     4966 2020-05-06 13:48:50.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/eventdata_ev42/EventMessage.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      165 2020-05-06 13:48:50.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/eventdata_ev42/FacilityData.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-05-06 13:48:50.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/eventdata_ev42/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.976326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/finished_writing_wrdn/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3297 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/finished_writing_wrdn/FinishedWriting.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/finished_writing_wrdn/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.976326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/forwarder_config_update_rf5k/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1914 2020-07-16 14:41:09.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/forwarder_config_update_rf5k/ConfigUpdate.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      145 2020-07-16 14:41:09.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/forwarder_config_update_rf5k/Protocol.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2032 2020-07-16 14:41:09.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/forwarder_config_update_rf5k/Stream.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      156 2020-07-16 14:41:09.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/forwarder_config_update_rf5k/UpdateType.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-07-16 14:41:09.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/forwarder_config_update_rf5k/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.976326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/
--rw-rw-r--   0 matt      (1000) matt      (1000)      195 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/Array.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1686 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/ArrayDouble.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1675 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/ArrayFloat.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1662 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/ArrayUInt.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1673 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/ArrayULong.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2678 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/DimensionMetaData.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     7087 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/EventHistogram.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.980326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/isis_event_info_is84/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1689 2020-05-06 13:48:50.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/isis_event_info_is84/ISISData.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      139 2020-05-06 13:48:50.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/isis_event_info_is84/RunState.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-05-06 13:48:50.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/isis_event_info_is84/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/
--rw-rw-r--   0 matt      (1000) matt      (1000)      193 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/AlarmSeverity.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      457 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/AlarmStatus.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1658 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayByte.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1686 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayDouble.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1675 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayFloat.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1649 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayInt.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1660 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayLong.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1671 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayShort.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1383 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayString.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1671 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayUByte.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1662 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayUInt.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1673 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayULong.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1684 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayUShort.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      871 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Byte.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      927 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Double.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      919 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Float.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      865 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Int.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2853 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/LogData.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      873 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Long.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      881 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Short.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      931 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/String.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      881 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/UByte.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      905 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/UInt.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      913 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ULong.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      921 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/UShort.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      491 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Value.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/nicos_cache_ns10/
--rw-rw-r--   0 matt      (1000) matt      (1000)     2467 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/nicos_cache_ns10/CacheEntry.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/nicos_cache_ns10/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/run_start_pl72/
--rw-rw-r--   0 matt      (1000) matt      (1000)     5648 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/run_start_pl72/RunStart.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/run_start_pl72/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/run_stop_6s4t/
--rw-rw-r--   0 matt      (1000) matt      (1000)     2734 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/run_stop_6s4t/RunStop.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/run_stop_6s4t/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/status_x5f2/
--rw-rw-r--   0 matt      (1000) matt      (1000)     3549 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/status_x5f2/Status.py
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-05-07 08:01:44.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/status_x5f2/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/timestamps_tdct/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-05-23 08:22:13.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/timestamps_tdct/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2459 2020-05-23 08:22:13.000000 ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/timestamps_tdct/timestamp.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2790 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/finished_writing_wrdn.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3766 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/forwarder_config_update_rf5k.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     9823 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/histogram_hs00.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    21261 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/logdata_f142.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1513 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/nicos_cache_ns10.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3927 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/run_start_pl72.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2288 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/run_stop_6s4t.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2456 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/streaming_data_types/status_x5f2.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1638 2020-10-28 07:32:11.000000 ess_streaming_data_types-0.9.5/streaming_data_types/timestamps_tdct.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      716 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/streaming_data_types/utils.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2020-10-30 10:03:17.984326 ess_streaming_data_types-0.9.5/tests/
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2020-04-27 11:19:29.000000 ess_streaming_data_types-0.9.5/tests/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1367 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/tests/test_6s4t.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1410 2020-07-08 11:00:49.000000 ess_streaming_data_types-0.9.5/tests/test_ep00.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3974 2020-07-08 11:00:49.000000 ess_streaming_data_types-0.9.5/tests/test_ev42.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     7420 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/tests/test_f142.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    13886 2020-07-16 14:41:09.000000 ess_streaming_data_types-0.9.5/tests/test_hs00.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1506 2020-07-08 11:00:49.000000 ess_streaming_data_types-0.9.5/tests/test_ns10.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1989 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/tests/test_pl72.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1959 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/tests/test_rf5k.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2101 2020-08-11 09:25:13.000000 ess_streaming_data_types-0.9.5/tests/test_tdct.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1974 2020-10-22 07:36:42.000000 ess_streaming_data_types-0.9.5/tests/test_x52f.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.839036 ess_streaming_data_types-0.9.6/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1374 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/LICENSE
+-rw-r--r--   0 jonasnilsson (27861982) 14964212       75 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/MANIFEST.in
+-rw-r--r--   0 jonasnilsson (27861982) 14964212       66 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/Makefile
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2697 2020-12-02 11:46:59.838773 ess_streaming_data_types-0.9.6/PKG-INFO
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1838 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/README.md
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.764550 ess_streaming_data_types-0.9.6/ess_streaming_data_types.egg-info/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2697 2020-12-02 11:46:59.000000 ess_streaming_data_types-0.9.6/ess_streaming_data_types.egg-info/PKG-INFO
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     5261 2020-12-02 11:46:59.000000 ess_streaming_data_types-0.9.6/ess_streaming_data_types.egg-info/SOURCES.txt
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        1 2020-12-02 11:46:59.000000 ess_streaming_data_types-0.9.6/ess_streaming_data_types.egg-info/dependency_links.txt
+-rw-r--r--   0 jonasnilsson (27861982) 14964212       60 2020-12-02 11:46:59.000000 ess_streaming_data_types-0.9.6/ess_streaming_data_types.egg-info/requires.txt
+-rw-r--r--   0 jonasnilsson (27861982) 14964212       21 2020-12-02 11:46:59.000000 ess_streaming_data_types-0.9.6/ess_streaming_data_types.egg-info/top_level.txt
+-rw-r--r--   0 jonasnilsson (27861982) 14964212       67 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/requirements-dev.txt
+-rw-r--r--   0 jonasnilsson (27861982) 14964212       24 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/requirements.txt
+-rw-r--r--   0 jonasnilsson (27861982) 14964212       38 2020-12-02 11:46:59.839119 ess_streaming_data_types-0.9.6/setup.cfg
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      995 2020-12-02 11:44:05.000000 ess_streaming_data_types-0.9.6/setup.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.778026 ess_streaming_data_types-0.9.6/streaming_data_types/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1915 2020-12-02 11:43:00.000000 ess_streaming_data_types-0.9.6/streaming_data_types/__init__.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2883 2020-12-02 11:43:00.000000 ess_streaming_data_types-0.9.6/streaming_data_types/action_response_answ.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2202 2020-12-02 11:43:00.000000 ess_streaming_data_types-0.9.6/streaming_data_types/area_detector_NDAr.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1944 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/epics_connection_info_ep00.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     3669 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/eventdata_ev42.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      191 2020-12-02 11:46:28.000000 ess_streaming_data_types-0.9.6/streaming_data_types/exceptions.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.778666 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.780514 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/NDAr_NDArray_schema/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      280 2020-12-02 11:43:00.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/NDAr_NDArray_schema/DType.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     4929 2020-12-02 11:43:00.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/NDAr_NDArray_schema/NDArray.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     3037 2020-12-02 11:43:00.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/NDAr_NDArray_schema/NDAttribute.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/NDAr_NDArray_schema/__init__.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      793 2020-12-02 11:43:00.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/NDAr_NDArray_schema/epicsTimeStamp.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.784158 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/action_response_answ/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      146 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/action_response_answ/ActionOutcome.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     3892 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/action_response_answ/ActionResponse.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      148 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/action_response_answ/ActionType.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/action_response_answ/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.786706 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/epics_connection_info_ep00/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2228 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/epics_connection_info_ep00/EpicsConnectionInfo.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      207 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/epics_connection_info_ep00/EventType.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/epics_connection_info_ep00/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.789030 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/eventdata_ev42/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     4966 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/eventdata_ev42/EventMessage.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      165 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/eventdata_ev42/FacilityData.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/eventdata_ev42/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.790820 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/finished_writing_wrdn/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     3297 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/finished_writing_wrdn/FinishedWriting.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/finished_writing_wrdn/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.795010 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/forwarder_config_update_rf5k/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1914 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/forwarder_config_update_rf5k/ConfigUpdate.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      145 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/forwarder_config_update_rf5k/Protocol.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2032 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/forwarder_config_update_rf5k/Stream.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      156 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/forwarder_config_update_rf5k/UpdateType.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/forwarder_config_update_rf5k/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.802616 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      195 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/Array.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1686 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/ArrayDouble.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1675 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/ArrayFloat.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1662 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/ArrayUInt.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1673 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/ArrayULong.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2678 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/DimensionMetaData.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     7087 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/EventHistogram.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.804823 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/isis_event_info_is84/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1689 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/isis_event_info_is84/ISISData.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      139 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/isis_event_info_is84/RunState.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/isis_event_info_is84/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.830022 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      193 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/AlarmSeverity.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      457 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/AlarmStatus.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1658 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayByte.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1686 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayDouble.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1675 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayFloat.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1649 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayInt.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1660 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayLong.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1671 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayShort.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1383 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayString.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1671 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayUByte.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1662 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayUInt.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1673 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayULong.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1684 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayUShort.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      871 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Byte.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      927 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Double.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      919 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Float.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      865 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Int.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2853 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/LogData.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      873 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Long.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      881 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Short.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      931 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/String.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      881 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/UByte.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      905 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/UInt.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      913 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ULong.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      921 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/UShort.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      491 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Value.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.832016 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/nicos_cache_ns10/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2467 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/nicos_cache_ns10/CacheEntry.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/nicos_cache_ns10/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.833864 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/run_start_pl72/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     5648 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/run_start_pl72/RunStart.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/run_start_pl72/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.835386 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/run_stop_6s4t/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2734 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/run_stop_6s4t/RunStop.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/run_stop_6s4t/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.836947 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/status_x5f2/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     3549 2020-10-22 05:31:54.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/status_x5f2/Status.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/status_x5f2/__init__.py
+drwxr-xr-x   0 jonasnilsson (27861982) 14964212        0 2020-12-02 11:46:59.838358 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/timestamps_tdct/
+-rw-r--r--   0 jonasnilsson (27861982) 14964212        0 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/timestamps_tdct/__init__.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2459 2020-09-01 09:50:31.000000 ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/timestamps_tdct/timestamp.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2790 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/finished_writing_wrdn.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     3766 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/forwarder_config_update_rf5k.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     8781 2020-11-04 01:21:57.000000 ess_streaming_data_types-0.9.6/streaming_data_types/histogram_hs00.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212    21261 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/logdata_f142.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1513 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/nicos_cache_ns10.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     3927 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/run_start_pl72.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2288 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/run_stop_6s4t.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     2456 2020-10-27 22:54:05.000000 ess_streaming_data_types-0.9.6/streaming_data_types/status_x5f2.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212     1638 2020-11-04 01:21:57.000000 ess_streaming_data_types-0.9.6/streaming_data_types/timestamps_tdct.py
+-rw-r--r--   0 jonasnilsson (27861982) 14964212      921 2020-12-02 11:46:28.000000 ess_streaming_data_types-0.9.6/streaming_data_types/utils.py
```

### Comparing `ess_streaming_data_types-0.9.5/LICENSE` & `ess_streaming_data_types-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/PKG-INFO` & `ess_streaming_data_types-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ess_streaming_data_types
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python utilities for handling ESS streamed data
 Home-page: https://github.com/ess-dmsc/python-streaming-data-types
 Author: ScreamingUdder
 License: BSD 2-Clause License
 Description: 
         # Python Streaming Data Types
         Utilities for working with the FlatBuffers schemas used at the European
```

### Comparing `ess_streaming_data_types-0.9.5/README.md` & `ess_streaming_data_types-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/ess_streaming_data_types.egg-info/PKG-INFO` & `ess_streaming_data_types-0.9.6/ess_streaming_data_types.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ess-streaming-data-types
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python utilities for handling ESS streamed data
 Home-page: https://github.com/ess-dmsc/python-streaming-data-types
 Author: ScreamingUdder
 License: BSD 2-Clause License
 Description: 
         # Python Streaming Data Types
         Utilities for working with the FlatBuffers schemas used at the European
```

### Comparing `ess_streaming_data_types-0.9.5/ess_streaming_data_types.egg-info/SOURCES.txt` & `ess_streaming_data_types-0.9.6/ess_streaming_data_types.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ess_streaming_data_types.egg-info/requires.txt
 ess_streaming_data_types.egg-info/top_level.txt
 streaming_data_types/__init__.py
 streaming_data_types/action_response_answ.py
 streaming_data_types/area_detector_NDAr.py
 streaming_data_types/epics_connection_info_ep00.py
 streaming_data_types/eventdata_ev42.py
+streaming_data_types/exceptions.py
 streaming_data_types/finished_writing_wrdn.py
 streaming_data_types/forwarder_config_update_rf5k.py
 streaming_data_types/histogram_hs00.py
 streaming_data_types/logdata_f142.py
 streaming_data_types/nicos_cache_ns10.py
 streaming_data_types/run_start_pl72.py
 streaming_data_types/run_stop_6s4t.py
@@ -91,19 +92,8 @@
 streaming_data_types/fbschemas/run_start_pl72/RunStart.py
 streaming_data_types/fbschemas/run_start_pl72/__init__.py
 streaming_data_types/fbschemas/run_stop_6s4t/RunStop.py
 streaming_data_types/fbschemas/run_stop_6s4t/__init__.py
 streaming_data_types/fbschemas/status_x5f2/Status.py
 streaming_data_types/fbschemas/status_x5f2/__init__.py
 streaming_data_types/fbschemas/timestamps_tdct/__init__.py
-streaming_data_types/fbschemas/timestamps_tdct/timestamp.py
-tests/__init__.py
-tests/test_6s4t.py
-tests/test_ep00.py
-tests/test_ev42.py
-tests/test_f142.py
-tests/test_hs00.py
-tests/test_ns10.py
-tests/test_pl72.py
-tests/test_rf5k.py
-tests/test_tdct.py
-tests/test_x52f.py
+streaming_data_types/fbschemas/timestamps_tdct/timestamp.py
```

### Comparing `ess_streaming_data_types-0.9.5/setup.py` & `ess_streaming_data_types-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         LONG_DESCRIPTION = "\n" + f.read()
 except Exception as error:
     print("COULD NOT GET LONG DESC: {}".format(error))
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name="ess_streaming_data_types",
-    version="0.9.5",
+    version="0.9.6",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author="ScreamingUdder",
     url="https://github.com/ess-dmsc/python-streaming-data-types",
     license="BSD 2-Clause License",
     packages=find_packages(exclude=["tests", "tests.*"]),
```

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/__init__.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/action_response_answ.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/action_response_answ.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,17 +58,21 @@
     ),
 )
 
 
 def deserialise_answ(buffer: Union[bytearray, bytes]):
     check_schema_identifier(buffer, FILE_IDENTIFIER)
     answ_message = ActionResponse.ActionResponse.GetRootAsActionResponse(buffer, 0)
+    max_time = datetime(year=9000, month=1, day=1, hour=0, minute=0, second=0).timestamp()
+    used_timestamp = answ_message.StopTime() / 1000
+    if used_timestamp > max_time:
+        used_timestamp = max_time
     return Response(
         service_id=answ_message.ServiceId().decode("utf-8"),
         job_id=answ_message.JobId().decode("utf-8"),
         command_id=answ_message.CommandId().decode("utf-8"),
         action=answ_message.Action(),
         outcome=answ_message.Outcome(),
         message=answ_message.Message().decode("utf-8"),
         status_code=answ_message.StatusCode(),
-        stop_time=datetime.fromtimestamp(answ_message.StopTime() / 1000),
+        stop_time=datetime.fromtimestamp(used_timestamp),
     )
```

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/area_detector_NDAr.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/area_detector_NDAr.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/epics_connection_info_ep00.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/epics_connection_info_ep00.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/eventdata_ev42.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/eventdata_ev42.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/NDAr_NDArray_schema/NDArray.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/NDAr_NDArray_schema/NDArray.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/NDAr_NDArray_schema/NDAttribute.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/NDAr_NDArray_schema/NDAttribute.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/NDAr_NDArray_schema/epicsTimeStamp.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/NDAr_NDArray_schema/epicsTimeStamp.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/action_response_answ/ActionResponse.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/action_response_answ/ActionResponse.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/epics_connection_info_ep00/EpicsConnectionInfo.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/epics_connection_info_ep00/EpicsConnectionInfo.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/eventdata_ev42/EventMessage.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/eventdata_ev42/EventMessage.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/finished_writing_wrdn/FinishedWriting.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/finished_writing_wrdn/FinishedWriting.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/forwarder_config_update_rf5k/ConfigUpdate.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/forwarder_config_update_rf5k/ConfigUpdate.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/forwarder_config_update_rf5k/Stream.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/forwarder_config_update_rf5k/Stream.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/ArrayDouble.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/ArrayDouble.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/ArrayFloat.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/ArrayFloat.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/ArrayUInt.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/ArrayUInt.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/ArrayULong.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/ArrayULong.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/DimensionMetaData.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/DimensionMetaData.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/histogram_hs00/EventHistogram.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/histogram_hs00/EventHistogram.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/isis_event_info_is84/ISISData.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/isis_event_info_is84/ISISData.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayByte.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayByte.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayDouble.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayDouble.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayFloat.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayFloat.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayInt.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayInt.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayLong.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayLong.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayShort.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayShort.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayString.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayString.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayUByte.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayUByte.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayUInt.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayUInt.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayULong.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayULong.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ArrayUShort.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ArrayUShort.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Byte.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Byte.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Double.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Double.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Float.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Float.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Int.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Int.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/LogData.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/LogData.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Long.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Long.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/Short.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/Short.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/String.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/String.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/UByte.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/UByte.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/UInt.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/UInt.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/ULong.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/ULong.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/logdata_f142/UShort.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/logdata_f142/UShort.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/nicos_cache_ns10/CacheEntry.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/nicos_cache_ns10/CacheEntry.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/run_start_pl72/RunStart.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/run_start_pl72/RunStart.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/run_stop_6s4t/RunStop.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/run_stop_6s4t/RunStop.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/status_x5f2/Status.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/status_x5f2/Status.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/fbschemas/timestamps_tdct/timestamp.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/fbschemas/timestamps_tdct/timestamp.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/finished_writing_wrdn.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/finished_writing_wrdn.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/forwarder_config_update_rf5k.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/forwarder_config_update_rf5k.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/histogram_hs00.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/histogram_hs00.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from functools import reduce
-import operator
 import flatbuffers
 import numpy
 import streaming_data_types.fbschemas.histogram_hs00.ArrayFloat as ArrayFloat
 import streaming_data_types.fbschemas.histogram_hs00.ArrayDouble as ArrayDouble
 import streaming_data_types.fbschemas.histogram_hs00.ArrayUInt as ArrayUInt
 import streaming_data_types.fbschemas.histogram_hs00.ArrayULong as ArrayULong
 import streaming_data_types.fbschemas.histogram_hs00.DimensionMetaData as DimensionMetaData
@@ -89,15 +87,15 @@
     return hist
 
 
 def _serialise_metadata(builder, length, edges, unit, label):
     unit_offset = builder.CreateString(unit)
     label_offset = builder.CreateString(label)
 
-    bins_offset, bin_type = _serialise_array(builder, len(edges), edges)
+    bins_offset, bin_type = _serialise_array(builder, edges)
 
     DimensionMetaData.DimensionMetaDataStart(builder)
     DimensionMetaData.DimensionMetaDataAddLength(builder, length)
     DimensionMetaData.DimensionMetaDataAddBinBoundaries(builder, bins_offset)
     DimensionMetaData.DimensionMetaDataAddBinBoundariesType(builder, bin_type)
     DimensionMetaData.DimensionMetaDataAddLabel(builder, label_offset)
     DimensionMetaData.DimensionMetaDataAddUnit(builder, unit_offset)
@@ -120,47 +118,42 @@
     builder.ForceDefaults(True)
     if "source" in histogram:
         source_offset = builder.CreateString(histogram["source"])
     if "info" in histogram:
         info_offset = builder.CreateString(histogram["info"])
 
     # Build shape array
-    rank = len(histogram["current_shape"])
-    EventHistogram.EventHistogramStartCurrentShapeVector(builder, rank)
-    # FlatBuffers builds arrays backwards
-    for s in reversed(histogram["current_shape"]):
-        builder.PrependUint32(s)
-    shape_offset = builder.EndVector(rank)
+    shape_offset = builder.CreateNumpyVector(
+        numpy.array(histogram["current_shape"]).astype(numpy.uint32)
+    )
 
     # Build dimensions metadata
     metadata = []
     for meta in histogram["dim_metadata"]:
         unit = "" if "unit" not in meta else meta["unit"]
         label = "" if "label" not in meta else meta["label"]
         metadata.append(
             _serialise_metadata(
                 builder, meta["length"], meta["bin_boundaries"], unit, label
             )
         )
 
+    rank = len(histogram["current_shape"])
     EventHistogram.EventHistogramStartDimMetadataVector(builder, rank)
     # FlatBuffers builds arrays backwards
     for m in reversed(metadata):
         builder.PrependUOffsetTRelative(m)
     metadata_vector = builder.EndVector(rank)
 
     # Build the data
-    data_len = reduce(operator.mul, histogram["current_shape"], 1)
-    data_offset, data_type = _serialise_array(builder, data_len, histogram["data"])
+    data_offset, data_type = _serialise_array(builder, histogram["data"])
 
     errors_offset = None
     if "errors" in histogram:
-        errors_offset, error_type = _serialise_array(
-            builder, data_len, histogram["errors"]
-        )
+        errors_offset, error_type = _serialise_array(builder, histogram["errors"])
 
     # Build the actual buffer
     EventHistogram.EventHistogramStart(builder)
     if info_offset:
         EventHistogram.EventHistogramAddInfo(builder, info_offset)
     EventHistogram.EventHistogramAddData(builder, data_offset)
     EventHistogram.EventHistogramAddCurrentShape(builder, shape_offset)
@@ -178,77 +171,61 @@
         )
     hist_message = EventHistogram.EventHistogramEnd(builder)
 
     builder.Finish(hist_message, file_identifier=FILE_IDENTIFIER)
     return bytes(builder.Output())
 
 
-def _serialise_array(builder, data_len, data):
+def _serialise_array(builder, data):
     flattened_data = numpy.asarray(data).flatten()
 
     # Carefully preserve explicitly supported types
     if numpy.issubdtype(flattened_data.dtype, numpy.uint32):
-        return _serialise_uint32(builder, data_len, flattened_data)
+        return _serialise_uint32(builder, flattened_data)
     if numpy.issubdtype(flattened_data.dtype, numpy.uint64):
-        return _serialise_uint64(builder, data_len, flattened_data)
+        return _serialise_uint64(builder, flattened_data)
     if numpy.issubdtype(flattened_data.dtype, numpy.float32):
-        return _serialise_float(builder, data_len, flattened_data)
+        return _serialise_float(builder, flattened_data)
     if numpy.issubdtype(flattened_data.dtype, numpy.float64):
-        return _serialise_double(builder, data_len, flattened_data)
+        return _serialise_double(builder, flattened_data)
 
     # Otherwise if it looks like an int then use uint64, or use double as last resort
     if numpy.issubdtype(flattened_data.dtype, numpy.int64):
-        return _serialise_uint64(builder, data_len, flattened_data)
+        return _serialise_uint64(builder, flattened_data)
 
-    return _serialise_double(builder, data_len, flattened_data)
+    return _serialise_double(builder, flattened_data)
 
 
-def _serialise_float(builder, data_len, flattened_data):
+def _serialise_float(builder, flattened_data):
     data_type = Array.ArrayFloat
-    ArrayFloat.ArrayFloatStartValueVector(builder, data_len)
-    # FlatBuffers builds arrays backwards
-    for x in reversed(flattened_data):
-        builder.PrependFloat32(x)
-    data_vector = builder.EndVector(data_len)
+    data_vector = builder.CreateNumpyVector(flattened_data)
     ArrayFloat.ArrayFloatStart(builder)
     ArrayFloat.ArrayFloatAddValue(builder, data_vector)
     data_offset = ArrayFloat.ArrayFloatEnd(builder)
     return data_offset, data_type
 
 
-def _serialise_double(builder, data_len, flattened_data):
+def _serialise_double(builder, flattened_data):
     data_type = Array.ArrayDouble
-    ArrayDouble.ArrayDoubleStartValueVector(builder, data_len)
-    # FlatBuffers builds arrays backwards
-    for x in reversed(flattened_data):
-        builder.PrependFloat64(x)
-    data_vector = builder.EndVector(data_len)
+    data_vector = builder.CreateNumpyVector(flattened_data)
     ArrayDouble.ArrayDoubleStart(builder)
     ArrayDouble.ArrayDoubleAddValue(builder, data_vector)
     data_offset = ArrayDouble.ArrayDoubleEnd(builder)
     return data_offset, data_type
 
 
-def _serialise_uint32(builder, data_len, flattened_data):
+def _serialise_uint32(builder, flattened_data):
     data_type = Array.ArrayUInt
-    ArrayUInt.ArrayUIntStartValueVector(builder, data_len)
-    # FlatBuffers builds arrays backwards
-    for x in reversed(flattened_data):
-        builder.PrependUint32(x)
-    data_vector = builder.EndVector(data_len)
+    data_vector = builder.CreateNumpyVector(flattened_data)
     ArrayUInt.ArrayUIntStart(builder)
     ArrayUInt.ArrayUIntAddValue(builder, data_vector)
     data_offset = ArrayUInt.ArrayUIntEnd(builder)
     return data_offset, data_type
 
 
-def _serialise_uint64(builder, data_len, flattened_data):
+def _serialise_uint64(builder, flattened_data):
     data_type = Array.ArrayULong
-    ArrayULong.ArrayULongStartValueVector(builder, data_len)
-    # FlatBuffers builds arrays backwards
-    for x in reversed(flattened_data):
-        builder.PrependUint64(x)
-    data_vector = builder.EndVector(data_len)
+    data_vector = builder.CreateNumpyVector(flattened_data)
     ArrayULong.ArrayULongStart(builder)
     ArrayULong.ArrayULongAddValue(builder, data_vector)
     data_offset = ArrayULong.ArrayULongEnd(builder)
     return data_offset, data_type
```

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/logdata_f142.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/logdata_f142.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/nicos_cache_ns10.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/nicos_cache_ns10.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/run_start_pl72.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/run_start_pl72.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/run_stop_6s4t.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/run_stop_6s4t.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/status_x5f2.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/status_x5f2.py`

 * *Files identical despite different names*

### Comparing `ess_streaming_data_types-0.9.5/streaming_data_types/timestamps_tdct.py` & `ess_streaming_data_types-0.9.6/streaming_data_types/timestamps_tdct.py`

 * *Files identical despite different names*

