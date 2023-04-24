# Comparing `tmp/alibabacloud_eflo-controller20221215-1.0.2.tar.gz` & `tmp/alibabacloud_eflo-controller20221215-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eflo-controller20221215-1.0.2.tar", last modified: Tue Mar 28 02:43:20 2023, max compression
+gzip compressed data, was "dist/alibabacloud_eflo-controller20221215-1.0.3.tar", last modified: Mon Apr 24 08:13:43 2023, max compression
```

## Comparing `alibabacloud_eflo-controller20221215-1.0.2.tar` & `alibabacloud_eflo-controller20221215-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      148 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2400 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1058 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62687 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215/client.py
--rw-r--r--   0 root         (0) root         (0)   146289 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2400 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2672 2023-03-28 02:43:20.000000 alibabacloud_eflo-controller20221215-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62687 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/client.py
+-rw-r--r--   0 root         (0) root         (0)   146540 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-04-24 08:13:43.000000 alibabacloud_eflo-controller20221215-1.0.3/setup.py
```

### Comparing `alibabacloud_eflo-controller20221215-1.0.2/LICENSE` & `alibabacloud_eflo-controller20221215-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.2/PKG-INFO` & `alibabacloud_eflo-controller20221215-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eflo-controller20221215
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215-1.0.2/README-CN.md` & `alibabacloud_eflo-controller20221215-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.2/README.md` & `alibabacloud_eflo-controller20221215-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215/client.py` & `alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215/models.py` & `alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1528,14 +1528,15 @@
         self,
         cluster_id: str = None,
         cluster_name: str = None,
         create_time: str = None,
         expired_time: str = None,
         hostname: str = None,
         image_id: str = None,
+        image_name: str = None,
         machine_type: str = None,
         networks: List[DescribeNodeResponseBodyNetworks] = None,
         node_group_id: str = None,
         node_group_name: str = None,
         node_id: str = None,
         operating_state: str = None,
         request_id: str = None,
@@ -1544,14 +1545,15 @@
     ):
         self.cluster_id = cluster_id
         self.cluster_name = cluster_name
         self.create_time = create_time
         self.expired_time = expired_time
         self.hostname = hostname
         self.image_id = image_id
+        self.image_name = image_name
         self.machine_type = machine_type
         self.networks = networks
         self.node_group_id = node_group_id
         self.node_group_name = node_group_name
         self.node_id = node_id
         self.operating_state = operating_state
         self.request_id = request_id
@@ -1578,14 +1580,16 @@
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
@@ -1614,14 +1618,16 @@
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

### Comparing `alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215.egg-info/PKG-INFO` & `alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eflo-controller20221215
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215-1.0.2/alibabacloud_eflo_controller20221215.egg-info/SOURCES.txt` & `alibabacloud_eflo-controller20221215-1.0.3/alibabacloud_eflo_controller20221215.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215-1.0.2/setup.py` & `alibabacloud_eflo-controller20221215-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eflo-controller20221215.
 
-Created on 28/03/2023
+Created on 24/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eflo_controller20221215"
 NAME = "alibabacloud_eflo-controller20221215" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eflo-controller (20221215) SDK Library for Python"
```

