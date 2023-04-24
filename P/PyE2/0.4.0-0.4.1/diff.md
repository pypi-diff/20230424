# Comparing `tmp/pye2-0.4.0.tar.gz` & `tmp/pye2-0.4.1.tar.gz`

## Comparing `pye2-0.4.0.tar` & `pye2-0.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.4.0/TODOs.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.4.0/__init__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pye2-0.4.0/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.4.0/winrun.bat
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/version.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/base/__init__.py
--rw-r--r--   0        0        0    22351 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/base/generic_session.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/base/logger.py
--rw-r--r--   0        0        0    22904 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/base/pipeline.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/const/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/const/base.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/const/comms.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/const/misc.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/default/__init__.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/consts.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/mixins/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/io_formatter/mixins/plugins_manager_mixin.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/utils/code.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.4.0/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/.example_env
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/attach_example.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/ex1.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/hello.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/remote_exec.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/save_images.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/decentralized/dedist_example.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/decentralized/dedist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.4.0/xperimental/decentralized/dedist_example_worker.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.4.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.4.0/LICENSE
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 pye2-0.4.0/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pye2-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 pye2-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pye2-0.4.1/TODOs.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pye2-0.4.1/__init__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pye2-0.4.1/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.4.1/winrun.bat
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 pye2-0.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/version.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    22197 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/logger.py
+-rw-r--r--   0        0        0    22815 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/base.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/comms.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/misc.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/consts.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/mixins/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/io_formatter/mixins/plugins_manager_mixin.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pye2-0.4.1/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/.example_env
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/attach_example.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/ex1.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/hello.py
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/remote_exec.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/save_images.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/decentralized/dedist_example.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/decentralized/dedist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.4.1/xperimental/decentralized/dedist_example_worker.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pye2-0.4.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.4.1/LICENSE
+-rw-r--r--   0        0        0    11863 2020-02-02 00:00:00.000000 pye2-0.4.1/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pye2-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 pye2-0.4.1/PKG-INFO
```

### Comparing `pye2-0.4.0/.github/workflows/python-publish.yml` & `pye2-0.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/base/__init__.py` & `pye2-0.4.1/PyE2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/base/generic_session.py` & `pye2-0.4.1/PyE2/base/generic_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,20 +94,18 @@
         Callback that handles heartbeats received from this network.
         As arguments, it has a reference to this Session object, the node name and the heartbeat payload.
         Defaults to None.
     silent : bool, optional
         This flag will disable debug logs, set to 'False` for a more verbose log, by default True
     """
     if log is None:
-      log = Logger()
+      log = Logger(silent=silent)
 
     super(GenericSession, self).__init__()
 
-    self.silent = silent
-
     # maybe read config from file?
     self._config = {**self.default_config, **config}
     self.log = log
     self.name = name
 
     self._online_boxes = {}
     self._last_seen_boxes = {}
@@ -315,15 +313,15 @@
     -------
 
     """
     self.log.P(*args, **kwargs)
 
   def D(self, *args, **kwargs):
     """
-    Call the `Logger.P` method if the session was created with the silent argument set to `False`.
+    Call the `Logger.D` method.
     If using the default Logger, this call will print debug info to stdout if `silent` is set to `False`.
 
     Parameters
     ----------
     *args :
 
     msg : obj
@@ -333,16 +331,15 @@
     **kwargs :
 
 
     Returns
     -------
 
     """
-    if not self.silent:
-      self.log.P(*args, **kwargs)
+    self.log.D(*args, **kwargs)
     return
 
   def connect(self) -> None:
     """
     Connect to the communication server using the credentials provided when creating this instance.
     """
     raise NotImplementedError
@@ -424,15 +421,14 @@
         e2id=e2id,
         name=name,
         data_source=data_source,
         config=config,
         plugins=plugins,
         on_data=on_data,
         on_notification=on_notification,
-        silent=self.silent,
         **kwargs
     )
     self.own_pipelines.append(pipeline)
     return pipeline
 
   def close_own_pipelines(self):
     """
@@ -561,15 +557,15 @@
 
     if pipeline_name not in self._online_boxes[e2id]:
       raise Exception("Unable to attach to pipeline. Pipeline does not exist")
 
     pipeline_config = {
         k.lower(): v for k, v in self._online_boxes[e2id][pipeline_name].items()}
     data_source = pipeline_config['type']
-    return Pipeline(self, self.log, e2id=e2id, config={}, data_source=data_source, create_pipeline=False, silent=self.silent, on_data=on_data, on_notification=on_notification, **pipeline_config, **kwargs)
+    return Pipeline(self, self.log, e2id=e2id, config={}, data_source=data_source, create_pipeline=False, on_data=on_data, on_notification=on_notification, **pipeline_config, **kwargs)
 
   def run(self, wait=True, close_session=True, close_pipelines=False):
     """
     This simple method will lock the main thread in a loop.
     This method can call `self.connect()`.
     This method can close the session and can close all pipelines when doing so.
```

### Comparing `pye2-0.4.0/PyE2/base/logger.py` & `pye2-0.4.1/PyE2/base/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 import traceback
 from threading import Lock
 from time import localtime, strftime
 from time import time as tm
 
 
 class Logger():
-  def __init__(self, **kwargs) -> None:
+  def __init__(self, silent=False, **kwargs) -> None:
     self.print_lock = Lock()
+    self.silent = silent
     return
 
   def P(self, msg, **kwargs):
     with self.print_lock:
       print(msg, flush=True)
     return
 
+  def D(self, msg, **kwargs):
+    if not self.silent:
+      self.P(msg, **kwargs)
+
   def get_unique_id(self, size=8):
     """
     efficient and low-colision function for small unique id generation
     """
     import random
     import string
     alphabet = string.ascii_lowercase + string.digits
```

### Comparing `pye2-0.4.0/PyE2/base/pipeline.py` & `pye2-0.4.1/PyE2/base/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 @copyright: Lummetry.AI
 @author: Lummetry\.AI - Stefan Saraev
 @project: 
 @description:
 """
 from time import time
+from .payload import Payload
 from ..utils.code_exec import code_to_base64
 
 
 WAIT_FOR_WORKER = 15
 
 
 class Pipeline(object):
@@ -38,15 +39,15 @@
 
   In the documentation, the following reffer to the same thing:
     `Pipeline` == `Stream`
 
     `Plugin` == `Signature`
   """
 
-  def __init__(self, session, log, *, e2id, name, data_source, config={}, plugins, on_data, silent=True, on_notification=None, **kwargs) -> None:
+  def __init__(self, session, log, *, e2id, name, data_source, config={}, plugins, on_data, on_notification=None, **kwargs) -> None:
     """
     A `Pipeline` is a an object that encapsulates a one-to-many, data acquisition to data processing, flow of data.
 
     A `Pipeline` contains one thread of data acquisition (which does not mean only one source of data), and many
     processing units, usually named `Plugins`. 
 
     An `Instance` is a running thread of a `Plugin` type, and one may want to have multiple `Instances`, because each can be configured independently.
@@ -79,16 +80,14 @@
     on_data : Callable[[Pipeline, str, str, dict], None]
         Callback that handles messages received from any plugin instance. 
         As arguments, it has a reference to this Pipeline object, along with the payload itself.
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
     config : dict, optional
         This is the dictionary that contains the configuration of the acquisition source, by default {}
-    silent : bool, optional
-        This flag will disable debug logs, set to 'False` for a more verbose log, by default True
     on_notification : Callable[[Pipeline, dict], None], optional
         Callback that handles notifications received from this instance. 
         As arguments, it has a reference to this Pipeline object, along with the payload itself. 
         This callback acts as a default payload processor and will be called even if for a given instance
         the user has defined a specific callback.
         Defaults to None.
     create_pipeline : bool
@@ -105,16 +104,14 @@
     self.config = config
     self.plugins = plugins
     self.on_data = on_data
     self.on_notification = on_notification
 
     self.payload = {}
 
-    self.silent = silent
-
     self._create_new_pipeline_on_box(**kwargs)
     return
 
   def _create_new_pipeline_on_box(self, *, create_pipeline=True, **kwargs):
     # beautify the fields that enter in the config file
     kwargs = {k.upper(): v for k, v in kwargs.items()}
 
@@ -345,15 +342,15 @@
           self.P(data, color='r')
         exec_error = data['specificValue']['exec_errors']
 
       if exec_error is not None:
         self.P("Error received from <CUSTOM_EXEC_01:{}>: {}".format(
             instance_id, exec_error), color="r")
       if exec_data is not None:
-        on_data(self, exec_data)
+        on_data(self, Payload(exec_data))
       return
 
     if plain_code is None and plain_code_path is None:
       raise Exception(
           "Need to specify at least one of the following: plain_code, plain_code_path")
 
     if plain_code is not None and plain_code_path is not None:
@@ -482,19 +479,20 @@
     """
     Print info to stdout.
     """
     return self.log.P(*args, **kwargs)
 
   def D(self, *args, **kwargs):
     """
-    Print debug info to stdout if the session was created with the silent argument set to `False`. 
-    The silent argument is passed to the Pipeline object when creating it with `create_pipeline` or `attach_to_pipeline`.
+    Call the `Logger.D` method.
+    If using the default Logger, this call will print debug info to stdout if `silent` is set to `False`.
+    The logger object is passed from the Session object to the Pipeline object when creating
+    it with `create_pipeline` or `attach_to_pipeline`.
     """
-    if not self.silent:
-      return self.log.P(*args, **kwargs)
+    return self.log.D(*args, **kwargs)
 
   def attach_to_instance(self, signature, instance_id, on_data, on_notification=None):
     """
     Attach to an existing instance on this pipeline. 
     This method is useful when one wishes to attach an 
     `on_data` and `on_notification` callbacks to said instance.
```

### Comparing `pye2-0.4.0/PyE2/base/payload/payload.py` & `pye2-0.4.1/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/comm/__init__.py` & `pye2-0.4.1/PyE2/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/comm/amqp_wrapper.py` & `pye2-0.4.1/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/comm/mqtt_wrapper.py` & `pye2-0.4.1/PyE2/comm/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/const/__init__.py` & `pye2-0.4.1/PyE2/const/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/const/base.py` & `pye2-0.4.1/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/const/comms.py` & `pye2-0.4.1/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/const/heartbeat.py` & `pye2-0.4.1/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/const/misc.py` & `pye2-0.4.1/PyE2/const/misc.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/const/payload.py` & `pye2-0.4.1/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/default/mqtt_session.py` & `pye2-0.4.1/PyE2/default/mqtt_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from ..comm import MQTTWrapper
 from ..base import GenericSession
 
 
 # TODO: implement send_command, send_payload,
 #       to be used by the Pipeline class
 class MqttSession(GenericSession):
-  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, filter_workers=None, log=None, on_notification=None, on_heartbeat=None, silent=False, **kwargs) -> None:
+  def __init__(self, *, host, port, user, pwd, name='pySDK', config={}, filter_workers=None, log=None, on_notification=None, on_heartbeat=None, silent=True, **kwargs) -> None:
     super(MqttSession, self).__init__(host=host, port=port, user=user, pwd=pwd, name=name, config=config, filter_workers=filter_workers,
                                       log=log, on_notification=on_notification, on_heartbeat=on_heartbeat, silent=silent, **kwargs)
 
     self._payload_messages = deque()
     self._default_communicator = MQTTWrapper(
         log=self.log,
         config=self._config,
```

### Comparing `pye2-0.4.0/PyE2/io_formatter/__init__.py` & `pye2-0.4.1/PyE2/io_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/io_formatter/consts.py` & `pye2-0.4.1/PyE2/io_formatter/consts.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.4.1/PyE2/io_formatter/io_formatter_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         name=name,
         suffix=ct.PLUGIN_SEARCH.SUFFIX_IO_FORMATTER_PLUGINS,
         safe_locations=ct.PLUGIN_SEARCH.LOC_SAFE_FORMATTER_PLUGINS,
     )
 
     if _class_def is None:
       msg = "Error loading io_formatter plugin '{}'".format(name)
-      self.P(msg, color='r')
+      self.D(msg, color='r')
       # self._create_notification(
       #     notif=ct.STATUS_TYPE.STATUS_EXCEPTION,
       #     msg=msg,
       #     info="No code/script defined for io_formatter plugin '{}' in {}".format(
       #         name, ct.PLUGIN_SEARCH.LOC_IO_FORMATTER_PLUGINS)
       # )
     # endif
@@ -61,33 +61,33 @@
   def get_formatter_by_name(self, name):
     if name not in self._dct_formatters:
       self._create_formatter(name)
     formatter = self._dct_formatters.get(name)
     return formatter
 
   def _create_formatter(self, name):
-    self.P("Creating formatter '{}'".format(name))
+    self.D("Creating formatter '{}'".format(name))
     _cls = self._get_plugin_class(name)
 
     try:
       formatter = _cls(log=self.log, signature=name.lower())
     except Exception as exc:
       msg = "Exception '{}' when initializing io_formatter plugin {}".format(
           exc, name)
-      self.P(msg, color='r')
+      self.D(msg, color='r')
       # self._create_notification(
       #     notif=ct.STATUS_TYPE.STATUS_EXCEPTION,
       #     msg=msg,
       #     autocomplete_info=True
       # )
       raise exc
     # end try-except
 
     self._dct_formatters[name] = formatter
-    self.P("Successfully created IO formatter {}.".format(name))
+    self.D("Successfully created IO formatter {}.".format(name))
     return formatter
 
   def _get_formatter_name_from_payload(self, msg):
     return msg.get(ct.PAYLOAD_DATA.EE_FORMATTER, msg.get(ct.PAYLOAD_DATA.SB_IMPLEMENTATION, ''))
 
   def get_required_formatter_from_payload(self, payload):
     name = self._get_formatter_name_from_payload(payload)
@@ -95,16 +95,19 @@
     if name is not None and name != '':
       if not self.formatter_ready(name):
         msg = "Creating formatter '{}' for decoding message originating <{}:{}>".format(
             name,
             payload.get(ct.PAYLOAD_DATA.INITIATOR_ID),
             payload.get(ct.PAYLOAD_DATA.SESSION_ID)
         )
-        self.P(msg)
+        self.D(msg)
         if False:
           # debug log the payload in question
-          self.P(self.log.dict_pretty_format(payload))
+          self.D(self.log.dict_pretty_format(payload))
       formatter = self.get_formatter_by_name(name)
     return formatter
 
+  def D(self, *args, **kwargs):
+    return self.log.D(*args, **kwargs)
+
   def P(self, *args, **kwargs):
     return self.log.P(*args, **kwargs)
```

### Comparing `pye2-0.4.0/PyE2/io_formatter/base/__init__.py` & `pye2-0.4.1/PyE2/io_formatter/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.4.1/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/io_formatter/default/__init__.py` & `pye2-0.4.1/PyE2/io_formatter/default/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.4.1/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/io_formatter/default/cavi2.py` & `pye2-0.4.1/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/io_formatter/mixins/plugins_manager_mixin.py` & `pye2-0.4.1/PyE2/io_formatter/mixins/plugins_manager_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/utils/code.py` & `pye2-0.4.1/PyE2/utils/code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/PyE2/utils/code_exec.py` & `pye2-0.4.1/PyE2/utils/code_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/xperimental/ex1.py` & `pye2-0.4.1/xperimental/ex1.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,29 +79,33 @@
       config={
           'URL': 0
       },
       plugins=None,
       on_data=pipeline_on_data
   )
 
-  # now we start a perimeter intrustion functionality for low-res cameras with all
+  # now we start a perimeter intrusion functionality for low-res cameras with all
   # the other params default
   pipeline.start_plugin_instance(  # should return an id
       signature='PERIMETER_VIOLATION_01',
       instance_id='inst01',
       params={
           'AI_ENGINE': 'lowres_general_detector'
       },
       on_data=instance_on_data  # default None
   )
 
-  # now start a ciclic process
+  plain_code = """
+result="Data on node"
+  """
+
+  # now start a cyclic process
   instance = pipeline.start_custom_plugin(
       instance_id='inst01',
-      plain_code_path="c:\\Users\\Stefan.saraev\\SolisBox\\core\\xperimental\\pye2sdk\\custom_exec_scripts\\custom_exec_example.txt",
+      plain_code=plain_code,
       params={},
       on_data=another_instance_on_data
   )
 
   try:
     sleep(30)  # wait for some info to appear adn trigger the stop
   except KeyboardInterrupt:
```

### Comparing `pye2-0.4.0/xperimental/remote_exec.py` & `pye2-0.4.1/xperimental/remote_exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,44 +58,50 @@
     plugin.P(payload)
     plugin.P(payload['EE_EVENT_TYPE'])
     plugin.P(payload_box_name)
     plugin.P(payload_active_plugins)
 """
 
 
-def instance_on_data(pipeline, data: Payload):
+def instance_on_data(pipeline: Pipeline, data: Payload):
   global boxes
   data['INSTANCES'].sort()
   boxes[data['BOX']] = (data['INSTANCES'], time())
   return
 
 
-def instance_on_data2(pipeline, data: Payload):
+def instance_on_data2(pipeline: Pipeline, data: Payload):
   return
 
 
-def pipeline_on_data(pipeline, signature, instance, data: Payload):
+def pipeline_on_data(pipeline: Pipeline, signature: str, instance: str, data: Payload):
   pass
 
 
-def pipeline_on_notification(pipeline, notification):
+def pipeline_on_notification(pipeline, notification: dict):
   pipeline.P(
       "Received specific notification for pipeline {}".format(pipeline.name))
   return
 
 
+def sess_on_hb(sess, e2id, hb):
+  act_plug = hb['ACTIVE_PLUGINS']
+  for plug in act_plug:
+    sess.P((e2id, plug['STREAM_ID'], plug['SIGNATURE'], plug['INSTANCE_ID']))
+
+
 dct_server = {
     'host': os.getenv('PYE2_HOSTNAME'),
     'port': int(os.getenv('PYE2_PORT')),
     'user': os.getenv('PYE2_USERNAME'),
     'pwd': os.getenv('PYE2_PASSWORD')
 }
 
 e2id = 'e2id'
-sess = Session(**dct_server)
+sess = Session(**dct_server, on_heartbeat=sess_on_hb)
 sess.connect()
 
 listener_params = {k.upper(): v for k, v in dct_server.items()}
 listener_params["PASS"] = listener_params["PWD"]
 listener_params["TOPIC"] = "lummetry/ctrl"
 
 pipeline = sess.create_pipeline(
@@ -132,15 +138,15 @@
       continue
     net_map_msgs.append(box + ":")
     for i in range(len(instances)):
       (pipeline, signature, instance) = instances[i]
 
       (o_pipeline, o_signature) = (None, None)
       if i != 0:
-        (o_pipeline, o_signature, _) = instances[i-1]
+        (o_pipeline, o_signature, _) = instances[i - 1]
 
       same_pipeline = pipeline == o_pipeline
       same_signature = signature == o_signature
 
       if not same_pipeline:
         net_map_msgs.append(" --- " + pipeline + ":")
       if not same_pipeline or not same_signature:
@@ -151,15 +157,15 @@
   return "\n".join(net_map_msgs)
 
 
 try:
   while True:
     sleep(10)
 
-    pipeline.P(generate_net_map(), color='m')
+    # pipeline.P(generate_net_map(), color='m')
 except KeyboardInterrupt:
   pipeline.P("CTRL+C detected. Closing example..", color='r')
 
 
 pipeline.close()
 # pipeline2.close()
 # now close conn to comm server
```

### Comparing `pye2-0.4.0/xperimental/decentralized/dedist_example.py` & `pye2-0.4.1/xperimental/decentralized/dedist_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/xperimental/decentralized/dedist_example_initiator.py` & `pye2-0.4.1/xperimental/decentralized/dedist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/.gitignore` & `pye2-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/LICENSE` & `pye2-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.4.0/pyproject.toml` & `pye2-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pika", "paho-mqtt", "Pillow", "numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Stefan Saraev", email="stefan.saraev@global-technical.com" },
   { name="Cristan Bleotiu", email="cristan.bleotiu@global-technical.com" },
   { name="Andrei Ionut Damian", email="andrei.damian@lummetry.ai" },
 ]
 description = "PyE2 is an SDK used to communicate with the AiXpand network"
 readme = "README.md"
```

