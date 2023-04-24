# Comparing `tmp/troposphere-dns-certificate-1.8.0.tar.gz` & `tmp/troposphere-dns-certificate-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troposphere-dns-certificate-1.8.0.tar", last modified: Sun Apr 23 17:55:03 2023, max compression
+gzip compressed data, was "troposphere-dns-certificate-2.0.0.tar", last modified: Mon Apr 24 20:35:35 2023, max compression
```

## Comparing `troposphere-dns-certificate-1.8.0.tar` & `troposphere-dns-certificate-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13415 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12939 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      939 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.205051 troposphere-dns-certificate-1.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/
--rw-r--r--   0 root         (0) root         (0)      916 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12595 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/certificate.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/certificatemanager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13415 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-23 17:55:03.000000 troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 17:55:03.209051 troposphere-dns-certificate-1.8.0/test/
--rw-r--r--   0 root         (0) root         (0)      420 2023-04-23 17:54:55.000000 troposphere-dns-certificate-1.8.0/test/test_lambda_code_size.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:35:35.421984 troposphere-dns-certificate-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15316 2023-04-24 20:35:35.421984 troposphere-dns-certificate-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14840 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 20:35:35.421984 troposphere-dns-certificate-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      939 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:35:35.417984 troposphere-dns-certificate-2.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:35:35.417984 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate/
+-rw-r--r--   0 root         (0) root         (0)      916 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14904 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate/certificate.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate/certificatemanager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:35:35.421984 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15316 2023-04-24 20:35:35.000000 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-24 20:35:35.000000 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 20:35:35.000000 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 20:35:35.000000 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-24 20:35:35.000000 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-24 20:35:35.000000 troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 20:35:35.421984 troposphere-dns-certificate-2.0.0/test/
+-rw-r--r--   0 root         (0) root         (0)     3256 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/test/test_domain_name.py
+-rw-r--r--   0 root         (0) root         (0)     5748 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/test/test_external_validation.py
+-rw-r--r--   0 root         (0) root         (0)     3774 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/test/test_key_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/test/test_lambda_code_size.py
+-rw-r--r--   0 root         (0) root         (0)     2826 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/test/test_region.py
+-rw-r--r--   0 root         (0) root         (0)     2512 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/test/test_route53_role_arn.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/test/test_tags.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/test/test_transparency_logging.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-04-24 20:35:27.000000 troposphere-dns-certificate-2.0.0/test/test_validation_option.py
```

### Comparing `troposphere-dns-certificate-1.8.0/LICENSE` & `troposphere-dns-certificate-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `troposphere-dns-certificate-1.8.0/PKG-INFO` & `troposphere-dns-certificate-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,14 @@
-Metadata-Version: 2.1
-Name: troposphere-dns-certificate
-Version: 1.8.0
-Summary: Cloudformation DNS validated certificate resource for troposphere
-Home-page: https://github.com/dflook/cloudformation-dns-certificate
-Author: Daniel Flook
-Author-email: daniel@flook.org
-License: MIT
-Project-URL: Issues, https://github.com/dflook/cloudformation-dns-certificate/issues
-Keywords: cloudformation troposphere certificate
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Cloudformation DNS Validated Certificate Resource
 
 This is a cloudformation custom resource which is an enhancement of the [AWS::CertificateManager::Certificate](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-certificatemanager-certificate.html) resource.
 
 It allows creating a certificate in a region different from the stack's region (e.g. `us-east-1` for cloudfront),
 and allows for creating a certificate for a Route 53 hosted zone in another AWS account.
+It also allows for setting the key algorithm.
 
 ## Usage
 
 To use this custom resource, copy the CustomAcmCertificateLambda and CustomAcmCertificateLambdaExecutionRole resources
 into your template. You can then create certificate resources of Type: `Custom::DNSCertificate`.
 
 This resource is also available as troposphere extension, in the [troposphere-dns-certificate](https://pypi.org/project/troposphere-dns-certificate/) package
@@ -31,17 +19,19 @@
 
 ### Differences from AWS::CertificateManager::Certificate
 It should behave similarly to [AWS::CertificateManager::Certificate](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-certificatemanager-certificate.html), 
 except for the differences described here.
 
 The additional `Region` property can be used to set the region to create the certificate in.
 
-The [DomainValidationOption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-certificatemanager-certificate-domainvalidationoption.html) has an additional property `Route53RoleArn`, which is a role to assume before creating DNS validation records.
+The [DomainValidationOption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-certificatemanager-certificate-domainvalidationoption.html) has a additional properties `Route53RoleArn` and `Route53RoleExternalId` which allow assuming a role before creating DNS validation records.
 This lets you create a certificate for a hosted zone in another account.
 
+The additional `KeyAlgorithm` property allows setting the key algorithm used to generate the key pair used by the certificate.
+
 ### Certificate Resource
 
 #### Syntax
 
 ```yaml
 Type: Custom::DNSCertificate
 Properties: 
@@ -50,14 +40,16 @@
     - DomainValidationOption
   SubjectAlternativeNames:
     - String
   Tags:
     - Resource Tag
   ValidationMethod: String
   Region: String
+  CertificateTransparencyLoggingPreference: String
+  KeyAlgorithm: String
   ServiceToken: !GetAtt 'CustomAcmCertificateLambda.Arn'  
 ```
 
 #### Properties
 
 * `DomainName`
 
@@ -70,15 +62,15 @@
 * `DomainValidationOptions`
 
   Information for validating domain ownership. A DomainValidationOption should be present for the DomainName and all 
   SubjectAlternativeNames. A DomainValidationOption for a parent domain can be used for names that have the same HostedZoneId.
 
   - Required: Yes
   - Type: List of `DomainValidationOption`
-  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)  
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement) if a HostedZoneId changes
 
 * `SubjectAlternativeNames`
 
   FQDNs to include in the Subject Alternative Name of the certificate.
 
   - Required: No
   - Type: List of String values
@@ -106,14 +98,35 @@
   The region to create the certificate in.
 
   - Required: No
   - Default: The Stack's region
   - Type: String
   - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement) 
 
+* `CertificateTransparencyLoggingPreference`
+
+  Certificate Transparency Logging Preference. This may be 'ENABLED' or 'DISABLED'.
+    
+  - Required: No
+  - Default: `ENABLED`
+  - Type: String
+  - Update requires: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)  
+
+* `KeyAlgorithm`
+
+  The algorithm that will be used to generate the key pair used by the certificate.
+  Currently, this may be `RSA_2048`, `EC_prime256v1`, or `EC_secp384r1` for new certificates.
+
+  :warning: Not all algorithms are supported by all clients, AWS services or regions.
+
+  - Required: No
+  - Default: `RSA_2048`
+  - Type: String
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)
+
 #### Return value
 
 * Ref
 
   When the [`Ref`](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-ref.html) 
   function is used on the logical ID of a Certificate resource the certificate ARN is returned.
 
@@ -132,37 +145,41 @@
 
 * `DomainName`
 
   Fully qualified domain name of the validation request.
 
   - Required: Yes
   - Type: String
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)
   
 * `HostedZoneId`
 
   The Route53 Hosted Zone to create validation records in.
 
   - Required: Yes
   - Type: String
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement) 
   
 * `Route53RoleArn`
 
   The arn of an IAM Role to assume when creating DNS validation records. This can be used to create the records for a
   Hosted Zone in another AWS account.
 
   - Required: No
   - Type: String
+  - Update requires: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)  
 
 * `Route53RoleExternalId`
 
   An External ID to use when assuming the Route53RoleArn. This can be set if required by the trust policy of the role. 
   See https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-user_externalid.html for details of using ExternalIds.
 
   - Required: No
   - Type: String
+  - Update requires: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)
 
 ## Troposphere
 
 If you are using troposphere you can install this resource as an extension using pip:
 
     $ pip install troposphere_dns_certificate
 
@@ -344,14 +361,15 @@
       - PolicyDocument:
           Statement:
             - Action:
                 - acm:AddTagsToCertificate
                 - acm:DeleteCertificate
                 - acm:DescribeCertificate
                 - acm:RemoveTagsFromCertificate
+                - acm:UpdateCertificateOptions
               Effect: Allow
               Resource:
                 - !Sub 'arn:${AWS::Partition}:acm:*:${AWS::AccountId}:certificate/*'
             - Action:
                 - acm:RequestCertificate
                 - acm:ListTagsForCertificate
                 - acm:ListCertificates
```

### Comparing `troposphere-dns-certificate-1.8.0/README.md` & `troposphere-dns-certificate-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+Metadata-Version: 2.1
+Name: troposphere-dns-certificate
+Version: 2.0.0
+Summary: Cloudformation DNS validated certificate resource for troposphere
+Home-page: https://github.com/dflook/cloudformation-dns-certificate
+Author: Daniel Flook
+Author-email: daniel@flook.org
+License: MIT
+Project-URL: Issues, https://github.com/dflook/cloudformation-dns-certificate/issues
+Keywords: cloudformation troposphere certificate
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Cloudformation DNS Validated Certificate Resource
 
 This is a cloudformation custom resource which is an enhancement of the [AWS::CertificateManager::Certificate](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-certificatemanager-certificate.html) resource.
 
 It allows creating a certificate in a region different from the stack's region (e.g. `us-east-1` for cloudfront),
 and allows for creating a certificate for a Route 53 hosted zone in another AWS account.
+It also allows for setting the key algorithm.
 
 ## Usage
 
 To use this custom resource, copy the CustomAcmCertificateLambda and CustomAcmCertificateLambdaExecutionRole resources
 into your template. You can then create certificate resources of Type: `Custom::DNSCertificate`.
 
 This resource is also available as troposphere extension, in the [troposphere-dns-certificate](https://pypi.org/project/troposphere-dns-certificate/) package
@@ -18,17 +32,19 @@
 
 ### Differences from AWS::CertificateManager::Certificate
 It should behave similarly to [AWS::CertificateManager::Certificate](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-certificatemanager-certificate.html), 
 except for the differences described here.
 
 The additional `Region` property can be used to set the region to create the certificate in.
 
-The [DomainValidationOption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-certificatemanager-certificate-domainvalidationoption.html) has an additional property `Route53RoleArn`, which is a role to assume before creating DNS validation records.
+The [DomainValidationOption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-certificatemanager-certificate-domainvalidationoption.html) has a additional properties `Route53RoleArn` and `Route53RoleExternalId` which allow assuming a role before creating DNS validation records.
 This lets you create a certificate for a hosted zone in another account.
 
+The additional `KeyAlgorithm` property allows setting the key algorithm used to generate the key pair used by the certificate.
+
 ### Certificate Resource
 
 #### Syntax
 
 ```yaml
 Type: Custom::DNSCertificate
 Properties: 
@@ -37,14 +53,16 @@
     - DomainValidationOption
   SubjectAlternativeNames:
     - String
   Tags:
     - Resource Tag
   ValidationMethod: String
   Region: String
+  CertificateTransparencyLoggingPreference: String
+  KeyAlgorithm: String
   ServiceToken: !GetAtt 'CustomAcmCertificateLambda.Arn'  
 ```
 
 #### Properties
 
 * `DomainName`
 
@@ -57,15 +75,15 @@
 * `DomainValidationOptions`
 
   Information for validating domain ownership. A DomainValidationOption should be present for the DomainName and all 
   SubjectAlternativeNames. A DomainValidationOption for a parent domain can be used for names that have the same HostedZoneId.
 
   - Required: Yes
   - Type: List of `DomainValidationOption`
-  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)  
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement) if a HostedZoneId changes
 
 * `SubjectAlternativeNames`
 
   FQDNs to include in the Subject Alternative Name of the certificate.
 
   - Required: No
   - Type: List of String values
@@ -93,14 +111,35 @@
   The region to create the certificate in.
 
   - Required: No
   - Default: The Stack's region
   - Type: String
   - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement) 
 
+* `CertificateTransparencyLoggingPreference`
+
+  Certificate Transparency Logging Preference. This may be 'ENABLED' or 'DISABLED'.
+    
+  - Required: No
+  - Default: `ENABLED`
+  - Type: String
+  - Update requires: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)  
+
+* `KeyAlgorithm`
+
+  The algorithm that will be used to generate the key pair used by the certificate.
+  Currently, this may be `RSA_2048`, `EC_prime256v1`, or `EC_secp384r1` for new certificates.
+
+  :warning: Not all algorithms are supported by all clients, AWS services or regions.
+
+  - Required: No
+  - Default: `RSA_2048`
+  - Type: String
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)
+
 #### Return value
 
 * Ref
 
   When the [`Ref`](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-ref.html) 
   function is used on the logical ID of a Certificate resource the certificate ARN is returned.
 
@@ -119,37 +158,41 @@
 
 * `DomainName`
 
   Fully qualified domain name of the validation request.
 
   - Required: Yes
   - Type: String
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)
   
 * `HostedZoneId`
 
   The Route53 Hosted Zone to create validation records in.
 
   - Required: Yes
   - Type: String
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement) 
   
 * `Route53RoleArn`
 
   The arn of an IAM Role to assume when creating DNS validation records. This can be used to create the records for a
   Hosted Zone in another AWS account.
 
   - Required: No
   - Type: String
+  - Update requires: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)  
 
 * `Route53RoleExternalId`
 
   An External ID to use when assuming the Route53RoleArn. This can be set if required by the trust policy of the role. 
   See https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-user_externalid.html for details of using ExternalIds.
 
   - Required: No
   - Type: String
+  - Update requires: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)
 
 ## Troposphere
 
 If you are using troposphere you can install this resource as an extension using pip:
 
     $ pip install troposphere_dns_certificate
 
@@ -331,14 +374,15 @@
       - PolicyDocument:
           Statement:
             - Action:
                 - acm:AddTagsToCertificate
                 - acm:DeleteCertificate
                 - acm:DescribeCertificate
                 - acm:RemoveTagsFromCertificate
+                - acm:UpdateCertificateOptions
               Effect: Allow
               Resource:
                 - !Sub 'arn:${AWS::Partition}:acm:*:${AWS::AccountId}:certificate/*'
             - Action:
                 - acm:RequestCertificate
                 - acm:ListTagsForCertificate
                 - acm:ListCertificates
```

### Comparing `troposphere-dns-certificate-1.8.0/setup.py` & `troposphere-dns-certificate-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 readme_path = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md')
 with open(readme_path) as f:
     long_desc = f.read()
 
 setup(
     name='troposphere-dns-certificate',
     description='Cloudformation DNS validated certificate resource for troposphere',
-    version='1.8.0',
+    version='2.0.0',
     author='Daniel Flook',
     author_email='daniel@flook.org',
     url='https://github.com/dflook/cloudformation-dns-certificate',
     license='MIT',
     project_urls={
         'Issues': 'https://github.com/dflook/cloudformation-dns-certificate/issues',
     },
```

### Comparing `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/__init__.py` & `troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/certificate.py` & `troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate/certificate.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from boto3 import client
 from botocore.exceptions import ClientError, ParamValidationError
 from urllib.request import Request, urlopen
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
+log_warning = logger.warning
 log_info = logger.info
 log_exception = logger.exception
 shallow_copy = copy.copy
 sleep = time.sleep
 
 json_dumps = lambda j: json.dumps(j, sort_keys=True).encode()
 
@@ -47,32 +48,45 @@
         This create an ACM certificate and update the event payload with the PhysicalResourceId.
         The certificate will not yet be issued.
 
         """
 
         api_request = shallow_copy(props)
 
-        for key in ['ServiceToken', 'Region', 'Tags', 'Route53RoleArn']:
+        for key in ['ServiceToken', 'Region', 'Tags', 'Route53RoleArn', 'CertificateTransparencyLoggingPreference']:
             api_request.pop(key, None)
 
+        if 'CertificateTransparencyLoggingPreference' in props:
+            api_request['Options'] = {'CertificateTransparencyLoggingPreference': props['CertificateTransparencyLoggingPreference']}
+
         if 'ValidationMethod' in props:
             if props['ValidationMethod'] == 'DNS':
 
                 # Check that we have all the hosted zone information we need to validate
                 # before we create the certificate
                 for name in set([props['DomainName']] + props.get('SubjectAlternativeNames', [])):
-                    get_zone_for(name)
+                    if get_zone_for(name) is None:
+                        log_warning(f'No DomainValidationOption found for {name} - the validation records will need to be created manually')
+
+                if 'DomainValidationOptions' in api_request:
+                    del api_request['DomainValidationOptions']
 
-                del api_request['DomainValidationOptions']
+        tags = shallow_copy(event['ResourceProperties'].get('Tags', []))
+        tags += [
+            {'Key': 'cloudformation:logical-id', 'Value': event['LogicalResourceId']},
+            {'Key': 'cloudformation:stack-id', 'Value': event['StackId']},
+            {'Key': 'cloudformation:stack-name', 'Value': event['StackId'].split('/')[1]},
+            {'Key': 'cloudformation:properties', 'Value': hash_func(event['ResourceProperties'])}
+        ]
 
         event['PhysicalResourceId'] = acm.request_certificate(
             IdempotencyToken=i_token,
+            Tags=tags,
             **api_request
         )['CertificateArn']
-        add_tags()
 
     def delete_certificate(arn, /):
         """
         Delete a certificate
 
         Attempts to delete a certificate.
 
@@ -119,21 +133,23 @@
 
         """
 
         for page in acm.get_paginator('list_certificates').paginate():
             for certificate in page['CertificateSummaryList']:
                 log_info(certificate)
 
-                if props['DomainName'].lower() == certificate['DomainName']:
+                # In certain cases the DomainName property may not be present yet at the time we called list_certificates
+                # We can go ahead and check the certificate tags anyway.
+                if 'DomainName' not in props or props['DomainName'].lower() == certificate['DomainName']:
                     tags = {tag['Key']: tag['Value'] for tag in
                             acm.list_tags_for_certificate(**{'CertificateArn': certificate['CertificateArn']})['Tags']}
 
-                    if (tags.get('cloudformation:' + 'logical-id') == event['LogicalResourceId'] and
-                            tags.get('cloudformation:' + 'stack-id') == event['StackId'] and
-                            tags.get('cloudformation:' + 'properties') == hash_func(props)
+                    if (tags.get('cloudformation:logical-id') == event['LogicalResourceId'] and
+                            tags.get('cloudformation:stack-id') == event['StackId'] and
+                            tags.get('cloudformation:properties') == hash_func(props)
                     ):
                         return certificate['CertificateArn']
 
     def reinvoke():
         """
         Reinvoke this lambda
 
@@ -182,59 +198,79 @@
 
         return False
 
     def replace_cert():
         """
         Does the update require replacement of the certificate?
 
-        Only tags can be updated without replacement
+        Only Tags and CertificateTransparencyLoggingPreference can be updated without replacement
 
         :rtype: bool
 
         """
 
-        old = shallow_copy(event['Old' + 'ResourceProperties'])
+        def replace_validation_option(validation_options: list[dict[str, str]]) -> list[dict[str, str]]:
+            options = []
+            for validation_option in validation_options:
+                options.append({
+                    'DomainName': validation_option.get('DomainName'),
+                    'HostedZoneId': validation_option.get('HostedZoneId'),
+                })
+            return options
+
+        old = shallow_copy(event['OldResourceProperties'])
         old.pop('Tags', None)
+        old.pop('CertificateTransparencyLoggingPreference', None)
+        old['DomainValidationOptions'] = replace_validation_option(old.get('DomainValidationOptions', []))
 
         new = shallow_copy(event['ResourceProperties'])
         new.pop('Tags', None)
+        new.pop('CertificateTransparencyLoggingPreference', None)
+        new['DomainValidationOptions'] = replace_validation_option(new.get('DomainValidationOptions', []))
 
         return old != new
 
     def validate():
         """
         Add DNS validation records for a certificate
-
         """
 
         if props.get('ValidationMethod') != 'DNS':
             return
 
+        def ready_to_validate(cert) -> bool:
+            if 'DomainValidationOptions' not in cert:
+                return False
+
+            for validation_option in cert['DomainValidationOptions']:
+                if 'ValidationStatus' not in validation_option or 'ResourceRecord' not in validation_option:
+                    return False
+
+            return True
+
         while True:
             cert = acm.describe_certificate(**{'CertificateArn': event['PhysicalResourceId']})['Certificate']
             log_info(cert)
 
             if cert['Status'] != 'PENDING_VALIDATION':
                 return
 
-            if not [
-                validation_option
-                for validation_option in cert.get('DomainValidationOptions', [{}])
-                if 'ValidationStatus' not in validation_option
-                   or 'ResourceRecord' not in validation_option
-            ]:
+            if ready_to_validate(cert):
                 # All validation options have a status and resource record to create
                 break
-
-            sleep(1)
+            else:
+                sleep(1)
 
         for validation_option in cert['DomainValidationOptions']:
 
             if validation_option['ValidationStatus'] == 'PENDING_VALIDATION':
                 hosted_zone = get_zone_for(validation_option['DomainName'])
+                if hosted_zone is None:
+                    log_info(f'No DomainValidationOption found for domain {validation_option["DomainName"]}, validation records must be created manually')
+                    continue
 
                 role_arn = hosted_zone.get('Route53RoleArn', props.get('Route53RoleArn'))
                 external_id = hosted_zone.get('Route53RoleExternalId')
 
                 sts_params = {
                     'RoleArn': role_arn,
                     'RoleSessionName': ('Certificate' + event['LogicalResourceId'])[:64],
@@ -261,61 +297,41 @@
                             'ResourceRecordSet': {
                                 'Name': validation_option['ResourceRecord']['Name'],
                                 'Type': validation_option['ResourceRecord']['Type'],
                                 'TTL': 60,
                                 'ResourceRecords': [{'Value': validation_option['ResourceRecord']['Value']}],
                             },
                         }],
-                    }},
+                    }}
                 )
 
                 log_info(route53)
 
     def get_zone_for(name, /):
         """
         Return the hosted zone to use for validating a name
 
         :param str name: The name to validate
         :rtype: dict
 
         """
 
         name = name.rstrip('.')
-        zones = {domain['DomainName'].rstrip('.'): domain for domain in props['DomainValidationOptions']}
+        zones = {domain['DomainName'].rstrip('.'): domain for domain in props.get('DomainValidationOptions', [])}
 
         parts = name.split('.')
 
         while len(parts):
             if '.'.join(parts) in zones:
                 return zones['.'.join(parts)]
 
             parts = parts[1:]
 
-        raise RuntimeError('DomainValidationOptions' + ' missing for ' + name)
-
     hash_func = lambda v: hashlib.new('md5', json_dumps(v)).hexdigest()
 
-    def add_tags():
-        """
-        Add tags from the ResourceProperties to the Certificate
-
-        Also adds logical-id, stack-id, stack-name and properties tags, which are used by the custom resource.
-
-        """
-
-        tags = shallow_copy(event['ResourceProperties'].get('Tags', []))
-        tags += [
-            {'Key': 'cloudformation:' + 'logical-id', 'Value': event['LogicalResourceId']},
-            {'Key': 'cloudformation:' + 'stack-id', 'Value': event['StackId']},
-            {'Key': 'cloudformation:' + 'stack-name', 'Value': event['StackId'].split('/')[1]},
-            {'Key': 'cloudformation:' + 'properties', 'Value': hash_func(event['ResourceProperties'])}
-        ]
-
-        acm.add_tags_to_certificate(**{'CertificateArn': event['PhysicalResourceId'], 'Tags': tags})
-
     def send_response():
         """
         Send a response to cloudformation
 
         """
 
         log_info(event)
@@ -343,23 +359,24 @@
 
             if not wait_for_issuance():
                 return reinvoke()
 
         elif event['RequestType'] == 'Delete':
 
             if event['PhysicalResourceId'] != 'None':
+
                 if event['PhysicalResourceId'].startswith('arn:'):
                     delete_certificate(event['PhysicalResourceId'])
                 else:
                     delete_certificate(find_certificate(props))
 
         elif event['RequestType'] == 'Update':
 
             if replace_cert():
-                log_info('Update')
+                log_info('Replacement required')
 
                 if find_certificate(props) == event['PhysicalResourceId']:
                     # This is an update cancel request.
 
                     # Try and delete the new certificate that is no longer required
                     try:
                         acm = client('acm', region_name=event['OldResourceProperties'].get('Region'))
@@ -374,22 +391,36 @@
                 if REINVOKED not in event:
                     request_cert()
 
                 validate()
 
                 if not wait_for_issuance():
                     return reinvoke()
+
             else:
-                if 'Tags' in event['Old' + 'ResourceProperties']:
+                log_info('Update in place')
+                if 'Tags' in event['OldResourceProperties']:
                     acm.remove_tags_from_certificate(**{
                         'CertificateArn': event['PhysicalResourceId'],
-                        'Tags': event['Old' + 'ResourceProperties']['Tags']
+                        'Tags': event['OldResourceProperties']['Tags']
                     })
 
-                add_tags()
+                if 'Tags' in event['ResourceProperties']:
+                    acm.add_tags_to_certificate(**{
+                        'CertificateArn': event['PhysicalResourceId'],
+                        'Tags': event['ResourceProperties'].get('Tags', [])
+                    })
+
+                if event['ResourceProperties'].get('CertificateTransparencyLoggingPreference') != event['OldResourceProperties'].get('CertificateTransparencyLoggingPreference'):
+                    acm.update_certificate_options(**{
+                        'CertificateArn': event['PhysicalResourceId'],
+                        'Options': {
+                            'CertificateTransparencyLoggingPreference': event['ResourceProperties'].get('CertificateTransparencyLoggingPreference', 'ENABLED'),
+                        }
+                    })
 
         else:
             raise RuntimeError(event['RequestType'])
 
         return send_response()
 
     except Exception as ex:
```

### Comparing `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate/certificatemanager.py` & `troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate/certificatemanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,15 @@
                                 Statement(
                                     Effect=Allow,
                                     Action=[
                                         Action('acm', 'AddTagsToCertificate'),
                                         Action('acm', 'DeleteCertificate'),
                                         Action('acm', 'DescribeCertificate'),
                                         Action('acm', 'RemoveTagsFromCertificate'),
+                                        Action('acm', 'UpdateCertificateOptions'),
 
                                     ],
                                     Resource=[Sub('arn:${AWS::Partition}:acm:*:${AWS::AccountId}:certificate/*')],
                                 ),
                                 Statement(
                                     Effect=Allow,
                                     Action=[
@@ -77,15 +78,15 @@
         with open(pkgutil.get_loader('troposphere_dns_certificate.certificate').get_filename()) as f:
             code = python_minifier.awslambda(f.read(), entrypoint='handler')
 
         template.add_resource(
             awslambda.Function(
                 CERTIFICATE_LAMBDA,
                 Code=awslambda.Code(ZipFile=code),
-                Runtime='python3.9',
+                Runtime='python3.10',
                 Handler='index.handler',
                 Timeout=900,
                 Role=GetAtt(LAMBDA_ROLE, 'Arn'),
                 Description='Cloudformation custom resource for DNS validated certificates',
                 Metadata={
                     'Source': 'https://github.com/dflook/cloudformation-dns-certificate',
                     'Version': pkg_resources.require('troposphere-dns-certificate')[0].version,
@@ -104,21 +105,24 @@
     }
 
 
 class Certificate(CustomResource, TroposphereExtension):
     resource_type = 'Custom::DNSCertificate'
 
     props = {
+        'CertificateAuthorityArn': (str, False),
+        'CertificateTransparencyLoggingPreference': (str, False),
         'DomainName': (str, True),
         'DomainValidationOptions': ([(DomainValidationOption, dict)], False),
         'SubjectAlternativeNames': ([str], False),
         'Tags': ((Tags, list), False),
         'ValidationMethod': (str, False),
         'Route53RoleArn': (str, False),
         'Region': (str, False),
+        'KeyAlgorithm': (str, False)
     }
 
     def add_extension(self, template, add_resource):
 
         add_helpers(template)
 
         def add_policy(policy_statement):
```

### Comparing `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/PKG-INFO` & `troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troposphere-dns-certificate
-Version: 1.8.0
+Version: 2.0.0
 Summary: Cloudformation DNS validated certificate resource for troposphere
 Home-page: https://github.com/dflook/cloudformation-dns-certificate
 Author: Daniel Flook
 Author-email: daniel@flook.org
 License: MIT
 Project-URL: Issues, https://github.com/dflook/cloudformation-dns-certificate/issues
 Keywords: cloudformation troposphere certificate
@@ -13,14 +13,15 @@
 
 # Cloudformation DNS Validated Certificate Resource
 
 This is a cloudformation custom resource which is an enhancement of the [AWS::CertificateManager::Certificate](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-certificatemanager-certificate.html) resource.
 
 It allows creating a certificate in a region different from the stack's region (e.g. `us-east-1` for cloudfront),
 and allows for creating a certificate for a Route 53 hosted zone in another AWS account.
+It also allows for setting the key algorithm.
 
 ## Usage
 
 To use this custom resource, copy the CustomAcmCertificateLambda and CustomAcmCertificateLambdaExecutionRole resources
 into your template. You can then create certificate resources of Type: `Custom::DNSCertificate`.
 
 This resource is also available as troposphere extension, in the [troposphere-dns-certificate](https://pypi.org/project/troposphere-dns-certificate/) package
@@ -31,17 +32,19 @@
 
 ### Differences from AWS::CertificateManager::Certificate
 It should behave similarly to [AWS::CertificateManager::Certificate](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-certificatemanager-certificate.html), 
 except for the differences described here.
 
 The additional `Region` property can be used to set the region to create the certificate in.
 
-The [DomainValidationOption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-certificatemanager-certificate-domainvalidationoption.html) has an additional property `Route53RoleArn`, which is a role to assume before creating DNS validation records.
+The [DomainValidationOption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-certificatemanager-certificate-domainvalidationoption.html) has a additional properties `Route53RoleArn` and `Route53RoleExternalId` which allow assuming a role before creating DNS validation records.
 This lets you create a certificate for a hosted zone in another account.
 
+The additional `KeyAlgorithm` property allows setting the key algorithm used to generate the key pair used by the certificate.
+
 ### Certificate Resource
 
 #### Syntax
 
 ```yaml
 Type: Custom::DNSCertificate
 Properties: 
@@ -50,14 +53,16 @@
     - DomainValidationOption
   SubjectAlternativeNames:
     - String
   Tags:
     - Resource Tag
   ValidationMethod: String
   Region: String
+  CertificateTransparencyLoggingPreference: String
+  KeyAlgorithm: String
   ServiceToken: !GetAtt 'CustomAcmCertificateLambda.Arn'  
 ```
 
 #### Properties
 
 * `DomainName`
 
@@ -70,15 +75,15 @@
 * `DomainValidationOptions`
 
   Information for validating domain ownership. A DomainValidationOption should be present for the DomainName and all 
   SubjectAlternativeNames. A DomainValidationOption for a parent domain can be used for names that have the same HostedZoneId.
 
   - Required: Yes
   - Type: List of `DomainValidationOption`
-  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)  
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement) if a HostedZoneId changes
 
 * `SubjectAlternativeNames`
 
   FQDNs to include in the Subject Alternative Name of the certificate.
 
   - Required: No
   - Type: List of String values
@@ -106,14 +111,35 @@
   The region to create the certificate in.
 
   - Required: No
   - Default: The Stack's region
   - Type: String
   - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement) 
 
+* `CertificateTransparencyLoggingPreference`
+
+  Certificate Transparency Logging Preference. This may be 'ENABLED' or 'DISABLED'.
+    
+  - Required: No
+  - Default: `ENABLED`
+  - Type: String
+  - Update requires: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)  
+
+* `KeyAlgorithm`
+
+  The algorithm that will be used to generate the key pair used by the certificate.
+  Currently, this may be `RSA_2048`, `EC_prime256v1`, or `EC_secp384r1` for new certificates.
+
+  :warning: Not all algorithms are supported by all clients, AWS services or regions.
+
+  - Required: No
+  - Default: `RSA_2048`
+  - Type: String
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)
+
 #### Return value
 
 * Ref
 
   When the [`Ref`](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-ref.html) 
   function is used on the logical ID of a Certificate resource the certificate ARN is returned.
 
@@ -132,37 +158,41 @@
 
 * `DomainName`
 
   Fully qualified domain name of the validation request.
 
   - Required: Yes
   - Type: String
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)
   
 * `HostedZoneId`
 
   The Route53 Hosted Zone to create validation records in.
 
   - Required: Yes
   - Type: String
+  - Update requires: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement) 
   
 * `Route53RoleArn`
 
   The arn of an IAM Role to assume when creating DNS validation records. This can be used to create the records for a
   Hosted Zone in another AWS account.
 
   - Required: No
   - Type: String
+  - Update requires: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)  
 
 * `Route53RoleExternalId`
 
   An External ID to use when assuming the Route53RoleArn. This can be set if required by the trust policy of the role. 
   See https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-user_externalid.html for details of using ExternalIds.
 
   - Required: No
   - Type: String
+  - Update requires: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)
 
 ## Troposphere
 
 If you are using troposphere you can install this resource as an extension using pip:
 
     $ pip install troposphere_dns_certificate
 
@@ -344,14 +374,15 @@
       - PolicyDocument:
           Statement:
             - Action:
                 - acm:AddTagsToCertificate
                 - acm:DeleteCertificate
                 - acm:DescribeCertificate
                 - acm:RemoveTagsFromCertificate
+                - acm:UpdateCertificateOptions
               Effect: Allow
               Resource:
                 - !Sub 'arn:${AWS::Partition}:acm:*:${AWS::AccountId}:certificate/*'
             - Action:
                 - acm:RequestCertificate
                 - acm:ListTagsForCertificate
                 - acm:ListCertificates
```

### Comparing `troposphere-dns-certificate-1.8.0/src/troposphere_dns_certificate.egg-info/SOURCES.txt` & `troposphere-dns-certificate-2.0.0/src/troposphere_dns_certificate.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -6,8 +6,16 @@
 src/troposphere_dns_certificate/certificatemanager.py
 src/troposphere_dns_certificate.egg-info/PKG-INFO
 src/troposphere_dns_certificate.egg-info/SOURCES.txt
 src/troposphere_dns_certificate.egg-info/dependency_links.txt
 src/troposphere_dns_certificate.egg-info/not-zip-safe
 src/troposphere_dns_certificate.egg-info/requires.txt
 src/troposphere_dns_certificate.egg-info/top_level.txt
-test/test_lambda_code_size.py
+test/test_domain_name.py
+test/test_external_validation.py
+test/test_key_algorithm.py
+test/test_lambda_code_size.py
+test/test_region.py
+test/test_route53_role_arn.py
+test/test_tags.py
+test/test_transparency_logging.py
+test/test_validation_option.py
```

