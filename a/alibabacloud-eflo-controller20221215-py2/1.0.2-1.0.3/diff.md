# Comparing `tmp/alibabacloud_eflo-controller20221215_py2-1.0.2.tar.gz` & `tmp/alibabacloud_eflo-controller20221215_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eflo-controller20221215_py2-1.0.2.tar", last modified: Tue Mar 28 02:43:08 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eflo-controller20221215_py2-1.0.3.tar", last modified: Mon Apr 24 08:13:20 2023, max compression
```

## Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2.tar` & `alibabacloud_eflo-controller20221215_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      148 2023-03-28 02:43:07.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-28 02:43:07.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-28 02:43:07.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2544 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1069 2023-03-28 02:43:07.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1152 2023-03-28 02:43:07.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-28 02:43:07.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26047 2023-03-28 02:43:07.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215/client.py
--rw-r--r--   0 root         (0) root         (0)   147226 2023-03-28 02:43:07.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2544 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      536 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-28 02:43:08.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2965 2023-03-28 02:43:07.000000 alibabacloud_eflo-controller20221215_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26047 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/client.py
+-rw-r--r--   0 root         (0) root         (0)   147475 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      536 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-24 08:13:20.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-04-24 08:13:19.000000 alibabacloud_eflo-controller20221215_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2/LICENSE` & `alibabacloud_eflo-controller20221215_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2/PKG-INFO` & `alibabacloud_eflo-controller20221215_py2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eflo-controller20221215_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2/README-CN.md` & `alibabacloud_eflo-controller20221215_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2/README.md` & `alibabacloud_eflo-controller20221215_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215/client.py` & `alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215/models.py` & `alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1349,22 +1349,23 @@
         if m.get('VpdId') is not None:
             self.vpd_id = m.get('VpdId')
         return self
 
 
 class DescribeNodeResponseBody(TeaModel):
     def __init__(self, cluster_id=None, cluster_name=None, create_time=None, expired_time=None, hostname=None,
-                 image_id=None, machine_type=None, networks=None, node_group_id=None, node_group_name=None, node_id=None,
-                 operating_state=None, request_id=None, sn=None, zone_id=None):
+                 image_id=None, image_name=None, machine_type=None, networks=None, node_group_id=None, node_group_name=None,
+                 node_id=None, operating_state=None, request_id=None, sn=None, zone_id=None):
         self.cluster_id = cluster_id  # type: str
         self.cluster_name = cluster_name  # type: str
         self.create_time = create_time  # type: str
         self.expired_time = expired_time  # type: str
         self.hostname = hostname  # type: str
         self.image_id = image_id  # type: str
+        self.image_name = image_name  # type: str
         self.machine_type = machine_type  # type: str
         self.networks = networks  # type: list[DescribeNodeResponseBodyNetworks]
         self.node_group_id = node_group_id  # type: str
         self.node_group_name = node_group_name  # type: str
         self.node_id = node_id  # type: str
         self.operating_state = operating_state  # type: str
         self.request_id = request_id  # type: str
@@ -1391,14 +1392,16 @@
             result['CreateTime'] = self.create_time
         if self.expired_time is not None:
             result['ExpiredTime'] = self.expired_time
         if self.hostname is not None:
             result['Hostname'] = self.hostname
         if self.image_id is not None:
             result['ImageId'] = self.image_id
+        if self.image_name is not None:
+            result['ImageName'] = self.image_name
         if self.machine_type is not None:
             result['MachineType'] = self.machine_type
         result['Networks'] = []
         if self.networks is not None:
             for k in self.networks:
                 result['Networks'].append(k.to_map() if k else None)
         if self.node_group_id is not None:
@@ -1427,14 +1430,16 @@
             self.create_time = m.get('CreateTime')
         if m.get('ExpiredTime') is not None:
             self.expired_time = m.get('ExpiredTime')
         if m.get('Hostname') is not None:
             self.hostname = m.get('Hostname')
         if m.get('ImageId') is not None:
             self.image_id = m.get('ImageId')
+        if m.get('ImageName') is not None:
+            self.image_name = m.get('ImageName')
         if m.get('MachineType') is not None:
             self.machine_type = m.get('MachineType')
         self.networks = []
         if m.get('Networks') is not None:
             for k in m.get('Networks'):
                 temp_model = DescribeNodeResponseBodyNetworks()
                 self.networks.append(temp_model.from_map(k))
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO` & `alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eflo-controller20221215-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt` & `alibabacloud_eflo-controller20221215_py2-1.0.3/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.0.2/setup.py` & `alibabacloud_eflo-controller20221215_py2-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eflo-controller20221215_py2.
 
-Created on 28/03/2023
+Created on 24/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eflo_controller20221215"
 NAME = "alibabacloud_eflo-controller20221215_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eflo-controller (20221215) SDK Library for Python2"
```

