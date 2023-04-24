# Comparing `tmp/cdk-image-pipeline-0.2.0.tar.gz` & `tmp/cdk-image-pipeline-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-image-pipeline-0.2.0.tar", last modified: Fri Apr 14 00:37:49 2023, max compression
+gzip compressed data, was "cdk-image-pipeline-0.2.1.tar", last modified: Mon Apr 24 15:27:31 2023, max compression
```

## Comparing `cdk-image-pipeline-0.2.0.tar` & `cdk-image-pipeline-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    35524 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26390 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.2.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.944847 cdk-image-pipeline-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27727 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.2.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:27:20.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:27:31.948847 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 15:27:31.000000 cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/top_level.txt
```

### Comparing `cdk-image-pipeline-0.2.0/LICENSE` & `cdk-image-pipeline-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.2.0/PKG-INFO` & `cdk-image-pipeline-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-image-pipeline-0.2.0/README.md` & `cdk-image-pipeline-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.2.0/setup.py` & `cdk-image-pipeline-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-image-pipeline",
-    "version": "0.2.0",
+    "version": "0.2.1",
     "description": "Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK",
     "license": "MIT-0",
     "url": "https://github.com/aws-samples/cdk-image-pipeline.git",
     "long_description_content_type": "text/markdown",
     "author": "Cameron Magee<magcamer@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "cdk_image_pipeline",
         "cdk_image_pipeline._jsii"
     ],
     "package_data": {
         "cdk_image_pipeline._jsii": [
-            "cdk-image-pipeline@0.2.0.jsii.tgz"
+            "cdk-image-pipeline@0.2.1.jsii.tgz"
         ],
         "cdk_image_pipeline": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.73.0, <3.0.0",
+        "aws-cdk-lib>=2.76.0, <3.0.0",
         "constructs>=10.1.215, <11.0.0",
         "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/__init__.py` & `cdk-image-pipeline-0.2.1/src/cdk_image_pipeline/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -284,17 +284,20 @@
         image_recipe: builtins.str,
         infra_config_name: builtins.str,
         kms_key_alias: builtins.str,
         parent_image: builtins.str,
         pipeline_name: builtins.str,
         profile_name: builtins.str,
         additional_policies: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.ManagedPolicy]] = None,
+        distribution_account_i_ds: typing.Optional[typing.Sequence[builtins.str]] = None,
+        distribution_regions: typing.Optional[typing.Sequence[builtins.str]] = None,
         ebs_volume_configuration: typing.Optional[typing.Union[_aws_cdk_aws_imagebuilder_ceddda9d.CfnImageRecipe.EbsInstanceBlockDeviceSpecificationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         ebs_volume_name: typing.Optional[builtins.str] = None,
         email: typing.Optional[builtins.str] = None,
+        enable_cross_account_distribution: typing.Optional[builtins.bool] = None,
         enable_vuln_scans: typing.Optional[builtins.bool] = None,
         image_recipe_version: typing.Optional[builtins.str] = None,
         instance_types: typing.Optional[typing.Sequence[builtins.str]] = None,
         platform: typing.Optional[builtins.str] = None,
         security_groups: typing.Optional[typing.Sequence[builtins.str]] = None,
         subnet_id: typing.Optional[builtins.str] = None,
         user_data_script: typing.Optional[builtins.str] = None,
@@ -310,17 +313,20 @@
         :param image_recipe: Name of the Image Recipe.
         :param infra_config_name: Name of the Infrastructure Configuration for Image Builder.
         :param kms_key_alias: KMS Key used to encrypt the SNS topic. Enter an existing KMS Key Alias in your target account/region.
         :param parent_image: The source (parent) image that the image recipe uses as its base environment. The value can be the parent image ARN or an Image Builder AMI ID
         :param pipeline_name: Name of the Image Pipeline.
         :param profile_name: Name of the instance profile that will be associated with the Instance Configuration.
         :param additional_policies: Additional policies to add to the instance profile associated with the Instance Configurations.
+        :param distribution_account_i_ds: List of accounts to copy this AMI to, if the option to do so is enabled.
+        :param distribution_regions: List of regions to copy this AMI to, if the option to do so is enabled.
         :param ebs_volume_configuration: Configuration for the AMI's EBS volume.
         :param ebs_volume_name: Name of the AMI's EBS volume.
         :param email: Email used to receive Image Builder Pipeline Notifications via SNS.
+        :param enable_cross_account_distribution: Set to true if you want to copy this AMI to other accounts using a Distribution Configuration.
         :param enable_vuln_scans: Set to true if you want to enable continuous vulnerability scans through AWS Inpector.
         :param image_recipe_version: Image recipe version (Default: 0.0.1).
         :param instance_types: List of instance types used in the Instance Configuration (Default: [ 't3.medium', 'm5.large', 'm5.xlarge' ]).
         :param platform: Platform type Linux or Windows (Default: Linux).
         :param security_groups: List of security group IDs for the Infrastructure Configuration.
         :param subnet_id: Subnet ID for the Infrastructure Configuration.
         :param user_data_script: UserData script that will override default one (if specified). Default: - none
@@ -338,17 +344,20 @@
             image_recipe=image_recipe,
             infra_config_name=infra_config_name,
             kms_key_alias=kms_key_alias,
             parent_image=parent_image,
             pipeline_name=pipeline_name,
             profile_name=profile_name,
             additional_policies=additional_policies,
+            distribution_account_i_ds=distribution_account_i_ds,
+            distribution_regions=distribution_regions,
             ebs_volume_configuration=ebs_volume_configuration,
             ebs_volume_name=ebs_volume_name,
             email=email,
+            enable_cross_account_distribution=enable_cross_account_distribution,
             enable_vuln_scans=enable_vuln_scans,
             image_recipe_version=image_recipe_version,
             instance_types=instance_types,
             platform=platform,
             security_groups=security_groups,
             subnet_id=subnet_id,
             user_data_script=user_data_script,
@@ -386,17 +395,20 @@
         "image_recipe": "imageRecipe",
         "infra_config_name": "infraConfigName",
         "kms_key_alias": "kmsKeyAlias",
         "parent_image": "parentImage",
         "pipeline_name": "pipelineName",
         "profile_name": "profileName",
         "additional_policies": "additionalPolicies",
+        "distribution_account_i_ds": "distributionAccountIDs",
+        "distribution_regions": "distributionRegions",
         "ebs_volume_configuration": "ebsVolumeConfiguration",
         "ebs_volume_name": "ebsVolumeName",
         "email": "email",
+        "enable_cross_account_distribution": "enableCrossAccountDistribution",
         "enable_vuln_scans": "enableVulnScans",
         "image_recipe_version": "imageRecipeVersion",
         "instance_types": "instanceTypes",
         "platform": "platform",
         "security_groups": "securityGroups",
         "subnet_id": "subnetId",
         "user_data_script": "userDataScript",
@@ -414,17 +426,20 @@
         image_recipe: builtins.str,
         infra_config_name: builtins.str,
         kms_key_alias: builtins.str,
         parent_image: builtins.str,
         pipeline_name: builtins.str,
         profile_name: builtins.str,
         additional_policies: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.ManagedPolicy]] = None,
+        distribution_account_i_ds: typing.Optional[typing.Sequence[builtins.str]] = None,
+        distribution_regions: typing.Optional[typing.Sequence[builtins.str]] = None,
         ebs_volume_configuration: typing.Optional[typing.Union[_aws_cdk_aws_imagebuilder_ceddda9d.CfnImageRecipe.EbsInstanceBlockDeviceSpecificationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         ebs_volume_name: typing.Optional[builtins.str] = None,
         email: typing.Optional[builtins.str] = None,
+        enable_cross_account_distribution: typing.Optional[builtins.bool] = None,
         enable_vuln_scans: typing.Optional[builtins.bool] = None,
         image_recipe_version: typing.Optional[builtins.str] = None,
         instance_types: typing.Optional[typing.Sequence[builtins.str]] = None,
         platform: typing.Optional[builtins.str] = None,
         security_groups: typing.Optional[typing.Sequence[builtins.str]] = None,
         subnet_id: typing.Optional[builtins.str] = None,
         user_data_script: typing.Optional[builtins.str] = None,
@@ -438,17 +453,20 @@
         :param image_recipe: Name of the Image Recipe.
         :param infra_config_name: Name of the Infrastructure Configuration for Image Builder.
         :param kms_key_alias: KMS Key used to encrypt the SNS topic. Enter an existing KMS Key Alias in your target account/region.
         :param parent_image: The source (parent) image that the image recipe uses as its base environment. The value can be the parent image ARN or an Image Builder AMI ID
         :param pipeline_name: Name of the Image Pipeline.
         :param profile_name: Name of the instance profile that will be associated with the Instance Configuration.
         :param additional_policies: Additional policies to add to the instance profile associated with the Instance Configurations.
+        :param distribution_account_i_ds: List of accounts to copy this AMI to, if the option to do so is enabled.
+        :param distribution_regions: List of regions to copy this AMI to, if the option to do so is enabled.
         :param ebs_volume_configuration: Configuration for the AMI's EBS volume.
         :param ebs_volume_name: Name of the AMI's EBS volume.
         :param email: Email used to receive Image Builder Pipeline Notifications via SNS.
+        :param enable_cross_account_distribution: Set to true if you want to copy this AMI to other accounts using a Distribution Configuration.
         :param enable_vuln_scans: Set to true if you want to enable continuous vulnerability scans through AWS Inpector.
         :param image_recipe_version: Image recipe version (Default: 0.0.1).
         :param instance_types: List of instance types used in the Instance Configuration (Default: [ 't3.medium', 'm5.large', 'm5.xlarge' ]).
         :param platform: Platform type Linux or Windows (Default: Linux).
         :param security_groups: List of security group IDs for the Infrastructure Configuration.
         :param subnet_id: Subnet ID for the Infrastructure Configuration.
         :param user_data_script: UserData script that will override default one (if specified). Default: - none
@@ -465,17 +483,20 @@
             check_type(argname="argument image_recipe", value=image_recipe, expected_type=type_hints["image_recipe"])
             check_type(argname="argument infra_config_name", value=infra_config_name, expected_type=type_hints["infra_config_name"])
             check_type(argname="argument kms_key_alias", value=kms_key_alias, expected_type=type_hints["kms_key_alias"])
             check_type(argname="argument parent_image", value=parent_image, expected_type=type_hints["parent_image"])
             check_type(argname="argument pipeline_name", value=pipeline_name, expected_type=type_hints["pipeline_name"])
             check_type(argname="argument profile_name", value=profile_name, expected_type=type_hints["profile_name"])
             check_type(argname="argument additional_policies", value=additional_policies, expected_type=type_hints["additional_policies"])
+            check_type(argname="argument distribution_account_i_ds", value=distribution_account_i_ds, expected_type=type_hints["distribution_account_i_ds"])
+            check_type(argname="argument distribution_regions", value=distribution_regions, expected_type=type_hints["distribution_regions"])
             check_type(argname="argument ebs_volume_configuration", value=ebs_volume_configuration, expected_type=type_hints["ebs_volume_configuration"])
             check_type(argname="argument ebs_volume_name", value=ebs_volume_name, expected_type=type_hints["ebs_volume_name"])
             check_type(argname="argument email", value=email, expected_type=type_hints["email"])
+            check_type(argname="argument enable_cross_account_distribution", value=enable_cross_account_distribution, expected_type=type_hints["enable_cross_account_distribution"])
             check_type(argname="argument enable_vuln_scans", value=enable_vuln_scans, expected_type=type_hints["enable_vuln_scans"])
             check_type(argname="argument image_recipe_version", value=image_recipe_version, expected_type=type_hints["image_recipe_version"])
             check_type(argname="argument instance_types", value=instance_types, expected_type=type_hints["instance_types"])
             check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
             check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
             check_type(argname="argument subnet_id", value=subnet_id, expected_type=type_hints["subnet_id"])
             check_type(argname="argument user_data_script", value=user_data_script, expected_type=type_hints["user_data_script"])
@@ -490,20 +511,26 @@
             "kms_key_alias": kms_key_alias,
             "parent_image": parent_image,
             "pipeline_name": pipeline_name,
             "profile_name": profile_name,
         }
         if additional_policies is not None:
             self._values["additional_policies"] = additional_policies
+        if distribution_account_i_ds is not None:
+            self._values["distribution_account_i_ds"] = distribution_account_i_ds
+        if distribution_regions is not None:
+            self._values["distribution_regions"] = distribution_regions
         if ebs_volume_configuration is not None:
             self._values["ebs_volume_configuration"] = ebs_volume_configuration
         if ebs_volume_name is not None:
             self._values["ebs_volume_name"] = ebs_volume_name
         if email is not None:
             self._values["email"] = email
+        if enable_cross_account_distribution is not None:
+            self._values["enable_cross_account_distribution"] = enable_cross_account_distribution
         if enable_vuln_scans is not None:
             self._values["enable_vuln_scans"] = enable_vuln_scans
         if image_recipe_version is not None:
             self._values["image_recipe_version"] = image_recipe_version
         if instance_types is not None:
             self._values["instance_types"] = instance_types
         if platform is not None:
@@ -593,14 +620,26 @@
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.ManagedPolicy]]:
         '''Additional policies to add to the instance profile associated with the Instance Configurations.'''
         result = self._values.get("additional_policies")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.ManagedPolicy]], result)
 
     @builtins.property
+    def distribution_account_i_ds(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''List of accounts to copy this AMI to, if the option to do so is enabled.'''
+        result = self._values.get("distribution_account_i_ds")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
+    def distribution_regions(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''List of regions to copy this AMI to, if the option to do so is enabled.'''
+        result = self._values.get("distribution_regions")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
     def ebs_volume_configuration(
         self,
     ) -> typing.Optional[_aws_cdk_aws_imagebuilder_ceddda9d.CfnImageRecipe.EbsInstanceBlockDeviceSpecificationProperty]:
         '''Configuration for the AMI's EBS volume.'''
         result = self._values.get("ebs_volume_configuration")
         return typing.cast(typing.Optional[_aws_cdk_aws_imagebuilder_ceddda9d.CfnImageRecipe.EbsInstanceBlockDeviceSpecificationProperty], result)
 
@@ -613,14 +652,20 @@
     @builtins.property
     def email(self) -> typing.Optional[builtins.str]:
         '''Email used to receive Image Builder Pipeline Notifications via SNS.'''
         result = self._values.get("email")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def enable_cross_account_distribution(self) -> typing.Optional[builtins.bool]:
+        '''Set to true if you want to copy this AMI to other accounts using a Distribution Configuration.'''
+        result = self._values.get("enable_cross_account_distribution")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def enable_vuln_scans(self) -> typing.Optional[builtins.bool]:
         '''Set to true if you want to enable continuous vulnerability scans through AWS Inpector.'''
         result = self._values.get("enable_vuln_scans")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def image_recipe_version(self) -> typing.Optional[builtins.str]:
@@ -702,17 +747,20 @@
     image_recipe: builtins.str,
     infra_config_name: builtins.str,
     kms_key_alias: builtins.str,
     parent_image: builtins.str,
     pipeline_name: builtins.str,
     profile_name: builtins.str,
     additional_policies: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.ManagedPolicy]] = None,
+    distribution_account_i_ds: typing.Optional[typing.Sequence[builtins.str]] = None,
+    distribution_regions: typing.Optional[typing.Sequence[builtins.str]] = None,
     ebs_volume_configuration: typing.Optional[typing.Union[_aws_cdk_aws_imagebuilder_ceddda9d.CfnImageRecipe.EbsInstanceBlockDeviceSpecificationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     ebs_volume_name: typing.Optional[builtins.str] = None,
     email: typing.Optional[builtins.str] = None,
+    enable_cross_account_distribution: typing.Optional[builtins.bool] = None,
     enable_vuln_scans: typing.Optional[builtins.bool] = None,
     image_recipe_version: typing.Optional[builtins.str] = None,
     instance_types: typing.Optional[typing.Sequence[builtins.str]] = None,
     platform: typing.Optional[builtins.str] = None,
     security_groups: typing.Optional[typing.Sequence[builtins.str]] = None,
     subnet_id: typing.Optional[builtins.str] = None,
     user_data_script: typing.Optional[builtins.str] = None,
@@ -736,17 +784,20 @@
     image_recipe: builtins.str,
     infra_config_name: builtins.str,
     kms_key_alias: builtins.str,
     parent_image: builtins.str,
     pipeline_name: builtins.str,
     profile_name: builtins.str,
     additional_policies: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.ManagedPolicy]] = None,
+    distribution_account_i_ds: typing.Optional[typing.Sequence[builtins.str]] = None,
+    distribution_regions: typing.Optional[typing.Sequence[builtins.str]] = None,
     ebs_volume_configuration: typing.Optional[typing.Union[_aws_cdk_aws_imagebuilder_ceddda9d.CfnImageRecipe.EbsInstanceBlockDeviceSpecificationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     ebs_volume_name: typing.Optional[builtins.str] = None,
     email: typing.Optional[builtins.str] = None,
+    enable_cross_account_distribution: typing.Optional[builtins.bool] = None,
     enable_vuln_scans: typing.Optional[builtins.bool] = None,
     image_recipe_version: typing.Optional[builtins.str] = None,
     instance_types: typing.Optional[typing.Sequence[builtins.str]] = None,
     platform: typing.Optional[builtins.str] = None,
     security_groups: typing.Optional[typing.Sequence[builtins.str]] = None,
     subnet_id: typing.Optional[builtins.str] = None,
     user_data_script: typing.Optional[builtins.str] = None,
```

### Comparing `cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/PKG-INFO` & `cdk-image-pipeline-0.2.1/src/cdk_image_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

