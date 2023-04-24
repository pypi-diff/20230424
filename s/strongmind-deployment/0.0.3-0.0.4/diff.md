# Comparing `tmp/strongmind_deployment-0.0.3-py3-none-any.whl.zip` & `tmp/strongmind_deployment-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3972 bytes, number of entries: 7
+Zip file size: 3977 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
--rw-r--r--  2.0 unx     2797 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
+-rw-r--r--  2.0 unx     2812 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
 -rw-r--r--  2.0 unx     1786 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
-?rw-r--r--  2.0 unx      646 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.3.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.3.dist-info/RECORD
-7 files, 6992 bytes uncompressed, 2850 bytes compressed:  59.2%
+?rw-r--r--  2.0 unx      646 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.4.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.4.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.4.dist-info/RECORD
+7 files, 7007 bytes uncompressed, 2855 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: strongmind_deployment/container.py
 Comment: 
 
 Filename: strongmind_deployment/rails.py
 Comment: 
 
-Filename: strongmind_deployment-0.0.3.dist-info/METADATA
+Filename: strongmind_deployment-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-0.0.3.dist-info/WHEEL
+Filename: strongmind_deployment-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-0.0.3.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-0.0.4.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-0.0.3.dist-info/RECORD
+Filename: strongmind_deployment-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/container.py

```diff
@@ -4,17 +4,17 @@
 import pulumi
 import pulumi_aws as aws
 import pulumi_awsx as awsx
 from pulumi import Config, export, Output
 
 
 def get_aws_account_and_region():
-    current_identity = aws.get_caller_identity()
-    current_region = aws.get_region()
-    return current_identity.account_id, current_region
+    account_id = aws.get_caller_identity().account_id
+    current_region = aws.get_region().name
+    return account_id, current_region
 
 
 class ContainerComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:container', name, None, opts)
 
         if kwargs.get("get_aws_account_and_region"):
@@ -37,14 +37,16 @@
                                                              )
         account_id, region = get_aws_account_and_region_func()
 
         repo_url = f"{account_id}.dkr.ecr.{region}.amazonaws.com/{name}"
         image_name = os.getenv('IMAGE_TAG', f'{name}:latest')
         image = f"{repo_url}/{image_name}"
 
+        print(image)
+
         task_definition_args = awsx.ecs.FargateServiceTaskDefinitionArgs(
                 container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
                     image=image,
                     cpu=self.cpu,
                     memory=self.memory,
                     essential=True,
                     port_mappings=[awsx.ecs.TaskDefinitionPortMappingArgs(
```

## Comparing `strongmind_deployment-0.0.3.dist-info/METADATA` & `strongmind_deployment-0.0.4.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 0.0.3
+Version: 0.0.4
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-0.0.3.dist-info/licenses/LICENSE` & `strongmind_deployment-0.0.4.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `strongmind_deployment-0.0.3.dist-info/RECORD` & `strongmind_deployment-0.0.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 strongmind_deployment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-strongmind_deployment/container.py,sha256=s34cuhUuoZ-Y1Bto-3Rt8kmMm1S6vnA3FXjXeOQVLsI,2797
+strongmind_deployment/container.py,sha256=Rd8Q6gE14-puzn-Lx3oKosbmfRG2Rc7dWOLjjbmNcCU,2812
 strongmind_deployment/rails.py,sha256=n1vt_e_VBidG1FBV3p7QqncMGxth3_cNzXUAeCdq6ho,1786
-strongmind_deployment-0.0.3.dist-info/METADATA,sha256=UWExAQ6PzQPENVWjevp0dwO3aGZzUtiMqVgs9_2ZY2c,646
-strongmind_deployment-0.0.3.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-strongmind_deployment-0.0.3.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
-strongmind_deployment-0.0.3.dist-info/RECORD,,
+strongmind_deployment-0.0.4.dist-info/METADATA,sha256=pvDxX0EJaJqX68qREzQ4KLpdOcmQGR-9M4E7niMnuJ4,646
+strongmind_deployment-0.0.4.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+strongmind_deployment-0.0.4.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
+strongmind_deployment-0.0.4.dist-info/RECORD,,
```

