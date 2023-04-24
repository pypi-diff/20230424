# Comparing `tmp/apache-airflow-providers-amazon-8.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-amazon-8.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-amazon-8.0.0rc1.tar", last modified: Fri Apr 21 19:47:52 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-amazon-8.0.0rc2.tar", last modified: Mon Apr 24 21:39:43 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.0.0rc1.tar` & `apache-airflow-providers-amazon-8.0.0rc2.tar`

### file list

```diff
@@ -1,168 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-04-21 19:47:47.000000 apache-airflow-providers-amazon-8.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    56663 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    54842 2023-04-21 19:47:47.000000 apache-airflow-providers-amazon-8.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12240 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    42181 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    20629 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)     9644 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7641 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    18990 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    13816 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     4823 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13108 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    42450 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)    15828 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    29018 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    31753 2023-04-14 11:39:41.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    49023 2023-04-20 13:52:20.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    29868 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    28218 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5559 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    49835 2023-03-01 07:06:45.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15533 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    18505 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2768 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     5857 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     7676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5863 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8475 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:51.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20348 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)     1378 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)    36826 2023-04-21 19:47:47.000000 apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    56663 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7207 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      777 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:47:50.000000 apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-amazon-8.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-04-21 19:47:52.000000 apache-airflow-providers-amazon-8.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2356 2023-04-21 19:47:47.000000 apache-airflow-providers-amazon-8.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-04-24 21:39:38.000000 apache-airflow-providers-amazon-8.0.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    57034 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    55213 2023-04-24 21:39:38.000000 apache-airflow-providers-amazon-8.0.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12240 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    45421 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    20629 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)     9697 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7641 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    20348 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    13816 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13108 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    42450 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    15828 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    29018 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    31753 2023-04-14 11:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    50180 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    29868 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    28991 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    49835 2023-03-01 07:06:45.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15533 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    18505 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     7676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8475 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20348 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/waiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      430 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)    36867 2023-04-24 21:39:38.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    57034 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7264 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      803 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-amazon-8.0.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-04-24 21:39:37.000000 apache-airflow-providers-amazon-8.0.0rc2/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/LICENSE` & `apache-airflow-providers-amazon-8.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/MANIFEST.in` & `apache-airflow-providers-amazon-8.0.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/PKG-INFO` & `apache-airflow-providers-amazon-8.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.0.0rc1
+Version: 8.0.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
@@ -60,15 +60,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.0.0rc1``
+Release: ``8.0.0rc2``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
@@ -102,14 +102,15 @@
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
 ``mypy-boto3-appflow``                   ``>=1.24.0``
+``aiobotocore[boto3]``                   ``>=2.2.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -172,16 +173,14 @@
   In this version of the provider, deprecated GCS hook's parameter ``delegate_to`` is removed from the following operators: ``GCSToS3Operator``, ``GlacierToGCSOperator`` and ``GoogleApiToS3Operator``.
   Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
 
   Removed deprecated parameter ``google_cloud_storage_conn_id`` from ``GCSToS3Operator``, ``gcp_conn_id`` should be used instead.
 
   Removed deprecated parameter ``max_tries`` from the Athena & EMR hook & operators in favor of ``max_polling_attempts``.
 
-  Disabled deprecated behavior of switching to an empty aws connection ID on error. You can set it to None explicitly.
-
   Removed deprecated method ``waiter`` from emr hook in favor of the more generic ``airflow.providers.amazon.aws.utils.waiter.waiter``
 
   Removed deprecated unused parameter ``cluster_identifier`` from Redshift Cluster's hook method ``get_cluster_snapshot_status``
 
   Removed deprecated method ``find_processing_job_by_name`` from Sagemaker hook, use ``count_processing_jobs_by_name`` instead.
 
   Removed deprecated module ``airflow.providers.amazon.aws.operators.aws_lambda`` in favor of ``airflow.providers.amazon.aws.operators.lambda_function``
@@ -207,14 +206,16 @@
 
 Features
 ~~~~~~~~
 
 * ``add a stop operator to emr serverless (#30720)``
 * ``SqlToS3Operator - Add feature to partition SQL table (#30460)``
 * ``New AWS sensor — DynamoDBValueSensor (#28338)``
+* ``Add a "force" option to emr serverless stop/delete operator (#30757)``
+* ``Add support for deferrable operators in AMPP (#30032)``
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fixed logging issue (#30703)``
 * ``DynamoDBHook - waiter_path() to consider 'resource_type' or 'client_type' (#30595)``
 * ``Add ability to override waiter delay in EcsRunTaskOperator (#30586)``
@@ -223,18 +224,23 @@
 
 Misc
 ~~~~
 
 * ``Remove @poke_mode_only from EmrStepSensor (#30774)``
 * ``Organize Amazon providers docs index (#30541)``
 * ``Remove duplicate param docstring in EksPodOperator (#30634)``
+* ``Update AWS EMR Cluster Link to use the new dashboard (#30844)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``fixes to system tests following obsolete cleanup (#30804)``
+   * ``restore fallback to empty connection behavior (#30806)``
+   * ``Prepare docs for adhoc release of providers (#30787)``
 
 7.4.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/README.rst` & `apache-airflow-providers-amazon-8.0.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.0.0rc1``
+Release: ``8.0.0rc2``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
@@ -57,14 +57,15 @@
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
 ``mypy-boto3-appflow``                   ``>=1.24.0``
+``aiobotocore[boto3]``                   ``>=2.2.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -127,16 +128,14 @@
   In this version of the provider, deprecated GCS hook's parameter ``delegate_to`` is removed from the following operators: ``GCSToS3Operator``, ``GlacierToGCSOperator`` and ``GoogleApiToS3Operator``.
   Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
 
   Removed deprecated parameter ``google_cloud_storage_conn_id`` from ``GCSToS3Operator``, ``gcp_conn_id`` should be used instead.
 
   Removed deprecated parameter ``max_tries`` from the Athena & EMR hook & operators in favor of ``max_polling_attempts``.
 
-  Disabled deprecated behavior of switching to an empty aws connection ID on error. You can set it to None explicitly.
-
   Removed deprecated method ``waiter`` from emr hook in favor of the more generic ``airflow.providers.amazon.aws.utils.waiter.waiter``
 
   Removed deprecated unused parameter ``cluster_identifier`` from Redshift Cluster's hook method ``get_cluster_snapshot_status``
 
   Removed deprecated method ``find_processing_job_by_name`` from Sagemaker hook, use ``count_processing_jobs_by_name`` instead.
 
   Removed deprecated module ``airflow.providers.amazon.aws.operators.aws_lambda`` in favor of ``airflow.providers.amazon.aws.operators.lambda_function``
@@ -162,14 +161,16 @@
 
 Features
 ~~~~~~~~
 
 * ``add a stop operator to emr serverless (#30720)``
 * ``SqlToS3Operator - Add feature to partition SQL table (#30460)``
 * ``New AWS sensor — DynamoDBValueSensor (#28338)``
+* ``Add a "force" option to emr serverless stop/delete operator (#30757)``
+* ``Add support for deferrable operators in AMPP (#30032)``
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fixed logging issue (#30703)``
 * ``DynamoDBHook - waiter_path() to consider 'resource_type' or 'client_type' (#30595)``
 * ``Add ability to override waiter delay in EcsRunTaskOperator (#30586)``
@@ -178,18 +179,23 @@
 
 Misc
 ~~~~
 
 * ``Remove @poke_mode_only from EmrStepSensor (#30774)``
 * ``Organize Amazon providers docs index (#30541)``
 * ``Remove duplicate param docstring in EksPodOperator (#30634)``
+* ``Update AWS EMR Cluster Link to use the new dashboard (#30844)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``fixes to system tests following obsolete cleanup (#30804)``
+   * ``restore fallback to empty connection behavior (#30806)``
+   * ``Prepare docs for adhoc release of providers (#30787)``
 
 7.4.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,37 +49,40 @@
 from dateutil.tz import tzlocal
 from slugify import slugify
 
 from airflow.compat.functools import cached_property
 from airflow.configuration import conf
 from airflow.exceptions import (
     AirflowException,
+    AirflowNotFoundException,
 )
 from airflow.hooks.base import BaseHook
 from airflow.providers.amazon.aws.utils.connection_wrapper import AwsConnectionWrapper
-from airflow.providers.amazon.aws.waiters.base_waiter import BaseBotoWaiter
 from airflow.providers_manager import ProvidersManager
 from airflow.utils.helpers import exactly_one
 from airflow.utils.log.logging_mixin import LoggingMixin
 from airflow.utils.log.secrets_masker import mask_secret
 
 BaseAwsConnection = TypeVar("BaseAwsConnection", bound=Union[boto3.client, boto3.resource])
 
 if TYPE_CHECKING:
     from airflow.models.connection import Connection  # Avoid circular imports.
 
 
 class BaseSessionFactory(LoggingMixin):
     """
-    Base AWS Session Factory class to handle boto3 session creation.
+    Base AWS Session Factory class to handle synchronous and async boto session creation.
     It can handle most of the AWS supported authentication methods.
 
     User can also derive from this class to have full control of boto3 session
     creation or to support custom federation.
 
+    Note: Not all features implemented for synchronous sessions are available for async
+    sessions.
+
     .. seealso::
         - :ref:`howto/connection:aws:session-factory`
     """
 
     def __init__(
         self,
         conn: Connection | AwsConnectionWrapper | None,
@@ -121,43 +124,82 @@
         return self.conn.botocore_config
 
     @property
     def role_arn(self) -> str | None:
         """Assume Role ARN from AWS Connection"""
         return self.conn.role_arn
 
-    def create_session(self) -> boto3.session.Session:
-        """Create boto3 Session from connection config."""
+    def _apply_session_kwargs(self, session):
+        if self.conn.session_kwargs.get("profile_name", None) is not None:
+            session.set_config_variable("profile", self.conn.session_kwargs["profile_name"])
+
+        if (
+            self.conn.session_kwargs.get("aws_access_key_id", None)
+            or self.conn.session_kwargs.get("aws_secret_access_key", None)
+            or self.conn.session_kwargs.get("aws_session_token", None)
+        ):
+            session.set_credentials(
+                self.conn.session_kwargs["aws_access_key_id"],
+                self.conn.session_kwargs["aws_secret_access_key"],
+                self.conn.session_kwargs["aws_session_token"],
+            )
+
+        if self.conn.session_kwargs.get("region_name", None) is not None:
+            session.set_config_variable("region", self.conn.session_kwargs["region_name"])
+
+    def get_async_session(self):
+        from aiobotocore.session import get_session as async_get_session
+
+        return async_get_session()
+
+    def create_session(self, deferrable: bool = False) -> boto3.session.Session:
+        """Create boto3 or aiobotocore Session from connection config."""
         if not self.conn:
             self.log.info(
                 "No connection ID provided. Fallback on boto3 credential strategy (region_name=%r). "
                 "See: https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html",
                 self.region_name,
             )
-            return boto3.session.Session(region_name=self.region_name)
+            if deferrable:
+                session = self.get_async_session()
+                self._apply_session_kwargs(session)
+                return session
+            else:
+                return boto3.session.Session(region_name=self.region_name)
         elif not self.role_arn:
-            return self.basic_session
+            if deferrable:
+                session = self.get_async_session()
+                self._apply_session_kwargs(session)
+                return session
+            else:
+                return self.basic_session
 
         # Values stored in ``AwsConnectionWrapper.session_kwargs`` are intended to be used only
         # to create the initial boto3 session.
         # If the user wants to use the 'assume_role' mechanism then only the 'region_name' needs to be
         # provided, otherwise other parameters might conflict with the base botocore session.
         # Unfortunately it is not a part of public boto3 API, see source of boto3.session.Session:
         # https://boto3.amazonaws.com/v1/documentation/api/latest/_modules/boto3/session.html#Session
         # If we provide 'aws_access_key_id' or 'aws_secret_access_key' or 'aws_session_token'
         # as part of session kwargs it will use them instead of assumed credentials.
         assume_session_kwargs = {}
         if self.conn.region_name:
             assume_session_kwargs["region_name"] = self.conn.region_name
-        return self._create_session_with_assume_role(session_kwargs=assume_session_kwargs)
+        return self._create_session_with_assume_role(
+            session_kwargs=assume_session_kwargs, deferrable=deferrable
+        )
 
     def _create_basic_session(self, session_kwargs: dict[str, Any]) -> boto3.session.Session:
         return boto3.session.Session(**session_kwargs)
 
-    def _create_session_with_assume_role(self, session_kwargs: dict[str, Any]) -> boto3.session.Session:
+    def _create_session_with_assume_role(
+        self, session_kwargs: dict[str, Any], deferrable: bool = False
+    ) -> boto3.session.Session:
+        from aiobotocore.session import get_session as async_get_session
+
         if self.conn.assume_role_method == "assume_role_with_web_identity":
             # Deferred credentials have no initial credentials
             credential_fetcher = self._get_web_identity_credential_fetcher()
             credentials = botocore.credentials.DeferredRefreshableCredentials(
                 method="assume-role-with-web-identity",
                 refresh_using=credential_fetcher.fetch_credentials,
                 time_fetcher=lambda: datetime.datetime.now(tz=tzlocal()),
@@ -166,18 +208,18 @@
             # Refreshable credentials do have initial credentials
             credentials = botocore.credentials.RefreshableCredentials.create_from_metadata(
                 metadata=self._refresh_credentials(),
                 refresh_using=self._refresh_credentials,
                 method="sts-assume-role",
             )
 
-        session = botocore.session.get_session()
+        session = async_get_session() if deferrable else botocore.session.get_session()
+
         session._credentials = credentials
-        region_name = self.basic_session.region_name
-        session.set_config_variable("region", region_name)
+        session.set_config_variable("region", self.basic_session.region_name)
 
         return boto3.session.Session(botocore_session=session, **session_kwargs)
 
     def _refresh_credentials(self) -> dict[str, Any]:
         self.log.debug("Refreshing credentials")
         assume_role_method = self.conn.assume_role_method
         if assume_role_method not in ("assume_role", "assume_role_with_saml"):
@@ -494,15 +536,20 @@
         return " ".join(user_agent_extra_values).strip()
 
     @cached_property
     def conn_config(self) -> AwsConnectionWrapper:
         """Get the Airflow Connection object and wrap it in helper (cached)."""
         connection = None
         if self.aws_conn_id:
-            connection = self.get_connection(self.aws_conn_id)
+            try:
+                connection = self.get_connection(self.aws_conn_id)
+            except AirflowNotFoundException:
+                self.log.warning(
+                    "Unable to find AWS Connection ID '%s', switching to empty.", self.aws_conn_id
+                )
 
         return AwsConnectionWrapper(
             conn=connection, region_name=self._region_name, botocore_config=self._config, verify=self._verify
         )
 
     @property
     def service_config(self) -> dict:
@@ -520,19 +567,19 @@
         return self.conn_config.botocore_config or botocore.config.Config()
 
     @property
     def verify(self) -> bool | str | None:
         """Verify or not SSL certificates boto3 client/resource read-only property."""
         return self.conn_config.verify
 
-    def get_session(self, region_name: str | None = None) -> boto3.session.Session:
+    def get_session(self, region_name: str | None = None, deferrable: bool = False) -> boto3.session.Session:
         """Get the underlying boto3.session.Session(region_name=region_name)."""
         return SessionFactory(
             conn=self.conn_config, region_name=region_name, config=self.config
-        ).create_session()
+        ).create_session(deferrable=deferrable)
 
     def _get_config(self, config: Config | None = None) -> Config:
         """
         No AWS Operators use the config argument to this method.
         Keep backward compatibility with other users who might use it
         """
         if config is None:
@@ -547,18 +594,27 @@
         )
         return config.merge(user_agent_config)  # type: ignore[union-attr]
 
     def get_client_type(
         self,
         region_name: str | None = None,
         config: Config | None = None,
+        deferrable: bool = False,
     ) -> boto3.client:
         """Get the underlying boto3 client using boto3 session"""
         client_type = self.client_type
-        session = self.get_session(region_name=region_name)
+        session = self.get_session(region_name=region_name, deferrable=deferrable)
+        if not isinstance(session, boto3.session.Session):
+            return session.create_client(
+                client_type,
+                endpoint_url=self.conn_config.endpoint_url,
+                config=self._get_config(config),
+                verify=self.verify,
+            )
+
         return session.client(
             client_type,
             endpoint_url=self.conn_config.endpoint_url,
             config=self._get_config(config),
             verify=self.verify,
         )
 
@@ -590,14 +646,22 @@
                 f"resource_type={self.resource_type!r} must be provided, not both."
             )
         elif self.client_type:
             return self.get_client_type(region_name=self.region_name)
         else:
             return self.get_resource_type(region_name=self.region_name)
 
+    @property
+    def async_conn(self):
+        """Get an aiobotocore client to use for async operations."""
+        if not self.client_type:
+            raise ValueError("client_type must be specified.")
+
+        return self.get_client_type(region_name=self.region_name, deferrable=True)
+
     @cached_property
     def conn_client_meta(self) -> ClientMeta:
         """Get botocore client metadata from Hook connection (cached)."""
         conn = self.conn
         if isinstance(conn, botocore.client.BaseClient):
             return conn.meta
         return conn.meta.client.meta
@@ -743,34 +807,53 @@
 
     @cached_property
     def waiter_path(self) -> PathLike[str] | None:
         filename = self.client_type if self.client_type else self.resource_type
         path = Path(__file__).parents[1].joinpath(f"waiters/{filename}.json").resolve()
         return path if path.exists() else None
 
-    def get_waiter(self, waiter_name: str, parameters: dict[str, str] | None = None) -> Waiter:
+    def get_waiter(
+        self,
+        waiter_name: str,
+        parameters: dict[str, str] | None = None,
+        deferrable: bool = False,
+        client=None,
+    ) -> Waiter:
         """
         First checks if there is a custom waiter with the provided waiter_name and
         uses that if it exists, otherwise it will check the service client for a
         waiter that matches the name and pass that through.
 
+        If `deferrable` is True, the waiter will be an AIOWaiter, generated from the
+        client that is passed as a parameter. If `deferrable` is True, `client` must be
+        provided.
+
         :param waiter_name: The name of the waiter.  The name should exactly match the
             name of the key in the waiter model file (typically this is CamelCase).
         :param parameters: will scan the waiter config for the keys of that dict, and replace them with the
             corresponding value. If a custom waiter has such keys to be expanded, they need to be provided
             here.
+        :param deferrable: If True, the waiter is going to be an async custom waiter.
+
         """
+        from airflow.providers.amazon.aws.waiters.base_waiter import BaseBotoWaiter
+
+        if deferrable and not client:
+            raise ValueError("client must be provided for a deferrable waiter.")
+        client = client or self.conn
         if self.waiter_path and (waiter_name in self._list_custom_waiters()):
             # Technically if waiter_name is in custom_waiters then self.waiter_path must
             # exist but MyPy doesn't like the fact that self.waiter_path could be None.
             with open(self.waiter_path) as config_file:
                 config = json.loads(config_file.read())
 
             config = self._apply_parameters_value(config, waiter_name, parameters)
-            return BaseBotoWaiter(client=self.conn, model_config=config).waiter(waiter_name)
+            return BaseBotoWaiter(client=client, model_config=config, deferrable=deferrable).waiter(
+                waiter_name
+            )
         # If there is no custom waiter found for the provided name,
         # then try checking the service's official waiters.
         return self.conn.get_waiter(waiter_name)
 
     @staticmethod
     def _apply_parameters_value(config: dict, waiter_name: str, parameters: dict[str, str] | None) -> dict:
         """Replaces potential jinja templates in acceptors definition"""
@@ -931,15 +1014,15 @@
                 secret_key=aws_secret_access_key,
                 token=aws_session_token,
             )
         if region_name is not None:
             aio_session.set_config_variable("region", region_name)
         return aio_session
 
-    def create_session(self) -> AioSession:
+    def create_session(self, deferrable: bool = False) -> AioSession:
         """Create aiobotocore Session from connection and config."""
         if not self._conn:
             self.log.info("No connection ID provided. Fallback on boto3 credential strategy")
             return get_session()
         elif not self.role_arn:
             return self._basic_session
         return self._get_session_with_assume_role()
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,17 @@
         """
         A configured waiter model used to generate waiters on AWS Batch services.
 
         :return: a waiter model for AWS Batch services
         """
         return self._waiter_model
 
-    def get_waiter(self, waiter_name: str, _: dict[str, str] | None = None) -> botocore.waiter.Waiter:
+    def get_waiter(
+        self, waiter_name: str, _: dict[str, str] | None = None, deferrable: bool = False, client=None
+    ) -> botocore.waiter.Waiter:
         """
         Get an AWS Batch service waiter, using the configured ``.waiter_model``.
 
         The ``.waiter_model`` is combined with the ``.client`` to get a specific waiter and
         the properties of that waiter can be modified without any accidental impact on the
         generation of new waiters from the ``.waiter_model``, e.g.
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 import json
 import warnings
 from time import sleep
 from typing import Any
 
 from botocore.exceptions import ClientError
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowNotFoundException
 from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
 from airflow.utils.helpers import prune_dict
 
 
 class EmrHook(AwsBaseHook):
     """
@@ -249,18 +248,49 @@
     APPLICATION_FAILURE_STATES = {"STOPPED", "TERMINATED"}
     APPLICATION_SUCCESS_STATES = {"CREATED", "STARTED"}
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         kwargs["client_type"] = "emr-serverless"
         super().__init__(*args, **kwargs)
 
-    @cached_property
-    def conn(self):
-        """Get the underlying boto3 EmrServerlessAPIService client (cached)"""
-        return super().conn
+    def cancel_running_jobs(self, application_id: str, waiter_config: dict = {}):
+        """
+        List all jobs in an intermediate state and cancel them.
+        Then wait for those jobs to reach a terminal state.
+        Note: if new jobs are triggered while this operation is ongoing,
+        it's going to time out and return an error.
+        """
+        paginator = self.conn.get_paginator("list_job_runs")
+        results_per_response = 50
+        iterator = paginator.paginate(
+            applicationId=application_id,
+            states=list(self.JOB_INTERMEDIATE_STATES),
+            PaginationConfig={
+                "PageSize": results_per_response,
+            },
+        )
+        count = 0
+        for r in iterator:
+            job_ids = [jr["id"] for jr in r["jobRuns"]]
+            count += len(job_ids)
+            if len(job_ids) > 0:
+                self.log.info(
+                    "Cancelling %s pending job(s) for the application %s so that it can be stopped",
+                    len(job_ids),
+                    application_id,
+                )
+                for job_id in job_ids:
+                    self.conn.cancel_job_run(applicationId=application_id, jobRunId=job_id)
+        if count > 0:
+            self.log.info("now waiting for the %s cancelled job(s) to terminate", count)
+            self.get_waiter("no_job_running").wait(
+                applicationId=application_id,
+                states=list(self.JOB_INTERMEDIATE_STATES.union({"CANCELLING"})),
+                WaiterConfig=waiter_config,
+            )
 
 
 class EmrContainerHook(AwsBaseHook):
     """
     Interact with Amazon EMR Containers (Amazon EMR on EKS).
     Provide thick wrapper around :py:class:`boto3.client("emr-containers") <EMRContainers.Client>`.
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/emr.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 
 
 class EmrClusterLink(BaseAwsLink):
     """Helper class for constructing AWS EMR Cluster Link"""
 
     name = "EMR Cluster"
     key = "emr_cluster"
-    format_str = (
-        BASE_AWS_CONSOLE_LINK + "/elasticmapreduce/home?region={region_name}#cluster-details:{job_flow_id}"
-    )
+    format_str = BASE_AWS_CONSOLE_LINK + "/emr/home?region={region_name}#/clusterDetails/{job_flow_id}"
 
 
 class EmrLogsLink(BaseAwsLink):
     """Helper class for constructing AWS EMR Logs Link"""
 
     name = "EMR Cluster Logs"
     key = "emr_logs"
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/emr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1021,41 +1021,57 @@
     :param application_id: ID of the EMR Serverless application to stop.
     :param wait_for_completion: If true, wait for the Application to stop before returning. Default to True
     :param aws_conn_id: AWS connection to use
     :param waiter_countdown: Total amount of time, in seconds, the operator will wait for
         the application be stopped. Defaults to 5 minutes.
     :param waiter_check_interval_seconds: Number of seconds between polling the state of the application.
         Defaults to 30 seconds.
+    :param force_stop: If set to True, any job for that app that is not in a terminal state will be cancelled.
+        Otherwise, trying to stop an app with running jobs will return an error.
+        If you want to wait for the jobs to finish gracefully, use
+        :class:`airflow.providers.amazon.aws.sensors.emr.EmrServerlessJobSensor`
     """
 
     template_fields: Sequence[str] = ("application_id",)
 
     def __init__(
         self,
         application_id: str,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
         waiter_countdown: int = 5 * 60,
         waiter_check_interval_seconds: int = 30,
+        force_stop: bool = False,
         **kwargs,
     ):
         self.aws_conn_id = aws_conn_id
         self.application_id = application_id
         self.wait_for_completion = wait_for_completion
         self.waiter_countdown = waiter_countdown
         self.waiter_check_interval_seconds = waiter_check_interval_seconds
+        self.force_stop = force_stop
         super().__init__(**kwargs)
 
     @cached_property
     def hook(self) -> EmrServerlessHook:
         """Create and return an EmrServerlessHook."""
         return EmrServerlessHook(aws_conn_id=self.aws_conn_id)
 
     def execute(self, context: Context) -> None:
         self.log.info("Stopping application: %s", self.application_id)
+
+        if self.force_stop:
+            self.hook.cancel_running_jobs(
+                self.application_id,
+                waiter_config={
+                    "Delay": self.waiter_check_interval_seconds,
+                    "MaxAttempts": self.waiter_countdown / self.waiter_check_interval_seconds,
+                },
+            )
+
         self.hook.conn.stop_application(applicationId=self.application_id)
 
         if self.wait_for_completion:
             # This should be replaced with a boto waiter when available.
             waiter(
                 get_state_callable=self.hook.conn.get_application,
                 get_state_args={
@@ -1084,36 +1100,42 @@
     :param wait_for_completion: If true, wait for the Application to be deleted before returning.
         Defaults to True. Note that this operator will always wait for the application to be STOPPED first.
     :param aws_conn_id: AWS connection to use
     :param waiter_countdown: Total amount of time, in seconds, the operator will wait for each step of first,
         the application to be stopped, and then deleted. Defaults to 25 minutes.
     :param waiter_check_interval_seconds: Number of seconds between polling the state of the application.
         Defaults to 60 seconds.
+    :param force_stop: If set to True, any job for that app that is not in a terminal state will be cancelled.
+        Otherwise, trying to delete an app with running jobs will return an error.
+        If you want to wait for the jobs to finish gracefully, use
+        :class:`airflow.providers.amazon.aws.sensors.emr.EmrServerlessJobSensor`
     """
 
     template_fields: Sequence[str] = ("application_id",)
 
     def __init__(
         self,
         application_id: str,
         wait_for_completion: bool = True,
         aws_conn_id: str = "aws_default",
         waiter_countdown: int = 25 * 60,
         waiter_check_interval_seconds: int = 60,
+        force_stop: bool = False,
         **kwargs,
     ):
         self.wait_for_delete_completion = wait_for_completion
         # super stops the app
         super().__init__(
             application_id=application_id,
             # when deleting an app, we always need to wait for it to stop before we can call delete()
             wait_for_completion=True,
             aws_conn_id=aws_conn_id,
             waiter_countdown=waiter_countdown,
             waiter_check_interval_seconds=waiter_check_interval_seconds,
+            force_stop=force_stop,
             **kwargs,
         )
 
     def execute(self, context: Context) -> None:
         # super stops the app (or makes sure it's already stopped)
         super().execute(context)
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/rds.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         self,
         *,
         db_type: str,
         db_identifier: str,
         db_snapshot_identifier: str,
         tags: Sequence[TagTypeDef] | dict | None = None,
         wait_for_completion: bool = True,
-        aws_conn_id: str = "aws_conn_id",
+        aws_conn_id: str = "aws_default",
         **kwargs,
     ):
         super().__init__(aws_conn_id=aws_conn_id, **kwargs)
         self.db_type = RdsDbType(db_type)
         self.db_identifier = db_identifier
         self.db_snapshot_identifier = db_snapshot_identifier
         self.tags = tags
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 
 import time
 from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator
 from airflow.providers.amazon.aws.hooks.redshift_cluster import RedshiftHook
-from airflow.providers.amazon.aws.triggers.redshift_cluster import RedshiftClusterTrigger
+from airflow.providers.amazon.aws.triggers.redshift_cluster import (
+    RedshiftClusterTrigger,
+    RedshiftCreateClusterTrigger,
+)
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class RedshiftCreateClusterOperator(BaseOperator):
     """Creates a new cluster with the specified parameters.
@@ -84,14 +87,15 @@
     :param aqua_configuration_status: The cluster is configured to use AQUA .
     :param default_iam_role_arn: ARN for the IAM role.
     :param aws_conn_id: str = The Airflow connection used for AWS credentials.
         The default connection id is ``aws_default``.
     :param wait_for_completion: Whether wait for the cluster to be in ``available`` state
     :param max_attempt: The maximum number of attempts to be made. Default: 5
     :param poll_interval: The amount of time in seconds to wait between attempts. Default: 60
+    :param deferrable: If True, the operator will run in deferrable mode
     """
 
     template_fields: Sequence[str] = (
         "cluster_identifier",
         "cluster_type",
         "node_type",
         "number_of_nodes",
@@ -136,14 +140,15 @@
         availability_zone_relocation: bool | None = None,
         aqua_configuration_status: str | None = None,
         default_iam_role_arn: str | None = None,
         aws_conn_id: str = "aws_default",
         wait_for_completion: bool = False,
         max_attempt: int = 5,
         poll_interval: int = 60,
+        deferrable: bool = False,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.cluster_identifier = cluster_identifier
         self.node_type = node_type
         self.master_username = master_username
         self.master_user_password = master_user_password
@@ -176,14 +181,15 @@
         self.availability_zone_relocation = availability_zone_relocation
         self.aqua_configuration_status = aqua_configuration_status
         self.default_iam_role_arn = default_iam_role_arn
         self.aws_conn_id = aws_conn_id
         self.wait_for_completion = wait_for_completion
         self.max_attempt = max_attempt
         self.poll_interval = poll_interval
+        self.deferrable = deferrable
         self.kwargs = kwargs
 
     def execute(self, context: Context):
         redshift_hook = RedshiftHook(aws_conn_id=self.aws_conn_id)
         self.log.info("Creating Redshift cluster %s", self.cluster_identifier)
         params: dict[str, Any] = {}
         if self.db_name:
@@ -248,26 +254,41 @@
         cluster = redshift_hook.create_cluster(
             self.cluster_identifier,
             self.node_type,
             self.master_username,
             self.master_user_password,
             params,
         )
+        if self.deferrable:
+            self.defer(
+                trigger=RedshiftCreateClusterTrigger(
+                    cluster_identifier=self.cluster_identifier,
+                    poll_interval=self.poll_interval,
+                    max_attempt=self.max_attempt,
+                    aws_conn_id=self.aws_conn_id,
+                ),
+                method_name="execute_complete",
+            )
         if self.wait_for_completion:
             redshift_hook.get_conn().get_waiter("cluster_available").wait(
                 ClusterIdentifier=self.cluster_identifier,
                 WaiterConfig={
                     "Delay": self.poll_interval,
                     "MaxAttempts": self.max_attempt,
                 },
             )
 
         self.log.info("Created Redshift cluster %s", self.cluster_identifier)
         self.log.info(cluster)
 
+    def execute_complete(self, context, event=None):
+        if event["status"] != "success":
+            raise AirflowException(f"Error creating cluster: {event}")
+        return
+
 
 class RedshiftCreateClusterSnapshotOperator(BaseOperator):
     """
     Creates a manual snapshot of the specified cluster. The cluster must be in the available state
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     :param dynamodb_table_name: Dynamodb table to replicate data from
     :param s3_bucket_name: S3 bucket to replicate data to
     :param file_size: Flush file to s3 if file size >= file_size
     :param dynamodb_scan_kwargs: kwargs pass to <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan>
     :param s3_key_prefix: Prefix of s3 object key
     :param process_func: How we transforms a dynamodb item to bytes. By default we dump the json
-    """  # noqa: E501
+    """
 
     template_fields: Sequence[str] = (
         *AwsToAwsBaseOperator.template_fields,
         "s3_bucket_name",
         "s3_key_prefix",
         "dynamodb_table_name",
     )
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 from typing import Any, AsyncIterator
 
-from airflow.providers.amazon.aws.hooks.redshift_cluster import RedshiftAsyncHook
+from airflow.compat.functools import cached_property
+from airflow.providers.amazon.aws.hooks.redshift_cluster import RedshiftAsyncHook, RedshiftHook
 from airflow.triggers.base import BaseTrigger, TriggerEvent
 
 
 class RedshiftClusterTrigger(BaseTrigger):
     """AWS Redshift trigger"""
 
     def __init__(
@@ -51,15 +52,15 @@
                 "aws_conn_id": self.aws_conn_id,
                 "cluster_identifier": self.cluster_identifier,
                 "attempts": self.attempts,
                 "operation_type": self.operation_type,
             },
         )
 
-    async def run(self) -> AsyncIterator["TriggerEvent"]:
+    async def run(self) -> AsyncIterator[TriggerEvent]:
         hook = RedshiftAsyncHook(aws_conn_id=self.aws_conn_id)
         while self.attempts >= 1:
             self.attempts = self.attempts - 1
             try:
                 if self.operation_type == "pause_cluster":
                     response = await hook.pause_cluster(
                         cluster_identifier=self.cluster_identifier,
@@ -81,7 +82,58 @@
                         error_message = f"{self.task_id} failed"
                         yield TriggerEvent({"status": "error", "message": error_message})
                 else:
                     yield TriggerEvent(f"{self.operation_type} is not supported")
             except Exception as e:
                 if self.attempts < 1:
                     yield TriggerEvent({"status": "error", "message": str(e)})
+
+
+class RedshiftCreateClusterTrigger(BaseTrigger):
+    """
+    Trigger for RedshiftCreateClusterOperator.
+    The trigger will asynchronously poll the boto3 API and wait for the
+    Redshift cluster to be in the `available` state.
+
+    :param cluster_identifier:  A unique identifier for the cluster.
+    :param poll_interval: The amount of time in seconds to wait between attempts.
+    :param max_attempt: The maximum number of attempts to be made.
+    :param aws_conn_id: The Airflow connection used for AWS credentials.
+    """
+
+    def __init__(
+        self,
+        cluster_identifier: str,
+        poll_interval: int,
+        max_attempt: int,
+        aws_conn_id: str,
+    ):
+        self.cluster_identifier = cluster_identifier
+        self.poll_interval = poll_interval
+        self.max_attempt = max_attempt
+        self.aws_conn_id = aws_conn_id
+
+    def serialize(self) -> tuple[str, dict[str, Any]]:
+        return (
+            "airflow.providers.amazon.aws.triggers.redshift_cluster.RedshiftCreateClusterTrigger",
+            {
+                "cluster_identifier": str(self.cluster_identifier),
+                "poll_interval": str(self.poll_interval),
+                "max_attempt": str(self.max_attempt),
+                "aws_conn_id": str(self.aws_conn_id),
+            },
+        )
+
+    @cached_property
+    def hook(self) -> RedshiftHook:
+        return RedshiftHook(aws_conn_id=self.aws_conn_id)
+
+    async def run(self):
+        async with self.hook.async_conn as client:
+            await client.get_waiter("cluster_available").wait(
+                ClusterIdentifier=self.cluster_identifier,
+                WaiterConfig={
+                    "Delay": int(self.poll_interval),
+                    "MaxAttempts": int(self.max_attempt),
+                },
+            )
+        yield TriggerEvent({"status": "success", "message": "Cluster Created"})
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,13 +24,24 @@
 class BaseBotoWaiter:
     """
     Used to create custom Boto3 Waiters.
 
     For more details, see airflow/providers/amazon/aws/waiters/README.md
     """
 
-    def __init__(self, client: boto3.client, model_config: dict) -> None:
+    def __init__(self, client: boto3.client, model_config: dict, deferrable: bool = False) -> None:
         self.model = WaiterModel(model_config)
         self.client = client
+        self.deferrable = deferrable
+
+    def _get_async_waiter_with_client(self, waiter_name: str):
+        from aiobotocore.waiter import create_waiter_with_client as create_async_waiter_with_client
+
+        return create_async_waiter_with_client(
+            waiter_name=waiter_name, waiter_model=self.model, client=self.client
+        )
 
     def waiter(self, waiter_name: str) -> Waiter:
+        if self.deferrable:
+            return self._get_async_waiter_with_client(waiter_name=waiter_name)
+
         return create_waiter_with_client(waiter_name=waiter_name, waiter_model=self.model, client=self.client)
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
             "watchtower~=2.0.1",
             "jsonpath_ng>=1.5.3",
             "redshift_connector>=2.0.888",
             "sqlalchemy_redshift>=0.8.6",
             "mypy-boto3-rds>=1.24.0",
             "mypy-boto3-redshift-data>=1.24.0",
             "mypy-boto3-appflow>=1.24.0",
+            "aiobotocore[boto3]>=2.2.0",
         ],
         "integrations": [
             {
                 "integration-name": "Amazon Athena",
                 "external-doc-url": "https://aws.amazon.com/athena/",
                 "logo": "/integration-logos/aws/Amazon-Athena_light-bg@4x.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/athena.rst"],
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.0.0rc1
+Version: 8.0.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
@@ -60,15 +60,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.0.0rc1``
+Release: ``8.0.0rc2``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
@@ -102,14 +102,15 @@
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
 ``mypy-boto3-appflow``                   ``>=1.24.0``
+``aiobotocore[boto3]``                   ``>=2.2.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -172,16 +173,14 @@
   In this version of the provider, deprecated GCS hook's parameter ``delegate_to`` is removed from the following operators: ``GCSToS3Operator``, ``GlacierToGCSOperator`` and ``GoogleApiToS3Operator``.
   Impersonation can be achieved instead by utilizing the ``impersonation_chain`` param.
 
   Removed deprecated parameter ``google_cloud_storage_conn_id`` from ``GCSToS3Operator``, ``gcp_conn_id`` should be used instead.
 
   Removed deprecated parameter ``max_tries`` from the Athena & EMR hook & operators in favor of ``max_polling_attempts``.
 
-  Disabled deprecated behavior of switching to an empty aws connection ID on error. You can set it to None explicitly.
-
   Removed deprecated method ``waiter`` from emr hook in favor of the more generic ``airflow.providers.amazon.aws.utils.waiter.waiter``
 
   Removed deprecated unused parameter ``cluster_identifier`` from Redshift Cluster's hook method ``get_cluster_snapshot_status``
 
   Removed deprecated method ``find_processing_job_by_name`` from Sagemaker hook, use ``count_processing_jobs_by_name`` instead.
 
   Removed deprecated module ``airflow.providers.amazon.aws.operators.aws_lambda`` in favor of ``airflow.providers.amazon.aws.operators.lambda_function``
@@ -207,14 +206,16 @@
 
 Features
 ~~~~~~~~
 
 * ``add a stop operator to emr serverless (#30720)``
 * ``SqlToS3Operator - Add feature to partition SQL table (#30460)``
 * ``New AWS sensor — DynamoDBValueSensor (#28338)``
+* ``Add a "force" option to emr serverless stop/delete operator (#30757)``
+* ``Add support for deferrable operators in AMPP (#30032)``
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fixed logging issue (#30703)``
 * ``DynamoDBHook - waiter_path() to consider 'resource_type' or 'client_type' (#30595)``
 * ``Add ability to override waiter delay in EcsRunTaskOperator (#30586)``
@@ -223,18 +224,23 @@
 
 Misc
 ~~~~
 
 * ``Remove @poke_mode_only from EmrStepSensor (#30774)``
 * ``Organize Amazon providers docs index (#30541)``
 * ``Remove duplicate param docstring in EksPodOperator (#30634)``
+* ``Update AWS EMR Cluster Link to use the new dashboard (#30844)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``fixes to system tests following obsolete cleanup (#30804)``
+   * ``restore fallback to empty connection behavior (#30806)``
+   * ``Prepare docs for adhoc release of providers (#30787)``
 
 7.4.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 airflow/providers/amazon/aws/utils/tags.py
 airflow/providers/amazon/aws/utils/waiter.py
 airflow/providers/amazon/aws/waiters/__init__.py
 airflow/providers/amazon/aws/waiters/appflow.json
 airflow/providers/amazon/aws/waiters/base_waiter.py
 airflow/providers/amazon/aws/waiters/ecs.json
 airflow/providers/amazon/aws/waiters/eks.json
+airflow/providers/amazon/aws/waiters/emr-serverless.json
 airflow/providers/amazon/aws/waiters/emr.json
 apache_airflow_providers_amazon.egg-info/PKG-INFO
 apache_airflow_providers_amazon.egg-info/SOURCES.txt
 apache_airflow_providers_amazon.egg-info/dependency_links.txt
 apache_airflow_providers_amazon.egg-info/entry_points.txt
 apache_airflow_providers_amazon.egg-info/not-zip-safe
 apache_airflow_providers_amazon.egg-info/requires.txt
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+aiobotocore[boto3]>=2.2.0
 apache-airflow-providers-common-sql>=1.3.1.dev0
 apache-airflow>=2.3.0.dev0
 asgiref
 boto3>=1.24.0
 jsonpath_ng>=1.5.3
 mypy-boto3-appflow>=1.24.0
 mypy-boto3-rds>=1.24.0
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/pyproject.toml` & `apache-airflow-providers-amazon-8.0.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/setup.cfg` & `apache-airflow-providers-amazon-8.0.0rc2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
+	aiobotocore[boto3]>=2.2.0
 	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow>=2.3.0.dev0
 	asgiref
 	boto3>=1.24.0
 	jsonpath_ng>=1.5.3
 	mypy-boto3-appflow>=1.24.0
 	mypy-boto3-rds>=1.24.0
@@ -62,10 +63,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.amazon.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.amazon
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc1/setup.py` & `apache-airflow-providers-amazon-8.0.0rc2/setup.py`

 * *Files identical despite different names*

