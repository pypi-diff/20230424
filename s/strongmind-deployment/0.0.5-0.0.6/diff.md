# Comparing `tmp/strongmind_deployment-0.0.5-py3-none-any.whl.zip` & `tmp/strongmind_deployment-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3971 bytes, number of entries: 7
+Zip file size: 3786 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
--rw-r--r--  2.0 unx     2790 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
+-rw-r--r--  2.0 unx     2225 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
 -rw-r--r--  2.0 unx     1786 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
-?rw-r--r--  2.0 unx      646 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.5.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.5.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.5.dist-info/RECORD
-7 files, 6985 bytes uncompressed, 2849 bytes compressed:  59.2%
+?rw-r--r--  2.0 unx      646 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.6.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.6.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.6.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-0.0.6.dist-info/RECORD
+7 files, 6420 bytes uncompressed, 2664 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: strongmind_deployment/container.py
 Comment: 
 
 Filename: strongmind_deployment/rails.py
 Comment: 
 
-Filename: strongmind_deployment-0.0.5.dist-info/METADATA
+Filename: strongmind_deployment-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-0.0.5.dist-info/WHEEL
+Filename: strongmind_deployment-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-0.0.5.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-0.0.6.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-0.0.5.dist-info/RECORD
+Filename: strongmind_deployment-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/container.py

```diff
@@ -3,51 +3,36 @@
 
 import pulumi
 import pulumi_aws as aws
 import pulumi_awsx as awsx
 from pulumi import Config, export, Output
 
 
-def get_aws_account_and_region():
-    account_id = aws.get_caller_identity().account_id
-    current_region = aws.get_region().name
-    return account_id, current_region
-
-
 class ContainerComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:container', name, None, opts)
 
-        if kwargs.get("get_aws_account_and_region"):
-            get_aws_account_and_region_func = kwargs.get("get_aws_account_and_region")
-        else:
-            get_aws_account_and_region_func = get_aws_account_and_region
-
+        self.container_image = kwargs.get('container_image')
         self.app_path = kwargs.get('app_path') or './'
         self.container_port = kwargs.get('container_port') or 3000
         self.cpu = kwargs.get('cpu') or 256
         self.memory = kwargs.get("memory") or 512
 
         self.ecs_cluster = aws.ecs.Cluster("cluster",
                                            name=name,
                                            opts=pulumi.ResourceOptions(parent=self),
                                            )
         self.load_balancer = awsx.lb.ApplicationLoadBalancer("loadbalancer",
                                                              name=name,
                                                              opts=pulumi.ResourceOptions(parent=self),
                                                              )
-        account_id, region = get_aws_account_and_region_func()
-
-        repo_url = f"{account_id}.dkr.ecr.{region}.amazonaws.com/{name}"
-        image_name = os.getenv('IMAGE_TAG', f'{name}:latest')
-        image = f"{repo_url}/{image_name}"
 
         task_definition_args = awsx.ecs.FargateServiceTaskDefinitionArgs(
                 container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
-                    image=image,
+                    image=self.container_image,
                     cpu=self.cpu,
                     memory=self.memory,
                     essential=True,
                     port_mappings=[awsx.ecs.TaskDefinitionPortMappingArgs(
                         container_port=self.container_port,
                         host_port=self.container_port,
                         target_group=self.load_balancer.default_target_group,
```

## Comparing `strongmind_deployment-0.0.5.dist-info/METADATA` & `strongmind_deployment-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 0.0.5
+Version: 0.0.6
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-0.0.5.dist-info/licenses/LICENSE` & `strongmind_deployment-0.0.6.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

