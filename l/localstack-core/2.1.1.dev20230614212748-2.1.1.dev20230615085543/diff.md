# Comparing `tmp/localstack-core-2.1.1.dev20230614212748.tar.gz` & `tmp/localstack-core-2.1.1.dev20230615085543.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230614212748.tar", last modified: Wed Jun 14 21:27:56 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230615085543.tar", last modified: Thu Jun 15 08:55:52 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230614212748.tar` & `localstack-core-2.1.1.dev20230615085543.tar`

### file list

```diff
@@ -1,851 +1,851 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.420010 localstack-core-2.1.1.dev20230614212748/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-14 21:27:56.420010 localstack-core-2.1.1.dev20230614212748/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.280010 localstack-core-2.1.1.dev20230614212748/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.280010 localstack-core-2.1.1.dev20230614212748/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-14 21:27:48.000000 localstack-core-2.1.1.dev20230614212748/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.280010 localstack-core-2.1.1.dev20230614212748/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.280010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   755634 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.284010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.288010 localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.292010 localstack-core-2.1.1.dev20230614212748/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.292010 localstack-core-2.1.1.dev20230614212748/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.292010 localstack-core-2.1.1.dev20230614212748/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.292010 localstack-core-2.1.1.dev20230614212748/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.292010 localstack-core-2.1.1.dev20230614212748/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.292010 localstack-core-2.1.1.dev20230614212748/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.292010 localstack-core-2.1.1.dev20230614212748/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.292010 localstack-core-2.1.1.dev20230614212748/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.296010 localstack-core-2.1.1.dev20230614212748/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.296010 localstack-core-2.1.1.dev20230614212748/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.296010 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    61609 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14059 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.296010 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.300010 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.300010 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.300010 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.300010 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.300010 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    64921 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.304010 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32657 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20947 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7009 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2126 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5391 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22846 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2585 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8984 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28333 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3062 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5326 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13557 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6426 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8745 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3812 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5502 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.304010 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.304010 localstack-core-2.1.1.dev20230614212748/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.304010 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.304010 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.304010 localstack-core-2.1.1.dev20230614212748/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.304010 localstack-core-2.1.1.dev20230614212748/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35960 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.308010 localstack-core-2.1.1.dev20230614212748/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.312010 localstack-core-2.1.1.dev20230614212748/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.312010 localstack-core-2.1.1.dev20230614212748/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.312010 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.312010 localstack-core-2.1.1.dev20230614212748/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.312010 localstack-core-2.1.1.dev20230614212748/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.312010 localstack-core-2.1.1.dev20230614212748/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.312010 localstack-core-2.1.1.dev20230614212748/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43470 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.312010 localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.312010 localstack-core-2.1.1.dev20230614212748/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.316010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.320010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.320010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.320010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.320010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.324010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.324010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.324010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.324010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.324010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.328010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.328010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.332010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.332010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.336010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.336010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.336010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.336010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.336010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.336010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.336010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.336010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.400010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.408010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69745 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.412010 localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.416010 localstack-core-2.1.1.dev20230614212748/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.416010 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.420010 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.420010 localstack-core-2.1.1.dev20230614212748/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.420010 localstack-core-2.1.1.dev20230614212748/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.420010 localstack-core-2.1.1.dev20230614212748/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.420010 localstack-core-2.1.1.dev20230614212748/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-14 21:27:56.420010 localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-14 21:27:56.000000 localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37808 2023-06-14 21:27:56.000000 localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-14 21:27:56.000000 localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-14 21:27:56.000000 localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-14 21:27:52.000000 localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-14 21:27:52.000000 localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-14 21:27:56.000000 localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-14 21:27:56.000000 localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-14 21:27:56.420010 localstack-core-2.1.1.dev20230614212748/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-14 20:49:43.000000 localstack-core-2.1.1.dev20230614212748/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.042594 localstack-core-2.1.1.dev20230615085543/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-15 08:55:52.042594 localstack-core-2.1.1.dev20230615085543/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.950594 localstack-core-2.1.1.dev20230615085543/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-15 08:55:43.000000 localstack-core-2.1.1.dev20230615085543/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86119 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.954594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   755634 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48826 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71940 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38087 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.958594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.962594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.962594 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.962594 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.962594 localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.962594 localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.962594 localstack-core-2.1.1.dev20230615085543/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.962594 localstack-core-2.1.1.dev20230615085543/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.962594 localstack-core-2.1.1.dev20230615085543/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.966594 localstack-core-2.1.1.dev20230615085543/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.966594 localstack-core-2.1.1.dev20230615085543/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.966594 localstack-core-2.1.1.dev20230615085543/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.966594 localstack-core-2.1.1.dev20230615085543/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.966594 localstack-core-2.1.1.dev20230615085543/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.970594 localstack-core-2.1.1.dev20230615085543/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.970594 localstack-core-2.1.1.dev20230615085543/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.970594 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61609 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14059 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.970594 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.970594 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.974594 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17831 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19612 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.974594 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.974594 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.974594 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    64921 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.978594 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33075 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20991 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2489 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7518 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2190 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5527 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21966 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2991 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3188 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9202 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28763 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3327 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2640 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13881 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6708 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8735 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5112 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3927 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5754 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3768 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5732 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.978594 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.978594 localstack-core-2.1.1.dev20230615085543/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.978594 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.978594 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.978594 localstack-core-2.1.1.dev20230615085543/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.978594 localstack-core-2.1.1.dev20230615085543/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.978594 localstack-core-2.1.1.dev20230615085543/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23351 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19690 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35960 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.982594 localstack-core-2.1.1.dev20230615085543/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.986594 localstack-core-2.1.1.dev20230615085543/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.986594 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.986594 localstack-core-2.1.1.dev20230615085543/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.986594 localstack-core-2.1.1.dev20230615085543/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.986594 localstack-core-2.1.1.dev20230615085543/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.986594 localstack-core-2.1.1.dev20230615085543/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43470 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.986594 localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.986594 localstack-core-2.1.1.dev20230615085543/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.990594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.990594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.990594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.990594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.990594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.990594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.990594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.990594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.994594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.994594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.994594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.994594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.994594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.994594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:51.994594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.002594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.002594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.002594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.002594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.002594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.002594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.006594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.006594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.006594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.010594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.010594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.010594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.010594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.010594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.010594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.010594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.010594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.014594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.014594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.014594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.018594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.018594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.018594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.018594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.018594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.022594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.022594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.026594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.034594 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.034594 localstack-core-2.1.1.dev20230615085543/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.034594 localstack-core-2.1.1.dev20230615085543/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.034594 localstack-core-2.1.1.dev20230615085543/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.034594 localstack-core-2.1.1.dev20230615085543/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.034594 localstack-core-2.1.1.dev20230615085543/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.034594 localstack-core-2.1.1.dev20230615085543/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.034594 localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.034594 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69745 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.038594 localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.038594 localstack-core-2.1.1.dev20230615085543/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.042594 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.042594 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.042594 localstack-core-2.1.1.dev20230615085543/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.042594 localstack-core-2.1.1.dev20230615085543/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45834 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.042594 localstack-core-2.1.1.dev20230615085543/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.042594 localstack-core-2.1.1.dev20230615085543/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23579 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-15 08:55:52.042594 localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-15 08:55:51.000000 localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37808 2023-06-15 08:55:51.000000 localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-15 08:55:51.000000 localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-15 08:55:51.000000 localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-15 08:55:47.000000 localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-15 08:55:47.000000 localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2855 2023-06-15 08:55:51.000000 localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-15 08:55:51.000000 localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3186 2023-06-15 08:55:52.046594 localstack-core-2.1.1.dev20230615085543/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-15 08:23:16.000000 localstack-core-2.1.1.dev20230615085543/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230614212748/LICENSE.txt` & `localstack-core-2.1.1.dev20230615085543/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/Makefile` & `localstack-core-2.1.1.dev20230615085543/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/README.md` & `localstack-core-2.1.1.dev20230615085543/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/bin/localstack` & `localstack-core-2.1.1.dev20230615085543/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230615085543/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230615085543/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230615085543/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230615085543/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230615085543/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230615085543/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230615085543/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/config.py` & `localstack-core-2.1.1.dev20230615085543/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/constants.py` & `localstack-core-2.1.1.dev20230615085543/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230615085543/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230615085543/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230615085543/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/client.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/request.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/response.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/http/router.py` & `localstack-core-2.1.1.dev20230615085543/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230615085543/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230615085543/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230615085543/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230615085543/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230615085543/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230615085543/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/packages/ffmpeg.py` & `localstack-core-2.1.1.dev20230615085543/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230615085543/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/plugins.py` & `localstack-core-2.1.1.dev20230615085543/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230615085543/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230615085543/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230615085543/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230615085543/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230615085543/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/apigateway.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import (
     generate_default_name,
     lambda_keys_to_lower,
     params_list_to_dict,
 )
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import aws_stack, queries
+from localstack.utils.aws import queries
 from localstack.utils.common import keys_to_lower, select_attributes, to_bytes
 from localstack.utils.strings import first_char_to_lower
 
 
 class GatewayResponse(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::GatewayResponse"
 
     def fetch_state(self, stack_name, resources):
         props = self.props
         api_id = props.get("RestApiId")
         if not api_id:
             return
-        client = aws_stack.connect_to_service("apigateway")
+        client = connect_to().apigateway
         result = client.get_gateway_response(restApiId=api_id, responseType=props["ResponseType"])
         return result if "responseType" in result else None
 
     @staticmethod
     def get_deploy_templates():
         return {
             "create": {
@@ -44,19 +44,16 @@
 
 
 class GatewayRequestValidator(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::RequestValidator"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("id")
-
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("apigateway")
+        client = connect_to().apigateway
         props = self.props
         api_id = props["RestApiId"]
         name = props["Name"]
         result = client.get_request_validators(restApiId=api_id).get("items", [])
         result = [r for r in result if r.get("name") == name]
         return result[0] if result else None
 
@@ -66,23 +63,27 @@
         if not role_name:
             resource["Properties"]["Name"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["id"]
+
         return {
             "create": {
                 "function": "create_request_validator",
                 "parameters": {
                     "name": "Name",
                     "restApiId": "RestApiId",
                     "validateRequestBody": "ValidateRequestBody",
                     "validateRequestParameters": "ValidateRequestParameters",
                 },
+                "result_handler": _handle_result,
             },
             "delete": {
                 "function": "delete_request_validator",
                 "parameters": {"restApiId": "RestApiId", "requestValidatorId": "id"},
             },
         }
 
@@ -91,50 +92,43 @@
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::RestApi"
 
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "RootResourceId":
             api_id = self.props.get("id")
-            resources = aws_stack.connect_to_service("apigateway").get_resources(restApiId=api_id)[
-                "items"
-            ]
+            resources = connect_to().apigateway.get_resources(restApiId=api_id)["items"]
             for res in resources:
                 if res["path"] == "/" and not res.get("parentId"):
                     return res["id"]
         return super(GatewayRestAPI, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("id")
-
     def fetch_state(self, stack_name, resources):
         if not self.props.get("id"):
             return None
 
-        return aws_stack.connect_to_service("apigateway").get_rest_api(
-            restApiId=self.props.get("id")
-        )
+        return connect_to().apigateway.get_rest_api(restApiId=self.props.get("id"))
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         # FIXME: this is only when Body or BodyS3Location is set, otherwise the deployment should fail without a name
         role_name = resource.get("Properties", {}).get("Name")
         if not role_name:
             resource["Properties"]["Name"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
         def _api_id(params, resources, resource_id, **kwargs):
             resource = cls(resources[resource_id])
-            return resource.physical_resource_id or resource.get_physical_resource_id()
+            return resource.physical_resource_id
 
         def _create(resource_id, resources, resource_type, func, stack_name):
-            client = aws_stack.connect_to_service("apigateway")
+            client = connect_to().apigateway
             resource = resources[resource_id]
             props = resource["Properties"]
 
             kwargs = select_attributes(
                 props,
                 [
                     "Name",
@@ -149,15 +143,15 @@
                     "Tags",
                     "DisableExecuteApiEndpoint",
                 ],
             )
             kwargs = keys_to_lower(kwargs, skip_children_of=["policy"])
             kwargs["tags"] = {tag["key"]: tag["value"] for tag in kwargs.get("tags", [])}
 
-            cfn_client = aws_stack.connect_to_service("cloudformation")
+            cfn_client = connect_to().cloudformation
             stack_id = cfn_client.describe_stacks(StackName=stack_name)["Stacks"][0]["StackId"]
             kwargs["tags"].update(
                 {
                     "aws:cloudformation:logical-id": resource_id,
                     "aws:cloudformation:stack-name": stack_name,
                     "aws:cloudformation:stack-id": stack_id,
                 }
@@ -208,16 +202,19 @@
                     parameters=import_parameters,
                     **put_kwargs,
                 )
 
             props["id"] = result["id"]
             return result
 
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["id"]
+
         return {
-            "create": {"function": _create},
+            "create": {"function": _create, "result_handler": _handle_result},
             "delete": {
                 "function": "delete_rest_api",
                 "parameters": {
                     "restApiId": _api_id,
                 },
             },
         }
@@ -230,57 +227,53 @@
 
     def fetch_state(self, stack_name, resources):
         api_id = self.props.get("RestApiId")
 
         if not api_id:
             return None
 
-        client = aws_stack.connect_to_service("apigateway")
+        client = connect_to().apigateway
         result = client.get_deployments(restApiId=api_id)["items"]
         # TODO possibly filter results by stage name or other criteria
 
         return result[0] if result else None
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("id")
-
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["id"]
+
         return {
             "create": {
                 "function": "create_deployment",
                 "parameters": {
                     "restApiId": "RestApiId",
                     "stageName": "StageName",
                     "stageDescription": "StageDescription",
                     "description": "Description",
                 },
+                "result_handler": _handle_result,
             }
         }
 
 
 class GatewayResource(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::Resource"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("id")
-
     def fetch_state(self, stack_name, resources):
         props = self.props
         api_id = props.get("RestApiId") or self.logical_resource_id
         parent_id = props.get("ParentId")
 
         if not api_id or not parent_id:
             return None
 
-        api_resources = aws_stack.connect_to_service("apigateway").get_resources(restApiId=api_id)[
-            "items"
-        ]
+        api_resources = connect_to().apigateway.get_resources(restApiId=api_id)["items"]
         target_resource = list(
             filter(
                 lambda res: res.get("parentId") == parent_id
                 and res["pathPart"] == props["PathPart"],
                 api_resources,
             )
         )
@@ -300,28 +293,32 @@
             result = {
                 "restApiId": params.get("RestApiId"),
                 "pathPart": params.get("PathPart"),
                 "parentId": params.get("ParentId"),
             }
             if not result.get("parentId"):
                 # get root resource id
-                apigw = aws_stack.connect_to_service("apigateway")
+                apigw = connect_to().apigateway
                 resources = apigw.get_resources(restApiId=result["restApiId"])["items"]
                 root_resource = ([r for r in resources if r["path"] == "/"] or [None])[0]
                 if not root_resource:
                     raise Exception(
                         "Unable to find root resource for REST API %s" % result["restApiId"]
                     )
                 result["parentId"] = root_resource["id"]
             return result
 
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["id"]
+
         return {
             "create": {
                 "function": "create_resource",
                 "parameters": get_apigw_resource_params,
+                "result_handler": _handle_result,
             }
         }
 
 
 class GatewayMethod(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
@@ -331,17 +328,15 @@
         props = self.props
 
         api_id = props["RestApiId"]
         res_id = props["ResourceId"]
         if not api_id or not res_id:
             return None
 
-        res_obj = aws_stack.connect_to_service("apigateway").get_resource(
-            restApiId=api_id, resourceId=res_id
-        )
+        res_obj = connect_to().apigateway.get_resource(restApiId=api_id, resourceId=res_id)
         match = [
             v
             for (k, v) in res_obj.get("resourceMethods", {}).items()
             if props["HttpMethod"] in (v.get("httpMethod"), k)
         ]
 
         int_props = props.get("Integration") or {}
@@ -354,15 +349,15 @@
                 == int_props.get("IntegrationHttpMethod")
             ]
 
         return match[0] if match else None
 
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
-        client = aws_stack.connect_to_service("apigateway")
+        client = connect_to().apigateway
         integration = props.get("Integration")
         kwargs = {
             "restApiId": props["RestApiId"],
             "resourceId": props["ResourceId"],
             "httpMethod": props["HttpMethod"],
             "requestParameters": props.get("RequestParameters") or {},
         }
@@ -375,23 +370,14 @@
             kwargs["requestParameters"] = integration.get("RequestParameters") or {}
             kwargs["requestTemplates"] = integration.get("RequestTemplates") or {}
             return client.put_integration(**kwargs)
         kwargs["authorizationType"] = props.get("AuthorizationType")
 
         return client.put_method(**kwargs)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        props = self.props
-        result = "%s-%s-%s" % (
-            props.get("RestApiId"),
-            props.get("ResourceId"),
-            props.get("HttpMethod"),
-        )
-        return result
-
     @classmethod
     def get_deploy_templates(cls):
         """
         https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigateway-method.html
         https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-apitgateway-method-methodresponse.html
         https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-apitgateway-method-integration.html
         https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-apitgateway-method-integration-integrationresponse.html
@@ -412,15 +398,15 @@
             ]
             result = select_attributes(result, param_names)
             result["requestModels"] = result.get("requestModels") or {}
             result["requestParameters"] = result.get("requestParameters") or {}
             return result
 
         def _subresources(resource_id, resources, resource_type, func, stack_name):
-            apigateway = aws_stack.connect_to_service("apigateway")
+            apigateway = connect_to().apigateway
             resource = cls(resources[resource_id])
             props = resource.props
 
             integration = props.get("Integration")
             if integration:
                 api_id = props["RestApiId"]
                 res_id = props["ResourceId"]
@@ -473,19 +459,29 @@
                     resourceId=res_id,
                     httpMethod=props["HttpMethod"],
                     statusCode=str(response["statusCode"]),
                     responseParameters=response.get("responseParameters") or {},
                     responseModels=response.get("responseModels") or {},
                 )
 
+        def _handle_result(result, resource_id, resources, resource_type):
+            resource = resources[resource_id]
+            rest_api_id = resource["Properties"]["RestApiId"]
+            apigw_resource_id = resource["Properties"]["ResourceId"]
+            http_method = resource["Properties"]["HttpMethod"]
+            resources[resource_id][
+                "PhysicalResourceId"
+            ] = f"{rest_api_id}-{apigw_resource_id}-{http_method}"
+
         return {
             "create": [
                 {
                     "function": "put_method",
                     "parameters": get_params,
+                    "result_handler": _handle_result,
                 },
                 {
                     "function": _subresources  # dynamic mapping for additional sdk calls for this CFn resource
                 },
             ]
         }
 
@@ -495,22 +491,19 @@
     def cloudformation_type():
         return "AWS::ApiGateway::Stage"
 
     def fetch_state(self, stack_name, resources):
         api_id = self.props.get("RestApiId") or self.logical_resource_id
         if not api_id:
             return None
-        result = aws_stack.connect_to_service("apigateway").get_stage(
+        result = connect_to().apigateway.get_stage(
             restApiId=api_id, stageName=self.props["StageName"]
         )
         return result
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("StageName")
-
     @staticmethod
     def get_deploy_templates():
         def get_params(resource_props, stack_name, resources, resource_id):
             stage_name = resource_props.get("StageName", "default")
             resources[resource_id]["Properties"]["StageName"] = stage_name
             result = keys_to_lower(resource_props)
             param_names = [
@@ -526,43 +519,50 @@
                 "tags",
             ]
             result = select_attributes(result, param_names)
             result["tags"] = {t["key"]: t["value"] for t in result.get("tags", [])}
             result["stageName"] = stage_name
             return result
 
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["stageName"]
+
         return {
             "create": {
                 "function": "create_stage",
                 "parameters": get_params,
+                "result_handler": _handle_result,
             }
         }
 
 
 class GatewayUsagePlan(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::UsagePlan"
 
     def fetch_state(self, stack_name, resources):
         plan_name = self.props.get("UsagePlanName")
-        result = aws_stack.connect_to_service("apigateway").get_usage_plans().get("items", [])
+        result = connect_to().apigateway.get_usage_plans().get("items", [])
         result = [r for r in result if r["name"] == plan_name]
         return (result or [None])[0]
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         role_name = resource.get("Properties", {}).get("UsagePlanName")
         if not role_name:
             resource["Properties"]["UsagePlanName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["id"]
+
         return {
             "create": {
                 "function": "create_usage_plan",
                 "parameters": {
                     "name": "UsagePlanName",
                     "description": "Description",
                     "apiStages": lambda_keys_to_lower("ApiStages"),
@@ -571,20 +571,18 @@
                     "tags": params_list_to_dict("Tags"),
                 },
                 "types": {
                     "limit": int,
                     "burstLimit": int,
                     "rateLimit": float,
                 },
+                "result_handler": _handle_result,
             }
         }
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("id")
-
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
         parameters_to_select = [
             "UsagePlanName",
             "Description",
             "ApiStages",
             "Quota",
@@ -636,28 +634,28 @@
                     last_value = value[item]
                     path = f"/{first_char_to_lower(parameter)}/{first_char_to_lower(item)}"
                     patch_operations.append({"op": "replace", "path": path, "value": last_value})
             else:
                 patch_operations.append(
                     {"op": "replace", "path": f"/{first_char_to_lower(parameter)}", "value": value}
                 )
-        client = aws_stack.connect_to_service("apigateway")
+        client = connect_to().apigateway
         client.update_usage_plan(usagePlanId=usage_plan_id, patchOperations=patch_operations)
 
 
 class GatewayApiKey(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::ApiKey"
 
     def fetch_state(self, stack_name, resources):
         props = self.props
         key_name = props.get("Name")
         cust_id = props.get("CustomerId")
-        result = aws_stack.connect_to_service("apigateway").get_api_keys().get("items", [])
+        result = connect_to().apigateway.get_api_keys().get("items", [])
         result = [
             r
             for r in result
             if r.get("name") == key_name and cust_id in (None, r.get("customerId"))
         ]
         return (result or [None])[0]
 
@@ -667,74 +665,77 @@
         if not role_name:
             resource["Properties"]["Name"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["id"]
+
         return {
             "create": {
                 "function": "create_api_key",
                 "parameters": {
                     "description": "Description",
                     "customerId": "CustomerId",
                     "name": "Name",
                     "value": "Value",
                     "enabled": "Enabled",
                     "stageKeys": lambda_keys_to_lower("StageKeys"),
                     "tags": params_list_to_dict("Tags"),
                 },
                 "types": {"enabled": bool},
+                "result_handler": _handle_result,
             }
         }
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("id")
-
 
 class GatewayUsagePlanKey(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::UsagePlanKey"
 
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("apigateway")
+        client = connect_to().apigateway
         key_id = self.props.get("KeyId")
         key_type = self.props.get("KeyType")
         plan_id = self.props.get("UsagePlanId")
         result = client.get_usage_plan_keys(usagePlanId=plan_id).get("items", [])
         result = [r for r in result if r["id"] == key_id and key_type in [None, r.get("type")]]
         return (result or [None])[0]
 
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["id"]
+
         return {
             "create": {
                 "function": "create_usage_plan_key",
                 "parameters": lambda_keys_to_lower(),
+                "result_handler": _handle_result,
             }
         }
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("id")
-
 
 # TODO: add tests for this resource type
 class GatewayDomain(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::DomainName"
 
     def fetch_state(self, stack_name, resources):
-        return aws_stack.connect_to_service("apigateway").get_domain_name(
-            domainName=self.props["DomainName"]
-        )
+        return connect_to().apigateway.get_domain_name(domainName=self.props["DomainName"])
 
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["domainName"]
+
         return {
             "create": {
                 "function": "create_domain_name",
                 "parameters": {
                     "certificateArn": lambda_keys_to_lower("CertificateArn"),
                     "domainName": lambda_keys_to_lower("DomainName"),
                     "endpointConfiguration": lambda_keys_to_lower("EndpointConfiguration"),
@@ -742,31 +743,29 @@
                     "ownershipVerificationCertificateArn": lambda_keys_to_lower(
                         "OwnershipVerificationCertificateArn"
                     ),
                     "regionalCertificateArn": lambda_keys_to_lower("RegionalCertificateArn"),
                     "securityPolicy": lambda_keys_to_lower("SecurityPolicy"),
                     "tags": params_list_to_dict("Tags"),
                 },
+                "result_handler": _handle_result,
             }
         }
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("domainName")
-
 
 # TODO: add tests for this resource type
 class GatewayBasePathMapping(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::BasePathMapping"
 
     def fetch_state(self, stack_name, resources):
         resources = (
-            aws_stack.connect_to_service("apigateway")
-            .get_base_path_mappings(domainName=self.props.get("DomainName"))
+            connect_to()
+            .apigateway.get_base_path_mappings(domainName=self.props.get("DomainName"))
             .get("items", [])
         )
 
         comparable = (
             [self.props.get("BasePath")] if self.props.get("BasePath") else [None, "", "(none)"]
         )
 
@@ -781,32 +780,34 @@
             kwargs = {
                 "domainName": props.get("DomainName"),
                 "restApiId": props.get("RestApiId"),
                 **({"basePath": props.get("BasePath")} if props.get("BasePath") else {}),
                 **({"stage": props.get("Stage")} if props.get("Stage") else {}),
             }
 
-            aws_stack.connect_to_service("apigateway").create_base_path_mapping(**kwargs)
+            return connect_to().apigateway.create_base_path_mapping(**kwargs)
 
-        return {"create": {"function": _create_base_path_mapping}}
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["restApiId"]
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("restApiId")
+        return {
+            "create": {
+                "function": _create_base_path_mapping,
+                "result_handler": _handle_result,
+            }
+        }
 
 
 class GatewayModel(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::Model"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("Name")
-
     def fetch_state(self, stack_name, resources):
-        client = aws_stack.connect_to_service("apigateway")
+        client = connect_to().apigateway
         api_id = self.props["RestApiId"]
 
         items = client.get_models(restApiId=api_id)["items"]
         if not items:
             return None
 
         model_name = self.props["Name"]
@@ -851,29 +852,26 @@
     @staticmethod
     def cloudformation_type():
         return "AWS::ApiGateway::Account"
 
     def fetch_state(self, stack_name, resources):
         if not self.physical_resource_id:
             return None
-        client = aws_stack.connect_to_service("apigateway")
+        client = connect_to().apigateway
         return client.get_account()
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.physical_resource_id
-
     @classmethod
     def get_deploy_templates(cls):
         def _create(resource_id, resources, *args, **kwargs):
             resource = resources[resource_id]
             props = cls(resource).props
 
             role_arn = props["CloudWatchRoleArn"]
 
-            aws_stack.connect_to_service("apigateway").update_account(
+            connect_to().apigateway.update_account(
                 patchOperations=[{"op": "replace", "path": "/cloudwatchRoleArn", "value": role_arn}]
             )
 
             resource["PhysicalResourceId"] = generate_default_name(
                 args[2], resource["LogicalResourceId"]
             )
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/awslambda.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 import random
 import string
+import uuid
 
 from localstack.aws.connect import connect_to
 from localstack.services.awslambda.lambda_utils import get_handler_file_from_name
 from localstack.services.cloudformation.deployment_utils import (
     generate_default_name,
     select_parameters,
 )
@@ -32,20 +33,14 @@
     def cloudformation_type():
         return "AWS::Lambda::Function"
 
     def fetch_state(self, stack_name, resources):
         func_name = self.props["FunctionName"]
         return connect_to().awslambda.get_function(FunctionName=func_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        func_name = self.props.get("FunctionName")
-        if attribute == "Arn":
-            return arns.lambda_function_arn(func_name)
-        return func_name
-
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
         client = aws_stack.connect_to_service("lambda")
         config_keys = [
             "Description",
             "Environment",
             "FunctionName",
@@ -132,16 +127,20 @@
             if "Environment" in params:
                 environment_variables = params["Environment"].get("Variables", {})
                 return {"Variables": {k: str(v) for k, v in environment_variables.items()}}
 
         def result_handler(result, resource_id, resources, resource_type):
             """waits for the lambda to be in a "terminal" state, i.e. not pending"""
             resources[resource_id]["Properties"]["Arn"] = result["FunctionArn"]
-            lambda_client = aws_stack.connect_to_service("lambda")
-            lambda_client.get_waiter("function_active_v2").wait(FunctionName=result["FunctionArn"])
+            resources[resource_id]["PhysicalResourceId"] = resources[resource_id]["Properties"][
+                "FunctionName"
+            ]
+            connect_to().awslambda.get_waiter("function_active_v2").wait(
+                FunctionName=result["FunctionArn"]
+            )
 
         return {
             "create": {
                 "function": "create_function",
                 "parameters": {
                     "Architectures": "Architectures",
                     "Code": LambdaFunction.get_lambda_code_param,
@@ -232,21 +231,21 @@
             raise Exception("ResourceNotFound")
         return mapping[0]
 
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "Id":
             return self.props.get("UUID")
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("UUID")
-
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["UUID"]
+
         return {
-            "create": {"function": "create_event_source_mapping"},
+            "create": {"function": "create_event_source_mapping", "result_handler": _handle_result},
             "delete": {"function": "delete_event_source_mapping", "parameters": ["UUID"]},
         }
 
 
 class LambdaPermission(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
@@ -329,25 +328,27 @@
         props = self.props
         result = client.get_function_event_invoke_config(
             FunctionName=props.get("FunctionName"),
             Qualifier=props.get("FunctionName", "$LATEST"),
         )
         return result
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        props = self.props
-        return "lambdaconfig-%s-%s" % (
-            props.get("FunctionName"),
-            props.get("Qualifier"),
-        )
-
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = str(
+                uuid.uuid4()
+            )  # TODO: not actually a UUIDv4
+            # example format: 6403f864-a20b-4373-ac8f-f8d888f6bc0f
+
         return {
-            "create": {"function": "put_function_event_invoke_config"},
+            "create": {
+                "function": "put_function_event_invoke_config",
+                "result_handler": _handle_result,
+            },
             "delete": {
                 "function": "delete_function_event_invoke_config",
                 "parameters": {
                     "FunctionName": "FunctionName",
                     "Qualifier": "Qualifier",
                 },
             },
@@ -355,19 +356,14 @@
 
 
 class LambdaUrl(GenericBaseModel):
     @classmethod
     def cloudformation_type(cls):
         return "AWS::Lambda::Url"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get(
-            "TargetFunctionArn"
-        )  # TODO: if this isn't an ARN we need to resolve the full ARN here
-
     def fetch_state(self, stack_name, resources):
         client = aws_stack.connect_to_service("lambda")
 
         kwargs = {"FunctionName": self.props.get("TargetFunctionArn")}
         qualifier = self.props.get("Qualifier")
         if qualifier:
             kwargs["Qualifier"] = qualifier
@@ -382,23 +378,29 @@
                 FunctionName=self.props.get("TargetFunctionArn")
             )
             return url_config["FunctionUrl"]
         return super(LambdaUrl, self).get_cfn_attribute(attribute_name)
 
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["FunctionArn"]
+            resources[resource_id]["Properties"]["FunctionArn"] = result["FunctionArn"]
+            resources[resource_id]["Properties"]["FunctionUrl"] = result["FunctionUrl"]
+
         return {
             "create": {
                 "function": "create_function_url_config",
                 "parameters": {
                     "Qualifier": "Qualifier",
                     "Cors": "Cors",
                     "FunctionName": "TargetFunctionArn",
                     "AuthType": "AuthType",
                 },
+                "result_handler": _handle_result,
             },
             "delete": {
                 "function": "delete_function_url_config",
                 "parameters": {"FunctionName": "TargetFunctionArn", "Qualifier": "Qualifier"},
             },
         }
 
@@ -442,54 +444,41 @@
 
         client = aws_stack.connect_to_service("lambda")
         result = client.get_code_signing_config(CodeSigningConfigArn=self.physical_resource_id)[
             "CodeSigningConfig"
         ]
         return result
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.physical_resource_id
-
-    def get_cfn_attribute(self, attribute_name):
-        if attribute_name == "CodeSigningConfigId":
-            return self.props["CodeSigningConfigId"]
-
-        return self.physical_resource_id
-
     @classmethod
     def get_deploy_templates(cls):
         def _store_arn(result, resource_id, resources, resource_type):
             resources[resource_id]["PhysicalResourceId"] = result["CodeSigningConfig"][
                 "CodeSigningConfigArn"
             ]
-
-        def _arn(params, resources, resource_id, **kwargs):
-            resource = cls(resources[resource_id])
-            return resource.physical_resource_id or resource.get_physical_resource_id()
+            resources[resource_id]["Properties"]["CodeSigningConfigArn"] = result[
+                "CodeSigningConfig"
+            ]["CodeSigningConfigArn"]
 
         return {
             "create": {"function": "create_code_signing_config", "result_handler": _store_arn},
             "delete": {
                 "function": "delete_code_signing_config",
                 "parameters": {
-                    "CodeSigningConfigArn": _arn,
+                    "CodeSigningConfigArn": "CodeSigningConfigArn",
                 },
             },
         }
 
 
 # TODO: test
 class LambdaLayerVersion(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Lambda::LayerVersion"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.state.get("LayerVersionArn")
-
     def fetch_state(self, stack_name, resources):
         layer_name = self.props.get("LayerName")
         # TODO extract region name if layer_name is an ARN
         client = aws_stack.connect_to_service("lambda")
         layers = client.list_layer_versions(LayerName=layer_name).get("LayerVersions", [])
         return layers[-1] if layers else None
 
@@ -497,15 +486,18 @@
     def add_defaults(resource, stack_name: str):
         resource["Properties"]["LayerName"] = (
             resource["Properties"].get("LayerName") or f"layer-{short_uid()}"
         )
 
     @staticmethod
     def get_deploy_templates():
-        return {"create": {"function": "publish_layer_version"}}
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["LayerVersionArn"]
+
+        return {"create": {"function": "publish_layer_version", "result_handler": _handle_result}}
 
 
 # TODO: test
 # TODO: remove inheritance
 class LambdaLayerVersionPermission(LambdaPermission):
     @staticmethod
     def cloudformation_type():
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/cdk.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,29 +9,30 @@
     @staticmethod
     def cloudformation_type():
         return "AWS::CDK::Metadata"
 
     def fetch_state(self, stack_name, resources):
         return self.props
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        # return a synthetic ID here, as some parts of the CFn engine depend on PhysicalResourceId being resolvable
-        return md5(canonical_json(self.props))
-
     @staticmethod
     def add_defaults(resource, stack_name: str):
         resource["Properties"]["PhysicalResourceId"] = (
             resource["Properties"].get("PhysicalResourceId") or f"cdk-meta-{short_uid()}"
         )
 
     def update_resource(self, new_resource, stack_name, resources):
         return True
 
     @staticmethod
     def get_deploy_templates():
         def _no_op(*args, **kwargs):
             pass
 
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = md5(
+                canonical_json(resources[resource_id]["Properties"])
+            )
+
         return {
-            "create": {"function": _no_op},
+            "create": {"function": _no_op, "result_handler": _handle_result},
             "delete": {"function": _no_op},
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,14 @@
     def fetch_state(self, stack_name, resources):
         client = aws_stack.connect_to_service("acm")
         result = client.list_certificates().get("CertificateSummaryList", [])
         domain_name = self.props.get("DomainName")
         result = [c for c in result if c["DomainName"] == domain_name]
         return (result or [None])[0]
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("CertificateArn")
-
     @classmethod
     def get_deploy_templates(cls):
         def _create_params(params, *args, **kwargs):
             result = select_attributes(
                 params,
                 [
                     "CertificateAuthorityArn",
@@ -47,14 +44,24 @@
             # adjust logging preferences
             logging_pref = result.get("CertificateTransparencyLoggingPreference")
             if logging_pref:
                 result["Options"] = {"CertificateTransparencyLoggingPreference": logging_pref}
 
             return result
 
+        def _handle_result(result, resource_id, resources, resource_type):
+            resource = resources[resource_id]
+            resource["Properties"]["CertificateArn"] = resource["PhysicalResourceId"] = result[
+                "CertificateArn"
+            ]
+
         return {
-            "create": {"function": "request_certificate", "parameters": _create_params},
+            "create": {
+                "function": "request_certificate",
+                "parameters": _create_params,
+                "result_handler": _handle_result,
+            },
             "delete": {
                 "function": "delete_certificate",
                 "parameters": ["CertificateArn"],
             },
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/cloudformation.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 
 
 class CloudFormationStack(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::CloudFormation::Stack"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("StackId")
-
     def fetch_state(self, stack_name, resources):
         client = aws_stack.connect_to_service("cloudformation")
         child_stack_name = self.props["StackName"]
         result = client.describe_stacks(StackName=child_stack_name)
         result = (result.get("Stacks") or [None])[0]
         return result
 
@@ -65,22 +62,29 @@
                 }
                 for k, v in stack_params.items()
             ]
             result = {
                 "StackName": nested_stack_name,
                 "TemplateURL": params.get("TemplateURL"),
                 "Parameters": stack_params,
-                # "Outputs":
             }
             return result
 
-        def result_handler(result, *args, **kwargs):
+        def result_handler(result, resource_id: str, resources: dict, resource_type: str):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = result["StackId"]
             connect_to().cloudformation.get_waiter("stack_create_complete").wait(
                 StackName=result["StackId"]
             )
+            # set outputs
+            stack_details = connect_to().cloudformation.describe_stacks(
+                StackName=result["StackId"]
+            )["Stacks"][0]
+            if "Outputs" in stack_details:
+                resource["Properties"]["Outputs"] = stack_details["Outputs"]
 
         return {
             "create": {
                 "function": "create_stack",
                 "parameters": get_nested_stack_params,
                 "result_handler": result_handler,
             }
@@ -88,17 +92,14 @@
 
 
 class CloudFormationMacro(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::CloudFormation::Macro"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("Name")
-
     def fetch_state(self, stack_name, resources):
         return get_cloudformation_store().macros.get(self.props.get("Name"))
 
     @classmethod
     def get_deploy_templates(cls):
         def _store_macro(resource_id, resources, resource_type, func, stack_name):
             resource = resources[resource_id]
@@ -108,17 +109,24 @@
 
         def _delete_macro(resource_id, resources, resource_type, func, stack_name):
             resource = resources[resource_id]
             properties = resource["Properties"]
             name = properties["Name"]
             get_cloudformation_store().macros.pop(name)
 
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = resource["Properties"]["Name"]
+
         return {
             "create": {
                 "function": _store_macro,
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": _delete_macro,
             },
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,14 @@
         return "AWS::CloudWatch::Alarm"
 
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "Arn":
             return self.props.get("AlarmArn")
         return super(CloudWatchAlarm, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        if attribute == "Arn":
-            return self.props.get("AlarmArn")
-        return self.props.get("AlarmName")
-
     def _response_name(self):
         return "MetricAlarms"
 
     @classmethod
     def _create_function_name(self):
         return "put_metric_alarm"
 
@@ -37,19 +32,23 @@
         if not role_name:
             resource["Properties"]["AlarmName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
+        def _handle_result(result, resource_id, resources, resource_type):
+            resource = resources[resource_id]
+            resources[resource_id]["PhysicalResourceId"] = resource["Properties"]["AlarmName"]
+
         def get_delete_params(params, **kwargs):
             return {"AlarmNames": [params["AlarmName"]]}
 
         return {
-            "create": {"function": cls._create_function_name()},
+            "create": {"function": cls._create_function_name(), "result_handler": _handle_result},
             "delete": {"function": "delete_alarms", "parameters": get_delete_params},
         }
 
 
 class CloudWatchCompositeAlarm(CloudWatchAlarm):
     @staticmethod
     def cloudformation_type():
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/dynamodb.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,32 +76,31 @@
             return self.props.get("TableArn", self.props.get("Table", {}).get("TableArn"))
         value = self.props.get("Table", {}).get(actual_attribute)
         if value:
             return value
 
         return super(DynamoDBTable, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        if attribute == "Arn":
-            return self.props.get("Table", {}).get("TableArn")
-        return self.props.get("TableName")
-
     def fetch_state(self, stack_name, resources):
         table_name = self.props.get("TableName") or self.logical_resource_id
         return aws_stack.connect_to_service("dynamodb").describe_table(TableName=table_name)
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         table_name = resource.get("Properties", {}).get("TableName")
         resource["Properties"]["TableName"] = table_name or generate_default_name(
             stack_name, resource["LogicalResourceId"]
         )
 
     @classmethod
     def get_deploy_templates(cls):
+        def _set_attributes(result: dict, resource_id: str, resources: dict, resource_type: str):
+            resources[resource_id]["PhysicalResourceId"] = result["TableDescription"]["TableName"]
+            resources[resource_id]["Properties"]["Table"] = result["TableDescription"]
+
         return {
             "create": [
                 {
                     "function": "create_table",
                     "parameters": {
                         "TableName": "TableName",
                         "AttributeDefinitions": "AttributeDefinitions",
@@ -114,14 +113,15 @@
                             common.merge_dicts(
                                 params.get("StreamSpecification"),
                                 {"StreamEnabled": True},
                                 default=None,
                             )
                         ),
                     },
+                    "result_handler": _set_attributes,
                 },
                 {
                     "function": "enable_kinesis_streaming_destination",
                     "parameters": get_ddb_kinesis_stream_specification,
                 },
             ],
             "delete": {
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/ec2.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,14 @@
     def fetch_state(self, stack_name, resources):
         client = aws_stack.connect_to_service("ec2")
         if not self.physical_resource_id:
             return None
         result = client.describe_route_tables(RouteTableIds=[self.physical_resource_id])
         return (result["RouteTables"] or [None])[0]
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.physical_resource_id or self.props.get("RouteTableId")
-
     @staticmethod
     def get_deploy_templates():
         def _store_id(result, resource_id, resources, resource_type):
             resources[resource_id]["PhysicalResourceId"] = result["RouteTable"]["RouteTableId"]
 
         return {
             "create": {
@@ -65,22 +62,14 @@
                 r
                 for r in routes
                 if r.get("DestinationCidrBlock") == (dst_cidr or "_not_set_")
                 or r.get("DestinationIpv6CidrBlock") == (dst_cidr6 or "_not_set_")
             ]
             return (route or [None])[0]
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        props = self.props
-        return generate_route_id(
-            props.get("RouteTableId"),
-            props.get("DestinationCidrBlock"),
-            props.get("DestinationIpv6CidrBlock"),
-        )
-
     @staticmethod
     def get_deploy_templates():
         def _id(result, resource_id, resources, resource_type):
             resource_props = resources[resource_id]["Properties"]
 
             resources[resource_id]["PhysicalResourceId"] = generate_route_id(
                 resource_props["RouteTableId"],
@@ -155,27 +144,30 @@
         if route_table:
             associations = route_table.get("Associations", [])
             association = [a for a in associations if a.get("GatewayId") == gw_id]
             if subnet_id:
                 association = [a for a in associations if a.get("SubnetId") == subnet_id]
             return (association or [None])[0]
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("RouteTableAssociationId")
-
     @staticmethod
     def get_deploy_templates():
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["AssociationId"]
+
         return {
             "create": {
                 "function": "associate_route_table",
                 "parameters": {
                     "GatewayId": "GatewayId",
                     "RouteTableId": "RouteTableId",
                     "SubnetId": "SubnetId",
                 },
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": "disassociate_route_table",
                 "parameters": {"AssociationId": "RouteTableAssociationId"},
             },
         }
 
@@ -199,37 +191,39 @@
             gateways = [g for g in gateways if g["VpnGatewayId"] == vpngw_id]
         gateway = (gateways or [{}])[0]
         attachments = gateway.get("Attachments") or gateway.get("VpcAttachments") or []
         result = [a for a in attachments if a.get("State") in ("attached", "available")]
         if result:
             return gateway
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        props = self.props
-        gw_id = props.get("VpnGatewayId") or props.get("InternetGatewayId")
-        attachment = (props.get("Attachments") or props.get("VpcAttachments") or [{}])[0]
-        if attachment:
-            result = "%s-%s" % (gw_id, attachment.get("VpcId"))
-            return result
-
     @classmethod
     def get_deploy_templates(cls):
         def _attach_gateway(resource_id, resources, *args, **kwargs):
             client = aws_stack.connect_to_service("ec2")
             resource = cls(resources[resource_id])
             props = resource.props
             igw_id = props.get("InternetGatewayId")
             vpngw_id = props.get("VpnGatewayId")
             vpc_id = props.get("VpcId")
             if igw_id:
-                client.attach_internet_gateway(VpcId=vpc_id, InternetGatewayId=igw_id)
+                return client.attach_internet_gateway(VpcId=vpc_id, InternetGatewayId=igw_id)
             elif vpngw_id:
-                client.attach_vpn_gateway(VpcId=vpc_id, VpnGatewayId=vpngw_id)
+                return client.attach_vpn_gateway(VpcId=vpc_id, VpnGatewayId=vpngw_id)
 
-        return {"create": {"function": _attach_gateway}}
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resource = resources[resource_id]
+            props = resource["Properties"]
+            gw_id = props.get("VpnGatewayId") or props.get("InternetGatewayId")
+            resource["PhysicalResourceId"] = f"{gw_id}-{props['VpcId']}"
+
+        return {
+            "create": {"function": _attach_gateway, "result_handler": _set_physical_resource_id}
+        }
 
 
 class SecurityGroup(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::SecurityGroup"
 
@@ -247,25 +241,14 @@
         return (resp["SecurityGroups"] or [None])[0]
 
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "GroupId":
             return self.props.get("GroupId")
         return super(SecurityGroup, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        if self.physical_resource_id:
-            return self.physical_resource_id
-        # see docs: "[...] Ref returns the resource ID. For SGs without a VPC, Ref returns the resource name."
-        props = self.props
-        if not props.get("GroupId"):
-            return
-        if not props.get("VpcId"):
-            return props.get("GroupName")
-        return props.get("GroupId")
-
     @staticmethod
     def add_defaults(resource, stack_name: str):
         role_name = resource.get("Properties", {}).get("GroupName")
         if not role_name:
             resource["Properties"]["GroupName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
@@ -306,17 +289,14 @@
         filters = [
             {"Name": "cidr-block", "Values": [props["CidrBlock"]]},
             {"Name": "vpc-id", "Values": [props["VpcId"]]},
         ]
         subnets = client.describe_subnets(Filters=filters)["Subnets"]
         return (subnets or [None])[0]
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("SubnetId")
-
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "SubnetId":
             return self.props.get("SubnetId")
         return super(EC2Subnet, self).get_cfn_attribute(attribute_name)
 
     @classmethod
     def get_deploy_templates(cls):
@@ -464,17 +444,14 @@
                 {
                     "function": "delete_vpc",
                     "parameters": ["VpcId"],
                 },
             ],
         }
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.physical_resource_id or self.props.get("VpcId")
-
 
 class EC2NatGateway(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::NatGateway"
 
     def fetch_state(self, stack_name, resources):
@@ -491,32 +468,35 @@
             for gw in result
             if assoc_id in [ga["AllocationId"] for ga in gw["NatGatewayAddresses"]]
         ]
         return (result or [None])[0]
 
     @staticmethod
     def get_deploy_templates():
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["NatGateway"]["NatGatewayId"]
+
         return {
             "create": {
                 "function": "create_nat_gateway",
                 "parameters": {
                     "SubnetId": "SubnetId",
                     "AllocationId": "AllocationId",
                     "TagSpecifications": get_tags_param("natgateway"),
                 },
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": "delete_nat_gateway",
                 "parameters": ["NatGatewayId"],
             },
         }
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.physical_resource_id or self.props.get("NatGatewayId")
-
 
 class EC2Instance(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::EC2::Instance"
 
     def fetch_state(self, stack_name, resources):
@@ -545,17 +525,14 @@
         instance_id = self.get_physical_resource_id()
         client = client or aws_stack.connect_to_service("ec2")
         resp = client.describe_instances(InstanceIds=[instance_id])
         reservation = (resp.get("Reservations") or [{}])[0]
         result = (reservation.get("Instances") or [None])[0]
         return result
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.physical_resource_id or self.props.get("InstanceId")
-
     @staticmethod
     def add_defaults(resource, stack_name: str):
         props = resource["Properties"]
 
         min_count = props.get("MinCount")
         if min_count is None:
             props["MinCount"] = 1
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/ecr.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,14 @@
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "Arn":
             return self.props.get("repositoryArn")
         if attribute_name == "RepositoryUri":
             return self.props.get("repositoryUri")
         return super(ECRRepository, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        repo_name = self.props.get("RepositoryName")
-        return arns.get_ecr_repository_arn(repo_name)
-
     def fetch_state(self, stack_name, resources):
         repo_name = default_repos_per_stack.get(stack_name)
         if repo_name:
             return {
                 "repositoryArn": arns.get_ecr_repository_arn(repo_name),
                 "registryId": "000000000000",
                 "repositoryName": repo_name,
@@ -56,15 +52,25 @@
                 "Creating a Mock ECR Repository for CloudFormation. This is only intended to be used for allowing a successful CDK bootstrap and does not provision any underlying ECR repository."
             )
 
         def _delete_repo(resource_id, resources, resource_type, func, stack_name):
             if default_repos_per_stack.get(stack_name):
                 del default_repos_per_stack[stack_name]
 
+        def _set_physical_resource_id(result, resource_id, resources, resource_type):
+            resource = resources[resource_id]
+            repo_name = resource["Properties"]["RepositoryName"]
+            resource["PhysicalResourceId"] = arns.get_ecr_repository_arn(repo_name)
+
+            # add in some properties required for GetAtt and Ref
+            resource["Properties"]["repositoryArn"] = arns.get_ecr_repository_arn(repo_name)
+            resource["Properties"]["repositoryUri"] = "http://localhost:4566"
+
         return {
             "create": {
                 "function": _create_repo,
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": _delete_repo,
             },
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from localstack.aws.api.es import CreateElasticsearchDomainRequest
+from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.deployment_utils import remove_none_values
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.utils.aws import arns, aws_stack
 from localstack.utils.collections import convert_to_typed_dict
 
 
 def es_add_tags_params(params, **kwargs):
@@ -12,20 +13,14 @@
 
 
 class ElasticsearchDomain(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Elasticsearch::Domain"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        domain_name = self._domain_name()
-        if attribute == "Arn":
-            return arns.elasticsearch_domain_arn(domain_name)
-        return domain_name
-
     def get_cfn_attribute(self, attribute_name):
         if attribute_name in ["Arn", "DomainArn"]:
             domain_name = self._domain_name()
             return arns.elasticsearch_domain_arn(domain_name)
         if attribute_name == "DomainEndpoint":
             domain_status = self.props.get("DomainStatus", {})
             result = domain_status.get("Endpoint")
@@ -50,19 +45,31 @@
             cluster_config = result.get("ElasticsearchClusterConfig")
             if isinstance(cluster_config, dict):
                 # set defaults required for boto3 calls
                 cluster_config.setdefault("DedicatedMasterType", "m3.medium.elasticsearch")
                 cluster_config.setdefault("WarmType", "ultrawarm1.medium.elasticsearch")
             return result
 
+        def _handle_result(result, resource_id, resources, resource_type):
+            resource = resources[resource_id]
+
+            domain_name = resource["Properties"].get("DomainName", resource_id)
+            resource["PhysicalResourceId"] = domain_name
+            # TODO: wait for resource
+            describe_result = connect_to().es.describe_elasticsearch_domain(DomainName=domain_name)[
+                "DomainStatus"
+            ]
+            resource["Properties"]["DomainStatus"] = {"Endpoint": describe_result["Endpoint"]}
+
         return {
             "create": [
                 {
                     "function": "create_elasticsearch_domain",
                     "parameters": _create_params,
+                    "result_handler": _handle_result,
                 },
                 {"function": "add_tags", "parameters": es_add_tags_params},
             ],
             "delete": {
                 "function": "delete_elasticsearch_domain",
                 "parameters": {"DomainName": "DomainName"},
             },
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,14 @@
         return "AWS::Events::Rule"
 
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "Arn":
             return self.props.get("Arn") or arns.events_rule_arn(self.props.get("Name"))
         return super(EventsRule, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("Name")
-
     def fetch_state(self, stack_name, resources):
         rule_name = self.props.get("Name")
 
         kwargs = {"Name": rule_name}
         if bus_name := self.props.get("EventBusName"):
             kwargs["EventBusName"] = bus_name
 
@@ -154,17 +151,26 @@
             event_bus_name = props.get("EventBusName")
             targets = props.get("Targets") or []
             if len(targets) > 0 and event_bus_name:
                 events.put_targets(Rule=rule_name, EventBusName=event_bus_name, Targets=targets)
             elif len(targets) > 0:
                 events.put_targets(Rule=rule_name, Targets=targets)
 
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = resources[resource_id]["Properties"][
+                "Name"
+            ]
+
         return {
             "create": [
-                {"function": "put_rule", "parameters": events_put_rule_params},
+                {
+                    "function": "put_rule",
+                    "parameters": events_put_rule_params,
+                    "result_handler": _handle_result,
+                },
                 {"function": _put_targets},
             ],
             "delete": {"function": _delete_rule},
         }
 
 
 class EventBusPolicy(GenericBaseModel):
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/iam.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 
 
 class IAMManagedPolicy(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::IAM::ManagedPolicy"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return arns.policy_arn(self.props["ManagedPolicyName"])
-
     def fetch_state(self, stack_name, resources):
         return IAMPolicy.get_policy_state(self, stack_name, resources, managed_policy=True)
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         role_name = resource.get("Properties", {}).get("ManagedPolicyName")
         if not role_name:
@@ -57,27 +54,29 @@
             policy_arn = policy["Policy"]["Arn"]
             for role in resource.get("Roles", []):
                 iam.attach_role_policy(RoleName=role, PolicyArn=policy_arn)
             for user in resource.get("Users", []):
                 iam.attach_user_policy(UserName=user, PolicyArn=policy_arn)
             for group in resource.get("Groups", []):
                 iam.attach_group_policy(GroupName=group, PolicyArn=policy_arn)
-            return {}
+            return policy
+
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["Policy"]["Arn"]
 
-        return {"create": {"function": _create}}
+        return {"create": {"function": _create, "result_handler": _set_physical_resource_id}}
 
 
 class IAMUser(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::IAM::User"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("UserName")
-
     def fetch_state(self, stack_name, resources):
         user_name = self.props.get("UserName")
         return aws_stack.connect_to_service("iam").get_user(UserName=user_name)["User"]
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         role_name = resource["Properties"].get("UserName")
@@ -134,19 +133,25 @@
                 client.remove_user_from_group(UserName=user_name, GroupName=group)
 
             # TODO: remove this after stack resource deletion order is fixed
             remaining_policies = client.list_user_policies(UserName=user_name)["PolicyNames"]
             for inline_policy_name in remaining_policies:
                 client.delete_user_policy(UserName=user_name, PolicyName=inline_policy_name)
 
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["User"]["UserName"]
+
         return {
             "create": [
                 {
                     "function": "create_user",
                     "parameters": ["Path", "UserName", "PermissionsBoundary", "Tags"],
+                    "result_handler": _set_physical_resource_id,
                 },
                 {"function": _post_create},
             ],
             "delete": [
                 {"function": _pre_delete},
                 {
                     "function": "delete_user",
@@ -157,17 +162,14 @@
 
 
 class IAMAccessKey(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::IAM::AccessKey"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.physical_resource_id
-
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "SecretAccessKey":
             return self.props.get("SecretAccessKey")
 
     def fetch_state(self, stack_name, resources):
         user_name = self.props.get("UserName")
         access_key_id = self.get_physical_resource_id()
@@ -232,22 +234,14 @@
         return "AWS::IAM::Role"
 
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "Arn":
             return self.props.get("Arn")
         return super(IAMRole, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        role_name = self.properties.get("RoleName")
-        if not role_name:
-            return role_name
-        if attribute == "Arn":
-            return arns.role_arn(role_name)
-        return role_name
-
     def fetch_state(self, stack_name, resources):
         role_name = self.props.get("RoleName")
         client = connect_to().iam
         return client.get_role(RoleName=role_name)["Role"]
 
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
@@ -371,14 +365,19 @@
                 )
         except Exception as e:
             if "NoSuchEntity" not in str(e):
                 raise
 
     @classmethod
     def get_deploy_templates(cls):
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["Role"]["RoleName"]
+
         return {
             "create": [
                 {
                     "function": "create_role",
                     "parameters": param_defaults(
                         dump_json_params(
                             select_parameters(
@@ -390,14 +389,15 @@
                                 "PermissionsBoundary",
                                 "Tags",
                             ),
                             "AssumeRolePolicyDocument",
                         ),
                         {"RoleName": "RoleName"},
                     ),
+                    "result_handler": _set_physical_resource_id,
                 },
                 {"function": IAMRole._post_create},
             ],
             "delete": [
                 {"function": IAMRole._pre_delete},
                 {"function": "delete_role", "parameters": {"RoleName": "RoleName"}},
             ],
@@ -417,21 +417,26 @@
         for role in roles:
             policy = role.get("AssumeRolePolicyDocument") or "{}"
             policy = json.loads(policy or "{}") if isinstance(policy, str) else policy
             statements = policy.get("Statement")
             if statements and statements[0].get("Principal") == {"Service": service_name}:
                 return role
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("RoleName")
-
     @classmethod
     def get_deploy_templates(cls):
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["Role"]["RoleName"]
+
         return {
-            "create": {"function": "create_service_linked_role"},
+            "create": {
+                "function": "create_service_linked_role",
+                "result_handler": _set_physical_resource_id,
+            },
             "delete": {"function": "delete_service_linked_role", "parameters": ["RoleName"]},
         }
 
 
 class IAMPolicy(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
@@ -547,17 +552,14 @@
         instance_profile_name = self.get_physical_resource_id()
         if not instance_profile_name:
             return None
         client = aws_stack.connect_to_service("iam")
         resp = client.get_instance_profile(InstanceProfileName=instance_profile_name)
         return resp["InstanceProfile"]
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.physical_resource_id or self.props.get("InstanceProfileName")
-
     @staticmethod
     def add_defaults(resource, stack_name):
         role_name = resource.get("Properties", {}).get("InstanceProfileName")
         if not role_name:
             resource["Properties"]["InstanceProfileName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
@@ -620,17 +622,14 @@
 
 
 class IAMGroup(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::IAM::Group"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("GroupName")
-
     def fetch_state(self, stack_name, resources):
         group_name = self.props.get("GroupName")
         return aws_stack.connect_to_service("iam").get_group(GroupName=group_name)["Group"]
 
     def update_resource(self, new_resource, stack_name, resources):
         props = new_resource["Properties"]
         return aws_stack.connect_to_service("iam").update_group(
@@ -673,19 +672,25 @@
                 )
 
             # TODO: remove this after stack resource deletion order is fixed
             remaining_policies = client.list_group_policies(GroupName=group_name)["PolicyNames"]
             for inline_policy_name in remaining_policies:
                 client.delete_group_policy(GroupName=group_name, PolicyName=inline_policy_name)
 
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["Group"]["GroupName"]
+
         return {
             "create": [
                 {
                     "function": "create_group",
                     "parameters": ["GroupName", "Path"],
+                    "result_handler": _set_physical_resource_id,
                 },
                 {"function": _post_create},
             ],
             "delete": [
                 {"function": _pre_delete},
                 {
                     "function": "delete_group",
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/kinesis.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,42 +4,43 @@
 
 
 class KinesisStreamConsumer(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Kinesis::StreamConsumer"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("ConsumerARN")
-
     def fetch_state(self, stack_name, resources):
         props = self.props
         stream_arn = props["StreamARN"]
         result = aws_stack.connect_to_service("kinesis").list_stream_consumers(StreamARN=stream_arn)
         result = [r for r in result["Consumers"] if r["ConsumerName"] == props["ConsumerName"]]
         return (result or [None])[0]
 
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = result["Consumer"]["ConsumerARN"]
+            resource["Properties"]["ConsumerARN"] = result["Consumer"]["ConsumerARN"]
+            resource["Properties"]["ConsumerCreationTimestamp"] = result["Consumer"][
+                "ConsumerCreationTimestamp"
+            ]
+            resource["Properties"]["ConsumerStatus"] = result["Consumer"]["ConsumerStatus"]
+
         return {
-            "create": {"function": "register_stream_consumer"},
+            "create": {"function": "register_stream_consumer", "result_handler": _handle_result},
             "delete": {"function": "deregister_stream_consumer"},
         }
 
 
 class KinesisStream(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Kinesis::Stream"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        if attribute == "Arn":
-            return self.props.get("Arn")
-        return self.physical_resource_id
-
     def fetch_state(self, stack_name, resources):
         stream_name = self.props["Name"]
         result = aws_stack.connect_to_service("kinesis").describe_stream(StreamName=stream_name)
         return result
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 from localstack.services.cloudformation.deployment_utils import select_parameters
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import aws_stack
 
 
 class FirehoseDeliveryStream(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::KinesisFirehose::DeliveryStream"
 
     def fetch_state(self, stack_name, resources):
         stream_name = self.props.get("DeliveryStreamName") or self.logical_resource_id
         return aws_stack.connect_to_service("firehose").describe_delivery_stream(
             DeliveryStreamName=stream_name
         )
 
-    def get_cfn_attribute(self, attribute_name):
-        if attribute_name == "Arn":
-            return arns.firehose_stream_arn(self.props.get("DeliveryStreamName"))
-        return super().get_cfn_attribute(attribute_name)
-
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        if attribute == "Arn":
-            return self.get_cfn_attribute("Arn")
-        return self.props.get("DeliveryStreamName")
-
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["Properties"]["Arn"] = result["DeliveryStreamARN"]
+            resources[resource_id]["PhysicalResourceId"] = resources[resource_id]["Properties"][
+                "DeliveryStreamName"
+            ]
+
         return {
             "create": {
                 "function": "create_delivery_stream",
                 "parameters": select_parameters(
                     "DeliveryStreamName",
                     "DeliveryStreamType",
                     "S3DestinationConfiguration",
@@ -39,13 +35,14 @@
                     "ExtendedS3DestinationConfiguration",
                     "HttpEndpointDestinationConfiguration",
                     "KinesisStreamSourceConfiguration",
                     "RedshiftDestinationConfiguration",
                     "SplunkDestinationConfiguration",
                     "Tags",
                 ),
+                "result_handler": _handle_result,
             },
             "delete": {
                 "function": "delete_delivery_stream",
                 "parameters": {"DeliveryStreamName": "DeliveryStreamName"},
             },
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/kms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 
 from localstack.aws.connect import connect_to
 from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.utils.aws import arns, aws_stack
-from localstack.utils.common import short_uid
 
 
 class KMSKey(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::KMS::Key"
 
@@ -37,28 +36,14 @@
                     #  chain the 'PhysicalResourceId' gets overwritten with None, hence setting it here
                     self.resource_json["PhysicalResourceId"] = physical_res_id
                     break
         if not physical_res_id:
             return
         return client.describe_key(KeyId=physical_res_id)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        # TODO: ?
-        return self.physical_resource_id and arns.kms_key_arn(self.physical_resource_id)
-
-    # TODO: try to remove this workaround (ensures idempotency)
-    @staticmethod
-    def add_defaults(resource, stack_name: str):
-        props = resource["Properties"] = resource.get("Properties", {})
-        tags = props["Tags"] = props.get("Tags", [])
-        existing = [t for t in tags if t["Key"] == "localstack-key-id"]
-        if not existing:
-            # append tags, to allow us to determine in fetch_state whether this key is already deployed
-            tags.append({"Key": "localstack-key-id", "Value": short_uid()})
-
     @classmethod
     def get_deploy_templates(cls):
         def _create(resource_id, resources, resource_type, func, stack_name):
             kms_client = aws_stack.connect_to_service("kms")
             resource = cls(resources[resource_id])
             props = resource.props
             params = {}
@@ -107,29 +92,33 @@
 
 
 class KMSAlias(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::KMS::Alias"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("AliasName")
-
     def fetch_state(self, stack_name, resources):
         aliases = connect_to().kms.list_aliases()["Aliases"]
         for alias in aliases:
             if alias["AliasName"] == self.props.get("AliasName"):
                 return alias
         return None
 
     @staticmethod
     def get_deploy_templates():
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = resource["Properties"]["AliasName"]
+
         return {
             "create": {
                 "function": "create_alias",
                 "parameters": {"AliasName": "AliasName", "TargetKeyId": "TargetKeyId"},
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": "delete_alias",
                 "parameters": {"AliasName": "AliasName"},
             },
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/logs.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,19 +10,14 @@
 
     def get_cfn_attribute(self, attribute_name):
         props = self.props
         if attribute_name == "Arn":
             return props.get("arn")
         return super(LogsLogGroup, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        if attribute == "Arn":
-            return self.get_cfn_attribute("Arn")
-        return self.props.get("LogGroupName")
-
     def fetch_state(self, stack_name, resources):
         group_name = self.props.get("LogGroupName")
         logs = aws_stack.connect_to_service("logs")
         groups = logs.describe_log_groups(logGroupNamePrefix=group_name)["logGroups"]
         return ([g for g in groups if g["logGroupName"] == group_name] or [None])[0]
 
     @staticmethod
@@ -31,18 +26,25 @@
         if not name:
             resource["Properties"]["LogGroupName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = resource["Properties"]["LogGroupName"]
+
         return {
             "create": {
                 "function": "create_log_group",
                 "parameters": {"logGroupName": "LogGroupName"},
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": "delete_log_group",
                 "parameters": {"logGroupName": "LogGroupName"},
             },
         }
 
@@ -51,17 +53,14 @@
     @staticmethod
     def cloudformation_type():
         return "AWS::Logs::LogStream"
 
     def get_cfn_attribute(self, attribute_name):
         return super(LogsLogStream, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("LogStreamName")
-
     def fetch_state(self, stack_name, resources):
         group_name = self.props.get("LogGroupName")
         stream_name = self.props.get("LogStreamName")
         logs = aws_stack.connect_to_service("logs")
         streams = logs.describe_log_streams(
             logGroupName=group_name, logStreamNamePrefix=stream_name
         )["logStreams"]
@@ -73,54 +72,65 @@
         if not name:
             resource["Properties"]["LogStreamName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = resource["Properties"]["LogStreamName"]
+
         return {
             "create": {
                 "function": "create_log_stream",
                 "parameters": {"logGroupName": "LogGroupName", "logStreamName": "LogStreamName"},
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": "delete_log_stream",
                 "parameters": {"logGroupName": "LogGroupName", "logStreamName": "LogStreamName"},
             },
         }
 
 
 class LogsSubscriptionFilter(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Logs::SubscriptionFilter"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("LogGroupName")
-
     def fetch_state(self, stack_name, resources):
         props = self.props
         group_name = props.get("LogGroupName")
         filter_pattern = props.get("FilterPattern")
         logs = aws_stack.connect_to_service("logs")
         groups = logs.describe_subscription_filters(logGroupName=group_name)["subscriptionFilters"]
         groups = [g for g in groups if g.get("filterPattern") == filter_pattern]
         return (groups or [None])[0]
 
     @staticmethod
     def get_deploy_templates():
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = resource["Properties"]["LogGroupName"]
+
         return {
             "create": {
                 "function": "put_subscription_filter",
                 "parameters": {
                     "logGroupName": "LogGroupName",
                     "filterName": "LogGroupName",  # there can only be one filter associated with a log group
                     "filterPattern": "FilterPattern",
                     "destinationArn": "DestinationArn",
                 },
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": "delete_subscription_filter",
                 "parameters": {
                     "logGroupName": "LogGroupName",
                     "filterName": "LogGroupName",
                 },
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/opensearch.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,21 +19,14 @@
 
 
 class OpenSearchDomain(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::OpenSearchService::Domain"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        domain_name = self._domain_name()
-        if attribute == "Arn":
-            # As mentioned above, OpenSearch still uses "es" ARNs
-            return arns.elasticsearch_domain_arn(domain_name)
-        return domain_name
-
     def fetch_state(self, stack_name, resources):
         domain_name = self._domain_name()
         return aws_stack.connect_to_service("opensearch").describe_domain(DomainName=domain_name)
 
     def _domain_name(self):
         return self.props.get("DomainName") or self.logical_resource_id
 
@@ -49,19 +42,25 @@
                     "DedicatedMasterType", OpenSearchPartitionInstanceType.m3_medium_search
                 )
                 cluster_config.setdefault(
                     "WarmType", OpenSearchWarmPartitionInstanceType.ultrawarm1_medium_search
                 )
             return result
 
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["DomainStatus"]["DomainName"]
+
         return {
             "create": [
                 {
                     "function": "create_domain",
                     "parameters": _create_params,
+                    "result_handler": _set_physical_resource_id,
                 },
                 {"function": "add_tags", "parameters": opensearch_add_tags_params},
             ],
             "delete": {
                 "function": "delete_domain",
                 "parameters": {"DomainName": "DomainName"},
             },
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/redshift.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 
 class RedshiftCluster(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Redshift::Cluster"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("ClusterIdentifier")
-
     def fetch_state(self, stack_name, resources):
         client = aws_stack.connect_to_service("redshift")
         cluster_id = self.props.get("ClusterIdentifier")
         result = client.describe_clusters(ClusterIdentifier=cluster_id)["Clusters"]
         return (result or [None])[0]
 
     @staticmethod
@@ -23,8 +20,11 @@
         if not role_name:
             resource["Properties"]["ClusterIdentifier"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @staticmethod
     def get_deploy_templates():
-        return {"create": {"function": "create_cluster"}}
+        def _handle_result(result, resource_id, resources, resource_type):
+            resources[resource_id]["PhysicalResourceId"] = result["Cluster"]["ClusterIdentifier"]
+
+        return {"create": {"function": "create_cluster", "result_handler": _handle_result}}
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,25 +14,28 @@
         result = [g for g in result if g["Name"] == self.props["Name"]]
         return (result or [None])[0]
 
     def get_cfn_attribute(self, attribute_name):
         if attribute_name == "Arn":
             return self.props.get("GroupArn")
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("Name")
-
     @classmethod
     def get_deploy_templates(cls):
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["Group"]["Name"]
+
         return {
             "create": {
                 "function": "create_group",
                 "parameters": {
                     "Name": "Name",
                     "Description": "Description",
                     "ResourceQuery": "ResourceQuery",
                     "Configuration": "Configuration",
                     "Tags": params_list_to_dict("Tags"),
                 },
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {"function": "delete_group", "parameters": {"Group": "Name"}},
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/route53.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 
 class Route53RecordSet(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::Route53::RecordSet"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("Name")  # Ref attribute is the domain name itself
-
     def fetch_state(self, stack_name, resources):
         route53 = aws_stack.connect_to_service("route53")
         props = self.props
         result = route53.list_resource_record_sets(HostedZoneId=props["HostedZoneId"])[
             "ResourceRecordSets"
         ]
         result = [r for r in result if r["Name"] == props["Name"] and r["Type"] == props["Type"]]
@@ -66,16 +63,21 @@
                 ]
                 if len(hosted_zones) != 1:
                     raise Exception(f"Ambiguous HostedZoneName {hosted_zone_name} provided.")
                 hosted_zone = hosted_zones[0]
                 hosted_zone_id = hosted_zone.get("Id")
             return hosted_zone_id
 
+        def _handle_result(result, resource_id, resources, resource_type):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = resource["Properties"]["Name"]
+
         return {
             "create": {
                 "function": "change_resource_record_sets",
                 "parameters": {
                     "HostedZoneId": hosted_zone_id_change_batch,
                     "ChangeBatch": param_change_batch,
                 },
+                "result_handler": _handle_result,
             }
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/s3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import re
 
 from botocore.exceptions import ClientError
 
 from localstack.config import get_edge_port_http
 from localstack.constants import S3_STATIC_WEBSITE_HOSTNAME, S3_VIRTUAL_HOSTNAME
 from localstack.services.cloudformation.cfn_utils import rename_params
@@ -18,31 +17,36 @@
 
 
 class S3BucketPolicy(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::S3::BucketPolicy"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        policy = self.props.get("Policy")
-        return policy and md5(canonical_json(json.loads(policy)))
-
     def fetch_state(self, stack_name, resources):
         bucket_name = self.props.get("Bucket") or self.logical_resource_id
         return aws_stack.connect_to_service("s3").get_bucket_policy(Bucket=bucket_name)
 
     @staticmethod
     def get_deploy_templates():
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = md5(
+                canonical_json(resource["Properties"]["PolicyDocument"])
+            )
+
         return {
             "create": {
                 "function": "put_bucket_policy",
                 "parameters": rename_params(
                     dump_json_params(None, "PolicyDocument"),
                     {"PolicyDocument": "Policy", "Bucket": "Bucket"},
                 ),
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {"function": "delete_bucket_policy", "parameters": {"Bucket": "Bucket"}},
         }
 
 
 class S3Bucket(GenericBaseModel):
     @staticmethod
@@ -158,14 +162,20 @@
                     "LambdaFunctionConfigurations": lambda_configs,
                     "QueueConfigurations": queue_configs,
                     "TopicConfigurations": topic_configs,
                 },
             }
             return result
 
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = resource["Properties"]["BucketName"]
+
         def _pre_delete(resource_id, resources, resource_type, func, stack_name):
             s3 = aws_stack.connect_to_service("s3")
             resource = resources[resource_id]
             props = resource["Properties"]
             bucket_name = props.get("BucketName")
             try:
                 s3.delete_bucket_policy(Bucket=bucket_name)
@@ -246,15 +256,18 @@
                         params["CreateBucketConfiguration"] = {
                             "LocationConstraint": aws_stack.get_region()
                         }
                     s3_client.create_bucket(**params)
 
         result = {
             "create": [
-                {"function": _create_bucket},
+                {
+                    "function": _create_bucket,
+                    "result_handler": _set_physical_resource_id,
+                },
                 {
                     "function": "put_bucket_notification_configuration",
                     "parameters": s3_bucket_notification_config,
                 },
                 {"function": _put_bucket_versioning},
                 {"function": _put_bucket_cors_configuration},
                 {"function": _add_bucket_tags},
@@ -305,15 +318,9 @@
             #   https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html
             #   "Amazon S3 website endpoints do not support HTTPS. If you want to use HTTPS,
             #   you can use Amazon CloudFront [...]"
             return f"http://{bucket_name}.{S3_STATIC_WEBSITE_HOSTNAME}:{get_edge_port_http()}"
 
         return super(S3Bucket, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        bucket_name = self.props.get("BucketName")
-        if attribute == "Arn":
-            return arns.s3_bucket_arn(bucket_name)
-        return bucket_name
-
     def _get_bucket_name(self):
         return self.props.get("BucketName") or self.logical_resource_id
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 
 
 class SecretsManagerSecret(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::SecretsManager::Secret"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("ARN")
+    def get_cfn_attribute(self, attribute_name: str):
+        match attribute_name:
+            case "Id":
+                return self.properties["Name"]
 
-    def get_cfn_attribute(self, attribute_name):
         return super(SecretsManagerSecret, self).get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
         secret_name = self.props.get("Name") or self.logical_resource_id
         result = aws_stack.connect_to_service("secretsmanager").describe_secret(
             SecretId=secret_name
         )
@@ -104,57 +105,54 @@
                     gen_key = gen_secret.get("GenerateStringKey") or "secret"
                     template = json.loads(template)
                     template[gen_key] = secret_value
                     secret_value = json.dumps(template)
                 result["SecretString"] = secret_value
             return result
 
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["ARN"]
+
         return {
             "create": {
                 "function": "create_secret",
                 "parameters": _create_params,
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {"function": "delete_secret", "parameters": {"SecretId": "Name"}},
         }
 
 
 class SecretsManagerSecretTargetAttachment(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::SecretsManager::SecretTargetAttachment"
 
-    def get_physical_resource_id(self, attribute, **kwargs):
-        return arns.secretsmanager_secret_arn(self.props.get("SecretId"))
-
     def fetch_state(self, stack_name, resources):
         # TODO implement?
         return {"state": "dummy"}
 
 
 class SecretsManagerRotationSchedule(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::SecretsManager::RotationSchedule"
 
-    def get_physical_resource_id(self, attribute, **kwargs):
-        return arns.secretsmanager_secret_arn(self.props.get("SecretId"))
-
     def fetch_state(self, stack_name, resources):
         # TODO implement?
         return {"state": "dummy"}
 
 
 class SecretsManagerResourcePolicy(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::SecretsManager::ResourcePolicy"
 
-    def get_physical_resource_id(self, attribute, **kwargs):
-        return arns.secretsmanager_secret_arn(self.props.get("SecretId"))
-
     def fetch_state(self, stack_name, resources):
         secret_id = self.props.get("SecretId")
         result = aws_stack.connect_to_service("secretsmanager").get_resource_policy(
             SecretId=secret_id
         )
         return result
 
@@ -163,14 +161,26 @@
         def create_params(params, **kwargs):
             return {
                 "SecretId": params["SecretId"].split(":")[-1],
                 "ResourcePolicy": json.dumps(params["ResourcePolicy"]),
                 "BlockPublicPolicy": params.get("BlockPublicPolicy"),
             }
 
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = arns.secretsmanager_secret_arn(
+                resource["Properties"]["Name"]
+            )
+
         return {
-            "create": {"function": "put_resource_policy", "parameters": create_params},
+            "create": {
+                "function": "put_resource_policy",
+                "parameters": create_params,
+                "result_handler": _set_physical_resource_id,
+            },
             "delete": {
                 "function": "delete_resource_policy",
                 "parameters": {"SecretId": "SecretId"},
             },
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/sns.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 from botocore.exceptions import ClientError
 
 from localstack.services.cloudformation.deployment_utils import (
     generate_default_name,
     is_none_or_empty_value,
 )
 from localstack.services.cloudformation.service_models import GenericBaseModel
-from localstack.utils.aws import arns, aws_stack
+from localstack.utils.aws import aws_stack
 from localstack.utils.common import canonicalize_bool_to_str
 
 
 class SNSTopic(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::SNS::Topic"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return arns.sns_topic_arn(self.props["TopicName"])
-
     def fetch_state(self, stack_name, resources):
         topic_name = self.props["TopicName"]
         topics = aws_stack.connect_to_service("sns").list_topics()
         result = list(
             filter(
                 lambda item: item["TopicArn"].split(":")[-1] == topic_name,
                 topics.get("Topics", []),
@@ -57,15 +54,15 @@
             if kms_master_key:
                 attributes["KmsMasterKeyId"] = kms_master_key
             result = {"Name": topic_name, "Attributes": attributes, "Tags": tags}
             return result
 
         def _topic_arn(params, resources, resource_id, **kwargs):
             resource = cls(resources[resource_id])
-            return resource.physical_resource_id or resource.get_physical_resource_id()
+            return resource.physical_resource_id
 
         def _list_all_topics(sns_client):
             rs = sns_client.list_topics()
             topics = rs.get("Topics", [])
             key = rs.get("NextToken")
 
             while key and key != "":
@@ -114,17 +111,14 @@
 
 
 class SNSSubscription(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::SNS::Subscription"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("SubscriptionArn")
-
     def fetch_state(self, stack_name, resources):
         props = self.props
         topic_arn = props.get("TopicArn")
         if topic_arn is None:
             return
         subs = aws_stack.connect_to_service("sns").list_subscriptions_by_topic(TopicArn=topic_arn)
         result = [
@@ -150,23 +144,29 @@
                 "FilterPolicy",
                 "RawMessageDelivery",
                 "RedrivePolicy",
             ]
             result = {a: attr_val(params[a]) for a in attrs if a in params}
             return result
 
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["SubscriptionArn"]
+
         return {
             "create": {
                 "function": "subscribe",
                 "parameters": {
                     "TopicArn": "TopicArn",
                     "Protocol": "Protocol",
                     "Endpoint": "Endpoint",
                     "Attributes": sns_subscription_params,
                 },
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": "unsubscribe",
                 "parameters": {"SubscriptionArn": sns_subscription_arn},
             },
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/sqs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 from botocore.exceptions import ClientError
 
 from localstack.services.cloudformation.deployment_utils import (
     generate_default_name,
     params_list_to_dict,
     params_select_attributes,
 )
-from localstack.services.cloudformation.service_models import (
-    DependencyNotYetSatisfied,
-    GenericBaseModel,
-)
+from localstack.services.cloudformation.service_models import GenericBaseModel
 from localstack.utils.aws import arns, aws_stack
 from localstack.utils.common import short_uid
 
 LOG = logging.getLogger(__name__)
 
 
 class QueuePolicy(GenericBaseModel):
@@ -30,15 +27,14 @@
     @classmethod
     def get_deploy_templates(cls):
         def _create(resource_id, resources, resource_type, func, stack_name):
             sqs_client = aws_stack.connect_to_service("sqs")
             resource = cls(resources[resource_id])
             props = resource.props
 
-            # TODO: generalize/support in get_physical_resource_id
             resources[resource_id]["PhysicalResourceId"] = "%s-%s-%s" % (
                 stack_name,
                 resource_id,
                 short_uid(),
             )
 
             policy = json.dumps(props["PolicyDocument"])
@@ -66,27 +62,18 @@
 
 
 class SQSQueue(GenericBaseModel):
     @classmethod
     def cloudformation_type(cls):
         return "AWS::SQS::Queue"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        queue_url = None
-        props = self.props
-        try:
-            queue_url = arns.get_sqs_queue_url(props.get("QueueName"))
-        except Exception as e:
-            if "NonExistentQueue" in str(e):
-                raise DependencyNotYetSatisfied(
-                    resource_ids=self.logical_resource_id, message="Unable to get queue: %s" % e
-                )
-        if attribute == "Arn":
-            return arns.sqs_queue_arn(props.get("QueueName"))
-        return queue_url
+    def get_cfn_attribute(self, attribute_name):
+        if attribute_name == "Arn":
+            return arns.sqs_queue_arn(self.properties["QueueName"])
+        return super().get_cfn_attribute(attribute_name)
 
     def fetch_state(self, stack_name, resources):
         queue_name = self.props["QueueName"]
         sqs_client = aws_stack.connect_to_service("sqs")
         queues = sqs_client.list_queues()
         result = list(
             filter(
@@ -121,14 +108,19 @@
             resource = cls(resources[resource_id])
             props = resource.props
             queue_url = resource.physical_resource_id or props.get("QueueUrl")
             if queue_url:
                 return queue_url
             return arns.sqs_queue_url_for_arn(props["QueueArn"])
 
+        def _set_physical_resource_id(
+            result: dict, resource_id: str, resources: dict, resource_type: str
+        ):
+            resources[resource_id]["PhysicalResourceId"] = result["QueueUrl"]
+
         return {
             "create": {
                 "function": "create_queue",
                 "parameters": {
                     "QueueName": "QueueName",
                     "Attributes": params_select_attributes(
                         "ContentBasedDeduplication",
@@ -138,13 +130,14 @@
                         "MessageRetentionPeriod",
                         "VisibilityTimeout",
                         "RedrivePolicy",
                         "ReceiveMessageWaitTimeSeconds",
                     ),
                     "tags": params_list_to_dict("Tags"),
                 },
+                "result_handler": _set_physical_resource_id,
             },
             "delete": {
                 "function": "delete_queue",
                 "parameters": {"QueueUrl": _queue_url},
             },
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/ssm.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 
 
 class SSMParameter(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::SSM::Parameter"
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("Name") or self.logical_resource_id
-
     def fetch_state(self, stack_name, resources):
         param_name = self.props.get("Name") or self.logical_resource_id
         return aws_stack.connect_to_service("ssm").get_parameter(Name=param_name)["Parameter"]
 
     @staticmethod
     def add_defaults(resource, stack_name: str):
         name = resource.get("Properties", {}).get("Name")
@@ -79,14 +76,18 @@
                 ResourceType="Parameter", ResourceId=self.props.get("Name"), Tags=tag_keys_to_remove
             )
 
         return ssm_client.put_parameter(Overwrite=True, **update_config_props)
 
     @staticmethod
     def get_deploy_templates():
+        def _handle_result(result, resource_id, resources, resource_type):
+            resource = resources[resource_id]
+            resource["PhysicalResourceId"] = resource["Properties"]["Name"]
+
         return {
             "create": {
                 "function": "put_parameter",
                 "parameters": merge_parameters(
                     params_dict_to_list("Tags", wrapper="Tags"),
                     select_parameters(
                         "Name",
@@ -95,10 +96,11 @@
                         "Description",
                         "AllowedPattern",
                         "Policies",
                         "Tier",
                     ),
                 ),
                 "types": {"Value": str},
+                "result_handler": _handle_result,
             },
             "delete": {"function": "delete_parameter", "parameters": ["Name"]},
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         client = aws_stack.connect_to_service("stepfunctions")
         result = client.describe_activity(activityArn=activity_arn)
         return result
 
     @staticmethod
     def get_deploy_templates():
         def _store_arn(result, resource_id, resources, resource_type):
+            resources[resource_id]["Properties"]["Arn"] = result["activityArn"]
             resources[resource_id]["PhysicalResourceId"] = result["activityArn"]
 
         return {
             "create": {
                 "function": "create_activity",
                 "parameters": {"name": "Name", "tags": "Tags"},
                 "result_handler": _store_arn,
@@ -42,24 +43,21 @@
 
 
 class SFNStateMachine(GenericBaseModel):
     @staticmethod
     def cloudformation_type():
         return "AWS::StepFunctions::StateMachine"
 
-    def get_cfn_attribute(self, attribute_name):
+    def get_cfn_attribute(self, attribute_name: str):
         if attribute_name == "Arn":
-            return self.props.get("stateMachineArn")
+            return self.props.get("Arn")
         if attribute_name == "Name":
             return self.props.get("StateMachineName")
         return super(SFNStateMachine, self).get_cfn_attribute(attribute_name)
 
-    def get_physical_resource_id(self, attribute=None, **kwargs):
-        return self.props.get("stateMachineArn")
-
     def fetch_state(self, stack_name, resources):
         sm_name = self.props.get("StateMachineName") or self.logical_resource_id
         sfn_client = aws_stack.connect_to_service("stepfunctions")
         state_machines = sfn_client.list_state_machines()["stateMachines"]
         sm_arn = [m["stateMachineArn"] for m in state_machines if m["name"] == sm_name]
         if not sm_arn:
             return None
@@ -85,14 +83,18 @@
         if not role_name:
             resource["Properties"]["StateMachineName"] = generate_default_name(
                 stack_name, resource["LogicalResourceId"]
             )
 
     @classmethod
     def get_deploy_templates(cls):
+        def result_handler(result, resource_id, resources, resource_type):
+            resources[resource_id]["Properties"]["Arn"] = result["stateMachineArn"]
+            resources[resource_id]["PhysicalResourceId"] = result["stateMachineArn"]
+
         def _create_params(params, **kwargs):
             def _get_definition(params):
                 # TODO: support "Definition" parameter
                 definition_str = params.get("DefinitionString")
                 s3_location = params.get("DefinitionS3Location")
                 if not definition_str and s3_location:
                     # TODO: currently not covered by tests - add a test to mimick the behavior of "sam deploy ..."
@@ -114,14 +116,15 @@
                 "type": params.get("StateMachineType", None),
             }
 
         return {
             "create": {
                 "function": "create_state_machine",
                 "parameters": _create_params,
+                "result_handler": result_handler,
             },
             "delete": {
                 "function": "delete_state_machine",
                 "parameters": {"stateMachineArn": "PhysicalResourceId"},
             },
         }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/service_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     # ----------------------
     # ABSTRACT BASE METHODS
     # ----------------------
 
     def get_physical_resource_id(self, attribute=None, **kwargs):
         """Determine the physical resource ID (Ref) of this resource (to be overwritten by subclasses)"""
-        return None
+        return self.physical_resource_id
 
     def fetch_state(self, stack_name, resources):
         """Fetch the latest deployment state of this resource, or return None if not currently deployed (NOTE: THIS IS NOT ALWAYS TRUE)."""
         return None
 
     def update_resource(self, new_resource, stack_name, resources):
         """Update the deployment of this resource, using the updated properties (implemented by subclasses)."""
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230615085543/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/state/core.py` & `localstack-core-2.1.1.dev20230615085543/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230615085543/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230615085543/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230615085543/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230615085543/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/collections.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230615085543/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8428362573099415%*

 * *Differences: {"'localstack.hooks.on_infra_ready'": '{insert: [(1, '*

 * *                                      "'_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready')], "*

 * *                                      'delete: [0]}',*

 * * "'localstack.hooks.on_infra_shutdown'": '{insert: [(1, '*

 * *                                         "'run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers')], "*

 * *                                         'delete: [0]}',*

 * * "'localstack.hooks.on_infra_start'": '{ins […]*

```diff
@@ -45,44 +45,44 @@
         "swf:default=localstack.services.providers:swf",
         "transcribe:default=localstack.services.providers:transcribe"
     ],
     "localstack.hooks.configure_localstack_container": [
         "configure_edge_port=localstack.plugins:configure_edge_port"
     ],
     "localstack.hooks.on_infra_ready": [
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
+        "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
         "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser"
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
+        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
+        "terraform/community=localstack.packages.plugins:terraform_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
-        "terraform/community=localstack.packages.plugins:terraform_package",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
         "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
         "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package"
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230614212748/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230615085543/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/pyproject.toml` & `localstack-core-2.1.1.dev20230615085543/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230614212748/setup.cfg` & `localstack-core-2.1.1.dev20230615085543/setup.cfg`

 * *Files identical despite different names*

