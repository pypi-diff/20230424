# Comparing `tmp/moto-4.1.9.dev5.tar.gz` & `tmp/moto-4.1.9.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moto-4.1.9.dev5.tar", last modified: Mon Apr 24 13:34:35 2023, max compression
+gzip compressed data, was "moto-4.1.9.dev6.tar", last modified: Mon Apr 24 20:39:58 2023, max compression
```

## Comparing `moto-4.1.9.dev5.tar` & `moto-4.1.9.dev6.tar`

### file list

```diff
@@ -1,2078 +1,2078 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto/
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-24 13:34:27.000000 moto-4.1.9.dev5/moto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto/acm/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto/acmpca/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/acmpca/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto/amp/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/amp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/apigateway/integration_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/integration_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/integration_parsers/aws_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/integration_parsers/http_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/integration_parsers/unknown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    91751 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40056 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigateway/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    64715 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    36307 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/apigatewayv2/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/applicationautoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/applicationautoscaling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/appsync/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/appsync/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.036035 moto-4.1.9.dev5/moto/athena/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/athena/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    61357 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    65472 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/autoscaling/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/awslambda/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    74928 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/awslambda/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/backend_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/batch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    69404 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/batch_simple/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch_simple/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch_simple/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/batch_simple/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/budgets/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/budgets/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.040036 moto-4.1.9.dev5/moto/ce/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ce/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    37709 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    53038 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudformation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudfront/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudtrail/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33739 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30696 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cloudwatch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.044036 moto-4.1.9.dev5/moto/codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codebuild/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codecommit/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/codepipeline/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/cognitoidentity/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidentity/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/cognitoidp/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    83922 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/cognitoidp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/resources/jwks-private.json
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/resources/jwks-public.json
--rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/cognitoidp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.048036 moto-4.1.9.dev5/moto/comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/comprehend/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/config/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    81665 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/config/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   117575 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/resources/aws_managed_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/config/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/core/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/botocore_stubber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/common_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/custom_responses_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/model_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    40468 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/responses_custom_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/databrew/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25372 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19227 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/databrew/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datapipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.052037 moto-4.1.9.dev5/moto/datasync/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/datasync/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/dax/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/dms/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/ds/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ds/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42639 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/limits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.056037 moto-4.1.9.dev5/moto/dynamodb/models/
--rw-r--r--   0 runner    (1001) docker     (123)    33457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17443 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/models/dynamo_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    39809 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/models/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/models/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/dynamodb/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/ast_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    34656 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/key_condition_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/partiql.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/reserved_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/reserved_keywords.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/parsing/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    45017 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/dynamodb_v20111205/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodb_v20111205/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodbstreams/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodbstreams/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/dynamodbstreams/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/ebs/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ebs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ebs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ebs/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.060037 moto-4.1.9.dev5/moto/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.064038 moto-4.1.9.dev5/moto/ec2/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/amis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/availability_zones_and_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/carrier_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/customer_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/dhcp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/elastic_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/elastic_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/iam_instance_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/managed_prefixes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/nat_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/network_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/spot_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/transit_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/transit_gateway_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/transit_gateway_route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpc_peering_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpc_service_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpn_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/vpn_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/models/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.068038 moto-4.1.9.dev5/moto/ec2/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/amis.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.008033 moto-4.1.9.dev5/moto/ec2/resources/ecs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.076039 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/
--rw-r--r--   0 runner    (1001) docker     (123)   110385 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   184754 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   205924 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    76970 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   233439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   224300 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    41214 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   204442 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   236846 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   196475 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   151250 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   205418 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   205543 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   170773 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   216660 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   244124 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   219056 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   243613 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.008033 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.080039 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/
--rw-r--r--   0 runner    (1001) docker     (123)    40620 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    38329 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   112314 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    79281 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    42533 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    73186 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   100264 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   100490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    31415 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    64924 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   102387 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    23689 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    51746 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   121670 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    71490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    58608 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    38649 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    65537 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   200128 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   112258 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   147926 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.088040 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/
--rw-r--r--   0 runner    (1001) docker     (123)    38820 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37177 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   102960 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    72651 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    38975 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    69946 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    91900 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    92102 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    28787 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    60279 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    95067 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    50561 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    49457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   118040 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    69350 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    56856 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    36936 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    63575 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   194154 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   108910 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    47322 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   143512 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.092040 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    40058 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    36191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    34296 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    35491 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    40817 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    41887 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    37998 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    41546 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)  1306310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/instance_types.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.096041 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.100041 moto-4.1.9.dev5/moto/ec2/responses/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/_base_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/account_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/amis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/availability_zones_and_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/carrier_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/customer_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/dhcp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/egress_only_internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/elastic_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/elastic_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/iam_instance_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/nat_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/network_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/reserved_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/spot_fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/spot_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/transit_gateway_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/transit_gateway_route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/transit_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/virtual_private_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/vpc_peering_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/vpc_service_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    39221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/vpn_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/responses/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    28837 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.100041 moto-4.1.9.dev5/moto/ec2instanceconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2instanceconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2instanceconnect/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2instanceconnect/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ec2instanceconnect/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.100041 moto-4.1.9.dev5/moto/ecr/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/policy_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecr/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    86640 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ecs/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/efs/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    26760 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/efs/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/eks/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30391 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/eks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticache/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    57275 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elasticbeanstalk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.104042 moto-4.1.9.dev5/moto/elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elastictranscoder/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elastictranscoder/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elastictranscoder/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/elb/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25335 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    37722 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elb/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    70076 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    68565 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/elbv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/emr/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    65244 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/emrcontainers/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrcontainers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.108042 moto-4.1.9.dev5/moto/emrserverless/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/emrserverless/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/es/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/es/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/events/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    66807 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29565 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/firehose/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/forecast/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/forecast/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.112042 moto-4.1.9.dev5/moto/glacier/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glacier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.116043 moto-4.1.9.dev5/moto/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/glue_schema_registry_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/glue_schema_registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22412 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/glue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.116043 moto-4.1.9.dev5/moto/greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    54499 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30895 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/greengrass/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.116043 moto-4.1.9.dev5/moto/guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/guardduty/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.120043 moto-4.1.9.dev5/moto/iam/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)  1599363 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/aws_managed_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   118618 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/policy_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)   107097 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.120043 moto-4.1.9.dev5/moto/identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/identitystore/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.120043 moto-4.1.9.dev5/moto/instance_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/instance_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/instance_metadata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/instance_metadata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/instance_metadata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.120043 moto-4.1.9.dev5/moto/iot/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    70619 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    32365 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/iotdata/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/iotdata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37257 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideo/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/kms/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24852 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/policy_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/kms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.124043 moto-4.1.9.dev5/moto/lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/lakeformation/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/metric_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    37576 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/logs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37565 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/managedblockchain/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediaconnect/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/medialive/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/medialive/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.128044 moto-4.1.9.dev5/moto/mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediapackage/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastore/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/mediastoredata/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mediastoredata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/meteringmarketplace/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/moto_api/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/moto_api/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/managed_state_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/moto_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/moto_api/_internal/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/recorder/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/recorder/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_api/_internal/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.132044 moto-4.1.9.dev5/moto/moto_server/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/moto_server/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_server/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_server/threaded_moto_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_server/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/moto_server/werkzeug_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/mq/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19975 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/mq/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/neptune/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16695 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/neptune/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opensearch/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.136045 moto-4.1.9.dev5/moto/opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    24989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/opsworks/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/organizations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/packages/boto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/packages/boto/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/blockdevicemapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/ec2object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/instancetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/boto/ec2/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/packages/cfnresponse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/cfnresponse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/packages/cfnresponse/cfnresponse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/personalize/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/personalize/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/pinpoint/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.140045 moto-4.1.9.dev5/moto/polly/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/polly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/quicksight/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/ram/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ram/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/rds/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)   182267 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.016033 moto-4.1.9.dev5/moto/rds/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/rds/resources/cluster_options/
--rw-r--r--   0 runner    (1001) docker     (123)   480836 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/resources/cluster_options/aurora-postgresql.json
--rw-r--r--   0 runner    (1001) docker     (123)   133645 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/resources/cluster_options/neptune.json
--rw-r--r--   0 runner    (1001) docker     (123)    64354 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rds/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.144045 moto-4.1.9.dev5/moto/rdsdata/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rdsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rdsdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rdsdata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rdsdata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42945 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29591 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/redshiftdata/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/redshiftdata/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rekognition/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rekognition/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/rekognition/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/resourcegroups/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroups/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.148046 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28011 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/resourcegroupstaggingapi/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/route53/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37075 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    35235 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37251 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/route53resolver/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/cloud_formation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    90986 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)   119897 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/select_object_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/s3bucket_path/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3bucket_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3bucket_path/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.152046 moto-4.1.9.dev5/moto/s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/s3control/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    99020 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29641 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sagemaker/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/scheduler/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/sdb/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sdb/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/secretsmanager/list_secrets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/list_secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/list_secrets/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    32283 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/secretsmanager/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.156046 moto-4.1.9.dev5/moto/servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicediscovery/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/servicequotas/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/servicequotas/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/servicequotas/resources/default_quotas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/resources/default_quotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/resources/default_quotas/vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/servicequotas/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/ses/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/feedback.py
--rw-r--r--   0 runner    (1001) docker     (123)    21690 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    31667 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ses/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/signer/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/signer/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.160047 moto-4.1.9.dev5/moto/sns/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42303 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    46479 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sns/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.164047 moto-4.1.9.dev5/moto/sqs/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41436 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    29029 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sqs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.164047 moto-4.1.9.dev5/moto/ssm/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    80116 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.164047 moto-4.1.9.dev5/moto/ssm/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.172048 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.016033 moto-4.1.9.dev5/moto/ssm/resources/ecs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.192050 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/
--rw-r--r--   0 runner    (1001) docker     (123)   416937 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/af-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   688021 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   738181 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   360357 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   798560 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    85325 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   778515 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   239300 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   734929 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   806032 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    84904 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   717425 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   618637 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    99223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   737073 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   737391 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json
--rw-r--r--   0 runner    (1001) docker     (123)   164329 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/me-central-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   659463 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/me-south-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   761741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   823629 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-2.json
--rw-r--r--   0 runner    (1001) docker     (123)   767008 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   820874 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-2.json
--rw-r--r--   0 runner    (1001) docker     (123)  1745761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/regions.json
--rw-r--r--   0 runner    (1001) docker     (123)  1824341 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/resources/services.json
--rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.192050 moto-4.1.9.dev5/moto/ssoadmin/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/ssoadmin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.192050 moto-4.1.9.dev5/moto/stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21993 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/stepfunctions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/sts/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/sts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/support/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/support/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   172189 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/resources/describe_trusted_advisor_checks.json
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/support/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/swf/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.196050 moto-4.1.9.dev5/moto/swf/models/
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/activity_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/activity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/decision_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/generic_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/history_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30491 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/workflow_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/models/workflow_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    21829 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/swf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/textract/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/textract/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/timestreamwrite/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/timestreamwrite/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/transcribe/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/aws_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/distutils_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/docker_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/tagging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/wafv2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/moto/xray/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/moto/xray/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.032035 moto-4.1.9.dev5/moto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66096 2023-04-24 13:34:35.000000 moto-4.1.9.dev5/moto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 13:34:34.000000 moto-4.1.9.dev5/moto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-24 13:34:35.320062 moto-4.1.9.dev5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.200050 moto-4.1.9.dev5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_acm/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_acm/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/ca.key
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/ca.pem
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/ca.srl
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com-bad.pem
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.csr
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.key
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.pem
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acm/test_acm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_acmpca/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acmpca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_acmpca/test_acmpca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_amp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_amp/test_amp_logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_amp/test_amp_rulegroupnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_amp/test_amp_workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.204051 moto-4.1.9.dev5/tests/test_apigateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_apigateway/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/petstore-swagger-v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_api.json
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_api_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_api_invalid_version.json
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/resources/test_deep_api.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    91558 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_gatewayresponses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_importrestapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_putrestapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_vpclink.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigateway/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_reimport.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_apigatewayv2/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_applicationautoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_applicationautoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_applicationautoscaling/test_applicationautoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_applicationautoscaling/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_appsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_appsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_appsync_apikeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_appsync_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_appsync_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_appsync/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.208051 moto-4.1.9.dev5/tests/test_athena/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_athena/test_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_athena/test_athena_server_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.212052 moto-4.1.9.dev5/tests/test_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_scheduledactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_elb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_launch_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_autoscaling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.212052 moto-4.1.9.dev5/tests/test_awslambda/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_awslambda_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_eventsourcemapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_function_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_lambda_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_awslambda/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_compute_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    34446 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_tags_job_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_tags_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_tags_scheduling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_batch_task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_batch_simple/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch_simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch_simple/test_batch_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch_simple/test_batch_compute_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_batch_simple/test_batch_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_budgets/test_budgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_budgets/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_budgets/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_ce/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ce/test_ce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ce/test_ce_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.216052 moto-4.1.9.dev5/tests/test_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.220052 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/custom_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/ec2_classic_eip.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/fn_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/kms_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_roundrobin.py
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_eip.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_eni.py
--rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_custom_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_depends_on.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_multi_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_nested_stacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    85564 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    69300 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_import_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_stack_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudformation/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.220052 moto-4.1.9.dev5/tests/test_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/cloudfront_test_scaffolding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_dist_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    28631 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_invalidation.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudfront/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.220052 moto-4.1.9.dev5/tests/test_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail_eventselectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudtrail/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.220052 moto-4.1.9.dev5/tests/test_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)    54006 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_codebuild/test_codebuild.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_codecommit/test_codecommit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_codepipeline/test_codepipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_cognitoidentity/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidentity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidentity/test_cognitoidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidentity/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_cognitoidp/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   161791 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_cognitoidp/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_comprehend/test_comprehend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.224053 moto-4.1.9.dev5/tests/test_config/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83099 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/test_config_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/test_config_rules_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_config/test_config_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_account_id_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_backenddict.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_decorator_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_environ_patching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_importorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_instance_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_mock_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_mock_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_moto_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_request_mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_responses_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_url_base_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_url_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_databrew/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/test_databrew_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/test_databrew_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/test_databrew_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_databrew/test_databrew_rulesets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datapipeline/test_datapipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datapipeline/test_datapipeline_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datapipeline/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_datasync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_datasync/test_datasync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_dax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dax/test_dax.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dax/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.228053 moto-4.1.9.dev5/tests/test_dms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dms/test_dms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.232054 moto-4.1.9.dev5/tests/test_ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds_ad_connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds_microsoft_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds_simple_ad_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ds/test_ds_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.232054 moto-4.1.9.dev5/tests/test_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_dynamodb/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/exceptions/test_key_length_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_dynamodb/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/models/test_key_condition_expression_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   205697 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_batch_get_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_condition_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_consumedcapacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_create_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)    39804 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_table_with_range_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_table_without_range_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_update_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_update_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_dynamodb_v20111205/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb_v20111205/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43145 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb_v20111205/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodb_v20111205/test_servermode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_dynamodbstreams/test_dynamodbstreams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.236054 moto-4.1.9.dev5/tests/test_ebs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ebs/test_ebs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.244055 moto-4.1.9.dev5/tests/test_ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_account_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_amazon_dev_pay.py
--rw-r--r--   0 runner    (1001) docker     (123)    44698 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_amis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_availability_zones_and_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_carrier_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_customer_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_dhcp_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_ec2_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_ec2_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_ec2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_egress_only_igw.py
--rw-r--r--   0 runner    (1001) docker     (123)    42808 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_elastic_block_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_elastic_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    41728 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_elastic_network_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_fleets.py
--rw-r--r--   0 runner    (1001) docker     (123)    24744 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_flow_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_flow_logs_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_iam_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_instance_type_offerings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    98932 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_internet_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_ip_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_key_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_launch_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_nat_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_network_acls.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_placement_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_prefix_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_reserved_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    40328 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_route_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    65961 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_security_groups_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_spot_fleet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_spot_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway_peering_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_virtual_private_gateways.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vm_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vm_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpc_endpoint_services_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpc_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpc_service_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    45725 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_vpn_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2/test_windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.244055 moto-4.1.9.dev5/tests/test_ec2instanceconnect/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.244055 moto-4.1.9.dev5/tests/test_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92826 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/test_ecr_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/test_ecr_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/test_ecr_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecr/test_ecr_policy_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_account_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)   122563 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_capacity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    14232 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_efs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_task_def_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ecs/test_ecs_tasksets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_efs/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/junk_drawer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_access_point_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_access_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_filesystem_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_lifecycle_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_mount_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_mount_target_security_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_efs/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52255 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_eks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_eks_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_eks_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_eks_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_eks/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elasticache/test_elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elasticache/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elasticbeanstalk/test_eb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.248055 moto-4.1.9.dev5/tests/test_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elastictranscoder/__init__
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elastictranscoder/test_elastictranscoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elastictranscoder/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_elb/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41073 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb_availabilityzones.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_elb_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elb/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_elbv2/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66616 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_rule_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_set_subnets.py
--rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_target_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_elbv2/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_emr/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/test_emr_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/test_emr_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_emrcontainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrcontainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrcontainers/test_emrcontainers.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrcontainers/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.252055 moto-4.1.9.dev5/tests/test_emrserverless/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrserverless/test_emrserverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_emrserverless/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_es/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_es/test_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_es/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_events/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_event_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    81682 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_events_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_events_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_events/test_events_lambdatriggers_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose.py
--rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose_destination_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_firehose_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_firehose/test_http_destinations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_forecast/test_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.256056 moto-4.1.9.dev5/tests/test_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test_glacier_archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test_glacier_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test_glacier_vaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glacier/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.260056 moto-4.1.9.dev5/tests/test_glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.260056 moto-4.1.9.dev5/tests/test_glue/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/fixtures/datacatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/fixtures/schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    48038 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_datacatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_glue_job_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_partition_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    47112 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_glue/test_schema_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.260056 moto-4.1.9.dev5/tests/test_greengrass/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    20373 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.260056 moto-4.1.9.dev5/tests/test_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/test_guardduty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/test_guardduty_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/test_guardduty_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_guardduty/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.264057 moto-4.1.9.dev5/tests/test_iam/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   167646 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_access_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_account_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)    51772 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_password_last_used.py
--rw-r--r--   0 runner    (1001) docker     (123)    51265 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_iam_server_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iam/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.264057 moto-4.1.9.dev5/tests/test_identitystore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_identitystore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_identitystore/test_identitystore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.264057 moto-4.1.9.dev5/tests/test_iot/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_ca_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_deprecate_thing_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_domain_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_job_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    28056 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_thing_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_thing_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_things.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_iot_topic_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iot/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.264057 moto-4.1.9.dev5/tests/test_iotdata/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iotdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iotdata/test_iotdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_iotdata/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31019 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_stream_consumers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_stream_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesis/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideo/test_kinesisvideo.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideo/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_kms/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_kms_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_kms_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_kms_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_kms_policy_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_kms/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_lakeformation/test_lakeformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.268057 moto-4.1.9.dev5/tests/test_logs/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    47011 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/test_logs_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_logs/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_proposals.py
--rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediaconnect/test_mediaconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediaconnect/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_medialive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_medialive/test_medialive.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_medialive/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediapackage/test_mediapackage.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediapackage/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastore/test_mediastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastore/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_mediastoredata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastoredata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastoredata/test_mediastoredata.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mediastoredata/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_meteringmarketplace/test_meteringmarketplace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_moto_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_moto_api/mock_random/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/mock_random/test_mock_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.272057 moto-4.1.9.dev5/tests/test_moto_api/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/recorder/test_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_moto_api/state_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/test_state_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_batch_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_managed_state_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_mq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_mq_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_mq_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_mq_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_mq/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_neptune/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/test_cluster_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/test_cluster_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_neptune/test_global_clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opensearch/test_domain_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opensearch/test_opensearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/test_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_opsworks/test_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.276058 moto-4.1.9.dev5/tests/test_organizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_organizations/organizations_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    85363 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_organizations/test_organizations_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_personalize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_personalize/test_personalize_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_pinpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_pinpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint_application_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint_event_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_polly/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_polly/test_polly.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_polly/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_quicksight/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.280058 moto-4.1.9.dev5/tests/test_ram/
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ram/test_ram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_rds/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_db_cluster_param_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_db_cluster_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_global_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)    91218 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_clusters_with_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_event_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_rds_export_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rds/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_rdsdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rdsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rdsdata/test_rdsdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73309 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshift/test_redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshift/test_redshift_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshift/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_redshiftdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshiftdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshiftdata/test_redshiftdata.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshiftdata/test_redshiftdata_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_redshiftdata/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_rekognition/test_rekognition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_resourcegroups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroups/test_resourcegroups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.284058 moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.292059 moto-4.1.9.dev5/tests/test_route53/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_change_set_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52862 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53.py
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_delegationsets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_healthchecks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_query_logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_route53_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.292059 moto-4.1.9.dev5/tests/test_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40356 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    21968 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_rule_associations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.296059 moto-4.1.9.dev5/tests/test_s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_multiple_accounts_server.py
--rw-r--r--   0 runner    (1001) docker     (123)   115875 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_bucket_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_classdecorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18825 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_copyobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_custom_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_file_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_lambda_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    31026 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_multipart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_object_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_ownership.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_storageclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_tagging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.296059 moto-4.1.9.dev5/tests/test_s3bucket_path/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3bucket_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3bucket_path/test_s3bucket_path_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3bucket_path/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.296059 moto-4.1.9.dev5/tests/test_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control_access_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control_accesspoint_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control_config_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_s3control/test_s3control_s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/cloudformation_test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20469 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24758 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_trial_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/test_schedule_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/test_scheduler_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_scheduler/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_sdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sdb/test_sdb_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sdb/test_sdb_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sdb/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/test_list_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    57270 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/test_secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    33302 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_secretsmanager/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.300060 moto-4.1.9.dev5/tests/test_servicediscovery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_servicequotas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicequotas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_servicequotas/test_servicequotas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_ses/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    52328 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_ses_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_ses_sns_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_ses_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ses/test_templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_signer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_signer/test_signing_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_signer/test_signing_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_sns/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_application_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_publish_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    42807 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_publishing_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_sns_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_subscriptions_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sns/test_topics_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_special_cases/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_special_cases/test_custom_amis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.304060 moto-4.1.9.dev5/tests/test_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)   110801 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_sqs_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_sqs_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sqs/test_sqs_multiaccount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72442 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_default_amis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_doc_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28425 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_ec2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_ecs_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_maintenance_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_parameterstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_ssm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_ssm/test_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssm/test_templates/good.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_ssoadmin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssoadmin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssoadmin/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_ssoadmin/test_ssoadmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34241 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_stepfunctions/test_stepfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_stepfunctions/test_stepfunctions_cloudformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_sts/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sts/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sts/test_sts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_sts/test_sts_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.308061 moto-4.1.9.dev5/tests/test_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_support/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_support/test_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.312061 moto-4.1.9.dev5/tests/test_swf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.312061 moto-4.1.9.dev5/tests/test_swf/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_activity_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_decision_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_generic_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_history_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25245 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/models/test_workflow_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.312061 moto-4.1.9.dev5/tests/test_swf/responses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_activity_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_activity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21702 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_decision_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_workflow_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/responses/test_workflow_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_swf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.312061 moto-4.1.9.dev5/tests/test_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_textract/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_textract/test_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_timestreamwrite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_transcribe/test_transcribe_boto3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_utilities/test_docker_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_utilities/test_paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_utilities/test_tagging_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_utilities/test_threaded_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_wafv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:34:35.316061 moto-4.1.9.dev5/tests/test_xray/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_xray/test_xray_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-24 13:34:25.000000 moto-4.1.9.dev5/tests/test_xray/test_xray_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.661232 moto-4.1.9.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-24 20:39:58.661232 moto-4.1.9.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.437229 moto-4.1.9.dev6/moto/
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-24 20:39:52.000000 moto-4.1.9.dev6/moto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.441228 moto-4.1.9.dev6/moto/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acm/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acm/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.441228 moto-4.1.9.dev6/moto/acmpca/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acmpca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acmpca/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acmpca/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acmpca/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/acmpca/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.441228 moto-4.1.9.dev6/moto/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/amp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/amp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/amp/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/amp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/amp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.441228 moto-4.1.9.dev6/moto/apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.441228 moto-4.1.9.dev6/moto/apigateway/integration_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/integration_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/integration_parsers/aws_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/integration_parsers/http_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/integration_parsers/unknown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91751 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40056 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigateway/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.441228 moto-4.1.9.dev6/moto/apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigatewayv2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64715 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigatewayv2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36307 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigatewayv2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/apigatewayv2/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.445228 moto-4.1.9.dev6/moto/applicationautoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/applicationautoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/applicationautoscaling/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/applicationautoscaling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/applicationautoscaling/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/applicationautoscaling/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/applicationautoscaling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.445228 moto-4.1.9.dev6/moto/appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/appsync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/appsync/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/appsync/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/appsync/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.445228 moto-4.1.9.dev6/moto/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/athena/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12521 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/athena/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/athena/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/athena/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/athena/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.445228 moto-4.1.9.dev6/moto/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/autoscaling/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61357 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/autoscaling/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65472 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/autoscaling/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/autoscaling/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.445228 moto-4.1.9.dev6/moto/awslambda/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/awslambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/awslambda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74928 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/awslambda/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/awslambda/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/awslambda/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/awslambda/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/awslambda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/backend_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.445228 moto-4.1.9.dev6/moto/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69404 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.449229 moto-4.1.9.dev6/moto/batch_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch_simple/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch_simple/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/batch_simple/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.449229 moto-4.1.9.dev6/moto/budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/budgets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/budgets/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/budgets/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/budgets/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.449229 moto-4.1.9.dev6/moto/ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ce/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ce/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ce/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ce/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.449229 moto-4.1.9.dev6/moto/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudformation/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudformation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudformation/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37709 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudformation/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53038 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudformation/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudformation/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudformation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.449229 moto-4.1.9.dev6/moto/cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudfront/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudfront/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudfront/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudfront/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.449229 moto-4.1.9.dev6/moto/cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudtrail/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudtrail/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudtrail/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudtrail/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.449229 moto-4.1.9.dev6/moto/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudwatch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33739 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudwatch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30696 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudwatch/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudwatch/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cloudwatch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.453229 moto-4.1.9.dev6/moto/codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codebuild/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codebuild/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codebuild/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codebuild/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.453229 moto-4.1.9.dev6/moto/codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codecommit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codecommit/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codecommit/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codecommit/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.453229 moto-4.1.9.dev6/moto/codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codepipeline/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codepipeline/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codepipeline/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/codepipeline/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.453229 moto-4.1.9.dev6/moto/cognitoidentity/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidentity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidentity/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidentity/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidentity/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidentity/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidentity/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.453229 moto-4.1.9.dev6/moto/cognitoidp/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83922 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.453229 moto-4.1.9.dev6/moto/cognitoidp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidp/resources/jwks-private.json
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidp/resources/jwks-public.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24950 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidp/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/cognitoidp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.453229 moto-4.1.9.dev6/moto/comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/comprehend/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/comprehend/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/comprehend/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/comprehend/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.453229 moto-4.1.9.dev6/moto/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12433 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81665 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/config/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.453229 moto-4.1.9.dev6/moto/config/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   117575 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/config/resources/aws_managed_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/config/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/config/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.457229 moto-4.1.9.dev6/moto/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11074 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/botocore_stubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/common_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/custom_responses_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/model_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40468 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/responses_custom_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.457229 moto-4.1.9.dev6/moto/databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/databrew/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25372 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/databrew/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19227 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/databrew/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/databrew/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.457229 moto-4.1.9.dev6/moto/datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datapipeline/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datapipeline/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datapipeline/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datapipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.457229 moto-4.1.9.dev6/moto/datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datasync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datasync/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datasync/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/datasync/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.457229 moto-4.1.9.dev6/moto/dax/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dax/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dax/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dax/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dax/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.461229 moto-4.1.9.dev6/moto/dms/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dms/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.461229 moto-4.1.9.dev6/moto/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ds/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21712 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ds/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ds/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ds/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ds/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ds/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.461229 moto-4.1.9.dev6/moto/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42639 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/limits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.461229 moto-4.1.9.dev6/moto/dynamodb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    33457 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17443 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/models/dynamo_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39809 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/models/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.461229 moto-4.1.9.dev6/moto/dynamodb/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/ast_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12062 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34656 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/key_condition_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/partiql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/reserved_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/reserved_keywords.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/parsing/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45017 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.461229 moto-4.1.9.dev6/moto/dynamodb_v20111205/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb_v20111205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb_v20111205/comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb_v20111205/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb_v20111205/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodb_v20111205/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.465229 moto-4.1.9.dev6/moto/dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodbstreams/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodbstreams/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/dynamodbstreams/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.465229 moto-4.1.9.dev6/moto/ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ebs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ebs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ebs/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.465229 moto-4.1.9.dev6/moto/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.469229 moto-4.1.9.dev6/moto/ec2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/availability_zones_and_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/carrier_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/dhcp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19544 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/elastic_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16432 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/elastic_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/iam_instance_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/managed_prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/nat_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20404 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/spot_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/transit_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/transit_gateway_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/transit_gateway_route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/vpc_peering_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/vpc_service_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33929 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/vpn_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/vpn_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/models/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.469229 moto-4.1.9.dev6/moto/ec2/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    24777 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/amis.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.421228 moto-4.1.9.dev6/moto/ec2/resources/ecs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.477229 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/
+-rw-r--r--   0 runner    (1001) docker     (123)   110385 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   184754 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205924 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    76970 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   233439 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224300 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   237334 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41214 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   204442 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   236846 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   196475 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   151250 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205418 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205543 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27007 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   170773 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   216660 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   244124 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   241191 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219056 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   243613 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.421228 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.481229 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/
+-rw-r--r--   0 runner    (1001) docker     (123)    40620 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38329 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   112314 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79281 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42533 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    73186 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100264 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   100490 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31415 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64924 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   102387 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23689 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    52898 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51746 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23840 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121670 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71490 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58608 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38649 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65537 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   200128 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   112258 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147926 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.485229 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/
+-rw-r--r--   0 runner    (1001) docker     (123)    38820 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37177 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   102960 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72651 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38975 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    69946 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    91900 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    92102 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28787 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60279 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    95067 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50561 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49457 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   118040 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    69350 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56856 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22778 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36936 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63575 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   194154 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   108910 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47322 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   143512 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.489229 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12719 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40058 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25981 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36191 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34296 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35491 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40817 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24736 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41887 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37998 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41546 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/us-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1306310 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/instance_types.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.493229 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/resources/latest_amis/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.497229 moto-4.1.9.dev6/moto/ec2/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/_base_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/account_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/availability_zones_and_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/carrier_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/dhcp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/egress_only_internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/elastic_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/elastic_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24972 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/iam_instance_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40932 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/nat_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/reserved_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/spot_fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/spot_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24840 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/transit_gateway_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/transit_gateway_route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/transit_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/virtual_private_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/vpc_peering_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/vpc_service_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39221 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/vpn_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/responses/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28837 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.497229 moto-4.1.9.dev6/moto/ec2instanceconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2instanceconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2instanceconnect/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2instanceconnect/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ec2instanceconnect/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.497229 moto-4.1.9.dev6/moto/ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecr/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecr/policy_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecr/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecr/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.501229 moto-4.1.9.dev6/moto/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86640 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22481 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ecs/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.501229 moto-4.1.9.dev6/moto/efs/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/efs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26760 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/efs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/efs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/efs/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.501229 moto-4.1.9.dev6/moto/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/eks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30391 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/eks/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/eks/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/eks/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/eks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.501229 moto-4.1.9.dev6/moto/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticache/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticache/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticache/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticache/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.501229 moto-4.1.9.dev6/moto/elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticbeanstalk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticbeanstalk/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57275 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticbeanstalk/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticbeanstalk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elasticbeanstalk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.501229 moto-4.1.9.dev6/moto/elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elastictranscoder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elastictranscoder/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elastictranscoder/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.505229 moto-4.1.9.dev6/moto/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25335 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elb/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37722 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elb/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elb/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.505229 moto-4.1.9.dev6/moto/elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elbv2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70076 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elbv2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68565 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elbv2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elbv2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/elbv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.505229 moto-4.1.9.dev6/moto/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emr/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65244 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emr/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emr/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.505229 moto-4.1.9.dev6/moto/emrcontainers/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrcontainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrcontainers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrcontainers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrcontainers/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrcontainers/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrcontainers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.505229 moto-4.1.9.dev6/moto/emrserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrserverless/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrserverless/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrserverless/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrserverless/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/emrserverless/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.505229 moto-4.1.9.dev6/moto/es/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/es/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/es/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/es/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/es/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.509230 moto-4.1.9.dev6/moto/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66807 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/events/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/events/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/events/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.509230 moto-4.1.9.dev6/moto/firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/firehose/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29565 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/firehose/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/firehose/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/firehose/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.509230 moto-4.1.9.dev6/moto/forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/forecast/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/forecast/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/forecast/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/forecast/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.509230 moto-4.1.9.dev6/moto/glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glacier/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glacier/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glacier/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glacier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.509230 moto-4.1.9.dev6/moto/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glue/glue_schema_registry_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glue/glue_schema_registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glue/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22412 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glue/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12557 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/glue/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.509230 moto-4.1.9.dev6/moto/greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/greengrass/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54499 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/greengrass/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30895 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/greengrass/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/greengrass/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.509230 moto-4.1.9.dev6/moto/guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/guardduty/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/guardduty/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/guardduty/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/guardduty/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.513229 moto-4.1.9.dev6/moto/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1599363 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/aws_managed_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118618 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/policy_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107097 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.513229 moto-4.1.9.dev6/moto/identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/identitystore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/identitystore/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/identitystore/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/identitystore/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.513229 moto-4.1.9.dev6/moto/instance_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/instance_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/instance_metadata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/instance_metadata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/instance_metadata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.513229 moto-4.1.9.dev6/moto/iot/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70619 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32365 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iot/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iot/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.517229 moto-4.1.9.dev6/moto/iotdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iotdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iotdata/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iotdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iotdata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/iotdata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.517229 moto-4.1.9.dev6/moto/kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37257 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesis/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesis/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesis/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.517229 moto-4.1.9.dev6/moto/kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideo/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideo/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.517229 moto-4.1.9.dev6/moto/kinesisvideoarchivedmedia/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideoarchivedmedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideoarchivedmedia/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideoarchivedmedia/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideoarchivedmedia/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kinesisvideoarchivedmedia/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.517229 moto-4.1.9.dev6/moto/kms/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24852 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kms/policy_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26610 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kms/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/kms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.517229 moto-4.1.9.dev6/moto/lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/lakeformation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/lakeformation/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/lakeformation/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/lakeformation/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.517229 moto-4.1.9.dev6/moto/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/logs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/logs/metric_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37576 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/logs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/logs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/logs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/logs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.521230 moto-4.1.9.dev6/moto/managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/managedblockchain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37565 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/managedblockchain/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/managedblockchain/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/managedblockchain/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/managedblockchain/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.521230 moto-4.1.9.dev6/moto/mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediaconnect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediaconnect/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediaconnect/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediaconnect/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.521230 moto-4.1.9.dev6/moto/medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/medialive/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/medialive/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/medialive/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/medialive/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.521230 moto-4.1.9.dev6/moto/mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediapackage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediapackage/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediapackage/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediapackage/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.521230 moto-4.1.9.dev6/moto/mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastore/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastore/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastore/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.521230 moto-4.1.9.dev6/moto/mediastoredata/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastoredata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastoredata/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastoredata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastoredata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mediastoredata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.521230 moto-4.1.9.dev6/moto/meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/meteringmarketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/meteringmarketplace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/meteringmarketplace/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/meteringmarketplace/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/meteringmarketplace/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.521230 moto-4.1.9.dev6/moto/moto_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/moto_api/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/managed_state_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/moto_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/moto_api/_internal/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/recorder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/recorder/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_api/_internal/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/moto_server/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/moto_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_server/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_server/threaded_moto_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_server/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/moto_server/werkzeug_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mq/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19975 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mq/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mq/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/mq/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/neptune/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16695 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/neptune/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/neptune/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/neptune/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opensearch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opensearch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opensearch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opensearch/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opensearch/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opsworks/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opsworks/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opsworks/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/opsworks/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/organizations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/organizations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/organizations/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/organizations/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/organizations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.525230 moto-4.1.9.dev6/moto/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.529230 moto-4.1.9.dev6/moto/packages/boto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/boto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.529230 moto-4.1.9.dev6/moto/packages/boto/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/boto/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/boto/ec2/blockdevicemapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/boto/ec2/ec2object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/boto/ec2/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/boto/ec2/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/boto/ec2/instancetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/boto/ec2/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.529230 moto-4.1.9.dev6/moto/packages/cfnresponse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/cfnresponse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/packages/cfnresponse/cfnresponse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.529230 moto-4.1.9.dev6/moto/personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/personalize/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/personalize/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/personalize/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/personalize/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.529230 moto-4.1.9.dev6/moto/pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/pinpoint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/pinpoint/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/pinpoint/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/pinpoint/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.529230 moto-4.1.9.dev6/moto/polly/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/polly/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/polly/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/polly/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/polly/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/polly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.529230 moto-4.1.9.dev6/moto/quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/quicksight/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/quicksight/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/quicksight/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/quicksight/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.529230 moto-4.1.9.dev6/moto/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ram/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ram/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ram/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ram/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.533230 moto-4.1.9.dev6/moto/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rds/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182267 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rds/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.425228 moto-4.1.9.dev6/moto/rds/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.533230 moto-4.1.9.dev6/moto/rds/resources/cluster_options/
+-rw-r--r--   0 runner    (1001) docker     (123)   480836 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rds/resources/cluster_options/aurora-postgresql.json
+-rw-r--r--   0 runner    (1001) docker     (123)   133645 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rds/resources/cluster_options/neptune.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64354 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rds/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rds/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rds/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.533230 moto-4.1.9.dev6/moto/rdsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rdsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rdsdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rdsdata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rdsdata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.533230 moto-4.1.9.dev6/moto/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshift/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42945 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshift/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29591 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshift/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshift/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.533230 moto-4.1.9.dev6/moto/redshiftdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshiftdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshiftdata/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshiftdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshiftdata/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/redshiftdata/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.533230 moto-4.1.9.dev6/moto/rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rekognition/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rekognition/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/rekognition/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.533230 moto-4.1.9.dev6/moto/resourcegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/resourcegroups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/resourcegroups/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/resourcegroups/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/resourcegroups/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/resourcegroups/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.533230 moto-4.1.9.dev6/moto/resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28011 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/resourcegroupstaggingapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/resourcegroupstaggingapi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/resourcegroupstaggingapi/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.537230 moto-4.1.9.dev6/moto/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37075 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35235 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.537230 moto-4.1.9.dev6/moto/route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53resolver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37251 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53resolver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53resolver/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53resolver/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53resolver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/route53resolver/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.537230 moto-4.1.9.dev6/moto/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/cloud_formation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90986 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119897 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/select_object_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.537230 moto-4.1.9.dev6/moto/s3bucket_path/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3bucket_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3bucket_path/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.537230 moto-4.1.9.dev6/moto/s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3control/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3control/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3control/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3control/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/s3control/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.537230 moto-4.1.9.dev6/moto/sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sagemaker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99020 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sagemaker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29641 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sagemaker/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sagemaker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sagemaker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sagemaker/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.541230 moto-4.1.9.dev6/moto/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/scheduler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/scheduler/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/scheduler/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/scheduler/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.541230 moto-4.1.9.dev6/moto/sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sdb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sdb/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sdb/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.541230 moto-4.1.9.dev6/moto/secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/secretsmanager/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.541230 moto-4.1.9.dev6/moto/secretsmanager/list_secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/secretsmanager/list_secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/secretsmanager/list_secrets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32283 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/secretsmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/secretsmanager/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/secretsmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/secretsmanager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.541230 moto-4.1.9.dev6/moto/servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicediscovery/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicediscovery/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicediscovery/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicediscovery/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.541230 moto-4.1.9.dev6/moto/servicequotas/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicequotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicequotas/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicequotas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.541230 moto-4.1.9.dev6/moto/servicequotas/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicequotas/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.541230 moto-4.1.9.dev6/moto/servicequotas/resources/default_quotas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicequotas/resources/default_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicequotas/resources/default_quotas/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicequotas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/servicequotas/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.541230 moto-4.1.9.dev6/moto/ses/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ses/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ses/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21690 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ses/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31667 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ses/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ses/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ses/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ses/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.545230 moto-4.1.9.dev6/moto/signer/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/signer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/signer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/signer/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/signer/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.545230 moto-4.1.9.dev6/moto/sns/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sns/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42303 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sns/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46479 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sns/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sns/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sns/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.545230 moto-4.1.9.dev6/moto/sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sqs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sqs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44150 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sqs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29662 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sqs/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sqs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sqs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.545230 moto-4.1.9.dev6/moto/ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80116 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.549230 moto-4.1.9.dev6/moto/ssm/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.553230 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.429228 moto-4.1.9.dev6/moto/ssm/resources/ecs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.569230 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/
+-rw-r--r--   0 runner    (1001) docker     (123)   416937 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/af-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   688021 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   738181 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   360357 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   798560 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85325 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   778515 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   807102 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   239300 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   734929 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   806032 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    84904 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   717425 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   618637 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    99223 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   737073 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   737391 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)   164329 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/me-central-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   659463 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/me-south-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   761741 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   823629 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   815560 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/us-east-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)   767008 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/us-west-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   820874 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/us-west-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1745761 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1824341 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/resources/services.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.569230 moto-4.1.9.dev6/moto/ssoadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssoadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssoadmin/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssoadmin/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssoadmin/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssoadmin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/ssoadmin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.569230 moto-4.1.9.dev6/moto/stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/stepfunctions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21993 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/stepfunctions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/stepfunctions/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/stepfunctions/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/stepfunctions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.569230 moto-4.1.9.dev6/moto/sts/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sts/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sts/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sts/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/sts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.573230 moto-4.1.9.dev6/moto/support/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/support/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/support/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.573230 moto-4.1.9.dev6/moto/support/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   172189 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/support/resources/describe_trusted_advisor_checks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/support/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/support/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.573230 moto-4.1.9.dev6/moto/swf/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.573230 moto-4.1.9.dev6/moto/swf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/activity_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/decision_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/generic_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/history_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30491 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/workflow_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/models/workflow_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21829 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/swf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.573230 moto-4.1.9.dev6/moto/textract/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/textract/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/textract/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/textract/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/textract/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.573230 moto-4.1.9.dev6/moto/timestreamwrite/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/timestreamwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/timestreamwrite/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/timestreamwrite/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/timestreamwrite/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/timestreamwrite/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.573230 moto-4.1.9.dev6/moto/transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/transcribe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/transcribe/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/transcribe/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/transcribe/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.577230 moto-4.1.9.dev6/moto/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/utilities/aws_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/utilities/distutils_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/utilities/docker_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/utilities/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/utilities/tagging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/utilities/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.577230 moto-4.1.9.dev6/moto/wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/wafv2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/wafv2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/wafv2/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/wafv2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/wafv2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.577230 moto-4.1.9.dev6/moto/xray/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/xray/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/xray/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/xray/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/xray/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/moto/xray/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.441228 moto-4.1.9.dev6/moto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-24 20:39:58.000000 moto-4.1.9.dev6/moto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66096 2023-04-24 20:39:58.000000 moto-4.1.9.dev6/moto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:39:58.000000 moto-4.1.9.dev6/moto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 20:39:58.000000 moto-4.1.9.dev6/moto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-24 20:39:58.000000 moto-4.1.9.dev6/moto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 20:39:58.000000 moto-4.1.9.dev6/moto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-24 20:39:58.661232 moto-4.1.9.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.577230 moto-4.1.9.dev6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.577230 moto-4.1.9.dev6/tests/test_acm/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.577230 moto-4.1.9.dev6/tests/test_acm/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/resources/ca.key
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/resources/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/resources/ca.srl
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/resources/star_moto_com-bad.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/resources/star_moto_com.csr
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/resources/star_moto_com.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/resources/star_moto_com.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acm/test_acm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.577230 moto-4.1.9.dev6/tests/test_acmpca/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acmpca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12974 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_acmpca/test_acmpca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.577230 moto-4.1.9.dev6/tests/test_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_amp/test_amp_logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_amp/test_amp_rulegroupnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_amp/test_amp_workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.581230 moto-4.1.9.dev6/tests/test_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.581230 moto-4.1.9.dev6/tests/test_apigateway/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/resources/petstore-swagger-v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/resources/test_api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/resources/test_api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/resources/test_api_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/resources/test_api_invalid_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/resources/test_deep_api.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    91558 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_gatewayresponses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_importrestapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_putrestapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18926 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_vpclink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigateway/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.581230 moto-4.1.9.dev6/tests/test_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_reimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_apigatewayv2/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.581230 moto-4.1.9.dev6/tests/test_applicationautoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_applicationautoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25223 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_applicationautoscaling/test_applicationautoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_applicationautoscaling/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.585230 moto-4.1.9.dev6/tests/test_appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_appsync/test_appsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_appsync/test_appsync_apikeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_appsync/test_appsync_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_appsync/test_appsync_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_appsync/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.585230 moto-4.1.9.dev6/tests/test_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15059 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_athena/test_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_athena/test_athena_server_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.585230 moto-4.1.9.dev6/tests/test_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48170 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_scheduledactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_launch_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_autoscaling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.585230 moto-4.1.9.dev6/tests/test_awslambda/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_awslambda_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46812 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_lambda_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_lambda_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_lambda_eventsourcemapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_lambda_function_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_lambda_invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_lambda_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_lambda_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_lambda_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_awslambda/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.589231 moto-4.1.9.dev6/tests/test_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch_compute_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34446 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch_scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch_tags_job_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch_tags_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch_tags_scheduling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_batch_task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.589231 moto-4.1.9.dev6/tests/test_batch_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch_simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch_simple/test_batch_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch_simple/test_batch_compute_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_batch_simple/test_batch_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.589231 moto-4.1.9.dev6/tests/test_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_budgets/test_budgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_budgets/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_budgets/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.589231 moto-4.1.9.dev6/tests/test_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ce/test_ce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ce/test_ce_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.589231 moto-4.1.9.dev6/tests/test_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/custom_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/ec2_classic_eip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/fn_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/kms_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/route53_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/route53_roundrobin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/vpc_eip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/vpc_eni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12162 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_custom_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_depends_on.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_multi_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_nested_stacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85564 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69300 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_stack_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_stack_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_import_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21917 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_stack_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudformation/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudfront/cloudfront_test_scaffolding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudfront/test_cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudfront/test_cloudfront_dist_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28631 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudfront/test_cloudfront_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudfront/test_cloudfront_invalidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudfront/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudtrail/test_cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudtrail/test_cloudtrail_eventselectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudtrail/test_cloudtrail_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudtrail/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8634 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudwatch/test_cloudwatch_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54006 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudwatch/test_cloudwatch_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudwatch/test_cloudwatch_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cloudwatch/test_cloudwatch_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_codebuild/test_codebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_codecommit/test_codecommit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_codepipeline/test_codepipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_cognitoidentity/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cognitoidentity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cognitoidentity/test_cognitoidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cognitoidentity/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_cognitoidp/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cognitoidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161791 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cognitoidp/test_cognitoidp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cognitoidp/test_cognitoidp_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cognitoidp/test_cognitoidp_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_cognitoidp/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.593231 moto-4.1.9.dev6/tests/test_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_comprehend/test_comprehend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.597231 moto-4.1.9.dev6/tests/test_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83099 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18070 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_config/test_config_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_config/test_config_rules_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_config/test_config_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.597231 moto-4.1.9.dev6/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_account_id_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26898 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_backenddict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_decorator_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_environ_patching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_importorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_instance_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_mock_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_mock_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_moto_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_request_mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_responses_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_url_base_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_url_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.597231 moto-4.1.9.dev6/tests/test_databrew/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_databrew/test_databrew_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_databrew/test_databrew_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_databrew/test_databrew_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_databrew/test_databrew_rulesets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.597231 moto-4.1.9.dev6/tests/test_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_datapipeline/test_datapipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_datapipeline/test_datapipeline_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_datapipeline/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.597231 moto-4.1.9.dev6/tests/test_datasync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_datasync/test_datasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.601231 moto-4.1.9.dev6/tests/test_dax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16182 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dax/test_dax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dax/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.601231 moto-4.1.9.dev6/tests/test_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dms/test_dms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.601231 moto-4.1.9.dev6/tests/test_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ds/test_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ds/test_ds_ad_connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ds/test_ds_microsoft_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ds/test_ds_simple_ad_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ds/test_ds_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.601231 moto-4.1.9.dev6/tests/test_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.601231 moto-4.1.9.dev6/tests/test_dynamodb/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12004 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/exceptions/test_key_length_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.601231 moto-4.1.9.dev6/tests/test_dynamodb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/models/test_key_condition_expression_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   205697 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_batch_get_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_condition_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_consumedcapacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17832 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39804 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_table_with_range_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_table_without_range_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_update_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_update_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.601231 moto-4.1.9.dev6/tests/test_dynamodb_v20111205/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb_v20111205/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43145 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb_v20111205/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodb_v20111205/test_servermode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.605231 moto-4.1.9.dev6/tests/test_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_dynamodbstreams/test_dynamodbstreams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.605231 moto-4.1.9.dev6/tests/test_ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ebs/test_ebs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.609231 moto-4.1.9.dev6/tests/test_ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_account_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_amazon_dev_pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44698 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_availability_zones_and_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_carrier_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_customer_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_dhcp_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_ec2_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_ec2_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_ec2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_egress_only_igw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42808 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_elastic_block_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_elastic_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41728 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_elastic_network_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_fleets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24744 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_flow_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_flow_logs_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_iam_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_instance_type_offerings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98932 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_internet_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_ip_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_key_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_launch_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_nat_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_network_acls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_placement_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_prefix_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_reserved_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40328 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_route_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65961 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_security_groups_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_spot_fleet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_spot_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_transit_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_transit_gateway_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_transit_gateway_peering_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_virtual_private_gateways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_vm_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_vm_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_vpc_endpoint_services_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19510 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_vpc_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_vpc_service_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45725 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_vpn_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2/test_windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.609231 moto-4.1.9.dev6/tests/test_ec2instanceconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.609231 moto-4.1.9.dev6/tests/test_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92826 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecr/test_ecr_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecr/test_ecr_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecr/test_ecr_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecr/test_ecr_policy_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.613231 moto-4.1.9.dev6/tests/test_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecs/test_ecs_account_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122563 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecs/test_ecs_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecs/test_ecs_capacity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14232 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecs/test_ecs_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecs/test_ecs_efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecs/test_ecs_task_def_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ecs/test_ecs_tasksets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.613231 moto-4.1.9.dev6/tests/test_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/junk_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/test_access_point_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/test_access_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/test_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/test_filesystem_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/test_lifecycle_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/test_mount_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/test_mount_target_security_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_efs/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.613231 moto-4.1.9.dev6/tests/test_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52255 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_eks/test_eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_eks/test_eks_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_eks/test_eks_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_eks/test_eks_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_eks/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.613231 moto-4.1.9.dev6/tests/test_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elasticache/test_elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elasticache/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.613231 moto-4.1.9.dev6/tests/test_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elasticbeanstalk/test_eb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.613231 moto-4.1.9.dev6/tests/test_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elastictranscoder/__init__
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elastictranscoder/test_elastictranscoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elastictranscoder/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.613231 moto-4.1.9.dev6/tests/test_elb/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41073 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elb/test_elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elb/test_elb_availabilityzones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elb/test_elb_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elb/test_elb_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elb/test_elb_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elb/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.617231 moto-4.1.9.dev6/tests/test_elbv2/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66616 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/test_elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_listener_rule_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_listener_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_listener_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_set_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_target_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_elbv2/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.617231 moto-4.1.9.dev6/tests/test_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emr/test_emr_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emr/test_emr_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emr/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.617231 moto-4.1.9.dev6/tests/test_emrcontainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emrcontainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emrcontainers/test_emrcontainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emrcontainers/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.617231 moto-4.1.9.dev6/tests/test_emrserverless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emrserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emrserverless/test_emrserverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_emrserverless/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.617231 moto-4.1.9.dev6/tests/test_es/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_es/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_es/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.617231 moto-4.1.9.dev6/tests/test_events/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_events/test_event_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81682 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_events/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_events/test_events_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_events/test_events_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_events/test_events_lambdatriggers_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.617231 moto-4.1.9.dev6/tests/test_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_firehose/test_firehose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_firehose/test_firehose_destination_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_firehose/test_firehose_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_firehose/test_firehose_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_firehose/test_firehose_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_firehose/test_http_destinations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.617231 moto-4.1.9.dev6/tests/test_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_forecast/test_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.621231 moto-4.1.9.dev6/tests/test_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glacier/test.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glacier/test_glacier_archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glacier/test_glacier_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glacier/test_glacier_vaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glacier/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.621231 moto-4.1.9.dev6/tests/test_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.621231 moto-4.1.9.dev6/tests/test_glue/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/fixtures/datacatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/fixtures/schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48038 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/test_datacatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14918 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/test_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/test_glue_job_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14929 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/test_partition_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47112 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_glue/test_schema_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.621231 moto-4.1.9.dev6/tests/test_greengrass/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_greengrass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13441 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18455 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21905 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20373 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.621231 moto-4.1.9.dev6/tests/test_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_guardduty/test_guardduty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_guardduty/test_guardduty_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_guardduty/test_guardduty_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_guardduty/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.625231 moto-4.1.9.dev6/tests/test_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167646 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_iam_access_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_iam_account_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51772 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_iam_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11597 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_iam_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_iam_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_iam_password_last_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51265 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_iam_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_iam_server_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iam/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.625231 moto-4.1.9.dev6/tests/test_identitystore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_identitystore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_identitystore/test_identitystore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.625231 moto-4.1.9.dev6/tests/test_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_ca_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_deprecate_thing_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_domain_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_job_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28056 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_thing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_thing_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_iot_topic_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iot/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.625231 moto-4.1.9.dev6/tests/test_iotdata/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iotdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iotdata/test_iotdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_iotdata/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.625231 moto-4.1.9.dev6/tests/test_kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31019 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesis/test_kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_stream_consumers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_stream_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesis/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.625231 moto-4.1.9.dev6/tests/test_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesisvideo/test_kinesisvideo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesisvideo/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.625231 moto-4.1.9.dev6/tests/test_kinesisvideoarchivedmedia/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesisvideoarchivedmedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kinesisvideoarchivedmedia/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.629231 moto-4.1.9.dev6/tests/test_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kms/test_kms_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kms/test_kms_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kms/test_kms_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kms/test_kms_policy_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kms/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kms/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_kms/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.629231 moto-4.1.9.dev6/tests/test_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_lakeformation/test_lakeformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.629231 moto-4.1.9.dev6/tests/test_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_logs/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47011 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_logs/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_logs/test_logs_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_logs/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.629231 moto-4.1.9.dev6/tests/test_managedblockchain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_managedblockchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_managedblockchain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_proposals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22370 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.629231 moto-4.1.9.dev6/tests/test_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25975 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediaconnect/test_mediaconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediaconnect/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.629231 moto-4.1.9.dev6/tests/test_medialive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12296 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_medialive/test_medialive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_medialive/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.629231 moto-4.1.9.dev6/tests/test_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediapackage/test_mediapackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediapackage/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.629231 moto-4.1.9.dev6/tests/test_mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediastore/test_mediastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediastore/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.629231 moto-4.1.9.dev6/tests/test_mediastoredata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediastoredata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediastoredata/test_mediastoredata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mediastoredata/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_meteringmarketplace/test_meteringmarketplace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_moto_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_moto_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_moto_api/mock_random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_moto_api/mock_random/test_mock_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_moto_api/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_moto_api/recorder/test_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_moto_api/state_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_moto_api/state_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_moto_api/state_manager/servermode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_moto_api/state_manager/servermode/test_state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_moto_api/state_manager/test_batch_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_moto_api/state_manager/test_managed_state_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_moto_api/state_manager/test_state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mq/test_mq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mq/test_mq_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mq/test_mq_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mq/test_mq_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_mq/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_neptune/test_cluster_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_neptune/test_cluster_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_neptune/test_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_neptune/test_global_clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_opensearch/test_domain_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_opensearch/test_opensearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_opsworks/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_opsworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_opsworks/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_opsworks/test_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_opsworks/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_opsworks/test_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_organizations/organizations_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85363 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_organizations/test_organizations_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_personalize/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_personalize/test_personalize_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_pinpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_pinpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_pinpoint/test_pinpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_pinpoint/test_pinpoint_application_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_pinpoint/test_pinpoint_event_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.633231 moto-4.1.9.dev6/tests/test_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_polly/test_polly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_polly/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.637231 moto-4.1.9.dev6/tests/test_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_quicksight/test_quicksight_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_quicksight/test_quicksight_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_quicksight/test_quicksight_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.637231 moto-4.1.9.dev6/tests/test_ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ram/test_ram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.637231 moto-4.1.9.dev6/tests/test_rds/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_db_cluster_param_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_db_cluster_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_global_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91218 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_rds_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_rds_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_rds_clusters_with_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_rds_event_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_rds_export_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rds/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.637231 moto-4.1.9.dev6/tests/test_rdsdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rdsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rdsdata/test_rdsdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.637231 moto-4.1.9.dev6/tests/test_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73309 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_redshift/test_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_redshift/test_redshift_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_redshift/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.637231 moto-4.1.9.dev6/tests/test_redshiftdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_redshiftdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_redshiftdata/test_redshiftdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_redshiftdata/test_redshiftdata_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_redshiftdata/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.637231 moto-4.1.9.dev6/tests/test_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_rekognition/test_rekognition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.637231 moto-4.1.9.dev6/tests/test_resourcegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_resourcegroups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_resourcegroups/test_resourcegroups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.637231 moto-4.1.9.dev6/tests/test_resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_resourcegroupstaggingapi/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.641231 moto-4.1.9.dev6/tests/test_route53/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53/test_change_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52862 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53/test_route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53/test_route53_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53/test_route53_delegationsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53/test_route53_healthchecks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53/test_route53_query_logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53/test_route53_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.641231 moto-4.1.9.dev6/tests/test_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40356 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53resolver/test_route53resolver_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21968 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53resolver/test_route53resolver_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53resolver/test_route53resolver_rule_associations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_route53resolver/test_route53resolver_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.645231 moto-4.1.9.dev6/tests/test_s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_multiple_accounts_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115875 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_bucket_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_classdecorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18825 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_copyobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_custom_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_file_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_lambda_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31026 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_object_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_storageclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_tagging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.645231 moto-4.1.9.dev6/tests/test_s3bucket_path/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3bucket_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3bucket_path/test_s3bucket_path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3bucket_path/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.645231 moto-4.1.9.dev6/tests/test_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3control/test_s3control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3control/test_s3control_access_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3control/test_s3control_accesspoint_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3control/test_s3control_config_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_s3control/test_s3control_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.645231 moto-4.1.9.dev6/tests/test_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9953 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/cloudformation_test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15041 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20469 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24758 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_trial_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.645231 moto-4.1.9.dev6/tests/test_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_scheduler/test_schedule_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_scheduler/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_scheduler/test_scheduler_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_scheduler/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.645231 moto-4.1.9.dev6/tests/test_sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sdb/test_sdb_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sdb/test_sdb_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sdb/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.649231 moto-4.1.9.dev6/tests/test_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_secretsmanager/test_list_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_secretsmanager/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57270 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_secretsmanager/test_secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33302 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_secretsmanager/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.649231 moto-4.1.9.dev6/tests/test_servicediscovery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_servicediscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_servicediscovery/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_servicediscovery/test_servicediscovery_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_servicediscovery/test_servicediscovery_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_servicediscovery/test_servicediscovery_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.649231 moto-4.1.9.dev6/tests/test_servicequotas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_servicequotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_servicequotas/test_servicequotas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.649231 moto-4.1.9.dev6/tests/test_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ses/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52328 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ses/test_ses_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ses/test_ses_sns_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ses/test_ses_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ses/test_templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.649231 moto-4.1.9.dev6/tests/test_signer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_signer/test_signing_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_signer/test_signing_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.649231 moto-4.1.9.dev6/tests/test_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sns/test_application_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sns/test_publish_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42807 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sns/test_publishing_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sns/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sns/test_sns_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sns/test_subscriptions_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21472 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sns/test_topics_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.649231 moto-4.1.9.dev6/tests/test_special_cases/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_special_cases/test_custom_amis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.653231 moto-4.1.9.dev6/tests/test_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sqs/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110801 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sqs/test_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sqs/test_sqs_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sqs/test_sqs_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sqs/test_sqs_multiaccount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.653231 moto-4.1.9.dev6/tests/test_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72442 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_default_amis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_doc_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28425 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_ec2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_ecs_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_maintenance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_parameterstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_ssm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.653231 moto-4.1.9.dev6/tests/test_ssm/test_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssm/test_templates/good.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.653231 moto-4.1.9.dev6/tests/test_ssoadmin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssoadmin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssoadmin/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_ssoadmin/test_ssoadmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.653231 moto-4.1.9.dev6/tests/test_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34241 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_stepfunctions/test_stepfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_stepfunctions/test_stepfunctions_cloudformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.653231 moto-4.1.9.dev6/tests/test_sts/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sts/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sts/test_sts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_sts/test_sts_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.653231 moto-4.1.9.dev6/tests/test_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_support/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24299 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_support/test_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.653231 moto-4.1.9.dev6/tests/test_swf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.657231 moto-4.1.9.dev6/tests/test_swf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/models/test_activity_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/models/test_decision_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/models/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/models/test_generic_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/models/test_history_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/models/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/models/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25245 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/models/test_workflow_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.657231 moto-4.1.9.dev6/tests/test_swf/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/responses/test_activity_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/responses/test_activity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21702 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/responses/test_decision_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/responses/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/responses/test_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/responses/test_workflow_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/responses/test_workflow_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_swf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.657231 moto-4.1.9.dev6/tests/test_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_textract/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_textract/test_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.657231 moto-4.1.9.dev6/tests/test_timestreamwrite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_timestreamwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_timestreamwrite/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_timestreamwrite/test_timestreamwrite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_timestreamwrite/test_timestreamwrite_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_timestreamwrite/test_timestreamwrite_tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.657231 moto-4.1.9.dev6/tests/test_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42714 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_transcribe/test_transcribe_boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.657231 moto-4.1.9.dev6/tests/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_utilities/test_docker_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_utilities/test_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_utilities/test_tagging_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_utilities/test_threaded_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.657231 moto-4.1.9.dev6/tests/test_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_wafv2/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_wafv2/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_wafv2/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_wafv2/test_wafv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_wafv2/test_wafv2_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_wafv2/test_wafv2_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_wafv2/test_wafv2_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:39:58.661232 moto-4.1.9.dev6/tests/test_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_xray/test_xray_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-24 20:39:50.000000 moto-4.1.9.dev6/tests/test_xray/test_xray_client.py
```

### Comparing `moto-4.1.9.dev5/AUTHORS.md` & `moto-4.1.9.dev6/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/LICENSE` & `moto-4.1.9.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/MANIFEST.in` & `moto-4.1.9.dev6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/PKG-INFO` & `moto-4.1.9.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moto
-Version: 4.1.9.dev5
+Version: 4.1.9.dev6
 Home-page: https://github.com/getmoto/moto
 Author: Steve Pulec
 Author-email: "spulec@gmail.com"
 License: Apache License 2.0
 Project-URL: Documentation, http://docs.getmoto.org/en/latest/
 Project-URL: Issue tracker, https://github.com/getmoto/moto/issues
 Project-URL: Changelog, https://github.com/getmoto/moto/blob/master/CHANGELOG.md
```

### Comparing `moto-4.1.9.dev5/README.md` & `moto-4.1.9.dev6/README.md`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/__init__.py` & `moto-4.1.9.dev6/moto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
 mock_all = MockAll
 
 # import logging
 # logging.getLogger('boto').setLevel(logging.CRITICAL)
 
 __title__ = "moto"
-__version__ = "4.1.9.dev5"
+__version__ = "4.1.9.dev6"
 
 
 try:
     # Need to monkey-patch botocore requests back to underlying urllib3 classes
     from botocore.awsrequest import (
         HTTPSConnectionPool,
         HTTPConnectionPool,
```

### Comparing `moto-4.1.9.dev5/moto/acm/models.py` & `moto-4.1.9.dev6/moto/acm/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/acm/responses.py` & `moto-4.1.9.dev6/moto/acm/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/acmpca/models.py` & `moto-4.1.9.dev6/moto/acmpca/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/acmpca/responses.py` & `moto-4.1.9.dev6/moto/acmpca/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/amp/exceptions.py` & `moto-4.1.9.dev6/moto/amp/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/amp/models.py` & `moto-4.1.9.dev6/moto/amp/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/amp/responses.py` & `moto-4.1.9.dev6/moto/amp/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/amp/urls.py` & `moto-4.1.9.dev6/moto/amp/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigateway/exceptions.py` & `moto-4.1.9.dev6/moto/apigateway/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigateway/integration_parsers/aws_parser.py` & `moto-4.1.9.dev6/moto/apigateway/integration_parsers/aws_parser.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigateway/integration_parsers/http_parser.py` & `moto-4.1.9.dev6/moto/apigateway/integration_parsers/http_parser.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigateway/models.py` & `moto-4.1.9.dev6/moto/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigateway/responses.py` & `moto-4.1.9.dev6/moto/apigateway/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigateway/urls.py` & `moto-4.1.9.dev6/moto/apigateway/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigateway/utils.py` & `moto-4.1.9.dev6/moto/apigateway/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigatewayv2/exceptions.py` & `moto-4.1.9.dev6/moto/apigatewayv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigatewayv2/models.py` & `moto-4.1.9.dev6/moto/apigatewayv2/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigatewayv2/responses.py` & `moto-4.1.9.dev6/moto/apigatewayv2/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/apigatewayv2/urls.py` & `moto-4.1.9.dev6/moto/apigatewayv2/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/applicationautoscaling/models.py` & `moto-4.1.9.dev6/moto/applicationautoscaling/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/applicationautoscaling/responses.py` & `moto-4.1.9.dev6/moto/applicationautoscaling/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/appsync/models.py` & `moto-4.1.9.dev6/moto/appsync/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/appsync/responses.py` & `moto-4.1.9.dev6/moto/appsync/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/appsync/urls.py` & `moto-4.1.9.dev6/moto/appsync/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/athena/exceptions.py` & `moto-4.1.9.dev6/moto/athena/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/athena/models.py` & `moto-4.1.9.dev6/moto/athena/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/athena/responses.py` & `moto-4.1.9.dev6/moto/athena/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/autoscaling/exceptions.py` & `moto-4.1.9.dev6/moto/autoscaling/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/autoscaling/models.py` & `moto-4.1.9.dev6/moto/autoscaling/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/autoscaling/responses.py` & `moto-4.1.9.dev6/moto/autoscaling/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/awslambda/exceptions.py` & `moto-4.1.9.dev6/moto/awslambda/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/awslambda/models.py` & `moto-4.1.9.dev6/moto/awslambda/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/awslambda/policy.py` & `moto-4.1.9.dev6/moto/awslambda/policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/awslambda/responses.py` & `moto-4.1.9.dev6/moto/awslambda/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/awslambda/urls.py` & `moto-4.1.9.dev6/moto/awslambda/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/awslambda/utils.py` & `moto-4.1.9.dev6/moto/awslambda/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/backend_index.py` & `moto-4.1.9.dev6/moto/backend_index.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/backends.py` & `moto-4.1.9.dev6/moto/backends.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/batch/models.py` & `moto-4.1.9.dev6/moto/batch/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/batch/responses.py` & `moto-4.1.9.dev6/moto/batch/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/batch/urls.py` & `moto-4.1.9.dev6/moto/batch/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/batch/utils.py` & `moto-4.1.9.dev6/moto/batch/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/batch_simple/models.py` & `moto-4.1.9.dev6/moto/batch_simple/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/budgets/exceptions.py` & `moto-4.1.9.dev6/moto/budgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/budgets/models.py` & `moto-4.1.9.dev6/moto/budgets/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/budgets/responses.py` & `moto-4.1.9.dev6/moto/budgets/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ce/models.py` & `moto-4.1.9.dev6/moto/ce/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ce/responses.py` & `moto-4.1.9.dev6/moto/ce/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudformation/custom_model.py` & `moto-4.1.9.dev6/moto/cloudformation/custom_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudformation/exceptions.py` & `moto-4.1.9.dev6/moto/cloudformation/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudformation/models.py` & `moto-4.1.9.dev6/moto/cloudformation/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudformation/parsing.py` & `moto-4.1.9.dev6/moto/cloudformation/parsing.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudformation/responses.py` & `moto-4.1.9.dev6/moto/cloudformation/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudformation/utils.py` & `moto-4.1.9.dev6/moto/cloudformation/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudfront/exceptions.py` & `moto-4.1.9.dev6/moto/cloudfront/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudfront/models.py` & `moto-4.1.9.dev6/moto/cloudfront/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudfront/responses.py` & `moto-4.1.9.dev6/moto/cloudfront/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudfront/urls.py` & `moto-4.1.9.dev6/moto/cloudfront/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudtrail/exceptions.py` & `moto-4.1.9.dev6/moto/cloudtrail/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudtrail/models.py` & `moto-4.1.9.dev6/moto/cloudtrail/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudtrail/responses.py` & `moto-4.1.9.dev6/moto/cloudtrail/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudwatch/exceptions.py` & `moto-4.1.9.dev6/moto/cloudwatch/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudwatch/models.py` & `moto-4.1.9.dev6/moto/cloudwatch/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cloudwatch/responses.py` & `moto-4.1.9.dev6/moto/cloudwatch/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/codebuild/exceptions.py` & `moto-4.1.9.dev6/moto/codebuild/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/codebuild/models.py` & `moto-4.1.9.dev6/moto/codebuild/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/codebuild/responses.py` & `moto-4.1.9.dev6/moto/codebuild/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/codecommit/exceptions.py` & `moto-4.1.9.dev6/moto/codecommit/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/codecommit/models.py` & `moto-4.1.9.dev6/moto/codecommit/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/codecommit/responses.py` & `moto-4.1.9.dev6/moto/codecommit/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/codepipeline/exceptions.py` & `moto-4.1.9.dev6/moto/codepipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/codepipeline/models.py` & `moto-4.1.9.dev6/moto/codepipeline/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/codepipeline/responses.py` & `moto-4.1.9.dev6/moto/codepipeline/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cognitoidentity/exceptions.py` & `moto-4.1.9.dev6/moto/cognitoidentity/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cognitoidentity/models.py` & `moto-4.1.9.dev6/moto/cognitoidentity/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cognitoidentity/responses.py` & `moto-4.1.9.dev6/moto/cognitoidentity/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cognitoidp/exceptions.py` & `moto-4.1.9.dev6/moto/cognitoidp/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cognitoidp/models.py` & `moto-4.1.9.dev6/moto/cognitoidp/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cognitoidp/resources/jwks-private.json` & `moto-4.1.9.dev6/moto/cognitoidp/resources/jwks-private.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cognitoidp/responses.py` & `moto-4.1.9.dev6/moto/cognitoidp/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/cognitoidp/utils.py` & `moto-4.1.9.dev6/moto/cognitoidp/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/comprehend/models.py` & `moto-4.1.9.dev6/moto/comprehend/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/comprehend/responses.py` & `moto-4.1.9.dev6/moto/comprehend/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/config/exceptions.py` & `moto-4.1.9.dev6/moto/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/config/models.py` & `moto-4.1.9.dev6/moto/config/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/config/resources/aws_managed_rules.json` & `moto-4.1.9.dev6/moto/config/resources/aws_managed_rules.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/config/responses.py` & `moto-4.1.9.dev6/moto/config/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/core/base_backend.py` & `moto-4.1.9.dev6/moto/core/base_backend.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/core/botocore_stubber.py` & `moto-4.1.9.dev6/moto/core/botocore_stubber.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/core/common_models.py` & `moto-4.1.9.dev6/moto/core/common_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/core/custom_responses_mock.py` & `moto-4.1.9.dev6/moto/core/custom_responses_mock.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/core/exceptions.py` & `moto-4.1.9.dev6/moto/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/core/models.py` & `moto-4.1.9.dev6/moto/core/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/core/responses.py` & `moto-4.1.9.dev6/moto/core/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/core/responses_custom_registry.py` & `moto-4.1.9.dev6/moto/core/responses_custom_registry.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/core/utils.py` & `moto-4.1.9.dev6/moto/core/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/databrew/exceptions.py` & `moto-4.1.9.dev6/moto/databrew/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/databrew/models.py` & `moto-4.1.9.dev6/moto/databrew/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/databrew/responses.py` & `moto-4.1.9.dev6/moto/databrew/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/databrew/urls.py` & `moto-4.1.9.dev6/moto/databrew/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/datapipeline/models.py` & `moto-4.1.9.dev6/moto/datapipeline/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/datapipeline/responses.py` & `moto-4.1.9.dev6/moto/datapipeline/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/datapipeline/utils.py` & `moto-4.1.9.dev6/moto/datapipeline/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/datasync/models.py` & `moto-4.1.9.dev6/moto/datasync/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/datasync/responses.py` & `moto-4.1.9.dev6/moto/datasync/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dax/exceptions.py` & `moto-4.1.9.dev6/moto/dax/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dax/models.py` & `moto-4.1.9.dev6/moto/dax/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dax/responses.py` & `moto-4.1.9.dev6/moto/dax/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dms/exceptions.py` & `moto-4.1.9.dev6/moto/dms/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dms/models.py` & `moto-4.1.9.dev6/moto/dms/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dms/responses.py` & `moto-4.1.9.dev6/moto/dms/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dms/utils.py` & `moto-4.1.9.dev6/moto/dms/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ds/exceptions.py` & `moto-4.1.9.dev6/moto/ds/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ds/models.py` & `moto-4.1.9.dev6/moto/ds/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ds/responses.py` & `moto-4.1.9.dev6/moto/ds/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ds/validations.py` & `moto-4.1.9.dev6/moto/ds/validations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/comparisons.py` & `moto-4.1.9.dev6/moto/dynamodb/comparisons.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/exceptions.py` & `moto-4.1.9.dev6/moto/dynamodb/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/models/__init__.py` & `moto-4.1.9.dev6/moto/dynamodb/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/models/dynamo_type.py` & `moto-4.1.9.dev6/moto/dynamodb/models/dynamo_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/models/table.py` & `moto-4.1.9.dev6/moto/dynamodb/models/table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/parsing/ast_nodes.py` & `moto-4.1.9.dev6/moto/dynamodb/parsing/ast_nodes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/parsing/executors.py` & `moto-4.1.9.dev6/moto/dynamodb/parsing/executors.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/parsing/expressions.py` & `moto-4.1.9.dev6/moto/dynamodb/parsing/expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/parsing/key_condition_expression.py` & `moto-4.1.9.dev6/moto/dynamodb/parsing/key_condition_expression.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/parsing/reserved_keywords.py` & `moto-4.1.9.dev6/moto/dynamodb/parsing/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/parsing/reserved_keywords.txt` & `moto-4.1.9.dev6/moto/dynamodb/parsing/reserved_keywords.txt`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/parsing/tokens.py` & `moto-4.1.9.dev6/moto/dynamodb/parsing/tokens.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/parsing/validators.py` & `moto-4.1.9.dev6/moto/dynamodb/parsing/validators.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb/responses.py` & `moto-4.1.9.dev6/moto/dynamodb/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb_v20111205/comparisons.py` & `moto-4.1.9.dev6/moto/dynamodb_v20111205/comparisons.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb_v20111205/models.py` & `moto-4.1.9.dev6/moto/dynamodb_v20111205/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodb_v20111205/responses.py` & `moto-4.1.9.dev6/moto/dynamodb_v20111205/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodbstreams/models.py` & `moto-4.1.9.dev6/moto/dynamodbstreams/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/dynamodbstreams/responses.py` & `moto-4.1.9.dev6/moto/dynamodbstreams/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ebs/models.py` & `moto-4.1.9.dev6/moto/ebs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ebs/responses.py` & `moto-4.1.9.dev6/moto/ebs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ebs/urls.py` & `moto-4.1.9.dev6/moto/ebs/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/exceptions.py` & `moto-4.1.9.dev6/moto/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/__init__.py` & `moto-4.1.9.dev6/moto/ec2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/amis.py` & `moto-4.1.9.dev6/moto/ec2/models/amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/availability_zones_and_regions.py` & `moto-4.1.9.dev6/moto/ec2/models/availability_zones_and_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/carrier_gateways.py` & `moto-4.1.9.dev6/moto/ec2/models/carrier_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/core.py` & `moto-4.1.9.dev6/moto/ec2/models/core.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/customer_gateways.py` & `moto-4.1.9.dev6/moto/ec2/models/customer_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/dhcp_options.py` & `moto-4.1.9.dev6/moto/ec2/models/dhcp_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/elastic_block_store.py` & `moto-4.1.9.dev6/moto/ec2/models/elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/elastic_ip_addresses.py` & `moto-4.1.9.dev6/moto/ec2/models/elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/elastic_network_interfaces.py` & `moto-4.1.9.dev6/moto/ec2/models/elastic_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/fleets.py` & `moto-4.1.9.dev6/moto/ec2/models/fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/flow_logs.py` & `moto-4.1.9.dev6/moto/ec2/models/flow_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/hosts.py` & `moto-4.1.9.dev6/moto/ec2/models/hosts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/iam_instance_profile.py` & `moto-4.1.9.dev6/moto/ec2/models/iam_instance_profile.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/instance_types.py` & `moto-4.1.9.dev6/moto/ec2/models/instance_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/instances.py` & `moto-4.1.9.dev6/moto/ec2/models/instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/internet_gateways.py` & `moto-4.1.9.dev6/moto/ec2/models/internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/key_pairs.py` & `moto-4.1.9.dev6/moto/ec2/models/key_pairs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/launch_templates.py` & `moto-4.1.9.dev6/moto/ec2/models/launch_templates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/managed_prefixes.py` & `moto-4.1.9.dev6/moto/ec2/models/managed_prefixes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/nat_gateways.py` & `moto-4.1.9.dev6/moto/ec2/models/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/network_acls.py` & `moto-4.1.9.dev6/moto/ec2/models/network_acls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/route_tables.py` & `moto-4.1.9.dev6/moto/ec2/models/route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/security_groups.py` & `moto-4.1.9.dev6/moto/ec2/models/security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/spot_requests.py` & `moto-4.1.9.dev6/moto/ec2/models/spot_requests.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/subnets.py` & `moto-4.1.9.dev6/moto/ec2/models/subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/tags.py` & `moto-4.1.9.dev6/moto/ec2/models/tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/transit_gateway.py` & `moto-4.1.9.dev6/moto/ec2/models/transit_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/transit_gateway_attachments.py` & `moto-4.1.9.dev6/moto/ec2/models/transit_gateway_attachments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/transit_gateway_route_tables.py` & `moto-4.1.9.dev6/moto/ec2/models/transit_gateway_route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/vpc_peering_connections.py` & `moto-4.1.9.dev6/moto/ec2/models/vpc_peering_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/vpc_service_configuration.py` & `moto-4.1.9.dev6/moto/ec2/models/vpc_service_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/vpcs.py` & `moto-4.1.9.dev6/moto/ec2/models/vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/vpn_connections.py` & `moto-4.1.9.dev6/moto/ec2/models/vpn_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/models/vpn_gateway.py` & `moto-4.1.9.dev6/moto/ec2/models/vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/amis.json` & `moto-4.1.9.dev6/moto/ec2/resources/amis.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/af-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/me-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/me-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-east-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/ecs/optimized_amis/us-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/ecs/optimized_amis/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/availability-zone-id/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/af-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/me-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/me-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-east-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_type_offerings/region/us-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_type_offerings/region/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/instance_types.json` & `moto-4.1.9.dev6/moto/ec2/resources/instance_types.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/af-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-northeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ap-southeast-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/ca-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-central-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-north-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-south-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/eu-west-3.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/me-central-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/me-south-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/sa-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-east-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-east-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-west-1.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/resources/latest_amis/us-west-2.json` & `moto-4.1.9.dev6/moto/ec2/resources/latest_amis/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/__init__.py` & `moto-4.1.9.dev6/moto/ec2/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/_base_response.py` & `moto-4.1.9.dev6/moto/ec2/responses/_base_response.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/account_attributes.py` & `moto-4.1.9.dev6/moto/ec2/responses/account_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/amis.py` & `moto-4.1.9.dev6/moto/ec2/responses/amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/availability_zones_and_regions.py` & `moto-4.1.9.dev6/moto/ec2/responses/availability_zones_and_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/carrier_gateways.py` & `moto-4.1.9.dev6/moto/ec2/responses/carrier_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/customer_gateways.py` & `moto-4.1.9.dev6/moto/ec2/responses/customer_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/dhcp_options.py` & `moto-4.1.9.dev6/moto/ec2/responses/dhcp_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/egress_only_internet_gateways.py` & `moto-4.1.9.dev6/moto/ec2/responses/egress_only_internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/elastic_block_store.py` & `moto-4.1.9.dev6/moto/ec2/responses/elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/elastic_ip_addresses.py` & `moto-4.1.9.dev6/moto/ec2/responses/elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/elastic_network_interfaces.py` & `moto-4.1.9.dev6/moto/ec2/responses/elastic_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/fleets.py` & `moto-4.1.9.dev6/moto/ec2/responses/fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/flow_logs.py` & `moto-4.1.9.dev6/moto/ec2/responses/flow_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/general.py` & `moto-4.1.9.dev6/moto/ec2/responses/general.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/hosts.py` & `moto-4.1.9.dev6/moto/ec2/responses/hosts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/iam_instance_profiles.py` & `moto-4.1.9.dev6/moto/ec2/responses/iam_instance_profiles.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/instances.py` & `moto-4.1.9.dev6/moto/ec2/responses/instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/internet_gateways.py` & `moto-4.1.9.dev6/moto/ec2/responses/internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/key_pairs.py` & `moto-4.1.9.dev6/moto/ec2/responses/key_pairs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/launch_templates.py` & `moto-4.1.9.dev6/moto/ec2/responses/launch_templates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/nat_gateways.py` & `moto-4.1.9.dev6/moto/ec2/responses/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/network_acls.py` & `moto-4.1.9.dev6/moto/ec2/responses/network_acls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/reserved_instances.py` & `moto-4.1.9.dev6/moto/ec2/responses/reserved_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/route_tables.py` & `moto-4.1.9.dev6/moto/ec2/responses/route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/security_groups.py` & `moto-4.1.9.dev6/moto/ec2/responses/security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/settings.py` & `moto-4.1.9.dev6/moto/ec2/responses/settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/spot_fleets.py` & `moto-4.1.9.dev6/moto/ec2/responses/spot_fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/spot_instances.py` & `moto-4.1.9.dev6/moto/ec2/responses/spot_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/subnets.py` & `moto-4.1.9.dev6/moto/ec2/responses/subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/tags.py` & `moto-4.1.9.dev6/moto/ec2/responses/tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/transit_gateway_attachments.py` & `moto-4.1.9.dev6/moto/ec2/responses/transit_gateway_attachments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/transit_gateway_route_tables.py` & `moto-4.1.9.dev6/moto/ec2/responses/transit_gateway_route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/transit_gateways.py` & `moto-4.1.9.dev6/moto/ec2/responses/transit_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/virtual_private_gateways.py` & `moto-4.1.9.dev6/moto/ec2/responses/virtual_private_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/vpc_peering_connections.py` & `moto-4.1.9.dev6/moto/ec2/responses/vpc_peering_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/vpc_service_configuration.py` & `moto-4.1.9.dev6/moto/ec2/responses/vpc_service_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/vpcs.py` & `moto-4.1.9.dev6/moto/ec2/responses/vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/vpn_connections.py` & `moto-4.1.9.dev6/moto/ec2/responses/vpn_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/responses/windows.py` & `moto-4.1.9.dev6/moto/ec2/responses/windows.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2/utils.py` & `moto-4.1.9.dev6/moto/ec2/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ec2instanceconnect/responses.py` & `moto-4.1.9.dev6/moto/ec2instanceconnect/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ecr/exceptions.py` & `moto-4.1.9.dev6/moto/ecr/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ecr/models.py` & `moto-4.1.9.dev6/moto/ecr/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ecr/policy_validation.py` & `moto-4.1.9.dev6/moto/ecr/policy_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ecr/responses.py` & `moto-4.1.9.dev6/moto/ecr/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ecs/exceptions.py` & `moto-4.1.9.dev6/moto/ecs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ecs/models.py` & `moto-4.1.9.dev6/moto/ecs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ecs/responses.py` & `moto-4.1.9.dev6/moto/ecs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/efs/exceptions.py` & `moto-4.1.9.dev6/moto/efs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/efs/models.py` & `moto-4.1.9.dev6/moto/efs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/efs/responses.py` & `moto-4.1.9.dev6/moto/efs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/efs/urls.py` & `moto-4.1.9.dev6/moto/efs/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/eks/exceptions.py` & `moto-4.1.9.dev6/moto/eks/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/eks/models.py` & `moto-4.1.9.dev6/moto/eks/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/eks/responses.py` & `moto-4.1.9.dev6/moto/eks/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/eks/urls.py` & `moto-4.1.9.dev6/moto/eks/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/eks/utils.py` & `moto-4.1.9.dev6/moto/eks/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elasticache/exceptions.py` & `moto-4.1.9.dev6/moto/elasticache/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elasticache/models.py` & `moto-4.1.9.dev6/moto/elasticache/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elasticache/responses.py` & `moto-4.1.9.dev6/moto/elasticache/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elasticbeanstalk/models.py` & `moto-4.1.9.dev6/moto/elasticbeanstalk/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elasticbeanstalk/responses.py` & `moto-4.1.9.dev6/moto/elasticbeanstalk/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elastictranscoder/models.py` & `moto-4.1.9.dev6/moto/elastictranscoder/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elastictranscoder/responses.py` & `moto-4.1.9.dev6/moto/elastictranscoder/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elb/exceptions.py` & `moto-4.1.9.dev6/moto/elb/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elb/models.py` & `moto-4.1.9.dev6/moto/elb/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elb/policies.py` & `moto-4.1.9.dev6/moto/elb/policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elb/responses.py` & `moto-4.1.9.dev6/moto/elb/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elb/urls.py` & `moto-4.1.9.dev6/moto/elb/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elbv2/exceptions.py` & `moto-4.1.9.dev6/moto/elbv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elbv2/models.py` & `moto-4.1.9.dev6/moto/elbv2/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/elbv2/responses.py` & `moto-4.1.9.dev6/moto/elbv2/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emr/models.py` & `moto-4.1.9.dev6/moto/emr/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emr/responses.py` & `moto-4.1.9.dev6/moto/emr/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emr/utils.py` & `moto-4.1.9.dev6/moto/emr/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emrcontainers/models.py` & `moto-4.1.9.dev6/moto/emrcontainers/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emrcontainers/responses.py` & `moto-4.1.9.dev6/moto/emrcontainers/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emrcontainers/urls.py` & `moto-4.1.9.dev6/moto/emrcontainers/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emrcontainers/utils.py` & `moto-4.1.9.dev6/moto/emrcontainers/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emrserverless/models.py` & `moto-4.1.9.dev6/moto/emrserverless/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emrserverless/responses.py` & `moto-4.1.9.dev6/moto/emrserverless/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emrserverless/urls.py` & `moto-4.1.9.dev6/moto/emrserverless/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/emrserverless/utils.py` & `moto-4.1.9.dev6/moto/emrserverless/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/es/exceptions.py` & `moto-4.1.9.dev6/moto/es/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/es/models.py` & `moto-4.1.9.dev6/moto/es/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/es/responses.py` & `moto-4.1.9.dev6/moto/es/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/es/urls.py` & `moto-4.1.9.dev6/moto/es/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/events/exceptions.py` & `moto-4.1.9.dev6/moto/events/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/events/models.py` & `moto-4.1.9.dev6/moto/events/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/events/notifications.py` & `moto-4.1.9.dev6/moto/events/notifications.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/events/responses.py` & `moto-4.1.9.dev6/moto/events/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/firehose/exceptions.py` & `moto-4.1.9.dev6/moto/firehose/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/firehose/models.py` & `moto-4.1.9.dev6/moto/firehose/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/firehose/responses.py` & `moto-4.1.9.dev6/moto/firehose/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/forecast/exceptions.py` & `moto-4.1.9.dev6/moto/forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/forecast/models.py` & `moto-4.1.9.dev6/moto/forecast/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/forecast/responses.py` & `moto-4.1.9.dev6/moto/forecast/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/glacier/models.py` & `moto-4.1.9.dev6/moto/glacier/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/glacier/responses.py` & `moto-4.1.9.dev6/moto/glacier/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/glacier/urls.py` & `moto-4.1.9.dev6/moto/glacier/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/glue/exceptions.py` & `moto-4.1.9.dev6/moto/glue/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/glue/glue_schema_registry_constants.py` & `moto-4.1.9.dev6/moto/glue/glue_schema_registry_constants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/glue/glue_schema_registry_utils.py` & `moto-4.1.9.dev6/moto/glue/glue_schema_registry_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/glue/models.py` & `moto-4.1.9.dev6/moto/glue/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/glue/responses.py` & `moto-4.1.9.dev6/moto/glue/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/glue/utils.py` & `moto-4.1.9.dev6/moto/glue/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/greengrass/exceptions.py` & `moto-4.1.9.dev6/moto/greengrass/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/greengrass/models.py` & `moto-4.1.9.dev6/moto/greengrass/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/greengrass/responses.py` & `moto-4.1.9.dev6/moto/greengrass/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/greengrass/urls.py` & `moto-4.1.9.dev6/moto/greengrass/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/guardduty/exceptions.py` & `moto-4.1.9.dev6/moto/guardduty/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/guardduty/models.py` & `moto-4.1.9.dev6/moto/guardduty/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/guardduty/responses.py` & `moto-4.1.9.dev6/moto/guardduty/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/guardduty/urls.py` & `moto-4.1.9.dev6/moto/guardduty/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iam/access_control.py` & `moto-4.1.9.dev6/moto/iam/access_control.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iam/aws_managed_policies.py` & `moto-4.1.9.dev6/moto/iam/aws_managed_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iam/config.py` & `moto-4.1.9.dev6/moto/iam/config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iam/exceptions.py` & `moto-4.1.9.dev6/moto/iam/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iam/models.py` & `moto-4.1.9.dev6/moto/iam/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iam/policy_validation.py` & `moto-4.1.9.dev6/moto/iam/policy_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iam/responses.py` & `moto-4.1.9.dev6/moto/iam/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iam/utils.py` & `moto-4.1.9.dev6/moto/iam/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/identitystore/models.py` & `moto-4.1.9.dev6/moto/identitystore/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/identitystore/responses.py` & `moto-4.1.9.dev6/moto/identitystore/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/instance_metadata/responses.py` & `moto-4.1.9.dev6/moto/instance_metadata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iot/exceptions.py` & `moto-4.1.9.dev6/moto/iot/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iot/models.py` & `moto-4.1.9.dev6/moto/iot/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iot/responses.py` & `moto-4.1.9.dev6/moto/iot/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iot/urls.py` & `moto-4.1.9.dev6/moto/iot/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iotdata/exceptions.py` & `moto-4.1.9.dev6/moto/iotdata/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iotdata/models.py` & `moto-4.1.9.dev6/moto/iotdata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/iotdata/responses.py` & `moto-4.1.9.dev6/moto/iotdata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesis/exceptions.py` & `moto-4.1.9.dev6/moto/kinesis/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesis/models.py` & `moto-4.1.9.dev6/moto/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesis/responses.py` & `moto-4.1.9.dev6/moto/kinesis/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesis/urls.py` & `moto-4.1.9.dev6/moto/kinesis/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesis/utils.py` & `moto-4.1.9.dev6/moto/kinesis/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesisvideo/exceptions.py` & `moto-4.1.9.dev6/moto/kinesisvideo/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesisvideo/models.py` & `moto-4.1.9.dev6/moto/kinesisvideo/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesisvideo/responses.py` & `moto-4.1.9.dev6/moto/kinesisvideo/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/models.py` & `moto-4.1.9.dev6/moto/kinesisvideoarchivedmedia/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kinesisvideoarchivedmedia/responses.py` & `moto-4.1.9.dev6/moto/kinesisvideoarchivedmedia/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kms/exceptions.py` & `moto-4.1.9.dev6/moto/kms/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kms/models.py` & `moto-4.1.9.dev6/moto/kms/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kms/policy_validator.py` & `moto-4.1.9.dev6/moto/kms/policy_validator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kms/responses.py` & `moto-4.1.9.dev6/moto/kms/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/kms/utils.py` & `moto-4.1.9.dev6/moto/kms/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/lakeformation/models.py` & `moto-4.1.9.dev6/moto/lakeformation/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/lakeformation/responses.py` & `moto-4.1.9.dev6/moto/lakeformation/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/lakeformation/urls.py` & `moto-4.1.9.dev6/moto/lakeformation/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/logs/exceptions.py` & `moto-4.1.9.dev6/moto/logs/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/logs/metric_filters.py` & `moto-4.1.9.dev6/moto/logs/metric_filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/logs/models.py` & `moto-4.1.9.dev6/moto/logs/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/logs/responses.py` & `moto-4.1.9.dev6/moto/logs/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/logs/utils.py` & `moto-4.1.9.dev6/moto/logs/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/managedblockchain/exceptions.py` & `moto-4.1.9.dev6/moto/managedblockchain/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/managedblockchain/models.py` & `moto-4.1.9.dev6/moto/managedblockchain/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/managedblockchain/responses.py` & `moto-4.1.9.dev6/moto/managedblockchain/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/managedblockchain/urls.py` & `moto-4.1.9.dev6/moto/managedblockchain/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/managedblockchain/utils.py` & `moto-4.1.9.dev6/moto/managedblockchain/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediaconnect/models.py` & `moto-4.1.9.dev6/moto/mediaconnect/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediaconnect/responses.py` & `moto-4.1.9.dev6/moto/mediaconnect/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediaconnect/urls.py` & `moto-4.1.9.dev6/moto/mediaconnect/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/medialive/models.py` & `moto-4.1.9.dev6/moto/medialive/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/medialive/responses.py` & `moto-4.1.9.dev6/moto/medialive/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/medialive/urls.py` & `moto-4.1.9.dev6/moto/medialive/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediapackage/models.py` & `moto-4.1.9.dev6/moto/mediapackage/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediapackage/responses.py` & `moto-4.1.9.dev6/moto/mediapackage/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediastore/exceptions.py` & `moto-4.1.9.dev6/moto/mediastore/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediastore/models.py` & `moto-4.1.9.dev6/moto/mediastore/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediastore/responses.py` & `moto-4.1.9.dev6/moto/mediastore/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediastoredata/models.py` & `moto-4.1.9.dev6/moto/mediastoredata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mediastoredata/responses.py` & `moto-4.1.9.dev6/moto/mediastoredata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/meteringmarketplace/models.py` & `moto-4.1.9.dev6/moto/meteringmarketplace/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/meteringmarketplace/responses.py` & `moto-4.1.9.dev6/moto/meteringmarketplace/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_api/_internal/managed_state_model.py` & `moto-4.1.9.dev6/moto/moto_api/_internal/managed_state_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_api/_internal/models.py` & `moto-4.1.9.dev6/moto/moto_api/_internal/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_api/_internal/moto_random.py` & `moto-4.1.9.dev6/moto/moto_api/_internal/moto_random.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_api/_internal/recorder/models.py` & `moto-4.1.9.dev6/moto/moto_api/_internal/recorder/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_api/_internal/recorder/responses.py` & `moto-4.1.9.dev6/moto/moto_api/_internal/recorder/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_api/_internal/responses.py` & `moto-4.1.9.dev6/moto/moto_api/_internal/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_api/_internal/state_manager.py` & `moto-4.1.9.dev6/moto/moto_api/_internal/state_manager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_api/_internal/urls.py` & `moto-4.1.9.dev6/moto/moto_api/_internal/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_server/templates/dashboard.html` & `moto-4.1.9.dev6/moto/moto_server/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_server/threaded_moto_server.py` & `moto-4.1.9.dev6/moto/moto_server/threaded_moto_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_server/utilities.py` & `moto-4.1.9.dev6/moto/moto_server/utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/moto_server/werkzeug_app.py` & `moto-4.1.9.dev6/moto/moto_server/werkzeug_app.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mq/configuration.py` & `moto-4.1.9.dev6/moto/mq/configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mq/exceptions.py` & `moto-4.1.9.dev6/moto/mq/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mq/models.py` & `moto-4.1.9.dev6/moto/mq/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mq/responses.py` & `moto-4.1.9.dev6/moto/mq/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/mq/urls.py` & `moto-4.1.9.dev6/moto/mq/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/neptune/exceptions.py` & `moto-4.1.9.dev6/moto/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/neptune/models.py` & `moto-4.1.9.dev6/moto/neptune/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/neptune/responses.py` & `moto-4.1.9.dev6/moto/neptune/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/opensearch/data.py` & `moto-4.1.9.dev6/moto/opensearch/data.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/opensearch/models.py` & `moto-4.1.9.dev6/moto/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/opensearch/responses.py` & `moto-4.1.9.dev6/moto/opensearch/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/opsworks/models.py` & `moto-4.1.9.dev6/moto/opsworks/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/opsworks/responses.py` & `moto-4.1.9.dev6/moto/opsworks/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/organizations/exceptions.py` & `moto-4.1.9.dev6/moto/organizations/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/organizations/models.py` & `moto-4.1.9.dev6/moto/organizations/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/organizations/responses.py` & `moto-4.1.9.dev6/moto/organizations/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/organizations/utils.py` & `moto-4.1.9.dev6/moto/organizations/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/packages/boto/ec2/blockdevicemapping.py` & `moto-4.1.9.dev6/moto/packages/boto/ec2/blockdevicemapping.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/packages/boto/ec2/ec2object.py` & `moto-4.1.9.dev6/moto/packages/boto/ec2/ec2object.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/packages/boto/ec2/image.py` & `moto-4.1.9.dev6/moto/packages/boto/ec2/image.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/packages/boto/ec2/instance.py` & `moto-4.1.9.dev6/moto/packages/boto/ec2/instance.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/packages/boto/ec2/instancetype.py` & `moto-4.1.9.dev6/moto/packages/boto/ec2/instancetype.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/packages/boto/ec2/tag.py` & `moto-4.1.9.dev6/moto/packages/boto/ec2/tag.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/packages/cfnresponse/cfnresponse.py` & `moto-4.1.9.dev6/moto/packages/cfnresponse/cfnresponse.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/personalize/models.py` & `moto-4.1.9.dev6/moto/personalize/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/personalize/responses.py` & `moto-4.1.9.dev6/moto/personalize/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/pinpoint/models.py` & `moto-4.1.9.dev6/moto/pinpoint/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/pinpoint/responses.py` & `moto-4.1.9.dev6/moto/pinpoint/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/pinpoint/urls.py` & `moto-4.1.9.dev6/moto/pinpoint/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/polly/models.py` & `moto-4.1.9.dev6/moto/polly/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/polly/resources.py` & `moto-4.1.9.dev6/moto/polly/resources.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/polly/responses.py` & `moto-4.1.9.dev6/moto/polly/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/quicksight/models.py` & `moto-4.1.9.dev6/moto/quicksight/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/quicksight/responses.py` & `moto-4.1.9.dev6/moto/quicksight/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/quicksight/urls.py` & `moto-4.1.9.dev6/moto/quicksight/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ram/exceptions.py` & `moto-4.1.9.dev6/moto/ram/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ram/models.py` & `moto-4.1.9.dev6/moto/ram/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ram/responses.py` & `moto-4.1.9.dev6/moto/ram/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rds/exceptions.py` & `moto-4.1.9.dev6/moto/rds/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rds/models.py` & `moto-4.1.9.dev6/moto/rds/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rds/resources/cluster_options/aurora-postgresql.json` & `moto-4.1.9.dev6/moto/rds/resources/cluster_options/aurora-postgresql.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rds/resources/cluster_options/neptune.json` & `moto-4.1.9.dev6/moto/rds/resources/cluster_options/neptune.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rds/responses.py` & `moto-4.1.9.dev6/moto/rds/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rds/utils.py` & `moto-4.1.9.dev6/moto/rds/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rdsdata/models.py` & `moto-4.1.9.dev6/moto/rdsdata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rdsdata/responses.py` & `moto-4.1.9.dev6/moto/rdsdata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/redshift/exceptions.py` & `moto-4.1.9.dev6/moto/redshift/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/redshift/models.py` & `moto-4.1.9.dev6/moto/redshift/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/redshift/responses.py` & `moto-4.1.9.dev6/moto/redshift/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/redshiftdata/models.py` & `moto-4.1.9.dev6/moto/redshiftdata/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/redshiftdata/responses.py` & `moto-4.1.9.dev6/moto/redshiftdata/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rekognition/models.py` & `moto-4.1.9.dev6/moto/rekognition/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/rekognition/responses.py` & `moto-4.1.9.dev6/moto/rekognition/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/resourcegroups/models.py` & `moto-4.1.9.dev6/moto/resourcegroups/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/resourcegroups/responses.py` & `moto-4.1.9.dev6/moto/resourcegroups/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/resourcegroups/urls.py` & `moto-4.1.9.dev6/moto/resourcegroups/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/resourcegroupstaggingapi/models.py` & `moto-4.1.9.dev6/moto/resourcegroupstaggingapi/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/resourcegroupstaggingapi/responses.py` & `moto-4.1.9.dev6/moto/resourcegroupstaggingapi/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/route53/exceptions.py` & `moto-4.1.9.dev6/moto/route53/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/route53/models.py` & `moto-4.1.9.dev6/moto/route53/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/route53/responses.py` & `moto-4.1.9.dev6/moto/route53/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/route53/urls.py` & `moto-4.1.9.dev6/moto/route53/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/route53resolver/exceptions.py` & `moto-4.1.9.dev6/moto/route53resolver/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/route53resolver/models.py` & `moto-4.1.9.dev6/moto/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/route53resolver/responses.py` & `moto-4.1.9.dev6/moto/route53resolver/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/route53resolver/utils.py` & `moto-4.1.9.dev6/moto/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/route53resolver/validations.py` & `moto-4.1.9.dev6/moto/route53resolver/validations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3/cloud_formation.py` & `moto-4.1.9.dev6/moto/s3/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3/config.py` & `moto-4.1.9.dev6/moto/s3/config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3/exceptions.py` & `moto-4.1.9.dev6/moto/s3/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3/models.py` & `moto-4.1.9.dev6/moto/s3/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3/notifications.py` & `moto-4.1.9.dev6/moto/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3/responses.py` & `moto-4.1.9.dev6/moto/s3/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3/select_object_content.py` & `moto-4.1.9.dev6/moto/s3/select_object_content.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3/urls.py` & `moto-4.1.9.dev6/moto/s3/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3/utils.py` & `moto-4.1.9.dev6/moto/s3/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3control/config.py` & `moto-4.1.9.dev6/moto/s3control/config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3control/exceptions.py` & `moto-4.1.9.dev6/moto/s3control/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3control/models.py` & `moto-4.1.9.dev6/moto/s3control/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3control/responses.py` & `moto-4.1.9.dev6/moto/s3control/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/s3control/urls.py` & `moto-4.1.9.dev6/moto/s3control/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sagemaker/exceptions.py` & `moto-4.1.9.dev6/moto/sagemaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sagemaker/models.py` & `moto-4.1.9.dev6/moto/sagemaker/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sagemaker/responses.py` & `moto-4.1.9.dev6/moto/sagemaker/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sagemaker/utils.py` & `moto-4.1.9.dev6/moto/sagemaker/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sagemaker/validators.py` & `moto-4.1.9.dev6/moto/sagemaker/validators.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/scheduler/models.py` & `moto-4.1.9.dev6/moto/scheduler/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/scheduler/responses.py` & `moto-4.1.9.dev6/moto/scheduler/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/scheduler/urls.py` & `moto-4.1.9.dev6/moto/scheduler/urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sdb/exceptions.py` & `moto-4.1.9.dev6/moto/sdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sdb/models.py` & `moto-4.1.9.dev6/moto/sdb/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sdb/responses.py` & `moto-4.1.9.dev6/moto/sdb/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/secretsmanager/exceptions.py` & `moto-4.1.9.dev6/moto/secretsmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/secretsmanager/list_secrets/filters.py` & `moto-4.1.9.dev6/moto/secretsmanager/list_secrets/filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/secretsmanager/models.py` & `moto-4.1.9.dev6/moto/secretsmanager/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/secretsmanager/responses.py` & `moto-4.1.9.dev6/moto/secretsmanager/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/secretsmanager/utils.py` & `moto-4.1.9.dev6/moto/secretsmanager/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/server.py` & `moto-4.1.9.dev6/moto/server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/servicediscovery/exceptions.py` & `moto-4.1.9.dev6/moto/servicediscovery/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/servicediscovery/models.py` & `moto-4.1.9.dev6/moto/servicediscovery/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/servicediscovery/responses.py` & `moto-4.1.9.dev6/moto/servicediscovery/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/servicequotas/models.py` & `moto-4.1.9.dev6/moto/servicequotas/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/servicequotas/resources/default_quotas/vpc.py` & `moto-4.1.9.dev6/moto/servicequotas/resources/default_quotas/vpc.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/servicequotas/responses.py` & `moto-4.1.9.dev6/moto/servicequotas/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ses/exceptions.py` & `moto-4.1.9.dev6/moto/ses/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ses/feedback.py` & `moto-4.1.9.dev6/moto/ses/feedback.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ses/models.py` & `moto-4.1.9.dev6/moto/ses/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ses/responses.py` & `moto-4.1.9.dev6/moto/ses/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ses/template.py` & `moto-4.1.9.dev6/moto/ses/template.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ses/utils.py` & `moto-4.1.9.dev6/moto/ses/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/settings.py` & `moto-4.1.9.dev6/moto/settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/signer/models.py` & `moto-4.1.9.dev6/moto/signer/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/signer/responses.py` & `moto-4.1.9.dev6/moto/signer/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sns/exceptions.py` & `moto-4.1.9.dev6/moto/sns/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sns/models.py` & `moto-4.1.9.dev6/moto/sns/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sns/responses.py` & `moto-4.1.9.dev6/moto/sns/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sqs/exceptions.py` & `moto-4.1.9.dev6/moto/sqs/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 from moto.core.exceptions import RESTError
 
 
 class ReceiptHandleIsInvalid(RESTError):
     code = 400
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(
             "ReceiptHandleIsInvalid", "The input receipt handle is invalid."
         )
 
 
 class MessageAttributesInvalid(RESTError):
     code = 400
 
-    def __init__(self, description):
+    def __init__(self, description: str):
         super().__init__("MessageAttributesInvalid", description)
 
 
 class QueueDoesNotExist(RESTError):
     code = 400
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(
             "AWS.SimpleQueueService.NonExistentQueue",
             "The specified queue does not exist for this wsdl version.",
             template="wrapped_single_error",
         )
 
 
 class QueueAlreadyExists(RESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("QueueAlreadyExists", message)
 
 
 class EmptyBatchRequest(RESTError):
     code = 400
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(
             "EmptyBatchRequest",
             "There should be at least one SendMessageBatchRequestEntry in the request.",
         )
 
 
 class InvalidBatchEntryId(RESTError):
     code = 400
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(
             "InvalidBatchEntryId",
             "A batch entry id can only contain alphanumeric characters, "
             "hyphens and underscores. It can be at most 80 letters long.",
         )
 
 
 class BatchRequestTooLong(RESTError):
     code = 400
 
-    def __init__(self, length):
+    def __init__(self, length: int):
         super().__init__(
             "BatchRequestTooLong",
             "Batch requests cannot be longer than 262144 bytes. "
             f"You have sent {length} bytes.",
         )
 
 
 class BatchEntryIdsNotDistinct(RESTError):
     code = 400
 
-    def __init__(self, entry_id):
+    def __init__(self, entry_id: str):
         super().__init__("BatchEntryIdsNotDistinct", f"Id {entry_id} repeated.")
 
 
 class TooManyEntriesInBatchRequest(RESTError):
     code = 400
 
-    def __init__(self, number):
+    def __init__(self, number: int):
         super().__init__(
             "TooManyEntriesInBatchRequest",
             "Maximum number of entries per request are 10. " f"You have sent {number}.",
         )
 
 
 class InvalidAttributeName(RESTError):
     code = 400
 
-    def __init__(self, attribute_name):
+    def __init__(self, attribute_name: str):
         super().__init__("InvalidAttributeName", f"Unknown Attribute {attribute_name}.")
 
 
 class InvalidAttributeValue(RESTError):
     code = 400
 
-    def __init__(self, attribute_name):
+    def __init__(self, attribute_name: str):
         super().__init__(
             "InvalidAttributeValue",
             f"Invalid value for the parameter {attribute_name}.",
         )
 
 
 class InvalidParameterValue(RESTError):
     code = 400
 
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__("InvalidParameterValue", message)
 
 
 class MissingParameter(RESTError):
     code = 400
 
-    def __init__(self, parameter):
+    def __init__(self, parameter: str):
         super().__init__(
             "MissingParameter", f"The request must contain the parameter {parameter}."
         )
 
 
 class OverLimit(RESTError):
     code = 403
 
-    def __init__(self, count):
+    def __init__(self, count: int):
         super().__init__(
             "OverLimit", f"{count} Actions were found, maximum allowed is 7."
         )
```

### Comparing `moto-4.1.9.dev5/moto/sqs/models.py` & `moto-4.1.9.dev6/moto/sqs/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import hashlib
 import json
 import re
 import string
 
 import struct
 from copy import deepcopy
-from typing import Dict
+from typing import Any, Dict, List, Optional, Tuple, Set, TYPE_CHECKING
 from threading import Condition
+from urllib.parse import ParseResult
 from xml.sax.saxutils import escape
 
 from moto.core.exceptions import RESTError
 from moto.core import BaseBackend, BackendDict, BaseModel, CloudFormationModel
 from moto.core.utils import (
     camelcase_to_underscores,
     unix_time,
@@ -34,14 +35,17 @@
     InvalidAttributeName,
     InvalidParameterValue,
     MissingParameter,
     OverLimit,
     InvalidAttributeValue,
 )
 
+if TYPE_CHECKING:
+    from moto.awslambda.models import EventSourceMapping
+
 DEFAULT_SENDER_ID = "AIDAIT2UOQQY3AUEKVGXU"
 
 MAXIMUM_MESSAGE_LENGTH = 262144  # 256 KiB
 
 MAXIMUM_MESSAGE_SIZE_ATTR_LOWER_BOUND = 1024
 MAXIMUM_MESSAGE_SIZE_ATTR_UPPER_BOUND = MAXIMUM_MESSAGE_LENGTH
 
@@ -63,39 +67,44 @@
 # https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-message-metadata.html
 ATTRIBUTE_NAME_PATTERN = re.compile("^([a-z]|[A-Z]|[0-9]|[_.\\-])+$")
 
 DEDUPLICATION_TIME_IN_SECONDS = 300
 
 
 class Message(BaseModel):
-    def __init__(self, message_id, body, system_attributes=None):
+    def __init__(
+        self,
+        message_id: str,
+        body: str,
+        system_attributes: Optional[Dict[str, Any]] = None,
+    ):
         self.id = message_id
         self._body = body
-        self.message_attributes = {}
-        self.receipt_handle = None
-        self._old_receipt_handles = []
+        self.message_attributes: Dict[str, Any] = {}
+        self.receipt_handle: Optional[str] = None
+        self._old_receipt_handles: List[str] = []
         self.sender_id = DEFAULT_SENDER_ID
         self.sent_timestamp = None
-        self.approximate_first_receive_timestamp = None
+        self.approximate_first_receive_timestamp: Optional[int] = None
         self.approximate_receive_count = 0
-        self.deduplication_id = None
-        self.group_id = None
-        self.sequence_number = None
-        self.visible_at = 0
-        self.delayed_until = 0
+        self.deduplication_id: Optional[str] = None
+        self.group_id: Optional[str] = None
+        self.sequence_number: Optional[str] = None
+        self.visible_at = 0.0
+        self.delayed_until = 0.0
         self.system_attributes = system_attributes or {}
 
     @property
-    def body_md5(self):
+    def body_md5(self) -> str:
         md5 = md5_hash()
         md5.update(self._body.encode("utf-8"))
         return md5.hexdigest()
 
     @property
-    def attribute_md5(self):
+    def attribute_md5(self) -> str:
 
         md5 = md5_hash()
 
         for attrName in sorted(self.message_attributes.keys()):
             self.validate_attribute_name(attrName)
             attrValue = self.message_attributes[attrName]
             # Encode name
@@ -125,44 +134,44 @@
                 for strListMember in attrValue["binary_list_value"]:
                     decoded_binary_value = base64.b64decode(strListMember)
                     self.update_binary_length_and_value(md5, decoded_binary_value)
 
         return md5.hexdigest()
 
     @staticmethod
-    def update_binary_length_and_value(md5, value):
+    def update_binary_length_and_value(md5: Any, value: bytes) -> None:  # type: ignore[misc]
         length_bytes = struct.pack("!I".encode("ascii"), len(value))
         md5.update(length_bytes)
         md5.update(value)
 
     @staticmethod
-    def validate_attribute_name(name):
+    def validate_attribute_name(name: str) -> None:
         if not ATTRIBUTE_NAME_PATTERN.match(name):
             raise MessageAttributesInvalid(
                 f"The message attribute name '{name}' is invalid. "
                 "Attribute name can contain A-Z, a-z, 0-9, "
                 "underscore (_), hyphen (-), and period (.) characters."
             )
 
     @staticmethod
-    def utf8(value):
+    def utf8(value: Any) -> bytes:  # type: ignore[misc]
         if isinstance(value, str):
             return value.encode("utf-8")
         return value
 
     @property
-    def body(self):
+    def body(self) -> str:
         return escape(self._body).replace('"', "&quot;").replace("\r", "&#xD;")
 
-    def mark_sent(self, delay_seconds=None):
-        self.sent_timestamp = int(unix_time_millis())
+    def mark_sent(self, delay_seconds: Optional[int] = None) -> None:
+        self.sent_timestamp = int(unix_time_millis())  # type: ignore
         if delay_seconds:
             self.delay(delay_seconds=delay_seconds)
 
-    def mark_received(self, visibility_timeout=None):
+    def mark_received(self, visibility_timeout: Optional[int] = None) -> None:
         """
         When a message is received we will set the first receive timestamp,
         tap the ``approximate_receive_count`` and the ``visible_at`` time.
         """
         if visibility_timeout:
             visibility_timeout = int(visibility_timeout)
         else:
@@ -174,45 +183,45 @@
         self.approximate_receive_count += 1
 
         # Make message visible again in the future unless its
         # destroyed.
         if visibility_timeout:
             self.change_visibility(visibility_timeout)
 
-        self._old_receipt_handles.append(self.receipt_handle)
+        self._old_receipt_handles.append(self.receipt_handle)  # type: ignore
         self.receipt_handle = generate_receipt_handle()
 
-    def change_visibility(self, visibility_timeout):
+    def change_visibility(self, visibility_timeout: int) -> None:
         # We're dealing with milliseconds internally
         visibility_timeout_msec = int(visibility_timeout) * 1000
         self.visible_at = unix_time_millis() + visibility_timeout_msec
 
-    def delay(self, delay_seconds):
+    def delay(self, delay_seconds: int) -> None:
         delay_msec = int(delay_seconds) * 1000
         self.delayed_until = unix_time_millis() + delay_msec
 
     @property
-    def visible(self):
+    def visible(self) -> bool:
         current_time = unix_time_millis()
         if current_time > self.visible_at:
             return True
         return False
 
     @property
-    def delayed(self):
+    def delayed(self) -> bool:
         current_time = unix_time_millis()
         if current_time < self.delayed_until:
             return True
         return False
 
     @property
-    def all_receipt_handles(self):
-        return [self.receipt_handle] + self._old_receipt_handles
+    def all_receipt_handles(self) -> List[Optional[str]]:
+        return [self.receipt_handle] + self._old_receipt_handles  # type: ignore
 
-    def had_receipt_handle(self, receipt_handle):
+    def had_receipt_handle(self, receipt_handle: str) -> bool:
         """
         Check if this message ever had this receipt_handle in the past
         """
         return receipt_handle in self.all_receipt_handles
 
 
 class Queue(CloudFormationModel):
@@ -246,32 +255,33 @@
         "GetQueueUrl",
         "ListDeadLetterSourceQueues",
         "PurgeQueue",
         "ReceiveMessage",
         "SendMessage",
     )
 
-    def __init__(self, name, region, account_id, **kwargs):
+    def __init__(self, name: str, region: str, account_id: str, **kwargs: Any):
         self.name = name
         self.region = region
         self.account_id = account_id
-        self.tags = {}
-        self.permissions = {}
+        self.tags: Dict[str, str] = {}
+        self.permissions: Dict[str, Any] = {}
 
-        self._messages = []
-        self._pending_messages = set()
-        self.deleted_messages = set()
+        self._messages: List[Message] = []
+        self._pending_messages: Set[Message] = set()
+        self.deleted_messages: Set[str] = set()
         self._messages_lock = Condition()
 
         now = unix_time()
         self.created_timestamp = now
         self.queue_arn = f"arn:aws:sqs:{region}:{account_id}:{name}"
-        self.dead_letter_queue = None
+        self.dead_letter_queue: Optional["Queue"] = None
+        self.fifo_queue = False
 
-        self.lambda_event_source_mappings = {}
+        self.lambda_event_source_mappings: Dict[str, "EventSourceMapping"] = {}
 
         # default settings for a non fifo queue
         defaults = {
             "ContentBasedDeduplication": "false",
             "DeduplicationScope": "queue",
             "DelaySeconds": 0,
             "FifoQueue": "false",
@@ -289,32 +299,34 @@
         defaults.update(kwargs)
         self._set_attributes(defaults, now)
 
         # Check some conditions
         if self.fifo_queue and not self.name.endswith(".fifo"):
             raise InvalidParameterValue("Queue name must end in .fifo for FIFO queues")
         if (
-            self.maximum_message_size < MAXIMUM_MESSAGE_SIZE_ATTR_LOWER_BOUND
-            or self.maximum_message_size > MAXIMUM_MESSAGE_SIZE_ATTR_UPPER_BOUND
+            self.maximum_message_size < MAXIMUM_MESSAGE_SIZE_ATTR_LOWER_BOUND  # type: ignore
+            or self.maximum_message_size > MAXIMUM_MESSAGE_SIZE_ATTR_UPPER_BOUND  # type: ignore
         ):
             raise InvalidAttributeValue("MaximumMessageSize")
 
     @property
-    def pending_messages(self):
+    def pending_messages(self) -> Set[Message]:
         return self._pending_messages
 
     @property
-    def pending_message_groups(self):
+    def pending_message_groups(self) -> Set[str]:
         return set(
             message.group_id
             for message in self._pending_messages
             if message.group_id is not None
         )
 
-    def _set_attributes(self, attributes, now=None):
+    def _set_attributes(
+        self, attributes: Dict[str, Any], now: Optional[float] = None
+    ) -> None:
         if not now:
             now = unix_time()
 
         integer_fields = (
             "DelaySeconds",
             "KmsDataKeyreusePeriodSeconds",
             "MaximumMessageSize",
@@ -339,24 +351,24 @@
             self._setup_dlq(attributes["RedrivePolicy"])
 
         self.policy = attributes.get("Policy")
 
         self.last_modified_timestamp = now
 
     @staticmethod
-    def _is_empty_redrive_policy(policy):
+    def _is_empty_redrive_policy(policy: Any) -> bool:  # type: ignore[misc]
         if isinstance(policy, str):
             if policy == "" or len(json.loads(policy)) == 0:
                 return True
         elif isinstance(policy, dict) and len(policy) == 0:
             return True
 
         return False
 
-    def _setup_dlq(self, policy):
+    def _setup_dlq(self, policy: Any) -> None:
         if Queue._is_empty_redrive_policy(policy):
             self.redrive_policy = None
             self.dead_letter_queue = None
             return
 
         if isinstance(policy, str):
             try:
@@ -403,48 +415,53 @@
         else:
             raise RESTError(
                 "AWS.SimpleQueueService.NonExistentQueue",
                 f"Could not find DLQ for {self.redrive_policy['deadLetterTargetArn']}",
             )
 
     @staticmethod
-    def cloudformation_name_type():
+    def cloudformation_name_type() -> str:
         return "QueueName"
 
     @staticmethod
-    def cloudformation_type():
+    def cloudformation_type() -> str:
         # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-sqs-queue.html
         return "AWS::SQS::Queue"
 
     @classmethod
-    def create_from_cloudformation_json(
-        cls, resource_name, cloudformation_json, account_id, region_name, **kwargs
-    ):
+    def create_from_cloudformation_json(  # type: ignore[misc]
+        cls,
+        resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+        **kwargs: Any,
+    ) -> "Queue":
         properties = deepcopy(cloudformation_json["Properties"])
         # remove Tags from properties and convert tags list to dict
         tags = properties.pop("Tags", [])
         tags_dict = tags_from_cloudformation_tags_list(tags)
 
         # Could be passed as an integer - just treat it as a string
         resource_name = str(resource_name)
 
         sqs_backend = sqs_backends[account_id][region_name]
         return sqs_backend.create_queue(
             name=resource_name, tags=tags_dict, region=region_name, **properties
         )
 
     @classmethod
-    def update_from_cloudformation_json(
+    def update_from_cloudformation_json(  # type: ignore[misc]
         cls,
-        original_resource,
-        new_resource_name,
-        cloudformation_json,
-        account_id,
-        region_name,
-    ):
+        original_resource: Any,
+        new_resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+    ) -> "Queue":
         properties = cloudformation_json["Properties"]
         queue_name = original_resource.name
 
         sqs_backend = sqs_backends[account_id][region_name]
         queue = sqs_backend.get_queue(queue_name)
         if "VisibilityTimeout" in properties:
             queue.visibility_timeout = int(properties["VisibilityTimeout"])
@@ -452,53 +469,57 @@
         if "ReceiveMessageWaitTimeSeconds" in properties:
             queue.receive_message_wait_time_seconds = int(
                 properties["ReceiveMessageWaitTimeSeconds"]
             )
         return queue
 
     @classmethod
-    def delete_from_cloudformation_json(
-        cls, resource_name, cloudformation_json, account_id, region_name
-    ):
+    def delete_from_cloudformation_json(  # type: ignore[misc]
+        cls,
+        resource_name: str,
+        cloudformation_json: Any,
+        account_id: str,
+        region_name: str,
+    ) -> None:
         # ResourceName will be the full queue URL - we only need the name
         # https://sqs.us-west-1.amazonaws.com/123456789012/queue_name
         queue_name = resource_name.split("/")[-1]
         sqs_backend = sqs_backends[account_id][region_name]
         sqs_backend.delete_queue(queue_name)
 
     @property
-    def approximate_number_of_messages_delayed(self):
+    def approximate_number_of_messages_delayed(self) -> int:
         return len([m for m in self._messages if m.delayed])
 
     @property
-    def approximate_number_of_messages_not_visible(self):
+    def approximate_number_of_messages_not_visible(self) -> int:
         return len([m for m in self._messages if not m.visible])
 
     @property
-    def approximate_number_of_messages(self):
+    def approximate_number_of_messages(self) -> int:
         return len(self.messages)
 
     @property
-    def physical_resource_id(self):
+    def physical_resource_id(self) -> str:
         return f"https://sqs.{self.region}.amazonaws.com/{self.account_id}/{self.name}"
 
     @property
-    def attributes(self):
-        result = {}
+    def attributes(self) -> Dict[str, Any]:  # type: ignore[misc]
+        result: Dict[str, Any] = {}
 
         for attribute in self.BASE_ATTRIBUTES:
             attr = getattr(self, camelcase_to_underscores(attribute))
             result[attribute] = attr
 
         if self.fifo_queue:
             for attribute in self.FIFO_ATTRIBUTES:
                 attr = getattr(self, camelcase_to_underscores(attribute))
                 result[attribute] = attr
 
-        if self.kms_master_key_id:
+        if self.kms_master_key_id:  # type: ignore
             for attribute in self.KMS_ATTRIBUTES:
                 attr = getattr(self, camelcase_to_underscores(attribute))
                 result[attribute] = attr
 
         if self.policy:
             result["Policy"] = self.policy
 
@@ -507,41 +528,39 @@
 
         for key in result:
             if isinstance(result[key], bool):
                 result[key] = str(result[key]).lower()
 
         return result
 
-    def url(self, request_url):
-        return (
-            f"{request_url.scheme}://{request_url.netloc}/{self.account_id}/{self.name}"
-        )
+    def url(self, request_url: ParseResult) -> str:
+        return f"{request_url.scheme}://{request_url.netloc}/{self.account_id}/{self.name}"  # type: ignore
 
     @property
-    def messages(self):
+    def messages(self) -> List[Message]:
         # TODO: This can become very inefficient if a large number of messages are in-flight
         return [
             message
             for message in self._messages
             if message.visible and not message.delayed
         ]
 
-    def add_message(self, message):
+    def add_message(self, message: Message) -> None:
         if self.fifo_queue:
 
             # the cases in which we dedupe fifo messages
             # from https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/using-messagededuplicationid-property.html
             # https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_SendMessage.html
             if (
                 self.attributes.get("ContentBasedDeduplication") == "true"
                 or message.deduplication_id
             ):
                 for m in self._messages:
                     if m.deduplication_id == message.deduplication_id:
-                        diff = message.sent_timestamp - m.sent_timestamp
+                        diff = message.sent_timestamp - m.sent_timestamp  # type: ignore
                         # if a duplicate message is received within the deduplication time then it should
                         # not be added to the queue
                         if diff / 1000 < DEDUPLICATION_TIME_IN_SECONDS:
                             return
 
         with self._messages_lock:
             self._messages.append(message)
@@ -555,16 +574,16 @@
             that contains queue messages. Lambda reads messages in batches and invokes
             your function once for each batch. When your function successfully processes
             a batch, Lambda deletes its messages from the queue.
             """
             messages = backend.receive_message(
                 self.name,
                 esm.batch_size,
-                self.receive_message_wait_time_seconds,
-                self.visibility_timeout,
+                self.receive_message_wait_time_seconds,  # type: ignore
+                self.visibility_timeout,  # type: ignore
             )
 
             from moto.awslambda import lambda_backends
 
             result = lambda_backends[self.account_id][self.region].send_sqs_batch(
                 arn, messages, self.queue_arn
             )
@@ -576,92 +595,98 @@
                 [
                     backend.change_message_visibility(
                         self.name, m.receipt_handle, visibility_timeout=0
                     )
                     for m in messages
                 ]
 
-    def delete_message(self, receipt_handle):
+    def delete_message(self, receipt_handle: str) -> None:
         if receipt_handle in self.deleted_messages:
             # Already deleted - gracefully handle deleting it again
             return
 
         if not any(
             message.had_receipt_handle(receipt_handle) for message in self._messages
         ):
             raise ReceiptHandleIsInvalid()
 
         # Delete message from queue regardless of pending state
         new_messages = []
         for message in self._messages:
             if message.had_receipt_handle(receipt_handle):
                 self.pending_messages.discard(message)
-                self.deleted_messages.update(message.all_receipt_handles)
+                self.deleted_messages.update(message.all_receipt_handles)  # type: ignore
                 continue
             new_messages.append(message)
         self._messages = new_messages
 
-    def wait_for_messages(self, timeout):
+    def wait_for_messages(self, timeout: int) -> None:
         with self._messages_lock:
             self._messages_lock.wait_for(lambda: self.messages, timeout=timeout)
 
     @classmethod
-    def has_cfn_attr(cls, attr):
+    def has_cfn_attr(cls, attr: str) -> bool:
         return attr in ["Arn", "QueueName"]
 
-    def get_cfn_attribute(self, attribute_name):
+    def get_cfn_attribute(self, attribute_name: str) -> str:
         from moto.cloudformation.exceptions import UnformattedGetAttTemplateException
 
         if attribute_name == "Arn":
             return self.queue_arn
         elif attribute_name == "QueueName":
             return self.name
         raise UnformattedGetAttTemplateException()
 
     @property
-    def policy(self):
+    def policy(self) -> Any:  # type: ignore[misc]
         if self._policy_json.get("Statement"):
             return json.dumps(self._policy_json)
         else:
             return None
 
     @policy.setter
-    def policy(self, policy):
+    def policy(self, policy: Any) -> None:
         if policy:
             self._policy_json = json.loads(policy)
         else:
             self._policy_json = {
                 "Version": "2012-10-17",
                 "Id": f"{self.queue_arn}/SQSDefaultPolicy",
                 "Statement": [],
             }
 
 
-def _filter_message_attributes(message, input_message_attributes):
+def _filter_message_attributes(
+    message: Message, input_message_attributes: List[str]
+) -> None:
     filtered_message_attributes = {}
     return_all = "All" in input_message_attributes
     for key, value in message.message_attributes.items():
         if return_all or key in input_message_attributes:
             filtered_message_attributes[key] = value
     message.message_attributes = filtered_message_attributes
 
 
 class SQSBackend(BaseBackend):
-    def __init__(self, region_name, account_id):
+    def __init__(self, region_name: str, account_id: str):
         super().__init__(region_name, account_id)
         self.queues: Dict[str, Queue] = {}
 
     @staticmethod
-    def default_vpc_endpoint_service(service_region, zones):
+    def default_vpc_endpoint_service(
+        service_region: str, zones: List[str]
+    ) -> List[Dict[str, str]]:
         """Default VPC endpoint service."""
         return BaseBackend.default_vpc_endpoint_service_factory(
             service_region, zones, "sqs"
         )
 
-    def create_queue(self, name, tags=None, **kwargs):
+    def create_queue(
+        self, name: str, tags: Optional[Dict[str, str]] = None, **kwargs: Any
+    ) -> Queue:
         queue = self.queues.get(name)
         if queue:
             try:
                 kwargs.pop("region")
             except KeyError:
                 pass
 
@@ -688,40 +713,42 @@
             self.queues[name] = queue
 
         if tags:
             queue.tags = tags
 
         return queue
 
-    def get_queue_url(self, queue_name):
+    def get_queue_url(self, queue_name: str) -> Queue:
         return self.get_queue(queue_name)
 
-    def list_queues(self, queue_name_prefix):
+    def list_queues(self, queue_name_prefix: str) -> List[Queue]:
         re_str = ".*"
         if queue_name_prefix:
             re_str = f"^{queue_name_prefix}.*"
         prefix_re = re.compile(re_str)
         qs = []
         for name, q in self.queues.items():
             if prefix_re.search(name):
                 qs.append(q)
         return qs[:1000]
 
-    def get_queue(self, queue_name):
+    def get_queue(self, queue_name: str) -> Queue:
         queue = self.queues.get(queue_name)
         if queue is None:
             raise QueueDoesNotExist()
         return queue
 
-    def delete_queue(self, queue_name):
+    def delete_queue(self, queue_name: str) -> None:
         self.get_queue(queue_name)
 
         del self.queues[queue_name]
 
-    def get_queue_attributes(self, queue_name, attribute_names):
+    def get_queue_attributes(
+        self, queue_name: str, attribute_names: List[str]
+    ) -> Dict[str, Any]:
         queue = self.get_queue(queue_name)
         if not attribute_names:
             return {}
 
         valid_names = (
             ["All"]
             + queue.BASE_ATTRIBUTES
@@ -742,29 +769,31 @@
         else:
             for name in (name for name in attribute_names if name in queue.attributes):
                 if queue.attributes.get(name) is not None:
                     attributes[name] = queue.attributes.get(name)
 
         return attributes
 
-    def set_queue_attributes(self, queue_name, attributes):
+    def set_queue_attributes(
+        self, queue_name: str, attributes: Dict[str, Any]
+    ) -> Queue:
         queue = self.get_queue(queue_name)
         queue._set_attributes(attributes)
         return queue
 
     def send_message(
         self,
-        queue_name,
-        message_body,
-        message_attributes=None,
-        delay_seconds=None,
-        deduplication_id=None,
-        group_id=None,
-        system_attributes=None,
-    ):
+        queue_name: str,
+        message_body: str,
+        message_attributes: Optional[Dict[str, Any]] = None,
+        delay_seconds: Optional[int] = None,
+        deduplication_id: Optional[str] = None,
+        group_id: Optional[str] = None,
+        system_attributes: Optional[Dict[str, Any]] = None,
+    ) -> Message:
 
         queue = self.get_queue(queue_name)
 
         if queue.fifo_queue:
             if (
                 queue.attributes.get("ContentBasedDeduplication") == "false"
                 and not group_id
@@ -779,22 +808,22 @@
             ):
                 msg = (
                     "The queue should either have ContentBasedDeduplication enabled or "
                     "MessageDeduplicationId provided explicitly"
                 )
                 raise InvalidParameterValue(msg)
 
-        if len(message_body) > queue.maximum_message_size:
-            msg = f"One or more parameters are invalid. Reason: Message must be shorter than {queue.maximum_message_size} bytes."
+        if len(message_body) > queue.maximum_message_size:  # type: ignore
+            msg = f"One or more parameters are invalid. Reason: Message must be shorter than {queue.maximum_message_size} bytes."  # type: ignore
             raise InvalidParameterValue(msg)
 
         if delay_seconds:
             delay_seconds = int(delay_seconds)
         else:
-            delay_seconds = queue.delay_seconds
+            delay_seconds = queue.delay_seconds  # type: ignore
 
         message_id = str(random.uuid4())
         message = Message(message_id, message_body, system_attributes)
 
         # if content based deduplication is set then set sha256 hash of the message
         # as the deduplication_id
         if queue.attributes.get("ContentBasedDeduplication") == "true":
@@ -822,28 +851,30 @@
                 )
                 raise InvalidParameterValue(msg)
             message.group_id = group_id
 
         if message_attributes:
             message.message_attributes = message_attributes
 
-        if delay_seconds > MAXIMUM_MESSAGE_DELAY:
+        if delay_seconds > MAXIMUM_MESSAGE_DELAY:  # type: ignore
             msg = (
                 f"Value {delay_seconds} for parameter DelaySeconds is invalid. "
                 "Reason: DelaySeconds must be >= 0 and <= 900."
             )
             raise InvalidParameterValue(msg)
 
         message.mark_sent(delay_seconds=delay_seconds)
 
         queue.add_message(message)
 
         return message
 
-    def send_message_batch(self, queue_name, entries):
+    def send_message_batch(
+        self, queue_name: str, entries: Dict[str, Dict[str, Any]]
+    ) -> Tuple[List[Message], List[Dict[str, Any]]]:
         self.get_queue(queue_name)
 
         if any(
             not re.match(r"^[\w-]{1,80}$", entry["Id"]) for entry in entries.values()
         ):
             raise InvalidBatchEntryId()
 
@@ -876,60 +907,60 @@
                     queue_name,
                     entry["MessageBody"],
                     message_attributes=entry["MessageAttributes"],
                     delay_seconds=entry["DelaySeconds"],
                     group_id=entry.get("MessageGroupId"),
                     deduplication_id=entry.get("MessageDeduplicationId"),
                 )
-                message.user_id = entry["Id"]
+                message.user_id = entry["Id"]  # type: ignore[attr-defined]
                 messages.append(message)
             except InvalidParameterValue:
                 failedInvalidDelay.append(entry)
 
         return messages, failedInvalidDelay
 
-    def _get_first_duplicate_id(self, ids):
+    def _get_first_duplicate_id(self, ids: List[str]) -> Optional[str]:
         unique_ids = set()
         for _id in ids:
             if _id in unique_ids:
                 return _id
             unique_ids.add(_id)
         return None
 
     def receive_message(
         self,
-        queue_name,
-        count,
-        wait_seconds_timeout,
-        visibility_timeout,
-        message_attribute_names=None,
-    ):
+        queue_name: str,
+        count: int,
+        wait_seconds_timeout: int,
+        visibility_timeout: int,
+        message_attribute_names: Optional[List[str]] = None,
+    ) -> List[Message]:
         # Attempt to retrieve visible messages from a queue.
 
         # If a message was read by client and not deleted it is considered to be
         # "inflight" and cannot be read. We make attempts to obtain ``count``
         # messages but we may return less if messages are in-flight or there
         # are simple not enough messages in the queue.
 
         if message_attribute_names is None:
             message_attribute_names = []
         queue = self.get_queue(queue_name)
-        result = []
+        result: List[Message] = []
         previous_result_count = len(result)
 
         polling_end = unix_time() + wait_seconds_timeout
         currently_pending_groups = deepcopy(queue.pending_message_groups)
 
         # queue.messages only contains visible messages
         while True:
 
             if result or (wait_seconds_timeout and unix_time() > polling_end):
                 break
 
-            messages_to_dlq = []
+            messages_to_dlq: List[Message] = []
 
             for message in queue.messages:
                 if not message.visible:
                     continue
 
                 if message in queue.pending_messages:
                     # The message is pending but is visible again, so the
@@ -962,35 +993,37 @@
                     break
                 result.append(message_copy)
                 if len(result) >= count:
                     break
 
             for message in messages_to_dlq:
                 queue._messages.remove(message)
-                queue.dead_letter_queue.add_message(message)
+                queue.dead_letter_queue.add_message(message)  # type: ignore
 
             if previous_result_count == len(result):
                 if wait_seconds_timeout == 0:
                     # There is no timeout and no additional results,
                     # so break to avoid an infinite loop.
                     break
 
                 queue.wait_for_messages(1)
                 continue
 
             previous_result_count = len(result)
 
         return result
 
-    def delete_message(self, queue_name, receipt_handle):
+    def delete_message(self, queue_name: str, receipt_handle: str) -> None:
         queue = self.get_queue(queue_name)
 
         queue.delete_message(receipt_handle)
 
-    def delete_message_batch(self, queue_name, receipts):
+    def delete_message_batch(
+        self, queue_name: str, receipts: List[Dict[str, Any]]
+    ) -> Tuple[List[str], List[Dict[str, str]]]:
         success = []
         errors = []
         for receipt_and_id in receipts:
             try:
                 self.delete_message(queue_name, receipt_and_id["receipt_handle"])
                 success.append(receipt_and_id["msg_user_id"])
             except ReceiptHandleIsInvalid:
@@ -1000,36 +1033,40 @@
                         "SenderFault": "true",
                         "Code": "ReceiptHandleIsInvalid",
                         "Message": f'The input receipt handle "{receipt_and_id["receipt_handle"]}" is not a valid receipt handle.',
                     }
                 )
         return success, errors
 
-    def change_message_visibility(self, queue_name, receipt_handle, visibility_timeout):
+    def change_message_visibility(
+        self, queue_name: str, receipt_handle: str, visibility_timeout: int
+    ) -> None:
         queue = self.get_queue(queue_name)
         for message in queue._messages:
             if message.had_receipt_handle(receipt_handle):
 
                 visibility_timeout_msec = int(visibility_timeout) * 1000
                 given_visibility_timeout = unix_time_millis() + visibility_timeout_msec
-                if given_visibility_timeout - message.sent_timestamp > 43200 * 1000:
+                if given_visibility_timeout - message.sent_timestamp > 43200 * 1000:  # type: ignore
                     raise InvalidParameterValue(
                         f"Value {visibility_timeout} for parameter VisibilityTimeout is invalid. Reason: Total "
                         "VisibilityTimeout for the message is beyond the limit [43200 seconds]"
                     )
 
                 message.change_visibility(visibility_timeout)
                 if message.visible and message in queue.pending_messages:
                     # If the message is visible again, remove it from pending
                     # messages.
                     queue.pending_messages.remove(message)
                 return
         raise ReceiptHandleIsInvalid
 
-    def change_message_visibility_batch(self, queue_name: str, entries):
+    def change_message_visibility_batch(
+        self, queue_name: str, entries: List[Dict[str, Any]]
+    ) -> Tuple[List[str], List[Dict[str, str]]]:
         success = []
         error = []
         for entry in entries:
             try:
                 visibility_timeout = int(entry["visibility_timeout"])
                 assert visibility_timeout <= MAXIMUM_VISIBILITY_TIMEOUT
             except:  # noqa: E722 Do not use bare except
@@ -1057,30 +1094,32 @@
                         "SenderFault": "true",
                         "Code": "ReceiptHandleIsInvalid",
                         "Message": e.description,
                     }
                 )
         return success, error
 
-    def purge_queue(self, queue_name):
+    def purge_queue(self, queue_name: str) -> None:
         queue = self.get_queue(queue_name)
         queue._messages = []
         queue._pending_messages = set()
 
-    def list_dead_letter_source_queues(self, queue_name):
+    def list_dead_letter_source_queues(self, queue_name: str) -> List[Queue]:
         dlq = self.get_queue(queue_name)
 
-        queues = []
+        queues: List[Queue] = []
         for queue in self.queues.values():
             if queue.dead_letter_queue is dlq:
                 queues.append(queue)
 
         return queues
 
-    def add_permission(self, queue_name, actions, account_ids, label):
+    def add_permission(
+        self, queue_name: str, actions: List[str], account_ids: List[str], label: str
+    ) -> None:
         queue = self.get_queue(queue_name)
 
         if not actions:
             raise MissingParameter("Actions")
 
         if not account_ids:
             raise InvalidParameterValue(
@@ -1124,15 +1163,15 @@
             "Principal": {"AWS": principals[0] if len(principals) == 1 else principals},
             "Action": actions[0] if len(actions) == 1 else actions,
             "Resource": queue.queue_arn,
         }
 
         queue._policy_json["Statement"].append(statement)
 
-    def remove_permission(self, queue_name, label):
+    def remove_permission(self, queue_name: str, label: str) -> None:
         queue = self.get_queue(queue_name)
 
         statements = queue._policy_json["Statement"]
         statements_new = [
             statement for statement in statements if statement["Sid"] != label
         ]
 
@@ -1140,50 +1179,49 @@
             raise InvalidParameterValue(
                 f"Value {label} for parameter Label is invalid. "
                 "Reason: can't find label on existing policy."
             )
 
         queue._policy_json["Statement"] = statements_new
 
-    def tag_queue(self, queue_name, tags):
+    def tag_queue(self, queue_name: str, tags: Dict[str, str]) -> None:
         queue = self.get_queue(queue_name)
 
         if not len(tags):
             raise MissingParameter("Tags")
 
         if len(tags) > 50:
             raise InvalidParameterValue(f"Too many tags added for queue {queue_name}.")
 
         queue.tags.update(tags)
 
-    def untag_queue(self, queue_name, tag_keys):
+    def untag_queue(self, queue_name: str, tag_keys: List[str]) -> None:
         queue = self.get_queue(queue_name)
 
         if not len(tag_keys):
             raise RESTError(
                 "InvalidParameterValue",
                 "Tag keys must be between 1 and 128 characters in length.",
             )
 
         for key in tag_keys:
             try:
                 del queue.tags[key]
             except KeyError:
                 pass
 
-    def list_queue_tags(self, queue_name):
+    def list_queue_tags(self, queue_name: str) -> Queue:
         return self.get_queue(queue_name)
 
-    def is_message_valid_based_on_retention_period(self, queue_name, message):
-        message_attributes = self.get_queue_attributes(
+    def is_message_valid_based_on_retention_period(
+        self, queue_name: str, message: Message
+    ) -> bool:
+        retention_period = self.get_queue_attributes(
             queue_name, ["MessageRetentionPeriod"]
-        )
-        retain_until = (
-            message_attributes.get("MessageRetentionPeriod")
-            + message.sent_timestamp / 1000
-        )
+        )["MessageRetentionPeriod"]
+        retain_until = retention_period + message.sent_timestamp / 1000  # type: ignore
         if retain_until <= unix_time():
             return False
         return True
 
 
 sqs_backends = BackendDict(SQSBackend, "sqs")
```

### Comparing `moto-4.1.9.dev5/moto/sqs/responses.py` & `moto-4.1.9.dev6/moto/sqs/responses.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import re
+from typing import Any, Dict, Optional, Tuple, Union
 
+from moto.core.common_types import TYPE_RESPONSE
 from moto.core.exceptions import RESTError
 from moto.core.responses import BaseResponse
 from moto.core.utils import underscores_to_camelcase, camelcase_to_pascal
 from moto.utilities.aws_headers import amz_crc32, amzn_request_id
 from urllib.parse import urlparse
 
 from .constants import (
@@ -20,103 +22,105 @@
 from .utils import parse_message_attributes, extract_input_message_attributes
 
 
 class SQSResponse(BaseResponse):
 
     region_regex = re.compile(r"://(.+?)\.queue\.amazonaws\.com")
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(service_name="sqs")
 
     @property
     def sqs_backend(self) -> SQSBackend:
         return sqs_backends[self.current_account][self.region]
 
     @property
-    def attribute(self):
+    def attribute(self) -> Any:  # type: ignore[misc]
         if not hasattr(self, "_attribute"):
             self._attribute = self._get_map_prefix(
                 "Attribute", key_end=".Name", value_end=".Value"
             )
         return self._attribute
 
     @property
-    def tags(self):
+    def tags(self) -> Dict[str, str]:
         if not hasattr(self, "_tags"):
             self._tags = self._get_map_prefix("Tag", key_end=".Key", value_end=".Value")
         return self._tags
 
-    def _get_queue_name(self):
+    def _get_queue_name(self) -> str:
         try:
-            queue_url = self.querystring.get("QueueUrl")[0]
+            queue_url = self.querystring.get("QueueUrl")[0]  # type: ignore
             if queue_url.startswith("http://") or queue_url.startswith("https://"):
                 return queue_url.split("/")[-1]
             else:
                 # The parameter could be the name itself, which AWS also accepts
                 return queue_url
         except TypeError:
             # Fallback to reading from the URL for botocore
             return self.path.split("/")[-1]
 
-    def _get_validated_visibility_timeout(self, timeout=None):
+    def _get_validated_visibility_timeout(self, timeout: Optional[str] = None) -> int:
         """
         :raises ValueError: If specified visibility timeout exceeds MAXIMUM_VISIBILITY_TIMEOUT
         :raises TypeError: If visibility timeout was not specified
         """
         if timeout is not None:
             visibility_timeout = int(timeout)
         else:
-            visibility_timeout = int(self.querystring.get("VisibilityTimeout")[0])
+            visibility_timeout = int(self.querystring.get("VisibilityTimeout")[0])  # type: ignore
 
         if visibility_timeout > MAXIMUM_VISIBILITY_TIMEOUT:
             raise ValueError
 
         return visibility_timeout
 
     @amz_crc32  # crc last as request_id can edit XML
     @amzn_request_id
-    def call_action(self):
+    def call_action(self) -> TYPE_RESPONSE:
         status_code, headers, body = super().call_action()
         if status_code == 404:
             queue_name = self.querystring.get("QueueName", [""])[0]
             template = self.response_template(ERROR_INEXISTENT_QUEUE)
             response = template.render(queue_name=queue_name)
             return 404, headers, response
         return status_code, headers, body
 
-    def _error(self, code, message, status=400):
+    def _error(
+        self, code: str, message: str, status: int = 400
+    ) -> Tuple[str, Dict[str, int]]:
         template = self.response_template(ERROR_TEMPLATE)
         return template.render(code=code, message=message), dict(status=status)
 
-    def create_queue(self):
+    def create_queue(self) -> str:
         request_url = urlparse(self.uri)
         queue_name = self._get_param("QueueName")
 
         queue = self.sqs_backend.create_queue(queue_name, self.tags, **self.attribute)
 
         template = self.response_template(CREATE_QUEUE_RESPONSE)
         return template.render(queue_url=queue.url(request_url))
 
-    def get_queue_url(self):
+    def get_queue_url(self) -> str:
         request_url = urlparse(self.uri)
         queue_name = self._get_param("QueueName")
 
         queue = self.sqs_backend.get_queue_url(queue_name)
 
         template = self.response_template(GET_QUEUE_URL_RESPONSE)
         return template.render(queue_url=queue.url(request_url))
 
-    def list_queues(self):
+    def list_queues(self) -> str:
         request_url = urlparse(self.uri)
         queue_name_prefix = self._get_param("QueueNamePrefix")
         queues = self.sqs_backend.list_queues(queue_name_prefix)
         template = self.response_template(LIST_QUEUES_RESPONSE)
         return template.render(queues=queues, request_url=request_url)
 
-    def change_message_visibility(self):
+    def change_message_visibility(self) -> Union[str, Tuple[str, Dict[str, int]]]:
         queue_name = self._get_queue_name()
         receipt_handle = self._get_param("ReceiptHandle")
 
         try:
             visibility_timeout = self._get_validated_visibility_timeout()
         except ValueError:
             return ERROR_MAX_VISIBILITY_TIMEOUT_RESPONSE, dict(status=400)
@@ -126,43 +130,42 @@
             receipt_handle=receipt_handle,
             visibility_timeout=visibility_timeout,
         )
 
         template = self.response_template(CHANGE_MESSAGE_VISIBILITY_RESPONSE)
         return template.render()
 
-    def change_message_visibility_batch(self):
+    def change_message_visibility_batch(self) -> str:
         queue_name = self._get_queue_name()
         entries = self._get_list_prefix("ChangeMessageVisibilityBatchRequestEntry")
 
         success, error = self.sqs_backend.change_message_visibility_batch(
             queue_name, entries
         )
 
         template = self.response_template(CHANGE_MESSAGE_VISIBILITY_BATCH_RESPONSE)
         return template.render(success=success, errors=error)
 
-    def get_queue_attributes(self):
+    def get_queue_attributes(self) -> str:
         queue_name = self._get_queue_name()
 
         if self.querystring.get("AttributeNames"):
             raise InvalidAttributeName("")
 
-        attribute_names = self._get_multi_param("AttributeName")
-
         # if connecting to AWS via boto, then 'AttributeName' is just a normal parameter
-        if not attribute_names:
-            attribute_names = self.querystring.get("AttributeName")
+        attribute_names = self._get_multi_param(
+            "AttributeName"
+        ) or self.querystring.get("AttributeName")
 
-        attributes = self.sqs_backend.get_queue_attributes(queue_name, attribute_names)
+        attributes = self.sqs_backend.get_queue_attributes(queue_name, attribute_names)  # type: ignore
 
         template = self.response_template(GET_QUEUE_ATTRIBUTES_RESPONSE)
         return template.render(attributes=attributes)
 
-    def set_queue_attributes(self):
+    def set_queue_attributes(self) -> str:
         # TODO validate self.get_param('QueueUrl')
         attribute = self.attribute
 
         # Fixes issue with Policy set to empty str
         attribute_names = self._get_multi_param("Attribute")
         if attribute_names:
             for attr in attribute_names:
@@ -170,24 +173,24 @@
                     attribute = {attr["Name"]: None}
 
         queue_name = self._get_queue_name()
         self.sqs_backend.set_queue_attributes(queue_name, attribute)
 
         return SET_QUEUE_ATTRIBUTE_RESPONSE
 
-    def delete_queue(self):
+    def delete_queue(self) -> str:
         # TODO validate self.get_param('QueueUrl')
         queue_name = self._get_queue_name()
 
         self.sqs_backend.delete_queue(queue_name)
 
         template = self.response_template(DELETE_QUEUE_RESPONSE)
         return template.render()
 
-    def send_message(self):
+    def send_message(self) -> Union[str, Tuple[str, Dict[str, int]]]:
         message = self._get_param("MessageBody")
         delay_seconds = int(self._get_param("DelaySeconds", 0))
         message_group_id = self._get_param("MessageGroupId")
         message_dedupe_id = self._get_param("MessageDeduplicationId")
 
         if len(message) > MAXIMUM_MESSAGE_LENGTH:
             return ERROR_TOO_LONG_RESPONSE, dict(status=400)
@@ -211,15 +214,15 @@
             )
         except RESTError as err:
             return self._error(err.error_type, err.message)
 
         template = self.response_template(SEND_MESSAGE_RESPONSE)
         return template.render(message=message, message_attributes=message_attributes)
 
-    def send_message_batch(self):
+    def send_message_batch(self) -> str:
         """
         The querystring comes like this
 
         'SendMessageBatchRequestEntry.1.DelaySeconds': ['0'],
         'SendMessageBatchRequestEntry.1.MessageBody': ['test message 1'],
         'SendMessageBatchRequestEntry.1.Id': ['6d0f122d-4b13-da2c-378f-e74244d8ad11']
         'SendMessageBatchRequestEntry.2.Id': ['ff8cbf59-70a2-c1cb-44c7-b7469f1ba390'],
@@ -243,15 +246,15 @@
                 message_attributes = parse_message_attributes(
                     self.querystring,
                     base=f"SendMessageBatchRequestEntry.{index}.",
                 )
 
                 entries[index] = {
                     "Id": value[0],
-                    "MessageBody": self.querystring.get(
+                    "MessageBody": self.querystring.get(  # type: ignore
                         f"SendMessageBatchRequestEntry.{index}.MessageBody"
                     )[0],
                     "DelaySeconds": self.querystring.get(
                         f"SendMessageBatchRequestEntry.{index}.DelaySeconds",
                         [None],
                     )[0],
                     "MessageAttributes": message_attributes,
@@ -282,22 +285,22 @@
                     "Message": "Value 1800 for parameter DelaySeconds is invalid. Reason: DelaySeconds must be &gt;= 0 and &lt;= 900.",
                 }
             )
 
         template = self.response_template(SEND_MESSAGE_BATCH_RESPONSE)
         return template.render(messages=messages, errors=errors)
 
-    def delete_message(self):
+    def delete_message(self) -> str:
         queue_name = self._get_queue_name()
-        receipt_handle = self.querystring.get("ReceiptHandle")[0]
+        receipt_handle = self.querystring.get("ReceiptHandle")[0]  # type: ignore
         self.sqs_backend.delete_message(queue_name, receipt_handle)
         template = self.response_template(DELETE_MESSAGE_RESPONSE)
         return template.render()
 
-    def delete_message_batch(self):
+    def delete_message_batch(self) -> str:
         """
         The querystring comes like this
 
         'DeleteMessageBatchRequestEntry.1.Id': ['message_1'],
         'DeleteMessageBatchRequestEntry.1.ReceiptHandle': ['asdfsfs...'],
         'DeleteMessageBatchRequestEntry.2.Id': ['message_2'],
         'DeleteMessageBatchRequestEntry.2.ReceiptHandle': ['zxcvfda...'],
@@ -312,15 +315,15 @@
             receipt_key = f"DeleteMessageBatchRequestEntry.{index}.ReceiptHandle"
             receipt_handle = self.querystring.get(receipt_key)
             if not receipt_handle:
                 # Found all messages
                 break
 
             message_user_id_key = f"DeleteMessageBatchRequestEntry.{index}.Id"
-            message_user_id = self.querystring.get(message_user_id_key)[0]
+            message_user_id = self.querystring.get(message_user_id_key)[0]  # type: ignore
             receipts.append(
                 {"receipt_handle": receipt_handle[0], "msg_user_id": message_user_id}
             )
 
         receipt_seen = set()
         for receipt_and_id in receipts:
             receipt = receipt_and_id["receipt_handle"]
@@ -329,62 +332,62 @@
             receipt_seen.add(receipt)
 
         success, errors = self.sqs_backend.delete_message_batch(queue_name, receipts)
 
         template = self.response_template(DELETE_MESSAGE_BATCH_RESPONSE)
         return template.render(success=success, errors=errors)
 
-    def purge_queue(self):
+    def purge_queue(self) -> str:
         queue_name = self._get_queue_name()
         self.sqs_backend.purge_queue(queue_name)
         template = self.response_template(PURGE_QUEUE_RESPONSE)
         return template.render()
 
-    def receive_message(self):
+    def receive_message(self) -> Union[str, Tuple[str, Dict[str, int]]]:
         queue_name = self._get_queue_name()
         message_attributes = self._get_multi_param("message_attributes")
         if not message_attributes:
             message_attributes = extract_input_message_attributes(self.querystring)
 
         attribute_names = self._get_multi_param("AttributeName")
 
         queue = self.sqs_backend.get_queue(queue_name)
 
         try:
-            message_count = int(self.querystring.get("MaxNumberOfMessages")[0])
+            message_count = int(self.querystring.get("MaxNumberOfMessages")[0])  # type: ignore
         except TypeError:
             message_count = DEFAULT_RECEIVED_MESSAGES
 
         if message_count < 1 or message_count > 10:
             return self._error(
                 "InvalidParameterValue",
                 "An error occurred (InvalidParameterValue) when calling "
                 f"the ReceiveMessage operation: Value {message_count} for parameter "
                 "MaxNumberOfMessages is invalid. Reason: must be between "
                 "1 and 10, if provided.",
             )
 
         try:
-            wait_time = int(self.querystring.get("WaitTimeSeconds")[0])
+            wait_time = int(self.querystring.get("WaitTimeSeconds")[0])  # type: ignore
         except TypeError:
-            wait_time = int(queue.receive_message_wait_time_seconds)
+            wait_time = int(queue.receive_message_wait_time_seconds)  # type: ignore
 
         if wait_time < 0 or wait_time > 20:
             return self._error(
                 "InvalidParameterValue",
                 "An error occurred (InvalidParameterValue) when calling "
                 f"the ReceiveMessage operation: Value {wait_time} for parameter "
                 "WaitTimeSeconds is invalid. Reason: must be &lt;= 0 and "
                 "&gt;= 20 if provided.",
             )
 
         try:
             visibility_timeout = self._get_validated_visibility_timeout()
         except TypeError:
-            visibility_timeout = queue.visibility_timeout
+            visibility_timeout = queue.visibility_timeout  # type: ignore
         except ValueError:
             return ERROR_MAX_VISIBILITY_TIMEOUT_RESPONSE, dict(status=400)
 
         messages = self.sqs_backend.receive_message(
             queue_name, message_count, wait_time, visibility_timeout, message_attributes
         )
 
@@ -402,62 +405,62 @@
             pascalcase_name = camelcase_to_pascal(underscores_to_camelcase(attribute))
             if any(x in ["All", pascalcase_name] for x in attribute_names):
                 attributes[attribute] = True
 
         template = self.response_template(RECEIVE_MESSAGE_RESPONSE)
         return template.render(messages=messages, attributes=attributes)
 
-    def list_dead_letter_source_queues(self):
+    def list_dead_letter_source_queues(self) -> str:
         request_url = urlparse(self.uri)
         queue_name = self._get_queue_name()
 
         source_queue_urls = self.sqs_backend.list_dead_letter_source_queues(queue_name)
 
         template = self.response_template(LIST_DEAD_LETTER_SOURCE_QUEUES_RESPONSE)
         return template.render(queues=source_queue_urls, request_url=request_url)
 
-    def add_permission(self):
+    def add_permission(self) -> str:
         queue_name = self._get_queue_name()
         actions = self._get_multi_param("ActionName")
         account_ids = self._get_multi_param("AWSAccountId")
         label = self._get_param("Label")
 
         self.sqs_backend.add_permission(queue_name, actions, account_ids, label)
 
         template = self.response_template(ADD_PERMISSION_RESPONSE)
         return template.render()
 
-    def remove_permission(self):
+    def remove_permission(self) -> str:
         queue_name = self._get_queue_name()
         label = self._get_param("Label")
 
         self.sqs_backend.remove_permission(queue_name, label)
 
         template = self.response_template(REMOVE_PERMISSION_RESPONSE)
         return template.render()
 
-    def tag_queue(self):
+    def tag_queue(self) -> str:
         queue_name = self._get_queue_name()
         tags = self._get_map_prefix("Tag", key_end=".Key", value_end=".Value")
 
         self.sqs_backend.tag_queue(queue_name, tags)
 
         template = self.response_template(TAG_QUEUE_RESPONSE)
         return template.render()
 
-    def untag_queue(self):
+    def untag_queue(self) -> str:
         queue_name = self._get_queue_name()
         tag_keys = self._get_multi_param("TagKey")
 
         self.sqs_backend.untag_queue(queue_name, tag_keys)
 
         template = self.response_template(UNTAG_QUEUE_RESPONSE)
         return template.render()
 
-    def list_queue_tags(self):
+    def list_queue_tags(self) -> str:
         queue_name = self._get_queue_name()
 
         queue = self.sqs_backend.list_queue_tags(queue_name)
 
         template = self.response_template(LIST_QUEUE_TAGS_RESPONSE)
         return template.render(tags=queue.tags)
```

### Comparing `moto-4.1.9.dev5/moto/sqs/utils.py` & `moto-4.1.9.dev6/moto/sqs/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import string
+from typing import Any, Dict, List
+
 from moto.moto_api._internal import mock_random as random
 from .exceptions import MessageAttributesInvalid
 
 
-def generate_receipt_handle():
+def generate_receipt_handle() -> str:
     # http://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/ImportantIdentifiers.html#ImportantIdentifiers-receipt-handles
     length = 185
     return "".join(random.choice(string.ascii_lowercase) for x in range(length))
 
 
-def extract_input_message_attributes(querystring):
+def extract_input_message_attributes(querystring: Dict[str, Any]) -> List[str]:
     message_attributes = []
     index = 1
     while True:
         # Loop through looking for message attributes
         name_key = f"MessageAttributeName.{index}"
         name = querystring.get(name_key)
         if not name:
@@ -21,16 +23,19 @@
             break
         message_attributes.append(name[0])
         index = index + 1
     return message_attributes
 
 
 def parse_message_attributes(
-    querystring, key="MessageAttribute", base="", value_namespace="Value."
-):
+    querystring: Dict[str, Any],
+    key: str = "MessageAttribute",
+    base: str = "",
+    value_namespace: str = "Value.",
+) -> Dict[str, Any]:
     message_attributes = {}
     index = 1
     while True:
         # Loop through looking for message attributes
         name_key = base + f"{key}.{index}.Name"
         name = querystring.get(name_key)
         if not name:
```

### Comparing `moto-4.1.9.dev5/moto/ssm/exceptions.py` & `moto-4.1.9.dev6/moto/ssm/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/models.py` & `moto-4.1.9.dev6/moto/ssm/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ami-amazon-linux-latest/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/af-south-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/af-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-northeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ap-southeast-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/ca-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-central-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-north-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-south-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/eu-west-3.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/me-central-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/me-central-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/me-south-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/me-south-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/sa-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/us-east-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-east-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/us-east-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-1.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/us-west-1.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/ecs/optimized_amis/us-west-2.json` & `moto-4.1.9.dev6/moto/ssm/resources/ecs/optimized_amis/us-west-2.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/regions.json` & `moto-4.1.9.dev6/moto/ssm/resources/regions.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/resources/services.json` & `moto-4.1.9.dev6/moto/ssm/resources/services.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/responses.py` & `moto-4.1.9.dev6/moto/ssm/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssm/utils.py` & `moto-4.1.9.dev6/moto/ssm/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssoadmin/models.py` & `moto-4.1.9.dev6/moto/ssoadmin/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/ssoadmin/responses.py` & `moto-4.1.9.dev6/moto/ssoadmin/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/stepfunctions/exceptions.py` & `moto-4.1.9.dev6/moto/stepfunctions/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/stepfunctions/models.py` & `moto-4.1.9.dev6/moto/stepfunctions/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/stepfunctions/responses.py` & `moto-4.1.9.dev6/moto/stepfunctions/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/stepfunctions/utils.py` & `moto-4.1.9.dev6/moto/stepfunctions/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sts/models.py` & `moto-4.1.9.dev6/moto/sts/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sts/responses.py` & `moto-4.1.9.dev6/moto/sts/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/sts/utils.py` & `moto-4.1.9.dev6/moto/sts/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/support/models.py` & `moto-4.1.9.dev6/moto/support/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/support/resources/describe_trusted_advisor_checks.json` & `moto-4.1.9.dev6/moto/support/resources/describe_trusted_advisor_checks.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/support/responses.py` & `moto-4.1.9.dev6/moto/support/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/constants.py` & `moto-4.1.9.dev6/moto/swf/constants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/exceptions.py` & `moto-4.1.9.dev6/moto/swf/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/models/__init__.py` & `moto-4.1.9.dev6/moto/swf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/models/activity_task.py` & `moto-4.1.9.dev6/moto/swf/models/activity_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/models/decision_task.py` & `moto-4.1.9.dev6/moto/swf/models/decision_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/models/domain.py` & `moto-4.1.9.dev6/moto/swf/models/domain.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/models/generic_type.py` & `moto-4.1.9.dev6/moto/swf/models/generic_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/models/history_event.py` & `moto-4.1.9.dev6/moto/swf/models/history_event.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/models/workflow_execution.py` & `moto-4.1.9.dev6/moto/swf/models/workflow_execution.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/swf/responses.py` & `moto-4.1.9.dev6/moto/swf/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/textract/exceptions.py` & `moto-4.1.9.dev6/moto/textract/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/textract/models.py` & `moto-4.1.9.dev6/moto/textract/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/textract/responses.py` & `moto-4.1.9.dev6/moto/textract/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/timestreamwrite/models.py` & `moto-4.1.9.dev6/moto/timestreamwrite/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/timestreamwrite/responses.py` & `moto-4.1.9.dev6/moto/timestreamwrite/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/transcribe/models.py` & `moto-4.1.9.dev6/moto/transcribe/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/transcribe/responses.py` & `moto-4.1.9.dev6/moto/transcribe/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/utilities/aws_headers.py` & `moto-4.1.9.dev6/moto/utilities/aws_headers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/utilities/distutils_version.py` & `moto-4.1.9.dev6/moto/utilities/distutils_version.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/utilities/docker_utilities.py` & `moto-4.1.9.dev6/moto/utilities/docker_utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/utilities/paginator.py` & `moto-4.1.9.dev6/moto/utilities/paginator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/utilities/tagging_service.py` & `moto-4.1.9.dev6/moto/utilities/tagging_service.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/utilities/tokenizer.py` & `moto-4.1.9.dev6/moto/utilities/tokenizer.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/utilities/utils.py` & `moto-4.1.9.dev6/moto/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/wafv2/exceptions.py` & `moto-4.1.9.dev6/moto/wafv2/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/wafv2/models.py` & `moto-4.1.9.dev6/moto/wafv2/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/wafv2/responses.py` & `moto-4.1.9.dev6/moto/wafv2/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/xray/exceptions.py` & `moto-4.1.9.dev6/moto/xray/exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/xray/mock_client.py` & `moto-4.1.9.dev6/moto/xray/mock_client.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/xray/models.py` & `moto-4.1.9.dev6/moto/xray/models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto/xray/responses.py` & `moto-4.1.9.dev6/moto/xray/responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto.egg-info/PKG-INFO` & `moto-4.1.9.dev6/moto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moto
-Version: 4.1.9.dev5
+Version: 4.1.9.dev6
 Home-page: https://github.com/getmoto/moto
 Author: Steve Pulec
 Author-email: "spulec@gmail.com"
 License: Apache License 2.0
 Project-URL: Documentation, http://docs.getmoto.org/en/latest/
 Project-URL: Issue tracker, https://github.com/getmoto/moto/issues
 Project-URL: Changelog, https://github.com/getmoto/moto/blob/master/CHANGELOG.md
```

### Comparing `moto-4.1.9.dev5/moto.egg-info/SOURCES.txt` & `moto-4.1.9.dev6/moto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/moto.egg-info/requires.txt` & `moto-4.1.9.dev6/moto.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/setup.cfg` & `moto-4.1.9.dev6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = moto
-version = 4.1.9.dev5
+version = 4.1.9.dev6
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Steve Pulec
 author_email = "spulec@gmail.com"
 url = https://github.com/getmoto/moto
 license = Apache License 2.0
 test_suite = tests
@@ -232,15 +232,15 @@
 ignore-paths = moto/packages
 
 [pylint.'MESSAGES CONTROL']
 disable = W,C,R,E
 enable = anomalous-backslash-in-string, arguments-renamed, dangerous-default-value, deprecated-module, function-redefined, import-self, redefined-builtin, redefined-outer-name, reimported, pointless-statement, super-with-arguments, unused-argument, unused-import, unused-variable, useless-else-on-loop, wildcard-import
 
 [mypy]
-files = moto/a*,moto/b*,moto/c*,moto/d*,moto/e*,moto/f*,moto/g*,moto/i*,moto/k*,moto/l*,moto/m*,moto/n*,moto/o*,moto/p*,moto/q*,moto/r*,moto/s3*,moto/sagemaker,moto/secretsmanager,moto/ssm,moto/scheduler
+files = moto/a*,moto/b*,moto/c*,moto/d*,moto/e*,moto/f*,moto/g*,moto/i*,moto/k*,moto/l*,moto/m*,moto/n*,moto/o*,moto/p*,moto/q*,moto/r*,moto/s3*,moto/sagemaker,moto/secretsmanager,moto/sqs,moto/ssm,moto/scheduler
 show_column_numbers = True
 show_error_codes = True
 disable_error_code = abstract
 disallow_any_unimported = False
 disallow_any_expr = False
 disallow_any_decorated = True
 disallow_any_explicit = False
```

### Comparing `moto-4.1.9.dev5/tests/__init__.py` & `moto-4.1.9.dev6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/helpers.py` & `moto-4.1.9.dev6/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_acm/resources/README.md` & `moto-4.1.9.dev6/tests/test_acm/resources/README.md`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_acm/resources/ca.key` & `moto-4.1.9.dev6/tests/test_acm/resources/ca.key`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_acm/resources/ca.pem` & `moto-4.1.9.dev6/tests/test_acm/resources/ca.pem`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com-bad.pem` & `moto-4.1.9.dev6/tests/test_acm/resources/star_moto_com-bad.pem`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.csr` & `moto-4.1.9.dev6/tests/test_acm/resources/star_moto_com.csr`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.key` & `moto-4.1.9.dev6/tests/test_acm/resources/star_moto_com.key`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_acm/resources/star_moto_com.pem` & `moto-4.1.9.dev6/tests/test_acm/resources/star_moto_com.pem`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_acm/test_acm.py` & `moto-4.1.9.dev6/tests/test_acm/test_acm.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_acmpca/test_acmpca.py` & `moto-4.1.9.dev6/tests/test_acmpca/test_acmpca.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_amp/test_amp_logging_config.py` & `moto-4.1.9.dev6/tests/test_amp/test_amp_logging_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_amp/test_amp_rulegroupnamespaces.py` & `moto-4.1.9.dev6/tests/test_amp/test_amp_rulegroupnamespaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_amp/test_amp_workspaces.py` & `moto-4.1.9.dev6/tests/test_amp/test_amp_workspaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/resources/petstore-swagger-v3.yaml` & `moto-4.1.9.dev6/tests/test_apigateway/resources/petstore-swagger-v3.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/resources/test_api.json` & `moto-4.1.9.dev6/tests/test_apigateway/resources/test_api.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/resources/test_api.yaml` & `moto-4.1.9.dev6/tests/test_apigateway/resources/test_api.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/resources/test_api_invalid.json` & `moto-4.1.9.dev6/tests/test_apigateway/resources/test_api_invalid.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/resources/test_api_invalid_version.json` & `moto-4.1.9.dev6/tests/test_apigateway/resources/test_api_invalid_version.json`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/resources/test_deep_api.yaml` & `moto-4.1.9.dev6/tests/test_apigateway/resources/test_deep_api.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_cloudformation.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_deployments.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_deployments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_export.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_export.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_gatewayresponses.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_gatewayresponses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_importrestapi.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_importrestapi.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_integration.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_putrestapi.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_putrestapi.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_stage.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_stage.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_validators.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_validators.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_apigateway_vpclink.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_apigateway_vpclink.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigateway/test_server.py` & `moto-4.1.9.dev6/tests/test_apigateway/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_authorizers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_domains.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_domains.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_integrationresponses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_integrations.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_integrations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_mappings.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_mappings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_models.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_reimport.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_reimport.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_routes.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_routes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_tags.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py` & `moto-4.1.9.dev6/tests/test_apigatewayv2/test_apigatewayv2_vpclinks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_applicationautoscaling/test_applicationautoscaling.py` & `moto-4.1.9.dev6/tests/test_applicationautoscaling/test_applicationautoscaling.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_applicationautoscaling/test_validation.py` & `moto-4.1.9.dev6/tests/test_applicationautoscaling/test_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_appsync/test_appsync.py` & `moto-4.1.9.dev6/tests/test_appsync/test_appsync.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_appsync/test_appsync_apikeys.py` & `moto-4.1.9.dev6/tests/test_appsync/test_appsync_apikeys.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_appsync/test_appsync_schema.py` & `moto-4.1.9.dev6/tests/test_appsync/test_appsync_schema.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_appsync/test_appsync_tags.py` & `moto-4.1.9.dev6/tests/test_appsync/test_appsync_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_athena/test_athena.py` & `moto-4.1.9.dev6/tests/test_athena/test_athena.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_athena/test_athena_server_api.py` & `moto-4.1.9.dev6/tests/test_athena/test_athena_server_api.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_cloudformation.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_groups.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_metrics.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_metrics.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_scheduledactions.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_scheduledactions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_autoscaling_tags.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_autoscaling_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_elb.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_elb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_elbv2.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_elbv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_launch_configurations.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_launch_configurations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/test_policies.py` & `moto-4.1.9.dev6/tests/test_autoscaling/test_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_autoscaling/utils.py` & `moto-4.1.9.dev6/tests/test_autoscaling/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_awslambda_cloudformation.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_awslambda_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_lambda.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_lambda.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_alias.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_lambda_alias.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_concurrency.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_lambda_concurrency.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_eventsourcemapping.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_lambda_eventsourcemapping.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_function_urls.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_lambda_function_urls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_invoke.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_lambda_invoke.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_layers.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_lambda_layers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_policy.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_lambda_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_lambda_tags.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_lambda_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/test_policy.py` & `moto-4.1.9.dev6/tests/test_awslambda/test_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_awslambda/utilities.py` & `moto-4.1.9.dev6/tests/test_awslambda/utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch/__init__.py` & `moto-4.1.9.dev6/tests/test_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch/test_batch_cloudformation.py` & `moto-4.1.9.dev6/tests/test_batch/test_batch_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch/test_batch_compute_envs.py` & `moto-4.1.9.dev6/tests/test_batch/test_batch_compute_envs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch/test_batch_job_queue.py` & `moto-4.1.9.dev6/tests/test_batch/test_batch_job_queue.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch/test_batch_jobs.py` & `moto-4.1.9.dev6/tests/test_batch/test_batch_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch/test_batch_scheduling_policy.py` & `moto-4.1.9.dev6/tests/test_batch/test_batch_scheduling_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch/test_batch_tags_job_definition.py` & `moto-4.1.9.dev6/tests/test_batch/test_batch_tags_job_definition.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch/test_batch_tags_job_queue.py` & `moto-4.1.9.dev6/tests/test_batch/test_batch_tags_job_queue.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch/test_batch_task_definition.py` & `moto-4.1.9.dev6/tests/test_batch/test_batch_task_definition.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch_simple/test_batch_cloudformation.py` & `moto-4.1.9.dev6/tests/test_batch_simple/test_batch_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch_simple/test_batch_compute_envs.py` & `moto-4.1.9.dev6/tests/test_batch_simple/test_batch_compute_envs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_batch_simple/test_batch_jobs.py` & `moto-4.1.9.dev6/tests/test_batch_simple/test_batch_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_budgets/test_budgets.py` & `moto-4.1.9.dev6/tests/test_budgets/test_budgets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_budgets/test_notifications.py` & `moto-4.1.9.dev6/tests/test_budgets/test_notifications.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_budgets/test_server.py` & `moto-4.1.9.dev6/tests/test_budgets/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ce/test_ce.py` & `moto-4.1.9.dev6/tests/test_ce/test_ce.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ce/test_ce_tags.py` & `moto-4.1.9.dev6/tests/test_ce/test_ce_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/custom_lambda.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/custom_lambda.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/kms_key.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/kms_key.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/rds_mysql_with_db_parameter_group.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/rds_mysql_with_read_replica.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/redshift.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/redshift.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/route53_ec2_instance_with_public_ip.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_health_check.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/route53_health_check.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/route53_roundrobin.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/route53_roundrobin.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/single_instance_with_ebs_volume.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_eni.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/vpc_eni.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py` & `moto-4.1.9.dev6/tests/test_cloudformation/fixtures/vpc_single_instance_in_subnet.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_custom_resources.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_custom_resources.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_depends_on.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_depends_on.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_multi_accounts.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_multi_accounts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_nested_stacks.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_nested_stacks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_stack_crud_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_integration.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_stack_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_cloudformation_stack_policies.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_cloudformation_stack_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_import_value.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_import_value.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_server.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_stack_parsing.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_stack_parsing.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudformation/test_validate.py` & `moto-4.1.9.dev6/tests/test_cloudformation/test_validate.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudfront/cloudfront_test_scaffolding.py` & `moto-4.1.9.dev6/tests/test_cloudfront/cloudfront_test_scaffolding.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront.py` & `moto-4.1.9.dev6/tests/test_cloudfront/test_cloudfront.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_dist_tags.py` & `moto-4.1.9.dev6/tests/test_cloudfront/test_cloudfront_dist_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_distributions.py` & `moto-4.1.9.dev6/tests/test_cloudfront/test_cloudfront_distributions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudfront/test_cloudfront_invalidation.py` & `moto-4.1.9.dev6/tests/test_cloudfront/test_cloudfront_invalidation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail.py` & `moto-4.1.9.dev6/tests/test_cloudtrail/test_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail_eventselectors.py` & `moto-4.1.9.dev6/tests/test_cloudtrail/test_cloudtrail_eventselectors.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudtrail/test_cloudtrail_tags.py` & `moto-4.1.9.dev6/tests/test_cloudtrail/test_cloudtrail_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudtrail/test_server.py` & `moto-4.1.9.dev6/tests/test_cloudtrail/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_alarms.py` & `moto-4.1.9.dev6/tests/test_cloudwatch/test_cloudwatch_alarms.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_boto3.py` & `moto-4.1.9.dev6/tests/test_cloudwatch/test_cloudwatch_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_dashboards.py` & `moto-4.1.9.dev6/tests/test_cloudwatch/test_cloudwatch_dashboards.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cloudwatch/test_cloudwatch_tags.py` & `moto-4.1.9.dev6/tests/test_cloudwatch/test_cloudwatch_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_codebuild/test_codebuild.py` & `moto-4.1.9.dev6/tests/test_codebuild/test_codebuild.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_codecommit/test_codecommit.py` & `moto-4.1.9.dev6/tests/test_codecommit/test_codecommit.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_codepipeline/test_codepipeline.py` & `moto-4.1.9.dev6/tests/test_codepipeline/test_codepipeline.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cognitoidentity/test_cognitoidentity.py` & `moto-4.1.9.dev6/tests/test_cognitoidentity/test_cognitoidentity.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cognitoidentity/test_server.py` & `moto-4.1.9.dev6/tests/test_cognitoidentity/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp.py` & `moto-4.1.9.dev6/tests/test_cognitoidp/test_cognitoidp.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp_exceptions.py` & `moto-4.1.9.dev6/tests/test_cognitoidp/test_cognitoidp_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cognitoidp/test_cognitoidp_replay.py` & `moto-4.1.9.dev6/tests/test_cognitoidp/test_cognitoidp_replay.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_cognitoidp/test_server.py` & `moto-4.1.9.dev6/tests/test_cognitoidp/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_comprehend/test_comprehend.py` & `moto-4.1.9.dev6/tests/test_comprehend/test_comprehend.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_config/test_config.py` & `moto-4.1.9.dev6/tests/test_config/test_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_config/test_config_rules.py` & `moto-4.1.9.dev6/tests/test_config/test_config_rules.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_config/test_config_rules_integration.py` & `moto-4.1.9.dev6/tests/test_config/test_config_rules_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_config/test_config_tags.py` & `moto-4.1.9.dev6/tests/test_config/test_config_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_account_id_resolution.py` & `moto-4.1.9.dev6/tests/test_core/test_account_id_resolution.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_auth.py` & `moto-4.1.9.dev6/tests/test_core/test_auth.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_backenddict.py` & `moto-4.1.9.dev6/tests/test_core/test_backenddict.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_decorator_calls.py` & `moto-4.1.9.dev6/tests/test_core/test_decorator_calls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_docker.py` & `moto-4.1.9.dev6/tests/test_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_environ_patching.py` & `moto-4.1.9.dev6/tests/test_core/test_environ_patching.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_importorder.py` & `moto-4.1.9.dev6/tests/test_core/test_importorder.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_instance_metadata.py` & `moto-4.1.9.dev6/tests/test_core/test_instance_metadata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_mock_all.py` & `moto-4.1.9.dev6/tests/test_core/test_mock_all.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_mock_regions.py` & `moto-4.1.9.dev6/tests/test_core/test_mock_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_moto_api.py` & `moto-4.1.9.dev6/tests/test_core/test_moto_api.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_nested.py` & `moto-4.1.9.dev6/tests/test_core/test_nested.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_request_mocking.py` & `moto-4.1.9.dev6/tests/test_core/test_request_mocking.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_responses.py` & `moto-4.1.9.dev6/tests/test_core/test_responses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_responses_module.py` & `moto-4.1.9.dev6/tests/test_core/test_responses_module.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_server.py` & `moto-4.1.9.dev6/tests/test_core/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_settings.py` & `moto-4.1.9.dev6/tests/test_core/test_settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_url_base_regex.py` & `moto-4.1.9.dev6/tests/test_core/test_url_base_regex.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_url_mapping.py` & `moto-4.1.9.dev6/tests/test_core/test_url_mapping.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_core/test_utils.py` & `moto-4.1.9.dev6/tests/test_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_databrew/test_databrew_datasets.py` & `moto-4.1.9.dev6/tests/test_databrew/test_databrew_datasets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_databrew/test_databrew_jobs.py` & `moto-4.1.9.dev6/tests/test_databrew/test_databrew_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_databrew/test_databrew_recipes.py` & `moto-4.1.9.dev6/tests/test_databrew/test_databrew_recipes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_databrew/test_databrew_rulesets.py` & `moto-4.1.9.dev6/tests/test_databrew/test_databrew_rulesets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_datapipeline/test_datapipeline.py` & `moto-4.1.9.dev6/tests/test_datapipeline/test_datapipeline.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_datapipeline/test_datapipeline_cloudformation.py` & `moto-4.1.9.dev6/tests/test_datapipeline/test_datapipeline_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_datapipeline/test_server.py` & `moto-4.1.9.dev6/tests/test_datapipeline/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_datasync/test_datasync.py` & `moto-4.1.9.dev6/tests/test_datasync/test_datasync.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dax/test_dax.py` & `moto-4.1.9.dev6/tests/test_dax/test_dax.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dms/test_dms.py` & `moto-4.1.9.dev6/tests/test_dms/test_dms.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ds/test_ds.py` & `moto-4.1.9.dev6/tests/test_ds/test_ds.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ds/test_ds_ad_connect.py` & `moto-4.1.9.dev6/tests/test_ds/test_ds_ad_connect.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ds/test_ds_microsoft_ad.py` & `moto-4.1.9.dev6/tests/test_ds/test_ds_microsoft_ad.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ds/test_ds_simple_ad_directory.py` & `moto-4.1.9.dev6/tests/test_ds/test_ds_simple_ad_directory.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ds/test_ds_tags.py` & `moto-4.1.9.dev6/tests/test_ds/test_ds_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/conftest.py` & `moto-4.1.9.dev6/tests/test_dynamodb/conftest.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py` & `moto-4.1.9.dev6/tests/test_dynamodb/exceptions/test_dynamodb_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/exceptions/test_key_length_exceptions.py` & `moto-4.1.9.dev6/tests/test_dynamodb/exceptions/test_key_length_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/models/test_key_condition_expression_parser.py` & `moto-4.1.9.dev6/tests/test_dynamodb/models/test_key_condition_expression_parser.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_batch_get_item.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_batch_get_item.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_cloudformation.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_condition_expressions.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_condition_expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_consumedcapacity.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_consumedcapacity.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_create_table.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_create_table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_executor.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_executor.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_expression_tokenizer.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_expressions.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_statements.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_statements.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_table_with_range_key.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_table_with_range_key.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_table_without_range_key.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_table_without_range_key.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_update_expressions.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_update_expressions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_update_table.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_update_table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_dynamodb_validation.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_dynamodb_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb/test_server.py` & `moto-4.1.9.dev6/tests/test_dynamodb/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb_v20111205/test_server.py` & `moto-4.1.9.dev6/tests/test_dynamodb_v20111205/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodb_v20111205/test_servermode.py` & `moto-4.1.9.dev6/tests/test_dynamodb_v20111205/test_servermode.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_dynamodbstreams/test_dynamodbstreams.py` & `moto-4.1.9.dev6/tests/test_dynamodbstreams/test_dynamodbstreams.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ebs/test_ebs.py` & `moto-4.1.9.dev6/tests/test_ebs/test_ebs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_account_attributes.py` & `moto-4.1.9.dev6/tests/test_ec2/test_account_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_amis.py` & `moto-4.1.9.dev6/tests/test_ec2/test_amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_availability_zones_and_regions.py` & `moto-4.1.9.dev6/tests/test_ec2/test_availability_zones_and_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_carrier_gateways.py` & `moto-4.1.9.dev6/tests/test_ec2/test_carrier_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_customer_gateways.py` & `moto-4.1.9.dev6/tests/test_ec2/test_customer_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_dhcp_options.py` & `moto-4.1.9.dev6/tests/test_ec2/test_dhcp_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_ec2_cloudformation.py` & `moto-4.1.9.dev6/tests/test_ec2/test_ec2_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_ec2_integration.py` & `moto-4.1.9.dev6/tests/test_ec2/test_ec2_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_egress_only_igw.py` & `moto-4.1.9.dev6/tests/test_ec2/test_egress_only_igw.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_elastic_block_store.py` & `moto-4.1.9.dev6/tests/test_ec2/test_elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_elastic_ip_addresses.py` & `moto-4.1.9.dev6/tests/test_ec2/test_elastic_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_elastic_network_interfaces.py` & `moto-4.1.9.dev6/tests/test_ec2/test_elastic_network_interfaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_fleets.py` & `moto-4.1.9.dev6/tests/test_ec2/test_fleets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_flow_logs.py` & `moto-4.1.9.dev6/tests/test_ec2/test_flow_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_flow_logs_cloudformation.py` & `moto-4.1.9.dev6/tests/test_ec2/test_flow_logs_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_general.py` & `moto-4.1.9.dev6/tests/test_ec2/test_general.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_hosts.py` & `moto-4.1.9.dev6/tests/test_ec2/test_hosts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_iam_integration.py` & `moto-4.1.9.dev6/tests/test_ec2/test_iam_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_instance_type_offerings.py` & `moto-4.1.9.dev6/tests/test_ec2/test_instance_type_offerings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_instance_types.py` & `moto-4.1.9.dev6/tests/test_ec2/test_instance_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_instances.py` & `moto-4.1.9.dev6/tests/test_ec2/test_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_internet_gateways.py` & `moto-4.1.9.dev6/tests/test_ec2/test_internet_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_key_pairs.py` & `moto-4.1.9.dev6/tests/test_ec2/test_key_pairs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_launch_templates.py` & `moto-4.1.9.dev6/tests/test_ec2/test_launch_templates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_nat_gateway.py` & `moto-4.1.9.dev6/tests/test_ec2/test_nat_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_network_acls.py` & `moto-4.1.9.dev6/tests/test_ec2/test_network_acls.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_prefix_lists.py` & `moto-4.1.9.dev6/tests/test_ec2/test_prefix_lists.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_regions.py` & `moto-4.1.9.dev6/tests/test_ec2/test_regions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_route_tables.py` & `moto-4.1.9.dev6/tests/test_ec2/test_route_tables.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_security_groups.py` & `moto-4.1.9.dev6/tests/test_ec2/test_security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_security_groups_cloudformation.py` & `moto-4.1.9.dev6/tests/test_ec2/test_security_groups_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_server.py` & `moto-4.1.9.dev6/tests/test_ec2/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_settings.py` & `moto-4.1.9.dev6/tests/test_ec2/test_settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_spot_fleet.py` & `moto-4.1.9.dev6/tests/test_ec2/test_spot_fleet.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_spot_instances.py` & `moto-4.1.9.dev6/tests/test_ec2/test_spot_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_subnets.py` & `moto-4.1.9.dev6/tests/test_ec2/test_subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_tags.py` & `moto-4.1.9.dev6/tests/test_ec2/test_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway.py` & `moto-4.1.9.dev6/tests/test_ec2/test_transit_gateway.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway_cloudformation.py` & `moto-4.1.9.dev6/tests/test_ec2/test_transit_gateway_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_transit_gateway_peering_attachments.py` & `moto-4.1.9.dev6/tests/test_ec2/test_transit_gateway_peering_attachments.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_utils.py` & `moto-4.1.9.dev6/tests/test_ec2/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_virtual_private_gateways.py` & `moto-4.1.9.dev6/tests/test_ec2/test_virtual_private_gateways.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_vpc_endpoint_services_integration.py` & `moto-4.1.9.dev6/tests/test_ec2/test_vpc_endpoint_services_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_vpc_peering.py` & `moto-4.1.9.dev6/tests/test_ec2/test_vpc_peering.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_vpc_service_configuration.py` & `moto-4.1.9.dev6/tests/test_ec2/test_vpc_service_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_vpcs.py` & `moto-4.1.9.dev6/tests/test_ec2/test_vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_vpn_connections.py` & `moto-4.1.9.dev6/tests/test_ec2/test_vpn_connections.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2/test_windows.py` & `moto-4.1.9.dev6/tests/test_ec2/test_windows.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py` & `moto-4.1.9.dev6/tests/test_ec2instanceconnect/test_ec2instanceconnect_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecr/test_ecr_boto3.py` & `moto-4.1.9.dev6/tests/test_ecr/test_ecr_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecr/test_ecr_cloudformation.py` & `moto-4.1.9.dev6/tests/test_ecr/test_ecr_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecr/test_ecr_helpers.py` & `moto-4.1.9.dev6/tests/test_ecr/test_ecr_helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecr/test_ecr_policy_validation.py` & `moto-4.1.9.dev6/tests/test_ecr/test_ecr_policy_validation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecs/test_ecs_account_settings.py` & `moto-4.1.9.dev6/tests/test_ecs/test_ecs_account_settings.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecs/test_ecs_boto3.py` & `moto-4.1.9.dev6/tests/test_ecs/test_ecs_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecs/test_ecs_capacity_provider.py` & `moto-4.1.9.dev6/tests/test_ecs/test_ecs_capacity_provider.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecs/test_ecs_cloudformation.py` & `moto-4.1.9.dev6/tests/test_ecs/test_ecs_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecs/test_ecs_efs.py` & `moto-4.1.9.dev6/tests/test_ecs/test_ecs_efs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecs/test_ecs_task_def_tags.py` & `moto-4.1.9.dev6/tests/test_ecs/test_ecs_task_def_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ecs/test_ecs_tasksets.py` & `moto-4.1.9.dev6/tests/test_ecs/test_ecs_tasksets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_efs/test_access_point_tagging.py` & `moto-4.1.9.dev6/tests/test_efs/test_access_point_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_efs/test_access_points.py` & `moto-4.1.9.dev6/tests/test_efs/test_access_points.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_efs/test_file_system.py` & `moto-4.1.9.dev6/tests/test_efs/test_file_system.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_efs/test_filesystem_tagging.py` & `moto-4.1.9.dev6/tests/test_efs/test_filesystem_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_efs/test_lifecycle_config.py` & `moto-4.1.9.dev6/tests/test_efs/test_lifecycle_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_efs/test_mount_target.py` & `moto-4.1.9.dev6/tests/test_efs/test_mount_target.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_efs/test_mount_target_security_groups.py` & `moto-4.1.9.dev6/tests/test_efs/test_mount_target_security_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_efs/test_server.py` & `moto-4.1.9.dev6/tests/test_efs/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_eks/test_eks.py` & `moto-4.1.9.dev6/tests/test_eks/test_eks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_eks/test_eks_constants.py` & `moto-4.1.9.dev6/tests/test_eks/test_eks_constants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_eks/test_eks_ec2.py` & `moto-4.1.9.dev6/tests/test_eks/test_eks_ec2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_eks/test_eks_utils.py` & `moto-4.1.9.dev6/tests/test_eks/test_eks_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_eks/test_server.py` & `moto-4.1.9.dev6/tests/test_eks/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elasticache/test_elasticache.py` & `moto-4.1.9.dev6/tests/test_elasticache/test_elasticache.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elasticbeanstalk/test_eb.py` & `moto-4.1.9.dev6/tests/test_elasticbeanstalk/test_eb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elastictranscoder/test_elastictranscoder.py` & `moto-4.1.9.dev6/tests/test_elastictranscoder/test_elastictranscoder.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elb/test_elb.py` & `moto-4.1.9.dev6/tests/test_elb/test_elb.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elb/test_elb_availabilityzones.py` & `moto-4.1.9.dev6/tests/test_elb/test_elb_availabilityzones.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elb/test_elb_cloudformation.py` & `moto-4.1.9.dev6/tests/test_elb/test_elb_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elb/test_elb_policies.py` & `moto-4.1.9.dev6/tests/test_elb/test_elb_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elb/test_elb_subnets.py` & `moto-4.1.9.dev6/tests/test_elb/test_elb_subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2.py` & `moto-4.1.9.dev6/tests/test_elbv2/test_elbv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_cloudformation.py` & `moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_integration.py` & `moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_rule_tags.py` & `moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_listener_rule_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_rules.py` & `moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_listener_rules.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_listener_tags.py` & `moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_listener_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_set_subnets.py` & `moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_set_subnets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_elbv2/test_elbv2_target_groups.py` & `moto-4.1.9.dev6/tests/test_elbv2/test_elbv2_target_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_emr/test_emr_boto3.py` & `moto-4.1.9.dev6/tests/test_emr/test_emr_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_emr/test_emr_integration.py` & `moto-4.1.9.dev6/tests/test_emr/test_emr_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_emr/test_utils.py` & `moto-4.1.9.dev6/tests/test_emr/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_emrcontainers/test_emrcontainers.py` & `moto-4.1.9.dev6/tests/test_emrcontainers/test_emrcontainers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_emrserverless/test_emrserverless.py` & `moto-4.1.9.dev6/tests/test_emrserverless/test_emrserverless.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_es/test_es.py` & `moto-4.1.9.dev6/tests/test_es/test_es.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_events/test_event_pattern.py` & `moto-4.1.9.dev6/tests/test_events/test_event_pattern.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_events/test_events.py` & `moto-4.1.9.dev6/tests/test_events/test_events.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_events/test_events_cloudformation.py` & `moto-4.1.9.dev6/tests/test_events/test_events_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_events/test_events_integration.py` & `moto-4.1.9.dev6/tests/test_events/test_events_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_events/test_events_lambdatriggers_integration.py` & `moto-4.1.9.dev6/tests/test_events/test_events_lambdatriggers_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_firehose/test_firehose.py` & `moto-4.1.9.dev6/tests/test_firehose/test_firehose.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_firehose/test_firehose_destination_types.py` & `moto-4.1.9.dev6/tests/test_firehose/test_firehose_destination_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_firehose/test_firehose_encryption.py` & `moto-4.1.9.dev6/tests/test_firehose/test_firehose_encryption.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_firehose/test_firehose_put.py` & `moto-4.1.9.dev6/tests/test_firehose/test_firehose_put.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_firehose/test_firehose_tags.py` & `moto-4.1.9.dev6/tests/test_firehose/test_firehose_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_firehose/test_http_destinations.py` & `moto-4.1.9.dev6/tests/test_firehose/test_http_destinations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_forecast/test_forecast.py` & `moto-4.1.9.dev6/tests/test_forecast/test_forecast.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glacier/test_glacier_archives.py` & `moto-4.1.9.dev6/tests/test_glacier/test_glacier_archives.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glacier/test_glacier_jobs.py` & `moto-4.1.9.dev6/tests/test_glacier/test_glacier_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glacier/test_glacier_vaults.py` & `moto-4.1.9.dev6/tests/test_glacier/test_glacier_vaults.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glue/fixtures/datacatalog.py` & `moto-4.1.9.dev6/tests/test_glue/fixtures/datacatalog.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glue/fixtures/schema_registry.py` & `moto-4.1.9.dev6/tests/test_glue/fixtures/schema_registry.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glue/helpers.py` & `moto-4.1.9.dev6/tests/test_glue/helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glue/test_datacatalog.py` & `moto-4.1.9.dev6/tests/test_glue/test_datacatalog.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glue/test_glue.py` & `moto-4.1.9.dev6/tests/test_glue/test_glue.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glue/test_glue_job_runs.py` & `moto-4.1.9.dev6/tests/test_glue/test_glue_job_runs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glue/test_partition_filter.py` & `moto-4.1.9.dev6/tests/test_glue/test_partition_filter.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_glue/test_schema_registry.py` & `moto-4.1.9.dev6/tests/test_glue/test_schema_registry.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_core.py` & `moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_core.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_deployment.py` & `moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_deployment.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_device.py` & `moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_device.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_functions.py` & `moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_functions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_groups.py` & `moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_resource.py` & `moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_resource.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_greengrass/test_greengrass_subscriptions.py` & `moto-4.1.9.dev6/tests/test_greengrass/test_greengrass_subscriptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_guardduty/test_guardduty.py` & `moto-4.1.9.dev6/tests/test_guardduty/test_guardduty.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_guardduty/test_guardduty_filters.py` & `moto-4.1.9.dev6/tests/test_guardduty/test_guardduty_filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_guardduty/test_guardduty_organization.py` & `moto-4.1.9.dev6/tests/test_guardduty/test_guardduty_organization.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_iam.py` & `moto-4.1.9.dev6/tests/test_iam/test_iam.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_iam_access_integration.py` & `moto-4.1.9.dev6/tests/test_iam/test_iam_access_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_iam_account_aliases.py` & `moto-4.1.9.dev6/tests/test_iam/test_iam_account_aliases.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_iam_cloudformation.py` & `moto-4.1.9.dev6/tests/test_iam/test_iam_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_iam_groups.py` & `moto-4.1.9.dev6/tests/test_iam/test_iam_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_iam_oidc.py` & `moto-4.1.9.dev6/tests/test_iam/test_iam_oidc.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_iam_password_last_used.py` & `moto-4.1.9.dev6/tests/test_iam/test_iam_password_last_used.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_iam_policies.py` & `moto-4.1.9.dev6/tests/test_iam/test_iam_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_iam_server_certificates.py` & `moto-4.1.9.dev6/tests/test_iam/test_iam_server_certificates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iam/test_server.py` & `moto-4.1.9.dev6/tests/test_iam/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_identitystore/test_identitystore.py` & `moto-4.1.9.dev6/tests/test_identitystore/test_identitystore.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_ca_certificates.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_ca_certificates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_certificates.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_certificates.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_deprecate_thing_type.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_deprecate_thing_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_domain_configuration.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_domain_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_job_executions.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_job_executions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_jobs.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_jobs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_policies.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_policies.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_search.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_search.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_thing_groups.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_thing_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_thing_types.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_thing_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_things.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_things.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_iot_topic_rules.py` & `moto-4.1.9.dev6/tests/test_iot/test_iot_topic_rules.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iot/test_server.py` & `moto-4.1.9.dev6/tests/test_iot/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iotdata/test_iotdata.py` & `moto-4.1.9.dev6/tests/test_iotdata/test_iotdata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_iotdata/test_server.py` & `moto-4.1.9.dev6/tests/test_iotdata/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis.py` & `moto-4.1.9.dev6/tests/test_kinesis/test_kinesis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_boto3.py` & `moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_cloudformation.py` & `moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_encryption.py` & `moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_encryption.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_monitoring.py` & `moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_monitoring.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_stream_consumers.py` & `moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_stream_consumers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kinesis/test_kinesis_stream_limits.py` & `moto-4.1.9.dev6/tests/test_kinesis/test_kinesis_stream_limits.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kinesisvideo/test_kinesisvideo.py` & `moto-4.1.9.dev6/tests/test_kinesisvideo/test_kinesisvideo.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py` & `moto-4.1.9.dev6/tests/test_kinesisvideoarchivedmedia/test_kinesisvideoarchivedmedia.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kms/test_kms_boto3.py` & `moto-4.1.9.dev6/tests/test_kms/test_kms_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kms/test_kms_encrypt.py` & `moto-4.1.9.dev6/tests/test_kms/test_kms_encrypt.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kms/test_kms_grants.py` & `moto-4.1.9.dev6/tests/test_kms/test_kms_grants.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kms/test_kms_policy_enforcement.py` & `moto-4.1.9.dev6/tests/test_kms/test_kms_policy_enforcement.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kms/test_model.py` & `moto-4.1.9.dev6/tests/test_kms/test_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_kms/test_utils.py` & `moto-4.1.9.dev6/tests/test_kms/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_lakeformation/test_lakeformation.py` & `moto-4.1.9.dev6/tests/test_lakeformation/test_lakeformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_logs/test_integration.py` & `moto-4.1.9.dev6/tests/test_logs/test_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_logs/test_logs.py` & `moto-4.1.9.dev6/tests/test_logs/test_logs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_logs/test_logs_filter.py` & `moto-4.1.9.dev6/tests/test_logs/test_logs_filter.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_logs/test_models.py` & `moto-4.1.9.dev6/tests/test_logs/test_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_managedblockchain/helpers.py` & `moto-4.1.9.dev6/tests/test_managedblockchain/helpers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_invitations.py` & `moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_invitations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_members.py` & `moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_members.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_networks.py` & `moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_networks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_nodes.py` & `moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_nodes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_proposals.py` & `moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_proposals.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py` & `moto-4.1.9.dev6/tests/test_managedblockchain/test_managedblockchain_proposalvotes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_mediaconnect/test_mediaconnect.py` & `moto-4.1.9.dev6/tests/test_mediaconnect/test_mediaconnect.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_medialive/test_medialive.py` & `moto-4.1.9.dev6/tests/test_medialive/test_medialive.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_medialive/test_server.py` & `moto-4.1.9.dev6/tests/test_medialive/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_mediapackage/test_mediapackage.py` & `moto-4.1.9.dev6/tests/test_mediapackage/test_mediapackage.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_mediapackage/test_server.py` & `moto-4.1.9.dev6/tests/test_mediapackage/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_mediastore/test_mediastore.py` & `moto-4.1.9.dev6/tests/test_mediastore/test_mediastore.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_mediastoredata/test_mediastoredata.py` & `moto-4.1.9.dev6/tests/test_mediastoredata/test_mediastoredata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_meteringmarketplace/test_meteringmarketplace.py` & `moto-4.1.9.dev6/tests/test_meteringmarketplace/test_meteringmarketplace.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_moto_api/mock_random/test_mock_random.py` & `moto-4.1.9.dev6/tests/test_moto_api/mock_random/test_mock_random.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_moto_api/recorder/test_recorder.py` & `moto-4.1.9.dev6/tests/test_moto_api/recorder/test_recorder.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py` & `moto-4.1.9.dev6/tests/test_moto_api/state_manager/servermode/test_inmemory_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_moto_api/state_manager/servermode/test_state_manager.py` & `moto-4.1.9.dev6/tests/test_moto_api/state_manager/servermode/test_state_manager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_batch_integration.py` & `moto-4.1.9.dev6/tests/test_moto_api/state_manager/test_batch_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_managed_state_model.py` & `moto-4.1.9.dev6/tests/test_moto_api/state_manager/test_managed_state_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_moto_api/state_manager/test_state_manager.py` & `moto-4.1.9.dev6/tests/test_moto_api/state_manager/test_state_manager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_mq/test_mq.py` & `moto-4.1.9.dev6/tests/test_mq/test_mq.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_mq/test_mq_configuration.py` & `moto-4.1.9.dev6/tests/test_mq/test_mq_configuration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_mq/test_mq_tags.py` & `moto-4.1.9.dev6/tests/test_mq/test_mq_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_mq/test_mq_users.py` & `moto-4.1.9.dev6/tests/test_mq/test_mq_users.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_neptune/test_cluster_options.py` & `moto-4.1.9.dev6/tests/test_neptune/test_cluster_options.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_neptune/test_cluster_tags.py` & `moto-4.1.9.dev6/tests/test_neptune/test_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_neptune/test_clusters.py` & `moto-4.1.9.dev6/tests/test_neptune/test_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_neptune/test_global_clusters.py` & `moto-4.1.9.dev6/tests/test_neptune/test_global_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_opensearch/test_domain_tags.py` & `moto-4.1.9.dev6/tests/test_opensearch/test_domain_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_opensearch/test_opensearch.py` & `moto-4.1.9.dev6/tests/test_opensearch/test_opensearch.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_opsworks/test_apps.py` & `moto-4.1.9.dev6/tests/test_opsworks/test_apps.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_opsworks/test_instances.py` & `moto-4.1.9.dev6/tests/test_opsworks/test_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_opsworks/test_layers.py` & `moto-4.1.9.dev6/tests/test_opsworks/test_layers.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_opsworks/test_stack.py` & `moto-4.1.9.dev6/tests/test_opsworks/test_stack.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_organizations/organizations_test_utils.py` & `moto-4.1.9.dev6/tests/test_organizations/organizations_test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_organizations/test_organizations_boto3.py` & `moto-4.1.9.dev6/tests/test_organizations/test_organizations_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_personalize/test_personalize_schema.py` & `moto-4.1.9.dev6/tests/test_personalize/test_personalize_schema.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint.py` & `moto-4.1.9.dev6/tests/test_pinpoint/test_pinpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint_application_tags.py` & `moto-4.1.9.dev6/tests/test_pinpoint/test_pinpoint_application_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_pinpoint/test_pinpoint_event_stream.py` & `moto-4.1.9.dev6/tests/test_pinpoint/test_pinpoint_event_stream.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_polly/test_polly.py` & `moto-4.1.9.dev6/tests/test_polly/test_polly.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_datasets.py` & `moto-4.1.9.dev6/tests/test_quicksight/test_quicksight_datasets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_groups.py` & `moto-4.1.9.dev6/tests/test_quicksight/test_quicksight_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_quicksight/test_quicksight_users.py` & `moto-4.1.9.dev6/tests/test_quicksight/test_quicksight_users.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ram/test_ram.py` & `moto-4.1.9.dev6/tests/test_ram/test_ram.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_db_cluster_param_group.py` & `moto-4.1.9.dev6/tests/test_rds/test_db_cluster_param_group.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_filters.py` & `moto-4.1.9.dev6/tests/test_rds/test_filters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_global_clusters.py` & `moto-4.1.9.dev6/tests/test_rds/test_global_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_rds.py` & `moto-4.1.9.dev6/tests/test_rds/test_rds.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_rds_cloudformation.py` & `moto-4.1.9.dev6/tests/test_rds/test_rds_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_rds_clusters.py` & `moto-4.1.9.dev6/tests/test_rds/test_rds_clusters.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_rds_clusters_with_instances.py` & `moto-4.1.9.dev6/tests/test_rds/test_rds_clusters_with_instances.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_rds_event_subscriptions.py` & `moto-4.1.9.dev6/tests/test_rds/test_rds_event_subscriptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_rds_export_tasks.py` & `moto-4.1.9.dev6/tests/test_rds/test_rds_export_tasks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_server.py` & `moto-4.1.9.dev6/tests/test_rds/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rds/test_utils.py` & `moto-4.1.9.dev6/tests/test_rds/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rdsdata/test_rdsdata.py` & `moto-4.1.9.dev6/tests/test_rdsdata/test_rdsdata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_redshift/test_redshift.py` & `moto-4.1.9.dev6/tests/test_redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_redshift/test_redshift_cloudformation.py` & `moto-4.1.9.dev6/tests/test_redshift/test_redshift_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_redshift/test_server.py` & `moto-4.1.9.dev6/tests/test_redshift/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_redshiftdata/test_redshiftdata.py` & `moto-4.1.9.dev6/tests/test_redshiftdata/test_redshiftdata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_redshiftdata/test_server.py` & `moto-4.1.9.dev6/tests/test_redshiftdata/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_rekognition/test_rekognition.py` & `moto-4.1.9.dev6/tests/test_rekognition/test_rekognition.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_resourcegroups/test_resourcegroups.py` & `moto-4.1.9.dev6/tests/test_resourcegroups/test_resourcegroups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py` & `moto-4.1.9.dev6/tests/test_resourcegroupstaggingapi/test_resourcegroupstaggingapi.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_resourcegroupstaggingapi/test_server.py` & `moto-4.1.9.dev6/tests/test_resourcegroupstaggingapi/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53/test_change_set_model.py` & `moto-4.1.9.dev6/tests/test_route53/test_change_set_model.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53/test_route53.py` & `moto-4.1.9.dev6/tests/test_route53/test_route53.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53/test_route53_cloudformation.py` & `moto-4.1.9.dev6/tests/test_route53/test_route53_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53/test_route53_delegationsets.py` & `moto-4.1.9.dev6/tests/test_route53/test_route53_delegationsets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53/test_route53_healthchecks.py` & `moto-4.1.9.dev6/tests/test_route53/test_route53_healthchecks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53/test_route53_query_logging_config.py` & `moto-4.1.9.dev6/tests/test_route53/test_route53_query_logging_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53/test_route53_vpcs.py` & `moto-4.1.9.dev6/tests/test_route53/test_route53_vpcs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53/test_server.py` & `moto-4.1.9.dev6/tests/test_route53/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_endpoint.py` & `moto-4.1.9.dev6/tests/test_route53resolver/test_route53resolver_endpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_rule.py` & `moto-4.1.9.dev6/tests/test_route53resolver/test_route53resolver_rule.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_rule_associations.py` & `moto-4.1.9.dev6/tests/test_route53resolver/test_route53resolver_rule_associations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_route53resolver/test_route53resolver_tags.py` & `moto-4.1.9.dev6/tests/test_route53resolver/test_route53resolver_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_multiple_accounts_server.py` & `moto-4.1.9.dev6/tests/test_s3/test_multiple_accounts_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_acl.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_acl.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_auth.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_auth.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_bucket_policy.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_classdecorator.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_classdecorator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_cloudformation.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_config.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_config.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_copyobject.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_copyobject.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_custom_endpoint.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_custom_endpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_encryption.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_encryption.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_file_handles.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_file_handles.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_lambda_integration.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_lambda_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_lifecycle.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_lifecycle.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_lock.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_lock.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_logging.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_logging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_metadata.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_metadata.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_multipart.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_multipart.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_object_attributes.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_object_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_ownership.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_ownership.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_replication.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_replication.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_select.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_select.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_storageclass.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_storageclass.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_tagging.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_s3_utils.py` & `moto-4.1.9.dev6/tests/test_s3/test_s3_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3/test_server.py` & `moto-4.1.9.dev6/tests/test_s3/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3bucket_path/test_server.py` & `moto-4.1.9.dev6/tests/test_s3bucket_path/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3control/test_s3control.py` & `moto-4.1.9.dev6/tests/test_s3control/test_s3control.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3control/test_s3control_access_points.py` & `moto-4.1.9.dev6/tests/test_s3control/test_s3control_access_points.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3control/test_s3control_accesspoint_policy.py` & `moto-4.1.9.dev6/tests/test_s3control/test_s3control_accesspoint_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3control/test_s3control_config_integration.py` & `moto-4.1.9.dev6/tests/test_s3control/test_s3control_config_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_s3control/test_s3control_s3.py` & `moto-4.1.9.dev6/tests/test_s3control/test_s3control_s3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/cloudformation_test_configs.py` & `moto-4.1.9.dev6/tests/test_sagemaker/cloudformation_test_configs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_cloudformation.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_endpoint.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_experiment.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_experiment.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_models.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_models.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_notebooks.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_notebooks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_pipeline.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_pipeline.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_processing.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_processing.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_search.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_search.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_training.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_training.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_trial.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_trial.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sagemaker/test_sagemaker_trial_component.py` & `moto-4.1.9.dev6/tests/test_sagemaker/test_sagemaker_trial_component.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_scheduler/test_schedule_groups.py` & `moto-4.1.9.dev6/tests/test_scheduler/test_schedule_groups.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_scheduler/test_scheduler.py` & `moto-4.1.9.dev6/tests/test_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_scheduler/test_scheduler_tags.py` & `moto-4.1.9.dev6/tests/test_scheduler/test_scheduler_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sdb/test_sdb_attributes.py` & `moto-4.1.9.dev6/tests/test_sdb/test_sdb_attributes.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sdb/test_sdb_domains.py` & `moto-4.1.9.dev6/tests/test_sdb/test_sdb_domains.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_secretsmanager/test_list_secrets.py` & `moto-4.1.9.dev6/tests/test_secretsmanager/test_list_secrets.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_secretsmanager/test_policy.py` & `moto-4.1.9.dev6/tests/test_secretsmanager/test_policy.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_secretsmanager/test_secretsmanager.py` & `moto-4.1.9.dev6/tests/test_secretsmanager/test_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_secretsmanager/test_server.py` & `moto-4.1.9.dev6/tests/test_secretsmanager/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py` & `moto-4.1.9.dev6/tests/test_servicediscovery/test_servicediscovery_httpnamespaces.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_operations.py` & `moto-4.1.9.dev6/tests/test_servicediscovery/test_servicediscovery_operations.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_service.py` & `moto-4.1.9.dev6/tests/test_servicediscovery/test_servicediscovery_service.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_servicediscovery/test_servicediscovery_tags.py` & `moto-4.1.9.dev6/tests/test_servicediscovery/test_servicediscovery_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_servicequotas/test_servicequotas.py` & `moto-4.1.9.dev6/tests/test_servicequotas/test_servicequotas.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ses/test_server.py` & `moto-4.1.9.dev6/tests/test_ses/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ses/test_ses_boto3.py` & `moto-4.1.9.dev6/tests/test_ses/test_ses_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ses/test_ses_sns_boto3.py` & `moto-4.1.9.dev6/tests/test_ses/test_ses_sns_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ses/test_templating.py` & `moto-4.1.9.dev6/tests/test_ses/test_templating.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_signer/test_signing_platforms.py` & `moto-4.1.9.dev6/tests/test_signer/test_signing_platforms.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_signer/test_signing_profiles.py` & `moto-4.1.9.dev6/tests/test_signer/test_signing_profiles.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sns/test_application_boto3.py` & `moto-4.1.9.dev6/tests/test_sns/test_application_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sns/test_publish_batch.py` & `moto-4.1.9.dev6/tests/test_sns/test_publish_batch.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sns/test_publishing_boto3.py` & `moto-4.1.9.dev6/tests/test_sns/test_publishing_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sns/test_server.py` & `moto-4.1.9.dev6/tests/test_sns/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sns/test_sns_cloudformation.py` & `moto-4.1.9.dev6/tests/test_sns/test_sns_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sns/test_subscriptions_boto3.py` & `moto-4.1.9.dev6/tests/test_sns/test_subscriptions_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sns/test_topics_boto3.py` & `moto-4.1.9.dev6/tests/test_sns/test_topics_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_special_cases/test_custom_amis.py` & `moto-4.1.9.dev6/tests/test_special_cases/test_custom_amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sqs/test_server.py` & `moto-4.1.9.dev6/tests/test_sqs/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sqs/test_sqs.py` & `moto-4.1.9.dev6/tests/test_sqs/test_sqs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sqs/test_sqs_cloudformation.py` & `moto-4.1.9.dev6/tests/test_sqs/test_sqs_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sqs/test_sqs_integration.py` & `moto-4.1.9.dev6/tests/test_sqs/test_sqs_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sqs/test_sqs_multiaccount.py` & `moto-4.1.9.dev6/tests/test_sqs/test_sqs_multiaccount.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_boto3.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_cloudformation.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_default_amis.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_default_amis.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_defaults.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_defaults.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_doc_permissions.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_doc_permissions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_docs.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_docs.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_ecs_images.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_ecs_images.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_maintenance_windows.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_maintenance_windows.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_parameterstore.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_parameterstore.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_secretsmanager.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_ssm_utils.py` & `moto-4.1.9.dev6/tests/test_ssm/test_ssm_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssm/test_templates/good.yaml` & `moto-4.1.9.dev6/tests/test_ssm/test_templates/good.yaml`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssoadmin/test_server.py` & `moto-4.1.9.dev6/tests/test_ssoadmin/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_ssoadmin/test_ssoadmin.py` & `moto-4.1.9.dev6/tests/test_ssoadmin/test_ssoadmin.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_stepfunctions/test_stepfunctions.py` & `moto-4.1.9.dev6/tests/test_stepfunctions/test_stepfunctions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_stepfunctions/test_stepfunctions_cloudformation.py` & `moto-4.1.9.dev6/tests/test_stepfunctions/test_stepfunctions_cloudformation.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sts/test_server.py` & `moto-4.1.9.dev6/tests/test_sts/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sts/test_sts.py` & `moto-4.1.9.dev6/tests/test_sts/test_sts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_sts/test_sts_integration.py` & `moto-4.1.9.dev6/tests/test_sts/test_sts_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_support/test_server.py` & `moto-4.1.9.dev6/tests/test_support/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_support/test_support.py` & `moto-4.1.9.dev6/tests/test_support/test_support.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/models/test_activity_task.py` & `moto-4.1.9.dev6/tests/test_swf/models/test_activity_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/models/test_decision_task.py` & `moto-4.1.9.dev6/tests/test_swf/models/test_decision_task.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/models/test_domain.py` & `moto-4.1.9.dev6/tests/test_swf/models/test_domain.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/models/test_generic_type.py` & `moto-4.1.9.dev6/tests/test_swf/models/test_generic_type.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/models/test_history_event.py` & `moto-4.1.9.dev6/tests/test_swf/models/test_history_event.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/models/test_timeout.py` & `moto-4.1.9.dev6/tests/test_swf/models/test_timeout.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/models/test_timer.py` & `moto-4.1.9.dev6/tests/test_swf/models/test_timer.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/models/test_workflow_execution.py` & `moto-4.1.9.dev6/tests/test_swf/models/test_workflow_execution.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/responses/test_activity_tasks.py` & `moto-4.1.9.dev6/tests/test_swf/responses/test_activity_tasks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/responses/test_activity_types.py` & `moto-4.1.9.dev6/tests/test_swf/responses/test_activity_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/responses/test_decision_tasks.py` & `moto-4.1.9.dev6/tests/test_swf/responses/test_decision_tasks.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/responses/test_domains.py` & `moto-4.1.9.dev6/tests/test_swf/responses/test_domains.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/responses/test_timeouts.py` & `moto-4.1.9.dev6/tests/test_swf/responses/test_timeouts.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/responses/test_workflow_executions.py` & `moto-4.1.9.dev6/tests/test_swf/responses/test_workflow_executions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/responses/test_workflow_types.py` & `moto-4.1.9.dev6/tests/test_swf/responses/test_workflow_types.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/test_exceptions.py` & `moto-4.1.9.dev6/tests/test_swf/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_swf/utils.py` & `moto-4.1.9.dev6/tests/test_swf/utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_textract/test_server.py` & `moto-4.1.9.dev6/tests/test_textract/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_textract/test_textract.py` & `moto-4.1.9.dev6/tests/test_textract/test_textract.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_timestreamwrite/test_server.py` & `moto-4.1.9.dev6/tests/test_timestreamwrite/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_database.py` & `moto-4.1.9.dev6/tests/test_timestreamwrite/test_timestreamwrite_database.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_table.py` & `moto-4.1.9.dev6/tests/test_timestreamwrite/test_timestreamwrite_table.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_timestreamwrite/test_timestreamwrite_tagging.py` & `moto-4.1.9.dev6/tests/test_timestreamwrite/test_timestreamwrite_tagging.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_transcribe/test_transcribe_boto3.py` & `moto-4.1.9.dev6/tests/test_transcribe/test_transcribe_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_utilities/test_docker_utilities.py` & `moto-4.1.9.dev6/tests/test_utilities/test_docker_utilities.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_utilities/test_paginator.py` & `moto-4.1.9.dev6/tests/test_utilities/test_paginator.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_utilities/test_tagging_service.py` & `moto-4.1.9.dev6/tests/test_utilities/test_tagging_service.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_utilities/test_threaded_server.py` & `moto-4.1.9.dev6/tests/test_utilities/test_threaded_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_wafv2/test_server.py` & `moto-4.1.9.dev6/tests/test_wafv2/test_server.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_wafv2/test_utils.py` & `moto-4.1.9.dev6/tests/test_wafv2/test_utils.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_wafv2/test_wafv2.py` & `moto-4.1.9.dev6/tests/test_wafv2/test_wafv2.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_integration.py` & `moto-4.1.9.dev6/tests/test_wafv2/test_wafv2_integration.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_wafv2/test_wafv2_tags.py` & `moto-4.1.9.dev6/tests/test_wafv2/test_wafv2_tags.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_xray/test_xray_boto3.py` & `moto-4.1.9.dev6/tests/test_xray/test_xray_boto3.py`

 * *Files identical despite different names*

### Comparing `moto-4.1.9.dev5/tests/test_xray/test_xray_client.py` & `moto-4.1.9.dev6/tests/test_xray/test_xray_client.py`

 * *Files identical despite different names*

