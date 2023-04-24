# Comparing `tmp/robotframework-confluentkafkalibrary-1.9.0.post1.tar.gz` & `tmp/robotframework-confluentkafkalibrary-2.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-confluentkafkalibrary-1.9.0.post1.tar", last modified: Thu Jun 30 15:00:03 2022, max compression
+gzip compressed data, was "robotframework-confluentkafkalibrary-2.0.2.post1.tar", last modified: Mon Apr 24 19:04:41 2023, max compression
```

## Comparing `robotframework-confluentkafkalibrary-1.9.0.post1.tar` & `robotframework-confluentkafkalibrary-2.0.2.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 15:00:03.750795 robotframework-confluentkafkalibrary-1.9.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)    11344 2022-06-30 14:59:50.000000 robotframework-confluentkafkalibrary-1.9.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-06-30 15:00:03.746795 robotframework-confluentkafkalibrary-1.9.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2692 2022-06-30 14:59:50.000000 robotframework-confluentkafkalibrary-1.9.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-30 15:00:03.750795 robotframework-confluentkafkalibrary-1.9.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-06-30 14:59:50.000000 robotframework-confluentkafkalibrary-1.9.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 15:00:03.746795 robotframework-confluentkafkalibrary-1.9.0.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 15:00:03.746795 robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/
--rw-r--r--   0 runner    (1001) docker     (121)     6517 2022-06-30 14:59:50.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4289 2022-06-30 14:59:50.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/admin_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15004 2022-06-30 14:59:50.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-06-30 14:59:50.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/producer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-06-30 14:59:50.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-30 14:59:50.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 15:00:03.746795 robotframework-confluentkafkalibrary-1.9.0.post1/src/robotframework_confluentkafkalibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-06-30 15:00:03.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-06-30 15:00:03.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-30 15:00:03.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-06-30 15:00:03.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-30 15:00:03.000000 robotframework-confluentkafkalibrary-1.9.0.post1/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:04:41.340535 robotframework-confluentkafkalibrary-2.0.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-24 19:04:41.336535 robotframework-confluentkafkalibrary-2.0.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:04:41.340535 robotframework-confluentkafkalibrary-2.0.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:04:41.336535 robotframework-confluentkafkalibrary-2.0.2.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:04:41.336535 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 19:04:30.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:04:41.336535 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 19:04:41.000000 robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/top_level.txt
```

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/LICENSE` & `robotframework-confluentkafkalibrary-2.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/PKG-INFO` & `robotframework-confluentkafkalibrary-2.0.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 1.9.0.post1
+Version: 2.0.2.post1
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
```

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/README.md` & `robotframework-confluentkafkalibrary-2.0.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/setup.py` & `robotframework-confluentkafkalibrary-2.0.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,16 +24,17 @@
           "License :: OSI Approved :: Apache Software License",
           "Operating System :: OS Independent",
           "Programming Language :: Python",
           "Topic :: Software Development :: Testing"
       ],
       install_requires = [
           'robotframework >= 3.2.1',
-          'confluent-kafka == 1.9.0',
+          'confluent-kafka == 2.0.2',
           'requests >= 2.25.1',
           'avro-python3 >= 1.10.1',
           'fastavro >= 1.3.2',
-          'jsonschema >= 3.2.0'
+          'jsonschema >= 3.2.0',
+          'protobuf >= 4.22.0'
       ],
       package_dir  = {'' : 'src'},
       packages    = ['ConfluentKafkaLibrary'],
       )
```

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/__init__.py` & `robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import confluent_kafka
+from confluent_kafka import ConsumerGroupState
 from confluent_kafka.schema_registry import SchemaRegistryClient
 from confluent_kafka.admin import AdminClient, NewTopic, NewPartitions, ConfigResource
 from robot.libraries.BuiltIn import BuiltIn, RobotNotRunningError
 
 from .consumer import KafkaConsumer
 from .producer import KafkaProducer
 from .admin_client import KafkaAdminClient
@@ -83,14 +84,22 @@
             BuiltIn().set_global_variable('${OFFSET_BEGINNING}', confluent_kafka.OFFSET_BEGINNING)
             BuiltIn().set_global_variable('${OFFSET_END}', confluent_kafka.OFFSET_END)
             BuiltIn().set_global_variable('${OFFSET_STORED}', confluent_kafka.OFFSET_STORED)
             BuiltIn().set_global_variable('${OFFSET_INVALID}', confluent_kafka.OFFSET_INVALID)
             BuiltIn().set_global_variable('${ADMIN_RESOURCE_BROKER}', confluent_kafka.admin.RESOURCE_BROKER)
             BuiltIn().set_global_variable('${ADMIN_RESOURCE_GROUP}', confluent_kafka.admin.RESOURCE_GROUP)
             BuiltIn().set_global_variable('${ADMIN_RESOURCE_TOPIC}', confluent_kafka.admin.RESOURCE_TOPIC)
+
+            BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_UNKNOWN}', confluent_kafka.ConsumerGroupState.UNKOWN)
+            BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_PREPARING_REBALANCING}', confluent_kafka.ConsumerGroupState.PREPARING_REBALANCING)
+            BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_COMPLETING_REBALANCING}', confluent_kafka.ConsumerGroupState.COMPLETING_REBALANCING)
+            BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_STABLE}', confluent_kafka.ConsumerGroupState.STABLE)
+            BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_DEAD}', confluent_kafka.ConsumerGroupState.DEAD)
+            BuiltIn().set_global_variable('${CONSUMER_GROUP_STATE_EMPTY}', confluent_kafka.ConsumerGroupState.EMPTY)
+
         except RobotNotRunningError as e:
             pass
 
     def list_topics(self, group_id, topic=None):
         """Request Metadata from cluster. Could be executed with consumer or producer group_id too.
         - ``topic`` (str):  If specified, only request info about this topic, else return for all topics in cluster.
         Default: `None`.
```

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/consumer.py` & `robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/consumer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import uuid
 from threading import Thread
 from confluent_kafka import Consumer, KafkaException, KafkaError, TopicPartition
 from confluent_kafka import DeserializingConsumer
 from confluent_kafka.avro.serializer import SerializerError
 from confluent_kafka.avro import AvroConsumer
+from confluent_kafka.admin import AdminClient
 
 
 class GetMessagesThread(Thread):
 
     def __init__(
         self,
         server='127.0.0.1',
@@ -16,14 +17,16 @@
         group_id=None,
         only_value=True,
         **kwargs
     ):
 
         super().__init__()
         self.daemon = True
+        self.server = server
+        self.port = port
         self._is_running = True
         self.only_value = only_value
         self.consumer = KafkaConsumer()
         self.group_id = self.consumer.create_consumer(group_id=group_id,
                                                       server=server,
                                                       port=port,
                                                       **kwargs)
@@ -40,20 +43,36 @@
             try:
                 self.messages += self.consumer.poll(group_id=self.group_id, only_value=self.only_value)
             except RuntimeError:
                 self.consumer.unsubscribe(self.group_id)
                 self.consumer.close_consumer(self.group_id)
                 self._is_running = False
 
+    def get_group_id(self):
+        return self.group_id
+
     def get_messages(self):
         return self.messages[:]
 
     def clear_messages(self):
         self.messages.clear()
 
+    def stop_consumer(self):
+        self._is_running = False
+        self.join()
+        self.consumer.unsubscribe(self.group_id)
+        self.consumer.close_consumer(self.group_id)
+        admin_client = AdminClient({'bootstrap.servers': f'{self.server}:{self.port}'})
+        response = admin_client.delete_consumer_groups([self.group_id], request_timeout=10)
+        try:
+            response[self.group_id].result()
+        except Exception as e:
+            return e
+        return response[self.group_id].exception()
+
 
 class KafkaConsumer():
 
     def __init__(self):
         self.consumers = {}
 
     def create_consumer(
@@ -344,16 +363,23 @@
         """
         records = self._decode_data(
             data=running_thread.get_messages(),
             decode_format=decode_format
         )
         return records
 
+    def get_thread_group_id(self, running_thread):
+        return running_thread.get_group_id()
+
     def clear_messages_from_thread(self, running_thread):
         """Remove all records gathered from specific thread
         - ``running_thread`` (Thread object) - thread which was executed with
             `Start Consumer Threaded` keyword
         """
         try:
             running_thread.clear_messages()
-        except:
-            print('Messages was not removed from thread %s!', running_thread)
+        except Exception as e:
+            return f"Messages were not removed from thread {running_thread}!\n{e}"
+
+    def stop_consumer_threaded(self, running_thread):
+        resp = running_thread.stop_consumer()
+        return resp
```

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/producer.py` & `robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/producer.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/src/ConfluentKafkaLibrary/serialization.py` & `robotframework-confluentkafkalibrary-2.0.2.post1/src/ConfluentKafkaLibrary/serialization.py`

 * *Files identical despite different names*

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO` & `robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-confluentkafkalibrary
-Version: 1.9.0.post1
+Version: 2.0.2.post1
 Summary: Confluent Kafka library for Robot Framework
 Home-page: https://github.com/robooo/robotframework-ConfluentKafkaLibrary
 Author: Robert Karasek
 Author-email: <robo.karasek@gmail.com>
 License: Apache License 2.0
 Keywords: robotframework confluent kafka
 Platform: any
```

### Comparing `robotframework-confluentkafkalibrary-1.9.0.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt` & `robotframework-confluentkafkalibrary-2.0.2.post1/src/robotframework_confluentkafkalibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

